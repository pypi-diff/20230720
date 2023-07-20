# Comparing `tmp/pydantic_resolve-1.6.2.tar.gz` & `tmp/pydantic_resolve-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_resolve-1.6.2.tar", max compression
+gzip compressed data, was "pydantic_resolve-1.6.3.tar", max compression
```

## Comparing `pydantic_resolve-1.6.2.tar` & `pydantic_resolve-1.6.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.2/LICENSE
--rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.2/pydantic_resolve/__init__.py
--rw-r--r--   0        0        0      275 2023-07-12 15:10:11.331859 pydantic_resolve-1.6.2/pydantic_resolve/constant.py
--rw-r--r--   0        0        0     2093 2023-07-12 15:11:15.219960 pydantic_resolve-1.6.2/pydantic_resolve/core.py
--rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.2/pydantic_resolve/exceptions.py
--rw-r--r--   0        0        0     8436 2023-07-13 03:23:57.878973 pydantic_resolve-1.6.2/pydantic_resolve/resolver.py
--rw-r--r--   0        0        0     7372 2023-07-13 06:50:23.332925 pydantic_resolve-1.6.2/pydantic_resolve/util.py
--rw-r--r--   0        0        0      814 2023-07-13 06:52:24.072339 pydantic_resolve-1.6.2/pyproject.toml
--rw-r--r--   0        0        0    10929 2023-07-13 03:29:52.380099 pydantic_resolve-1.6.2/README.md
--rw-r--r--   0        0        0    11348 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-03-07 14:12:05.553679 pydantic_resolve-1.6.3/LICENSE
+-rw-r--r--   0        0        0      593 2023-07-12 08:04:20.448957 pydantic_resolve-1.6.3/pydantic_resolve/__init__.py
+-rw-r--r--   0        0        0      362 2023-07-19 12:50:41.795062 pydantic_resolve-1.6.3/pydantic_resolve/constant.py
+-rw-r--r--   0        0        0     2094 2023-07-19 09:08:47.652925 pydantic_resolve-1.6.3/pydantic_resolve/core.py
+-rw-r--r--   0        0        0      229 2023-06-01 01:21:44.326847 pydantic_resolve-1.6.3/pydantic_resolve/exceptions.py
+-rw-r--r--   0        0        0     8700 2023-07-20 15:32:02.047585 pydantic_resolve-1.6.3/pydantic_resolve/resolver.py
+-rw-r--r--   0        0        0     8446 2023-07-20 15:40:08.283768 pydantic_resolve-1.6.3/pydantic_resolve/util.py
+-rw-r--r--   0        0        0      814 2023-07-20 15:41:19.280695 pydantic_resolve-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0    11394 2023-07-15 15:05:51.080033 pydantic_resolve-1.6.3/README.md
+-rw-r--r--   0        0        0    11791 1970-01-01 00:00:00.000000 pydantic_resolve-1.6.3/PKG-INFO
```

### Comparing `pydantic_resolve-1.6.2/LICENSE` & `pydantic_resolve-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.2/pydantic_resolve/__init__.py` & `pydantic_resolve-1.6.3/pydantic_resolve/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_resolve-1.6.2/pydantic_resolve/core.py` & `pydantic_resolve-1.6.3/pydantic_resolve/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             yield (field, attr, RESOLVER)
 
     for field in attributes: 
         if (field in resolver_fields):  # skip field of resolve_[field]
             continue
         attr = target.__getattribute__(field)
         if is_acceptable_type(attr) or is_list(attr):
-            yield (field, attr,ATTRIBUTE)
+            yield (field, attr, ATTRIBUTE)
 
 def iter_over_object_post_methods(target):
     """get method starts with post_"""
     for k in dir(target):
         if k == POST_DEFAULT_HANDLER:  # skip
             continue
         if k.startswith(POST_PREFIX) and ismethod(target.__getattribute__(k)):
```

### Comparing `pydantic_resolve-1.6.2/pydantic_resolve/resolver.py` & `pydantic_resolve-1.6.3/pydantic_resolve/resolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import asyncio
+from dataclasses import is_dataclass
 import inspect
 import contextvars
 from inspect import iscoroutine
 from typing import Type, TypeVar, Dict
 from .exceptions import ResolverTargetAttrNotFound, LoaderFieldNotProvidedError, MissingAnnotationError
 from typing import Any, Callable, Optional
 from pydantic_resolve import core
 from aiodataloader import DataLoader
 from inspect import isclass
 from types import MappingProxyType
-
+from pydantic import BaseModel
 import pydantic_resolve.constant as const
 import pydantic_resolve.util as util
 
 
 def LoaderDepend(  # noqa: N802
     dependency: Optional[Callable[..., Any]] = None,
 ) -> Any:
@@ -208,11 +209,15 @@
                 default_post_method()
 
         return target
 
     async def resolve(self, target: T) -> T:
         # if raise forwardref related error, use this
         if self.annotation_class:
-            util.update_forward_refs(self.annotation_class)
+            if issubclass(self.annotation_class, BaseModel):
+                util.update_forward_refs(self.annotation_class)
+
+            if is_dataclass(self.annotation_class):
+                util.update_dataclass_forward_refs(self.annotation_class)
 
         await self._resolve(target)
         return target
```

### Comparing `pydantic_resolve-1.6.2/pydantic_resolve/util.py` & `pydantic_resolve-1.6.3/pydantic_resolve/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 import types
 import functools
 from collections import defaultdict
 from dataclasses import is_dataclass
-from pydantic import BaseModel, parse_obj_as
-from inspect import iscoroutine, ismethod, isfunction
-from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator, Dict
+from pydantic import BaseModel, parse_obj_as, ValidationError
+from inspect import iscoroutine, isfunction
+from typing import Any, DefaultDict, Sequence, Type, TypeVar, List, Callable, Optional, Mapping, Union, Iterator, Dict, get_type_hints
 import pydantic_resolve.constant as const
 
 
 
 def get_class_field_annotations(cls: Type):
     anno = cls.__dict__.get('__annotations__') or {}
     return anno.keys()
@@ -185,26 +185,38 @@
                     if base_field and base_field.type_ != field.type_:
                         raise AttributeError(f'type of {k} not consistent with {base.__name__}'  )
             return  kls
         return inner()
     return wrap
 
 
-def update_forward_refs(kls: BaseModel):
+def update_forward_refs(kls: Type[BaseModel]):
     """
     recursively update refs.
     """
     kls.update_forward_refs()
     setattr(kls, const.PYDANTIC_FORWARD_REF_UPDATED, True)
 
     for field in kls.__fields__.values():
         if issubclass(field.type_, BaseModel):
             update_forward_refs(field.type_)
 
 
+def update_dataclass_forward_refs(kls):
+    if not getattr(kls, const.DATACLASS_FORWARD_REF_UPDATED, False):
+        anno = get_type_hints(kls)
+        kls.__annotations__ = anno
+        setattr(kls, const.DATACLASS_FORWARD_REF_UPDATED, True)
+
+        for _, v in kls.__annotations__.items():
+            t = shelling_type(v)
+            if is_dataclass(t):
+                update_dataclass_forward_refs(t)
+
+
 def try_parse_data_to_target_field_type(target, field_name, data):
     """
     parse to pydantic or dataclass object
     1. get type of target field
     2. parse
     """
     field_type = None
@@ -215,17 +227,35 @@
         field_type = _fields[field_name].outer_type_
 
         # handle optional logic
         if data is None and _fields[field_name].required == False:
             return data
 
     elif is_dataclass(target):
-        _fields = target.__dataclass_fields__
-        field_type = _fields[field_name].type
+        field_type = target.__class__.__annotations__[field_name]
 
     # 2. parse
     if field_type:
-        result = parse_obj_as(field_type, data)
-        return result
+        try:
+            result = parse_obj_as(field_type, data)
+            return result
+        except ValidationError as e:
+            print(f'Warning: type mismatch, pls check the return type for "{field_name}", expected: {field_type}')
+            raise e
     
     else:
         return data  #noqa
+
+
+def is_optional(annotation):
+    annotation_origin = getattr(annotation, "__origin__", None)
+    return annotation_origin == Union \
+        and len(annotation.__args__) == 2 \
+        and annotation.__args__[1] == type(None)  # noqa
+
+def is_list(annotation):
+    return getattr(annotation, "__origin__", None) == list
+
+def shelling_type(type):
+    while is_optional(type) or is_list(type):
+        type = type.__args__[0]
+    return type
```

### Comparing `pydantic_resolve-1.6.2/pyproject.toml` & `pydantic_resolve-1.6.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-resolve"
-version = "1.6.2"
+version = "1.6.3"
 description = "Make pydantic have a GraphQL-like assembly experience."
 authors = ["tangkikodo <allmonday@126.com>"]
 readme = "README.md"
 repository = "https://github.com/allmonday/pydantic_resolve"
 keywords = ["pydantic", "fastapi"]
 license = "MIT"
 packages = [{include = "pydantic_resolve"}]
```

### Comparing `pydantic_resolve-1.6.2/README.md` & `pydantic_resolve-1.6.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
-# Pydantic-resolve
+![img](doc/imgs/resolver.png)
+
+> A small yet powerful package which can run resolvers to generate deep nested datasets.
 
-[![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
-![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
-![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
+![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
+![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
+[![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
+
+
 
-> A small yet powerful package which can run resolvers to generate deep nested datasets.
 
 [Change log](./changelog.md)
 
 
 ## Install
 
 ```shell
@@ -325,14 +328,33 @@
         }
       ]
     }
   ]
 }
 ```
 
+## Use cases:
+
+for more cases like: how to filter members, how to make post calculation after resolved?
+
+please read the following demos.
+
+```shell
+cd examples
+
+python -m readme_demo.0_basic
+python -m readme_demo.1_filter
+python -m readme_demo.2_post_methods
+python -m readme_demo.3_context
+python -m readme_demo.4_loader_instance
+python -m readme_demo.5_subset
+python -m readme_demo.6_mapper
+python -m readme_demo.7_single
+```
+
 
 ## API
 
 ### Resolver(loader_filters, loader_instances, ensure_type, annotation_class, context)
 
 - loader_filters: `dict`
```

### Comparing `pydantic_resolve-1.6.2/PKG-INFO` & `pydantic_resolve-1.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-resolve
-Version: 1.6.2
+Version: 1.6.3
 Summary: Make pydantic have a GraphQL-like assembly experience.
 Home-page: https://github.com/allmonday/pydantic_resolve
 License: MIT
 Keywords: pydantic,fastapi
 Author: tangkikodo
 Author-email: allmonday@126.com
 Requires-Python: >=3.7,<4.0
@@ -16,23 +16,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiodataloader (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=1.10.4,<2.0.0)
 Project-URL: Repository, https://github.com/allmonday/pydantic_resolve
 Description-Content-Type: text/markdown
 
-# Pydantic-resolve
+![img](doc/imgs/resolver.png)
+
+> A small yet powerful package which can run resolvers to generate deep nested datasets.
 
-[![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
-![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
-![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
 [![pypi](https://img.shields.io/pypi/v/pydantic-resolve.svg)](https://pypi.python.org/pypi/pydantic-resolve)
 [![Downloads](https://static.pepy.tech/personalized-badge/pydantic-resolve?period=month&units=abbreviation&left_color=grey&right_color=orange&left_text=Downloads)](https://pepy.tech/project/pydantic-resolve)
+![Python Versions](https://img.shields.io/pypi/pyversions/pydantic-resolve)
+![Test Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/allmonday/6f1661c6310e1b31c9a10b0d09d52d11/raw/covbadge.json)
+[![CI](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml/badge.svg)](https://github.com/allmonday/pydantic_resolve/actions/workflows/ci.yml)
+
+
 
-> A small yet powerful package which can run resolvers to generate deep nested datasets.
 
 [Change log](./changelog.md)
 
 
 ## Install
 
 ```shell
@@ -347,14 +350,33 @@
         }
       ]
     }
   ]
 }
 ```
 
+## Use cases:
+
+for more cases like: how to filter members, how to make post calculation after resolved?
+
+please read the following demos.
+
+```shell
+cd examples
+
+python -m readme_demo.0_basic
+python -m readme_demo.1_filter
+python -m readme_demo.2_post_methods
+python -m readme_demo.3_context
+python -m readme_demo.4_loader_instance
+python -m readme_demo.5_subset
+python -m readme_demo.6_mapper
+python -m readme_demo.7_single
+```
+
 
 ## API
 
 ### Resolver(loader_filters, loader_instances, ensure_type, annotation_class, context)
 
 - loader_filters: `dict`
```

