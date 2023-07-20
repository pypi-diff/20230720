# Comparing `tmp/apix_core-0.0.4.tar.gz` & `tmp/apix_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apix_core-0.0.4.tar", max compression
+gzip compressed data, was "apix_core-0.0.5.tar", max compression
```

## Comparing `apix_core-0.0.4.tar` & `apix_core-0.0.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1075 2023-07-20 12:44:40.682392 apix_core-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     4287 2023-07-20 12:44:40.682392 apix_core-0.0.4/README.md
--rw-r--r--   0        0        0      596 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/__init__.py
--rw-r--r--   0        0        0     7110 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/app.py
--rw-r--r--   0        0        0    40015 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/attribute.py
--rw-r--r--   0        0        0     1674 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/authenticator.py
--rw-r--r--   0        0        0    19333 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/collection.py
--rw-r--r--   0        0        0     4901 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/comparison.py
--rw-r--r--   0        0        0    12895 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/comparison_type.py
--rw-r--r--   0        0        0      902 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/context.py
--rw-r--r--   0        0        0     1255 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/cursor.py
--rw-r--r--   0        0        0      975 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/cursor_type.py
--rw-r--r--   0        0        0     2997 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/database.py
--rw-r--r--   0        0        0      711 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/direction.py
--rw-r--r--   0        0        0     1501 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/direction_type.py
--rw-r--r--   0        0        0     1072 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/document.py
--rw-r--r--   0        0        0     2584 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/enumeration.py
--rw-r--r--   0        0        0      700 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/error.py
--rw-r--r--   0        0        0     1362 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/error_handler.py
--rw-r--r--   0        0        0     1053 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/filter.py
--rw-r--r--   0        0        0     1421 2023-07-20 12:44:40.682392 apix_core-0.0.4/apix/filter_type.py
--rw-r--r--   0        0        0     4603 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/gql.py
--rw-r--r--   0        0        0     6353 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/model.py
--rw-r--r--   0        0        0     2196 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/operation.py
--rw-r--r--   0        0        0     6248 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/operation_type.py
--rw-r--r--   0        0        0     1622 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/operator.py
--rw-r--r--   0        0        0      798 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/order.py
--rw-r--r--   0        0        0     1332 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/order_type.py
--rw-r--r--   0        0        0     7685 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/resolver.py
--rw-r--r--   0        0        0      430 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/scalar.py
--rw-r--r--   0        0        0     3302 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/select.py
--rw-r--r--   0        0        0      553 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/select_type.py
--rw-r--r--   0        0        0      241 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/session.py
--rw-r--r--   0        0        0      827 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/update.py
--rw-r--r--   0        0        0     1303 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/update_type.py
--rw-r--r--   0        0        0      580 2023-07-20 12:44:40.686392 apix_core-0.0.4/apix/utils.py
--rw-r--r--   0        0        0      797 2023-07-20 12:44:40.686392 apix_core-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     5121 1970-01-01 00:00:00.000000 apix_core-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-20 13:42:28.654733 apix_core-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     4287 2023-07-20 13:42:28.654733 apix_core-0.0.5/README.md
+-rw-r--r--   0        0        0      596 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/__init__.py
+-rw-r--r--   0        0        0     7110 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/app.py
+-rw-r--r--   0        0        0    40015 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/attribute.py
+-rw-r--r--   0        0        0     1674 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/authenticator.py
+-rw-r--r--   0        0        0    19333 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/collection.py
+-rw-r--r--   0        0        0     4901 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/comparison.py
+-rw-r--r--   0        0        0    12895 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/comparison_type.py
+-rw-r--r--   0        0        0      902 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/context.py
+-rw-r--r--   0        0        0     1255 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/cursor.py
+-rw-r--r--   0        0        0      975 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/cursor_type.py
+-rw-r--r--   0        0        0     2997 2023-07-20 13:42:28.654733 apix_core-0.0.5/apix/database.py
+-rw-r--r--   0        0        0      711 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/direction.py
+-rw-r--r--   0        0        0     1501 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/direction_type.py
+-rw-r--r--   0        0        0     1072 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/document.py
+-rw-r--r--   0        0        0     2584 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/enumeration.py
+-rw-r--r--   0        0        0      700 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/error.py
+-rw-r--r--   0        0        0     1362 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/error_handler.py
+-rw-r--r--   0        0        0     1053 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/filter.py
+-rw-r--r--   0        0        0     1421 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/filter_type.py
+-rw-r--r--   0        0        0     4603 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/gql.py
+-rw-r--r--   0        0        0     7739 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/model.py
+-rw-r--r--   0        0        0     2196 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/operation.py
+-rw-r--r--   0        0        0     6248 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/operation_type.py
+-rw-r--r--   0        0        0     1622 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/operator.py
+-rw-r--r--   0        0        0      798 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/order.py
+-rw-r--r--   0        0        0     1332 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/order_type.py
+-rw-r--r--   0        0        0     8275 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/resolver.py
+-rw-r--r--   0        0        0      430 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/scalar.py
+-rw-r--r--   0        0        0     3302 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/select.py
+-rw-r--r--   0        0        0      553 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/select_type.py
+-rw-r--r--   0        0        0      241 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/session.py
+-rw-r--r--   0        0        0      827 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/update.py
+-rw-r--r--   0        0        0     1303 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/update_type.py
+-rw-r--r--   0        0        0      580 2023-07-20 13:42:28.658733 apix_core-0.0.5/apix/utils.py
+-rw-r--r--   0        0        0      797 2023-07-20 13:42:28.658733 apix_core-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5121 1970-01-01 00:00:00.000000 apix_core-0.0.5/PKG-INFO
```

### Comparing `apix_core-0.0.4/LICENSE.txt` & `apix_core-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/README.md` & `apix_core-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/__init__.py` & `apix_core-0.0.5/apix/__init__.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/app.py` & `apix_core-0.0.5/apix/app.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/attribute.py` & `apix_core-0.0.5/apix/attribute.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/authenticator.py` & `apix_core-0.0.5/apix/authenticator.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/collection.py` & `apix_core-0.0.5/apix/collection.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/comparison.py` & `apix_core-0.0.5/apix/comparison.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/comparison_type.py` & `apix_core-0.0.5/apix/comparison_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/context.py` & `apix_core-0.0.5/apix/context.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/cursor.py` & `apix_core-0.0.5/apix/cursor.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/cursor_type.py` & `apix_core-0.0.5/apix/cursor_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/database.py` & `apix_core-0.0.5/apix/database.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/direction.py` & `apix_core-0.0.5/apix/direction.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/direction_type.py` & `apix_core-0.0.5/apix/direction_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/document.py` & `apix_core-0.0.5/apix/document.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/enumeration.py` & `apix_core-0.0.5/apix/enumeration.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/error.py` & `apix_core-0.0.5/apix/error.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/error_handler.py` & `apix_core-0.0.5/apix/error_handler.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/filter.py` & `apix_core-0.0.5/apix/filter.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/filter_type.py` & `apix_core-0.0.5/apix/filter_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/gql.py` & `apix_core-0.0.5/apix/gql.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/model.py` & `apix_core-0.0.5/apix/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from inspect import signature
 from typing import Any, Callable, Dict, List, TYPE_CHECKING
 
 from apix.attribute import *
 from apix.cursor_type import *
 from apix.document import *
 from apix.filter_type import *
 from apix.gql import *
@@ -27,49 +28,75 @@
 
     def __new__(
             mcs,
             name: str,
             attributes: List[ApixAttribute] | Callable[[], List[ApixAttribute]],
             *,
             gql_output_type_description: str = None,
-            gql_output_field_description: str = None,
             gql_input_type_description: str = None,
-            gql_input_field_description: str = None,
             gql_update_type_description: str = None,
             gql_filter_type_description: str = None,
             gql_order_type_description: str = None,
     ):
 
-        if not is_snake_case(name):
-            raise ValueError(f"Name '{name}' must be snake case.")
+        if not isinstance(name, str):
+            raise TypeError("The argument 'name' must be a string")
+        elif not is_snake_case(name):
+            raise ValueError("The argument 'name' must be snake case")
+
+        if isinstance(attributes, list):
+            for attribute in attributes:
+                if not isinstance(attribute, ApixAttribute):
+                    raise TypeError("Each element of the argument 'attributes' must be an ApixAttribute")
+        elif callable(attributes):
+            if len(signature(attributes).parameters) > 0:
+                raise ValueError("The argument 'attributes' must be a function with no argument")
+        else:
+            raise TypeError("The argument 'attributes' must be a list or a function")
+
+        if gql_output_type_description is not None:
+            if not isinstance(gql_output_type_description, str):
+                raise TypeError("The argument 'gql_output_type_description' must be a string")
+
+        if gql_input_type_description is not None:
+            if not isinstance(gql_input_type_description, str):
+                raise TypeError("The argument 'gql_input_type_description' must be a string")
+
+        if gql_update_type_description is not None:
+            if not isinstance(gql_update_type_description, str):
+                raise TypeError("The argument 'gql_update_type_description' must be a string")
+
+        if gql_filter_type_description is not None:
+            if not isinstance(gql_filter_type_description, str):
+                raise TypeError("The argument 'gql_filter_type_description' must be a string")
+
+        if gql_order_type_description is not None:
+            if not isinstance(gql_order_type_description, str):
+                raise TypeError("The argument 'gql_order_type_description' must be a string")
 
         return super().__new__(mcs, mcs.__name__, (ApixDocument,), {})
 
     def __init__(
             cls,
             name: str,
             attributes: List[ApixAttribute] | Callable[[], List[ApixAttribute]],
             *,
             gql_output_type_description: str = None,
-            gql_output_field_description: str = None,
             gql_input_type_description: str = None,
-            gql_input_field_description: str = None,
             gql_update_type_description: str = None,
             gql_filter_type_description: str = None,
             gql_order_type_description: str = None,
     ):
 
         super().__init__(cls.__name__, (ApixDocument,), {})
 
         cls.name = name
         cls._attributes = attributes
         cls.gql_output_type_description = gql_output_type_description
-        cls.gql_output_field_description = gql_output_field_description
         cls.gql_input_type_description = gql_input_type_description
-        cls.gql_input_field_description = gql_input_field_description
         cls.gql_update_type_description = gql_update_type_description
         cls.gql_filter_type_description = gql_filter_type_description
         cls.gql_order_type_description = gql_order_type_description
 
         cls.Filter = ApixFilterType(cls)
         cls.Update = ApixUpdateType(cls)
         cls.Order = ApixOrderType(cls)
```

### Comparing `apix_core-0.0.4/apix/operation.py` & `apix_core-0.0.5/apix/operation.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/operation_type.py` & `apix_core-0.0.5/apix/operation_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/operator.py` & `apix_core-0.0.5/apix/operator.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/order.py` & `apix_core-0.0.5/apix/order.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/order_type.py` & `apix_core-0.0.5/apix/order_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/resolver.py` & `apix_core-0.0.5/apix/resolver.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,22 +20,38 @@
     'ApixQueryResolver',
     'ApixMutationResolver',
 ]
 
 
 class ApixResolver:
 
+    def __new__(
+            cls,
+            resolve: Callable,
+            *,
+            gql_resolver_field_description: str = None,
+    ):
+
+        if not callable(resolve):
+            raise TypeError("The argument 'attributes' must be a function")
+
+        if gql_resolver_field_description is not None:
+            if not isinstance(gql_resolver_field_description, str):
+                raise TypeError("The argument 'gql_resolver_field_description' must be a string")
+
+        return super().__new__(cls)
+
     def __init__(
             self,
             resolve: Callable,
-            description: str = None,
+            gql_resolver_field_description: str = None,
     ):
 
         self._resolve = resolve
-        self.description = description
+        self.gql_resolver_field_description = gql_resolver_field_description
 
         self._app = None
 
     def __repr__(self) -> str:
         return f'<{self.__class__.__name__}:{self.class_name}>'
 
     @cached_property
@@ -97,15 +113,15 @@
     @cached_property
     def gql_output_field(self) -> GraphQLField:
 
         return GraphQLField(
             type_=self.gql_output_type,
             args=self.gql_arguments,
             resolve=self.resolve,
-            description=self.description,
+            description=self.gql_resolver_field_description,
         )
 
     async def resolve(
             self,
             _,
             gql_resolve_info: GraphQLResolveInfo,
             **kwargs,
```

### Comparing `apix_core-0.0.4/apix/select.py` & `apix_core-0.0.5/apix/select.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/select_type.py` & `apix_core-0.0.5/apix/select_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/update.py` & `apix_core-0.0.5/apix/update.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/update_type.py` & `apix_core-0.0.5/apix/update_type.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/apix/utils.py` & `apix_core-0.0.5/apix/utils.py`

 * *Files identical despite different names*

### Comparing `apix_core-0.0.4/pyproject.toml` & `apix_core-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apix-core"
-version = "0.0.4"
+version = "0.0.5"
 description = "apiX - The Python framework to create MongoDB-backed applications with GraphQL API web interface."
 authors = ["Danijel Kivaranovic <dan@apix.org>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["graphql", "mongodb", "api", "starlette", "async"]
 homepage = "https://apix.org"
 repository = "https://github.com/ApixOrg/apix"
```

### Comparing `apix_core-0.0.4/PKG-INFO` & `apix_core-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apix-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: apiX - The Python framework to create MongoDB-backed applications with GraphQL API web interface.
 Home-page: https://apix.org
 License: MIT
 Keywords: graphql,mongodb,api,starlette,async
 Author: Danijel Kivaranovic
 Author-email: dan@apix.org
 Requires-Python: >=3.11,<4.0
```

