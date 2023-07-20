# Comparing `tmp/async_interrupt-1.1.0.tar.gz` & `tmp/async_interrupt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_interrupt-1.1.0.tar", max compression
+gzip compressed data, was "async_interrupt-1.1.1.tar", max compression
```

## Comparing `async_interrupt-1.1.0.tar` & `async_interrupt-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11345 2023-07-20 16:39:35.240234 async_interrupt-1.1.0/LICENSE
--rw-r--r--   0        0        0     3757 2023-07-20 16:39:35.240234 async_interrupt-1.1.0/README.md
--rw-r--r--   0        0        0     1957 2023-07-20 16:39:36.380228 async_interrupt-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4245 2023-07-20 16:39:36.336228 async_interrupt-1.1.0/src/async_interrupt/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 16:39:35.240234 async_interrupt-1.1.0/src/async_interrupt/py.typed
--rw-r--r--   0        0        0     4862 1970-01-01 00:00:00.000000 async_interrupt-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-07-20 16:47:13.631719 async_interrupt-1.1.1/LICENSE
+-rw-r--r--   0        0        0     3757 2023-07-20 16:47:13.631719 async_interrupt-1.1.1/README.md
+-rw-r--r--   0        0        0     1984 2023-07-20 16:47:14.551731 async_interrupt-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4245 2023-07-20 16:47:14.515731 async_interrupt-1.1.1/src/async_interrupt/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 16:47:13.631719 async_interrupt-1.1.1/src/async_interrupt/py.typed
+-rw-r--r--   0        0        0     4812 1970-01-01 00:00:00.000000 async_interrupt-1.1.1/PKG-INFO
```

### Comparing `async_interrupt-1.1.0/LICENSE` & `async_interrupt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_interrupt-1.1.0/README.md` & `async_interrupt-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `async_interrupt-1.1.0/pyproject.toml` & `async_interrupt-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_interrupt"
-version = "1.1.0"
+version = "1.1.1"
 description = "Context manager to raise an exception when a future is done"
 authors = ["J. Nick Koston <nick@koston.org>"]
 license = "Apache Software License 2.0"
 readme = "README.md"
 repository = "https://github.com/bdraco/async_interrupt"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -18,19 +18,20 @@
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/bdraco/async_interrupt/issues"
 "Changelog" = "https://github.com/bdraco/async_interrupt/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0"
 pytest-cov = "^3.0"
+pytest-asyncio = "^0.21.1"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/async_interrupt/__init__.py:__version__"
 build_command = "pip install poetry && poetry build"
```

### Comparing `async_interrupt-1.1.0/src/async_interrupt/__init__.py` & `async_interrupt-1.1.1/src/async_interrupt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 from __future__ import annotations
 
 import asyncio
 from types import TracebackType
 from typing import TYPE_CHECKING, Any, final
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 
 __all__ = ("interrupt",)
 
 
 @final
 class _Interrupt:
     """Interrupt context manager.
```

### Comparing `async_interrupt-1.1.0/PKG-INFO` & `async_interrupt-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: async-interrupt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Context manager to raise an exception when a future is done
 Home-page: https://github.com/bdraco/async_interrupt
 License: Apache Software License 2.0
 Author: J. Nick Koston
 Author-email: nick@koston.org
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Project-URL: Bug Tracker, https://github.com/bdraco/async_interrupt/issues
 Project-URL: Changelog, https://github.com/bdraco/async_interrupt/blob/main/CHANGELOG.md
 Project-URL: Repository, https://github.com/bdraco/async_interrupt
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: async-interrupt Version: 1.1.0 Summary: Context
+Metadata-Version: 2.1 Name: async-interrupt Version: 1.1.1 Summary: Context
 manager to raise an exception when a future is done Home-page: https://
 github.com/bdraco/async_interrupt License: Apache Software License 2.0 Author:
-J. Nick Koston Author-email: nick@koston.org Requires-Python: >=3.8,<4.0
+J. Nick Koston Author-email: nick@koston.org Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: License :: Other/Proprietary License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Software Development ::
-Libraries Project-URL: Bug Tracker, https://github.com/bdraco/async_interrupt/
-issues Project-URL: Changelog, https://github.com/bdraco/async_interrupt/blob/
-main/CHANGELOG.md Project-URL: Repository, https://github.com/bdraco/
-async_interrupt Description-Content-Type: text/markdown # async_interrupt
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Software Development :: Libraries Project-URL: Bug Tracker, https://github.com/
+bdraco/async_interrupt/issues Project-URL: Changelog, https://github.com/
+bdraco/async_interrupt/blob/main/CHANGELOG.md Project-URL: Repository, https://
+github.com/bdraco/async_interrupt Description-Content-Type: text/markdown #
+async_interrupt
                     [CI_Status] [Test_coverage_percentage]
                          [Poetry] [black] [pre-commit]
              [PyPI_Version] [Supported Python versions] [License]
 Interrupt context manager for asyncio. This module provides a context manager
 that can be used to interrupt a block of code as soon as possible when a future
 is done. The purpose is to raise as soon as possible to avoid any race
 conditions. This is based loosely on async_timeout by Andrew Svetlov and
```

