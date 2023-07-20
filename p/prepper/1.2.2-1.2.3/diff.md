# Comparing `tmp/prepper-1.2.2.tar.gz` & `tmp/prepper-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prepper-1.2.2.tar", last modified: Mon Jun 26 16:05:30 2023, max compression
+gzip compressed data, was "prepper-1.2.3.tar", last modified: Thu Jul 20 15:15:55 2023, max compression
```

## Comparing `prepper-1.2.2.tar` & `prepper-1.2.3.tar`

### file list

```diff
@@ -1,30 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.298766 prepper-1.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-26 16:05:18.000000 prepper-1.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-26 16:05:18.000000 prepper-1.2.2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-06-26 16:05:18.000000 prepper-1.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-26 16:05:18.000000 prepper-1.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 16:05:18.000000 prepper-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 16:05:30.302766 prepper-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-26 16:05:18.000000 prepper-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/prepper/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    19362 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/exportable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26985 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/io_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/prepper/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/tests/test_IO.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-26 16:05:18.000000 prepper-1.2.2/prepper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:05:30.302766 prepper-1.2.2/prepper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-26 16:05:30.000000 prepper-1.2.2/prepper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-26 16:05:18.000000 prepper-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 16:05:30.302766 prepper-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.039831 prepper-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.031831 prepper-1.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.035831 prepper-1.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-20 15:15:44.000000 prepper-1.2.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-20 15:15:44.000000 prepper-1.2.3/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-20 15:15:44.000000 prepper-1.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-20 15:15:44.000000 prepper-1.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-20 15:15:44.000000 prepper-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 15:15:55.039831 prepper-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:15:44.000000 prepper-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.035831 prepper-1.2.3/prepper/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 15:15:54.000000 prepper-1.2.3/prepper/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19511 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/exportable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27055 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/io_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.035831 prepper-1.2.3/prepper/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/tests/test_IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-07-20 15:15:44.000000 prepper-1.2.3/prepper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.035831 prepper-1.2.3/prepper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 15:15:55.000000 prepper-1.2.3/prepper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 15:15:55.000000 prepper-1.2.3/prepper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:55.000000 prepper-1.2.3/prepper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-20 15:15:55.000000 prepper-1.2.3/prepper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:15:55.000000 prepper-1.2.3/prepper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-20 15:15:44.000000 prepper-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:55.039831 prepper-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.031831 prepper-1.2.3/typings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.039831 prepper-1.2.3/typings/periodictable/
+-rw-r--r--   0 runner    (1001) docker     (123)     6065 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/activation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/chemicals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14693 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/covalent_radius.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/cromermann.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/crystal_structure.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/density.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/fasta.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/formulas.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/magnetic_ff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/mass.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36476 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/nsf.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/nsf_resonances.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/nsf_tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/plot.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-07-20 15:15:44.000000 prepper-1.2.3/typings/periodictable/xsf.pyi
```

### Comparing `prepper-1.2.2/.github/workflows/python-publish.yml` & `prepper-1.2.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.2.2/.github/workflows/python-test.yml` & `prepper-1.2.3/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `prepper-1.2.2/.gitignore` & `prepper-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `prepper-1.2.2/.pre-commit-config.yaml` & `prepper-1.2.3/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 repos:
 
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.0.275
+  hooks:
+    - id: ruff
+      args: [ --fix, --exit-non-zero-on-fix ]
 
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
     - id: isort
       name: isort (python)
```

### Comparing `prepper-1.2.2/LICENSE` & `prepper-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prepper-1.2.2/prepper/caching.py` & `prepper-1.2.3/prepper/caching.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from __future__ import annotations
 
 import functools
 from collections.abc import Callable
 from functools import update_wrapper
 from typing import Generic, overload, TYPE_CHECKING, TypeVar, Union
 
-import numpy as np
 from joblib import hash as joblib_hash
 from numpy import ndarray
 from typing_extensions import Concatenate, ParamSpec, Self
 
 if TYPE_CHECKING:
     from .exportable import ExportableClassMixin
 
@@ -41,15 +40,19 @@
             try:
                 hash_values.append(v.item())
             except Exception:
                 hash_values.append(v)
 
         self[:] = hash_values
 
-        self.hashvalue = int(joblib_hash(hash_values, hash_name="sha1"), 16)
+        hashvalue = joblib_hash(hash_values, hash_name="sha1")
+        if hashvalue is not None:
+            self.hashvalue = int(hashvalue, 16)
+        else:
+            self.hashvalue = None
 
     def __hash__(self):
         return self.hashvalue
 
 
 def break_key(key):
     "Breaks a function cache key into the args and kwargs"
@@ -125,15 +128,15 @@
     itself with an ordinary attribute. Deleting the attribute resets the
     property. Implementation adapted from https://github.com/pydanny/cached-property
     """
 
     func: Callable[[T], R]
 
     def __init__(self, func: Callable[[T], R]):
-        update_wrapper(self, func)
+        update_wrapper(self, func)  # type: ignore
         self.func = func
 
     @overload
     def __get__(self, instance: T, owner: object) -> R:
         ...
 
     @overload
@@ -186,15 +189,15 @@
         if instance is None:
             return self.user_func
         else:
             partial_function = functools.update_wrapper(
                 functools.partial(_cache_wrapper(self.user_func), instance),
                 self.user_func,
             )
-            return partial_function
+            return partial_function  # type: ignore
 
     def __set__(self, obj, value):
         fname = make_cache_name(self.user_func.__qualname__)
         if fname not in obj.__dict__:
             obj.__dict__[fname] = {}
 
         key, return_value = value
```

### Comparing `prepper-1.2.2/prepper/enums.py` & `prepper-1.2.3/prepper/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from enum import Enum, unique
+
+    from aenum import extend_enum
 else:
     from aenum import Enum, extend_enum, unique
 
-from aenum import extend_enum
-
 __all__ = ["H5StoreTypes", "add_enum_item"]
 
 
 @unique
 class H5StoreTypes(Enum):
     Sequence = 1
     Dictionary = 2
```

### Comparing `prepper-1.2.2/prepper/exportable.py` & `prepper-1.2.3/prepper/exportable.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,78 +31,14 @@
     NumpyDowncastWarning = None
 
 __all__ = [
     "ExportableClassMixin",
 ]
 
 
-def saveable_class(
-    api_version: float,
-    attributes: List[str] = None,
-    functions: List[str] = None,
-) -> Callable[[ExportableClassMixin], ExportableClassMixin]:
-    if attributes is None:
-        attributes = []
-    if functions is None:
-        functions = []
-
-    def decorator(cls: ExportableClassMixin) -> ExportableClassMixin:
-        if not issubclass(cls, ExportableClassMixin):
-            raise ValueError(
-                "Only subclasses of ExportableClassMixin can be decorated with saveable_class"
-            )
-        attribute_names = []
-        function_names = []
-
-        exportable_functions = []
-        exportable_attributes = []
-
-        for parent in reversed(inspect.getmro(cls)):
-            if hasattr(parent, "_exportable_attributes"):
-                for attr in parent._exportable_attributes:
-                    bound_class, symbol = attr.split(".")
-                    attribute_names.append(symbol)
-            if hasattr(parent, "_exportable_functions"):
-                for fcn in parent._exportable_functions:
-                    bound_class, symbol = fcn.split(".")
-                    function_names.append(symbol)
-        for attr in attributes:
-            attribute_names.append(attr)
-
-        for fcn in functions:
-            function_names.append(fcn)
-
-        for symbol in attribute_names:
-            if not hasattr(cls, symbol):
-                raise ValueError(
-                    f"{cls} and its parents does not have property/attribute {symbol} at runtime. Dynamically added attributes are not supported."
-                )
-            try:
-                exportable_attributes.append(getattr(cls, symbol).__qualname__)
-            except AttributeError as exc:
-                raise ValueError(
-                    f"{cls}.{symbol} is a property. Saving properties is not supported as they dont have __dict__ entries. Make {symbol} a cached property instead."
-                ) from None
-
-        for symbol in function_names:
-            if not hasattr(cls, symbol):
-                raise ValueError(
-                    f"{cls} and its parents does not have function {symbol}"
-                )
-            exportable_functions.append(getattr(cls, symbol).__qualname__)
-
-        cls._exportable_functions = set(exportable_functions)
-        cls._exportable_attributes = set(exportable_attributes)
-        cls.api_version = api_version
-
-        return cls
-
-    return decorator
-
-
 class ExportableClassMixin(metaclass=ABCMeta):
     """
     Allows the class to be saved and loaded from an HDF5 file
 
     """
 
     _constructor_args: Dict[str, Any] = {}
@@ -146,14 +82,16 @@
         return instance
 
     def __hash__(self):
         keys = list(self._constructor_args.keys())
         values = list(self._constructor_args.values())
 
         digest = joblib.hash(keys + values, hash_name="sha1")
+        if digest is None:
+            return None
         return int.from_bytes(bytes(digest, encoding="utf-8"), "big")
 
     def __getnewargs_ex__(self):
         return (), self._constructor_args
 
     def __eq__(self, other) -> bool:
         if not isinstance(self, type(other)):
@@ -200,15 +138,15 @@
         with h5py.File(path, mode="r", track_order=True) as hdf5_file:
             if group not in hdf5_file:
                 msg = f"Failed to load {group} because it does not exist!"
                 loguru.logger.error(msg)
                 raise H5StoreException(msg)
             entry = hdf5_file[group]
 
-            if cls.__name__ in entry:
+            if cls.__name__ in entry:  # type: ignore
                 init_kw_type, init_kws = ExportableClassMixin._load_h5_entry(
                     path, f"{group}/{cls.__name__}"
                 )
                 if init_kw_type != H5StoreTypes.ClassConstructor:
                     raise H5StoreException()
             else:
                 init_kws = {}
@@ -229,25 +167,25 @@
             entry_type = ExportableClassMixin._get_group_type(base)
             if entry_type != H5StoreTypes.PythonClass:
                 raise ValueError(
                     f"_read_hdf5_contents was called on a HDF5 group {group} that is not a python class spec!"
                 )
 
             try:
-                class_name = read_h5_attr(base, "class")
+                class_name = read_h5_attr(base, "class")  # type: ignore
             except KeyError as exc:
                 msg = f"Failed to load {group} because the class name was not stored!"
                 loguru.logger.error(msg)
                 raise H5StoreException(msg) from exc
             if class_name != self.__class__.__name__:
                 msg = f"Failed to load {group} because the stored class name ({class_name}) is not the same as the loading class ({self.__class__.__name__})!"
                 loguru.logger.error(msg)
                 raise H5StoreException(msg)
 
-            for entry_name in base:
+            for entry_name in base:  # type: ignore
                 # The class constructor should have already been read
                 if entry_name == self.__class__.__name__:
                     continue
 
                 entry_type, entry_value = self._load_h5_entry(
                     file, f"{group}/{entry_name}"
                 )
@@ -417,15 +355,15 @@
 
     @staticmethod
     def _dump_h5_entry(
         file: str,
         entry_name: str,
         value: Any,
         existing_groups: Dict[str, Any],
-        attributes: Dict[str, Any] = None,
+        attributes: Dict[str, Any] | None = None,
     ):
         from prepper.io_handlers import dump_custom_h5_type, write_h5_attr
 
         entry_name = entry_name.replace("//", "/").strip()
         if attributes is None:
             attributes = {}
 
@@ -439,15 +377,15 @@
             raise ValueError(msg) from exc
 
         # Add any attributes that were needed
         with h5py.File(file, mode="a", track_order=True) as hdf5_file:
             new_entry = hdf5_file[entry_name]
             for k, v in attributes.items():
                 try:
-                    write_h5_attr(new_entry, k, v)
+                    write_h5_attr(new_entry, k, v)  # type: ignore
                 except H5StoreException:
                     msg = (
                         f"Failed to write attribute {k} to group {new_entry}!"
                     )
                     loguru.logger.error(msg)
 
         return existing_groups
@@ -481,19 +419,85 @@
                 msg = f"Failed to load {group} because the group bound_class was not stored! Available attrs are {list(group.attrs.keys())}"
                 loguru.logger.error(msg)
                 raise H5StoreException(msg) from exc
 
             return entry_type
 
 
+C = Type[ExportableClassMixin]  # class being wrapped by the decorator
+
+
+def saveable_class(
+    api_version: float,
+    attributes: List[str] | None = None,
+    functions: List[str] | None = None,
+) -> Callable[[C], C]:
+    if attributes is None:
+        attributes = []
+    if functions is None:
+        functions = []
+
+    def decorator(cls: C) -> C:
+        if not issubclass(cls, ExportableClassMixin):
+            raise ValueError(
+                "Only subclasses of ExportableClassMixin can be decorated with saveable_class"
+            )
+        attribute_names: List[str] = []
+        function_names: List[str] = []
+
+        exportable_functions: List[str] = []
+        exportable_attributes: List[str] = []
+
+        for parent in reversed(inspect.getmro(cls)):
+            if hasattr(parent, "_exportable_attributes"):
+                for attr in parent._exportable_attributes:  # type: ignore
+                    bound_class, symbol = attr.split(".")
+                    attribute_names.append(symbol)
+            if hasattr(parent, "_exportable_functions"):
+                for fcn in parent._exportable_functions:  # type: ignore
+                    bound_class, symbol = fcn.split(".")
+                    function_names.append(symbol)
+        for attr in attributes:
+            attribute_names.append(attr)
+
+        for fcn in functions:
+            function_names.append(fcn)
+
+        for symbol in attribute_names:
+            if not hasattr(cls, symbol):
+                raise ValueError(
+                    f"{cls} and its parents does not have property/attribute {symbol} at runtime. Dynamically added attributes are not supported."
+                )
+            try:
+                exportable_attributes.append(getattr(cls, symbol).__qualname__)
+            except AttributeError:
+                raise ValueError(
+                    f"{cls}.{symbol} is a property. Saving properties is not supported as they dont have __dict__ entries. Make {symbol} a cached property instead."
+                ) from None
+
+        for symbol in function_names:
+            if not hasattr(cls, symbol):
+                raise ValueError(
+                    f"{cls} and its parents does not have function {symbol}"
+                )
+            exportable_functions.append(getattr(cls, symbol).__qualname__)
+
+        cls._exportable_functions = list(set(exportable_functions))
+        cls._exportable_attributes = list(set(exportable_attributes))
+        cls.api_version = api_version
+
+        return cls
+
+    return decorator
+
+
 if __name__ == "__main__":
-    from prepper import ExportableClassMixin, saveable_class
 
     @saveable_class(
-        "0.0.1", attributes=["test_string", "test_array", "test_array2"]
+        0.1, attributes=["test_string", "test_array", "test_array2"]
     )
     class SimpleSaveableClass(ExportableClassMixin):
         """
         A simple saveable class, used to test saving as an attribute of another
         saveable class
         """
```

### Comparing `prepper-1.2.2/prepper/io_handlers.py` & `prepper-1.2.3/prepper/io_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import importlib
 import numbers
 import re
 import tempfile
 import traceback
 from collections.abc import Iterable
 from enum import Enum
-from typing import Any, Dict, List, Sequence, Type, Union
+from typing import Any, Dict, List, Sequence, Tuple, Type, Union
 
 import h5py
 import loguru
 import numpy as np
 
 from prepper import H5StoreException
 from prepper.caching import _HashedSeq, _make_key
@@ -175,15 +175,15 @@
         with h5py.File(file, mode="a", track_order=True) as hdf5_file:
             hdf5_file[group] = h5py.SoftLink(clone_group)
         return existing_groups
 
     for name, (validator, writer) in writers.items():
         try:
             is_valid = validator(value)
-        except Exception as e:
+        except Exception:
             msg = f"Failed to check condition {name} for value {value} of type {type(value)}!"
             loguru.logger.error(msg, exc_info=True)
             is_valid = False
         if is_valid:
             attrs, existing_groups = writer(
                 file, group, value, existing_groups
             )
@@ -191,28 +191,30 @@
             with h5py.File(file, mode="a", track_order=True) as hdf5_file:
                 try:
                     entry = hdf5_file[group]
                 except KeyError:
                     entry = hdf5_file.require_group(group)
                 for k, v in attrs.items():
                     try:
-                        write_h5_attr(entry, k, v)
+                        write_h5_attr(entry, k, v)  # type: ignore
                     except H5StoreException:
                         msg = (
                             f"Failed to write attribute {k} to group {group}!"
                         )
                         loguru.logger.error(msg, exc_info=True)
 
             return existing_groups
     raise H5StoreException(
         f"None of the custom HDF5 writer functions supported a value of type {type(value)}!"
     )
 
 
-def load_custom_h5_type(file: str, group: str, entry_type: H5StoreTypes):
+def load_custom_h5_type(
+    file: str, group: str, entry_type: H5StoreTypes
+) -> Any:
     loaders = {}
     loaders.update(CUSTOM_H5_LOADERS)
     loaders.update(DEFAULT_H5_LOADERS)
     for loader_type, loader in loaders.values():
         if loader_type == entry_type:
             return loader(file, group)
     msg = (
@@ -253,15 +255,15 @@
     return name
 
 
 #### NONE ####
 @_register(DEFAULT_H5_WRITERS, lambda x: x is None)
 def dump_None(
     file: str, group: str, value: None, existing_groups: Dict[str, Any]
-) -> Dict[str, Any]:
+) -> Tuple[Dict[str, Any], Dict[str, Any]]:
     attributes = {}
     attributes["type"] = H5StoreTypes.Null.name
     return attributes, existing_groups
 
 
 @_register(DEFAULT_H5_LOADERS, H5StoreTypes.Null)
 def load_None(file: str, group: str):
@@ -270,15 +272,15 @@
 
 #### FunctionCache ####
 @_register(DEFAULT_H5_LOADERS, H5StoreTypes.FunctionCache)
 def load_hdf5_function_cache(file: str, group: str) -> Dict[_HashedSeq, Any]:
     function_calls = {}
     with h5py.File(file, mode="r", track_order=True) as hdf5_file:
         function_group = hdf5_file[group]
-        for function_call in function_group:
+        for function_call in function_group:  # type: ignore
             arg_group_name = f"{group}/{function_call}/args"
             kwarg_group_name = f"{group}/{function_call}/kwargs"
             value_group_name = f"{group}/{function_call}/value"
             _, args = ExportableClassMixin._load_h5_entry(file, arg_group_name)
             _, kwargs = ExportableClassMixin._load_h5_entry(
                 file, kwarg_group_name
             )
@@ -339,20 +341,20 @@
     return attributes, existing_groups
 
 
 @_register(DEFAULT_H5_LOADERS, H5StoreTypes.PythonClass)
 def load_exportable_class(file: str, group: str) -> Type[ExportableClassMixin]:
     with h5py.File(file, "r", track_order=True) as hdf5_file:
         entry = hdf5_file[group]
-        if not "module" in entry.attrs:
+        if "module" not in entry.attrs:
             msg = f"Failed to load {group} because it was a class entry, but didnt have the class module path in the attribute list!"
             loguru.logger.error(msg)
             raise H5StoreException(msg)
         class_module = importlib.import_module(entry.attrs["module"])
-        if not "class" in entry.attrs:
+        if "class" not in entry.attrs:
             msg = f"Failed to load {group} because it was a class entry, but didnt have the class name in the attribute list!"
             loguru.logger.error(msg)
             raise H5StoreException(msg)
         class_definition = getattr(class_module, entry.attrs["class"])
         return class_definition.from_hdf5(file, group)
```

### Comparing `prepper-1.2.2/prepper/tests/test_IO.py` & `prepper-1.2.3/prepper/tests/test_IO.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         shape=hnp.array_shapes(min_dims=1, max_dims=4),
         dtype=float,
     )
 )
 @settings(deadline=None)
 def test_cached_property(x):
     test_class = SimpleSaveableClass(x)
-    new_class = roundtrip(test_class, should_not_be_saved=["a", "mult"])
+    roundtrip(test_class, should_not_be_saved=["a", "mult"])
 
 
 @given(
     strategies.lists(
         strategies.one_of(
             strategies.integers(min_value=-100, max_value=100),
             strategies.floats(allow_nan=False, allow_infinity=False, width=32),
@@ -97,15 +97,15 @@
         max_size=4,
     )
 )
 @settings(deadline=None)
 def test_with_heterogenous_list(x):
     test_class = SimpleSaveableClass(x)
     _ = test_class.mult(2)
-    new_class = roundtrip(test_class)
+    roundtrip(test_class)
 
 
 @given(
     strategies.lists(
         strategies.text(
             min_size=1,
             alphabet=strategies.characters(
@@ -115,15 +115,15 @@
         min_size=1,
     )
 )
 @settings(deadline=None)
 def test_with_str_list(x):
     test_class = SimpleSaveableClass(x)
     _ = test_class.mult(2)
-    new_class = roundtrip(test_class)
+    roundtrip(test_class)
 
 
 @given(
     hnp.arrays(
         elements=strategies.floats(
             allow_nan=False, allow_infinity=False, width=32
         ),
@@ -131,55 +131,55 @@
         dtype=float,
     )
 )
 @settings(deadline=None)
 def test_with_floats(x):
     test_class = SimpleSaveableClass(x)
     _ = test_class.mult(2)
-    new_class = roundtrip(test_class)
+    roundtrip(test_class)
 
 
 @given(
     hnp.arrays(
         elements=strategies.integers(min_value=-100, max_value=100),
         shape=hnp.array_shapes(min_dims=1, max_dims=4),
         dtype=int,
     )
 )
 @settings(deadline=None)
 def test_with_ints(x):
     test_class = SimpleSaveableClass(x)
     _ = test_class.mult(2)
-    new_class = roundtrip(test_class)
+    roundtrip(test_class)
 
 
 @given(
     strategies.lists(
         strategies.floats(allow_nan=False, allow_infinity=False, width=32),
         min_size=1,
     )
 )
 @settings(deadline=None)
 def test_with_float_list(x):
     test_class = SimpleSaveableClass(x)
     _ = test_class.mult(2)
-    new_class = roundtrip(test_class)
+    roundtrip(test_class)
 
 
 @given(
     strategies.lists(
         strategies.integers(min_value=-100, max_value=100),
         min_size=1,
     )
 )
 @settings(deadline=None)
 def test_with_int_list(x):
     test_class = SimpleSaveableClass(x)
     _ = test_class.mult(2)
-    new_class = roundtrip(test_class)
+    roundtrip(test_class)
 
 
 # Lists of attributes required for different types of objects
 req_class_attrs = [
     "module",
     "class",
     "timestamp",
```

### Comparing `prepper-1.2.2/prepper/tests/test_decorators.py` & `prepper-1.2.3/prepper/tests/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,20 +77,19 @@
             api_version="0.0.1",
             attributes=["test_int", "test_string"],
             functions=["square"],
         ),
     ]
     pytest.raises(ValueError, decorator, NotASaveableClass)
     decorated = decorator(SimpleSaveableClass)
-    assert decorated._exportable_functions == set(
-        ["SimpleSaveableClass.square"]
-    )
-    assert decorated._exportable_attributes == set(
-        ["SimpleSaveableClass.test_string"]
-    )
+    assert decorated._exportable_functions == ["SimpleSaveableClass.square"]
+    assert decorated._exportable_attributes == [
+        "SimpleSaveableClass.test_string"
+    ]
+
     for d in bad_decorators:
         pytest.raises(ValueError, d, SimpleSaveableClass)
 
 
 def test_cached_property():
     test_class = SimpleSaveableClass2()
```

### Comparing `prepper-1.2.2/pyproject.toml` & `prepper-1.2.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 [build-system]
 requires = ["setuptools >= 67.0.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "prepper/_version.py"
 
+[tool.setuptools.packages.find]
+exclude = ["typings*"]
+
+[tool.ruff]
+line-length = 79
+target-version = "py311"
+ignore = ["E501"]
+exclude = ["**/*.pyi"]
+[tool.ruff.isort]
+force-sort-within-sections = true
+required-imports = ["from __future__ import annotations"]
 
 [tool.black]
 line-length = 79
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
@@ -73,7 +84,23 @@
 missing-class-docstring,
 too-many-locals,
 redefined-builtin,
 too-few-public-methods,
 global-statement
 """
 ignore = "tests"
+
+[tool.pyright]
+pythonVersion = "3.11"
+pythonPlatform = "Linux"
+stubPath = "typings"
+typeCheckingMode = "basic"
+reportUnusedImport = "none"
+reportUnusedClass = "none"
+reportUnusedFunction = "none"
+reportUnusedVariable = "none"
+reportDuplicateImport = "none"
+reportPrivateImportUsage = "none"
+reportUntypedFunctionDecorator = true
+reportUntypedClassDecorator = true
+reportMissingImports = false
+exclude = ["install*", "public*", "**/tests*", "**/resources*"]
```

