# Comparing `tmp/helptasker_common-0.0.2.tar.gz` & `tmp/helptasker_common-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helptasker_common-0.0.2.tar", max compression
+gzip compressed data, was "helptasker_common-0.0.3.tar", max compression
```

## Comparing `helptasker_common-0.0.2.tar` & `helptasker_common-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/LICENSE
--rw-r--r--   0        0        0      344 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/README.md
--rw-r--r--   0        0        0       22 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/__init__.py
--rw-r--r--   0        0        0      172 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/context.py
--rw-r--r--   0        0        0     2833 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/http_base_client.py
--rw-r--r--   0        0        0      389 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/instrumentation.py
--rw-r--r--   0        0        0     1774 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/logger.py
--rw-r--r--   0        0        0     4258 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/middlewares.py
--rw-r--r--   0        0        0        0 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/py.typed
--rw-r--r--   0        0        0     1790 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/settings.py
--rw-r--r--   0        0        0     1759 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/helptasker_common/trace.py
--rw-r--r--   0        0        0     2915 2023-07-19 19:39:16.780173 helptasker_common-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 helptasker_common-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/LICENSE
+-rw-r--r--   0        0        0      344 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/context.py
+-rw-r--r--   0        0        0     2833 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/http_base_client.py
+-rw-r--r--   0        0        0     1813 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/instrumentation.py
+-rw-r--r--   0        0        0     1774 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/logger.py
+-rw-r--r--   0        0        0     4258 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/middlewares.py
+-rw-r--r--   0        0        0        0 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/py.typed
+-rw-r--r--   0        0        0     1790 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/settings.py
+-rw-r--r--   0        0        0     1759 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/helptasker_common/trace.py
+-rw-r--r--   0        0        0     2915 2023-07-20 08:14:33.112605 helptasker_common-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 helptasker_common-0.0.3/PKG-INFO
```

### Comparing `helptasker_common-0.0.2/LICENSE` & `helptasker_common-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.0.2/helptasker_common/http_base_client.py` & `helptasker_common-0.0.3/helptasker_common/http_base_client.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.0.2/helptasker_common/logger.py` & `helptasker_common-0.0.3/helptasker_common/logger.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.0.2/helptasker_common/middlewares.py` & `helptasker_common-0.0.3/helptasker_common/middlewares.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.0.2/helptasker_common/settings.py` & `helptasker_common-0.0.3/helptasker_common/settings.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.0.2/helptasker_common/trace.py` & `helptasker_common-0.0.3/helptasker_common/trace.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.0.2/pyproject.toml` & `helptasker_common-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "helptasker-common"
-version = "0.0.2"
+version = "0.0.3"
 description = "Shared Library"
 authors = [
     "Kostya Ten <kostya@yandex.com>"
 ]
 repository = "https://github.com/helptasker/common/"
 keywords = ["fastapi", "pydantic", "asyncio"]
 homepage = "https://github.com/helptasker/common/"
```

### Comparing `helptasker_common-0.0.2/PKG-INFO` & `helptasker_common-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helptasker-common
-Version: 0.0.2
+Version: 0.0.3
 Summary: Shared Library
 Home-page: https://github.com/helptasker/common/
 Keywords: fastapi,pydantic,asyncio
 Author: Kostya Ten
 Author-email: kostya@yandex.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

