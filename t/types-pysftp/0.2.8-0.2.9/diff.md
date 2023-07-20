# Comparing `tmp/types-pysftp-0.2.8.tar.gz` & `tmp/types-pysftp-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pysftp-0.2.8.tar", last modified: Sat Jan  8 15:20:12 2022, max compression
+gzip compressed data, was "types-pysftp-0.2.9.tar", last modified: Sun Jan 16 18:21:14 2022, max compression
```

## Comparing `types-pysftp-0.2.8.tar` & `types-pysftp-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:12.483269 types-pysftp-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-01-08 15:20:11.000000 types-pysftp-0.2.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-08 15:20:11.000000 types-pysftp-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-01-08 15:20:12.483269 types-pysftp-0.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:12.483269 types-pysftp-0.2.8/pysftp-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-08 15:20:11.000000 types-pysftp-0.2.8/pysftp-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5388 2022-01-08 15:18:10.000000 types-pysftp-0.2.8/pysftp-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-01-08 15:18:10.000000 types-pysftp-0.2.8/pysftp-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-01-08 15:18:10.000000 types-pysftp-0.2.8/pysftp-stubs/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-08 15:20:12.483269 types-pysftp-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-01-08 15:20:11.000000 types-pysftp-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:20:12.483269 types-pysftp-0.2.8/types_pysftp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-01-08 15:20:12.000000 types-pysftp-0.2.8/types_pysftp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-01-08 15:20:12.000000 types-pysftp-0.2.8/types_pysftp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-08 15:20:12.000000 types-pysftp-0.2.8/types_pysftp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-08 15:20:12.000000 types-pysftp-0.2.8/types_pysftp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-08 15:20:12.000000 types-pysftp-0.2.8/types_pysftp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 18:21:14.679987 types-pysftp-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-01-16 18:21:14.679987 types-pysftp-0.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 18:21:14.679987 types-pysftp-0.2.9/pysftp-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/pysftp-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     5413 2022-01-16 18:20:48.000000 types-pysftp-0.2.9/pysftp-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-01-16 18:20:48.000000 types-pysftp-0.2.9/pysftp-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-01-16 18:20:48.000000 types-pysftp-0.2.9/pysftp-stubs/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-16 18:21:14.679987 types-pysftp-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-16 18:21:14.679987 types-pysftp-0.2.9/types_pysftp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      853 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/types_pysftp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/types_pysftp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/types_pysftp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/types_pysftp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-01-16 18:21:14.000000 types-pysftp-0.2.9/types_pysftp.egg-info/top_level.txt
```

### Comparing `types-pysftp-0.2.8/PKG-INFO` & `types-pysftp-0.2.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pysftp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Typing stubs for pysftp
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `pysftp` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `pysftp`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/pysftp. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
+This package was generated from typeshed commit `85318d1b215a32825fd4ecb7fa6466fe75f7c428`.
```

### Comparing `types-pysftp-0.2.8/pysftp-stubs/__init__.pyi` & `types-pysftp-0.2.9/pysftp-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from _typeshed import Self
 from stat import S_IMODE as S_IMODE
 from types import TracebackType
 from typing import IO, Any, Callable, ContextManager, Sequence, Text, Union
 from typing_extensions import Literal
 
 import paramiko
 from paramiko import AuthenticationException as AuthenticationException
@@ -116,11 +117,11 @@
     @property
     def timeout(self) -> float | None: ...
     @timeout.setter
     def timeout(self, val: float | None) -> None: ...
     @property
     def remote_server_key(self) -> paramiko.PKey: ...
     def __del__(self) -> None: ...
-    def __enter__(self) -> "Connection": ...
+    def __enter__(self: Self) -> Self: ...
     def __exit__(
         self, etype: type[BaseException] | None, value: BaseException | None, traceback: TracebackType | None
     ) -> None: ...
```

### Comparing `types-pysftp-0.2.8/pysftp-stubs/helpers.pyi` & `types-pysftp-0.2.9/pysftp-stubs/helpers.pyi`

 * *Files identical despite different names*

### Comparing `types-pysftp-0.2.8/setup.py` & `types-pysftp-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `pysftp` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `pysftp`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/pysftp. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
+This package was generated from typeshed commit `85318d1b215a32825fd4ecb7fa6466fe75f7c428`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.2.8",
+      version="0.2.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=['types-paramiko'],
       packages=['pysftp-stubs'],
       package_data={'pysftp-stubs': ['__init__.pyi', 'exceptions.pyi', 'helpers.pyi', 'METADATA.toml']},
```

### Comparing `types-pysftp-0.2.8/types_pysftp.egg-info/PKG-INFO` & `types-pysftp-0.2.9/types_pysftp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pysftp
-Version: 0.2.8
+Version: 0.2.9
 Summary: Typing stubs for pysftp
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `pysftp` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `pysftp`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/pysftp. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
+This package was generated from typeshed commit `85318d1b215a32825fd4ecb7fa6466fe75f7c428`.
```

