# Comparing `tmp/types-psycopg2-2.9.8.tar.gz` & `tmp/types-psycopg2-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-psycopg2-2.9.8.tar", last modified: Tue Mar  8 18:21:08 2022, max compression
+gzip compressed data, was "types-psycopg2-2.9.9.tar", last modified: Wed Mar 16 06:22:04 2022, max compression
```

## Comparing `types-psycopg2-2.9.8.tar` & `types-psycopg2-2.9.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 18:21:08.618368 types-psycopg2-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-03-08 18:21:07.000000 types-psycopg2-2.9.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-08 18:21:07.000000 types-psycopg2-2.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-03-08 18:21:08.618368 types-psycopg2-2.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 18:21:08.618368 types-psycopg2-2.9.8/psycopg2-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-03-08 18:21:07.000000 types-psycopg2-2.9.8/psycopg2-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/_ipaddress.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      750 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/_json.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11894 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/_psycopg.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/_range.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9308 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/errorcodes.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12762 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/extensions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/extras.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/pool.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/sql.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-03-08 18:20:56.000000 types-psycopg2-2.9.8/psycopg2-stubs/tz.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-08 18:21:08.618368 types-psycopg2-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-03-08 18:21:07.000000 types-psycopg2-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-08 18:21:08.618368 types-psycopg2-2.9.8/types_psycopg2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-03-08 18:21:08.000000 types-psycopg2-2.9.8/types_psycopg2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      532 2022-03-08 18:21:08.000000 types-psycopg2-2.9.8/types_psycopg2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-08 18:21:08.000000 types-psycopg2-2.9.8/types_psycopg2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-08 18:21:08.000000 types-psycopg2-2.9.8/types_psycopg2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 06:22:04.192680 types-psycopg2-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1008 2022-03-16 06:22:03.000000 types-psycopg2-2.9.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-03-16 06:22:03.000000 types-psycopg2-2.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-03-16 06:22:04.192680 types-psycopg2-2.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 06:22:04.192680 types-psycopg2-2.9.9/psycopg2-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-03-16 06:22:03.000000 types-psycopg2-2.9.9/psycopg2-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     1100 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      236 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/_ipaddress.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      750 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/_json.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    11982 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/_psycopg.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1621 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/_range.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     9308 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/errorcodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)    12762 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/extensions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     6009 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/extras.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/pool.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/sql.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2022-03-16 06:21:52.000000 types-psycopg2-2.9.9/psycopg2-stubs/tz.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-16 06:22:04.192680 types-psycopg2-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-03-16 06:22:03.000000 types-psycopg2-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 06:22:04.192680 types-psycopg2-2.9.9/types_psycopg2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-03-16 06:22:04.000000 types-psycopg2-2.9.9/types_psycopg2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      532 2022-03-16 06:22:04.000000 types-psycopg2-2.9.9/types_psycopg2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 06:22:04.000000 types-psycopg2-2.9.9/types_psycopg2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-16 06:22:04.000000 types-psycopg2-2.9.9/types_psycopg2.egg-info/top_level.txt
```

### Comparing `types-psycopg2-2.9.8/PKG-INFO` & `types-psycopg2-2.9.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-psycopg2
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for psycopg2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/psycopg2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `psycopg2` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `psycopg2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/psycopg2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `889164cb0c15f2ba9b57ad0154f0986bd22b9b87`.
+This package was generated from typeshed commit `b78f0c21bacd73fb1c7b588508146405fd08e169`.
```

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/__init__.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/_json.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/_json.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/_psycopg.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/_psycopg.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from _typeshed import Self
 from collections.abc import Callable, Iterable, Mapping, Sequence
 from types import TracebackType
 from typing import Any, TypeVar, overload
 
 import psycopg2
 import psycopg2.extensions
+from psycopg2.sql import Composable
 
 _Vars = Sequence[Any] | Mapping[str, Any] | None
 
 BINARY: Any
 BINARYARRAY: Any
 BOOLEAN: Any
 BOOLEANARRAY: Any
@@ -356,19 +357,19 @@
     typecaster: Any
     tzinfo_factory: Any
     withhold: Any
     def __init__(self, *args, **kwargs) -> None: ...
     def callproc(self, procname, parameters=...): ...
     def cast(self, oid, s): ...
     def close(self): ...
-    def copy_expert(self, sql, file, size=...): ...
+    def copy_expert(self, sql: str | bytes | Composable, file, size=...): ...
     def copy_from(self, file, table, sep=..., null=..., size=..., columns=...): ...
     def copy_to(self, file, table, sep=..., null=..., columns=...): ...
-    def execute(self, query: str | bytes, vars: _Vars = ...) -> None: ...
-    def executemany(self, query: str | bytes, vars_list: Iterable[_Vars]) -> None: ...
+    def execute(self, query: str | bytes | Composable, vars: _Vars = ...) -> None: ...
+    def executemany(self, query: str | bytes | Composable, vars_list: Iterable[_Vars]) -> None: ...
     def fetchall(self) -> list[tuple[Any, ...]]: ...
     def fetchmany(self, size=...) -> list[tuple[Any, ...]]: ...
     def fetchone(self) -> tuple[Any, ...] | Any: ...
     def mogrify(self, *args, **kwargs): ...
     def nextset(self): ...
     def scroll(self, value, mode=...): ...
     def setinputsizes(self, sizes): ...
```

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/_range.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/_range.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/errorcodes.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/errorcodes.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/errors.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/extensions.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/extensions.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/extras.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/extras.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/pool.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/pool.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/sql.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/sql.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/psycopg2-stubs/tz.pyi` & `types-psycopg2-2.9.9/psycopg2-stubs/tz.pyi`

 * *Files identical despite different names*

### Comparing `types-psycopg2-2.9.8/setup.py` & `types-psycopg2-2.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `psycopg2` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `psycopg2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/psycopg2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `889164cb0c15f2ba9b57ad0154f0986bd22b9b87`.
+This package was generated from typeshed commit `b78f0c21bacd73fb1c7b588508146405fd08e169`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.9.8",
+      version="2.9.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/psycopg2.md",
```

### Comparing `types-psycopg2-2.9.8/types_psycopg2.egg-info/PKG-INFO` & `types-psycopg2-2.9.9/types_psycopg2.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-psycopg2
-Version: 2.9.8
+Version: 2.9.9
 Summary: Typing stubs for psycopg2
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/psycopg2.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -18,10 +18,10 @@
 This is a PEP 561 type stub package for the `psycopg2` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `psycopg2`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/psycopg2. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `889164cb0c15f2ba9b57ad0154f0986bd22b9b87`.
+This package was generated from typeshed commit `b78f0c21bacd73fb1c7b588508146405fd08e169`.
```

### Comparing `types-psycopg2-2.9.8/types_psycopg2.egg-info/SOURCES.txt` & `types-psycopg2-2.9.9/types_psycopg2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

