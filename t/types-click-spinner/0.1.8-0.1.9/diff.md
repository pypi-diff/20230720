# Comparing `tmp/types-click-spinner-0.1.8.tar.gz` & `tmp/types-click-spinner-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-click-spinner-0.1.8.tar", last modified: Fri Jan  7 11:29:16 2022, max compression
+gzip compressed data, was "types-click-spinner-0.1.9.tar", last modified: Sat Jan  8 15:18:57 2022, max compression
```

## Comparing `types-click-spinner-0.1.8.tar` & `types-click-spinner-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:29:16.592405 types-click-spinner-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-01-07 11:29:16.592405 types-click-spinner-0.1.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:29:16.592405 types-click-spinner-0.1.8/click_spinner-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/click_spinner-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-01-07 11:27:57.000000 types-click-spinner-0.1.8/click_spinner-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-07 11:29:16.592405 types-click-spinner-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-07 11:29:16.592405 types-click-spinner-0.1.8/types_click_spinner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/types_click_spinner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/types_click_spinner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/types_click_spinner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-07 11:29:16.000000 types-click-spinner-0.1.8/types_click_spinner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:18:57.614848 types-click-spinner-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-01-08 15:18:57.614848 types-click-spinner-0.1.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:18:57.610848 types-click-spinner-0.1.9/click_spinner-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/click_spinner-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      964 2022-01-08 15:18:10.000000 types-click-spinner-0.1.9/click_spinner-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-08 15:18:57.614848 types-click-spinner-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-08 15:18:57.614848 types-click-spinner-0.1.9/types_click_spinner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      895 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/types_click_spinner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/types_click_spinner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/types_click_spinner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-01-08 15:18:57.000000 types-click-spinner-0.1.9/types_click_spinner.egg-info/top_level.txt
```

### Comparing `types-click-spinner-0.1.8/PKG-INFO` & `types-click-spinner-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-click-spinner
-Version: 0.1.8
+Version: 0.1.9
 Summary: Typing stubs for click-spinner
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `click-spinner` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `click-spinner`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/click-spinner. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
```

### Comparing `types-click-spinner-0.1.8/click_spinner-stubs/__init__.pyi` & `types-click-spinner-0.1.9/click_spinner-stubs/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import threading
 from types import TracebackType
-from typing import Iterator, Protocol, Type
+from typing import Iterator, Protocol
 from typing_extensions import Literal
 
 __version__: str
 
 class _Stream(Protocol):
     def isatty(self) -> bool: ...
     def flush(self) -> None: ...
@@ -20,11 +20,11 @@
     spin_thread: threading.Thread | None
     def __init__(self, beep: bool, disable: bool, force: bool, stream: _Stream) -> None: ...
     def start(self) -> None: ...
     def stop(self) -> None: ...
     def init_spin(self) -> None: ...
     def __enter__(self) -> Spinner: ...
     def __exit__(
-        self, exc_type: Type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None
+        self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None
     ) -> Literal[False]: ...
 
 def spinner(beep: bool, disable: bool, force: bool, stream: _Stream) -> Spinner: ...
```

### Comparing `types-click-spinner-0.1.8/setup.py` & `types-click-spinner-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `click-spinner` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `click-spinner`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/click-spinner. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.1.8",
+      version="0.1.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       install_requires=[],
       packages=['click_spinner-stubs'],
       package_data={'click_spinner-stubs': ['__init__.pyi', 'METADATA.toml']},
```

### Comparing `types-click-spinner-0.1.8/types_click_spinner.egg-info/PKG-INFO` & `types-click-spinner-0.1.9/types_click_spinner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-click-spinner
-Version: 0.1.8
+Version: 0.1.9
 Summary: Typing stubs for click-spinner
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
@@ -14,10 +14,10 @@
 This is a PEP 561 type stub package for the `click-spinner` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `click-spinner`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/click-spinner. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `032e6ee90cbb938259a2aa2183966502de19108e`.
+This package was generated from typeshed commit `a40d79a4e63c4e750a8d3a8012305da942251eb4`.
```

