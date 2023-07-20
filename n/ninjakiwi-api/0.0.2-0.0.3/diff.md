# Comparing `tmp/ninjakiwi_api-0.0.2.tar.gz` & `tmp/ninjakiwi_api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjakiwi_api-0.0.2.tar", max compression
+gzip compressed data, was "ninjakiwi_api-0.0.3.tar", max compression
```

## Comparing `ninjakiwi_api-0.0.2.tar` & `ninjakiwi_api-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.2/LICENSE
--rw-r--r--   0        0        0      229 2023-07-20 10:17:22.489408 ninjakiwi_api-0.0.2/README.md
--rw-r--r--   0        0        0       83 2023-07-19 19:59:45.011619 ninjakiwi_api-0.0.2/ninjakiwi_api/API/BTD6/__init__.py
--rw-r--r--   0        0        0     2995 2023-07-19 21:02:28.521583 ninjakiwi_api-0.0.2/ninjakiwi_api/API/BTD6/function.py
--rw-r--r--   0        0        0       84 2023-07-19 20:22:35.650851 ninjakiwi_api-0.0.2/ninjakiwi_api/API/BTDB2/__init__.py
--rw-r--r--   0        0        0     1083 2023-07-19 21:46:09.966399 ninjakiwi_api-0.0.2/ninjakiwi_api/API/BTDB2/function.py
--rw-r--r--   0        0        0      149 2023-07-19 20:22:35.654184 ninjakiwi_api-0.0.2/ninjakiwi_api/API/__init__.py
--rw-r--r--   0        0        0       85 2023-07-19 19:24:51.057767 ninjakiwi_api-0.0.2/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-19 21:02:36.858446 ninjakiwi_api-0.0.2/ninjakiwi_api/FUNCTIONS/ERROR/function.py
--rw-r--r--   0        0        0       81 2023-07-19 17:03:25.664468 ninjakiwi_api-0.0.2/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
--rw-r--r--   0        0        0      486 2023-07-19 21:02:28.548250 ninjakiwi_api-0.0.2/ninjakiwi_api/FUNCTIONS/FETCH/function.py
--rw-r--r--   0        0        0       91 2023-07-19 19:50:16.262880 ninjakiwi_api-0.0.2/ninjakiwi_api/FUNCTIONS/__init__.py
--rw-r--r--   0        0        0      240 2023-07-19 21:03:11.849270 ninjakiwi_api-0.0.2/ninjakiwi_api/__init__.py
--rw-r--r--   0        0        0      748 2023-07-19 21:02:28.518250 ninjakiwi_api-0.0.2/ninjakiwi_api/main.py
--rw-r--r--   0        0        0     2641 2023-07-20 10:17:50.500110 ninjakiwi_api-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      526 2023-07-19 21:43:29.909004 ninjakiwi_api-0.0.2/tests/test_main.py
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-19 16:03:17.395151 ninjakiwi_api-0.0.3/LICENSE
+-rw-r--r--   0        0        0      229 2023-07-20 10:17:22.489408 ninjakiwi_api-0.0.3/README.md
+-rw-r--r--   0        0        0       83 2023-07-19 19:59:45.011619 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTD6/__init__.py
+-rw-r--r--   0        0        0     2995 2023-07-19 21:02:28.521583 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTD6/function.py
+-rw-r--r--   0        0        0       84 2023-07-19 20:22:35.650851 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTDB2/__init__.py
+-rw-r--r--   0        0        0     1083 2023-07-19 21:46:09.966399 ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTDB2/function.py
+-rw-r--r--   0        0        0      149 2023-07-19 20:22:35.654184 ninjakiwi_api-0.0.3/ninjakiwi_api/API/__init__.py
+-rw-r--r--   0        0        0      116 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/ERROR/__init__.py
+-rw-r--r--   0        0        0     1807 2023-07-20 10:44:10.487649 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/ERROR/function.py
+-rw-r--r--   0        0        0      108 2023-07-20 10:45:23.339278 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/FETCH/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-20 10:45:03.488833 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/FETCH/function.py
+-rw-r--r--   0        0        0      135 2023-07-20 10:45:23.342612 ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-20 10:44:10.497649 ninjakiwi_api-0.0.3/ninjakiwi_api/__init__.py
+-rw-r--r--   0        0        0     2830 2023-07-20 10:44:10.477649 ninjakiwi_api-0.0.3/ninjakiwi_api/main.py
+-rw-r--r--   0        0        0     2641 2023-07-20 10:45:40.236325 ninjakiwi_api-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-07-19 16:03:17.421818 ninjakiwi_api-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      526 2023-07-19 21:43:29.909004 ninjakiwi_api-0.0.3/tests/test_main.py
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 ninjakiwi_api-0.0.3/PKG-INFO
```

### Comparing `ninjakiwi_api-0.0.2/LICENSE` & `ninjakiwi_api-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.2/ninjakiwi_api/API/BTD6/function.py` & `ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTD6/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.2/ninjakiwi_api/API/BTDB2/function.py` & `ninjakiwi_api-0.0.3/ninjakiwi_api/API/BTDB2/function.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.2/ninjakiwi_api/FUNCTIONS/ERROR/function.py` & `ninjakiwi_api-0.0.3/ninjakiwi_api/FUNCTIONS/ERROR/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """FUNCTION-level package for NinjaKiwi API."""
 
 from aiohttp import ClientResponse
 
 
-async def error_handler(
+async def _error_handler(
     act: str, response: ClientResponse = None, exception: str = None
 ) -> None:
 
     err = None
 
     if act == "http":
         if response is not None:
```

### Comparing `ninjakiwi_api-0.0.2/pyproject.toml` & `ninjakiwi_api-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "ninjakiwi_api"
-version = "0.0.2"
+version = "0.0.3"
 homepage = "https://github.com/GustavoSchip/ninjakiwi_api"
 description = "Skeleton project created by Python Project Wizard (ppw)."
 authors = ["Gustavo Schip <gustavoschip@proton.me>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `ninjakiwi_api-0.0.2/tests/test_main.py` & `ninjakiwi_api-0.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `ninjakiwi_api-0.0.2/PKG-INFO` & `ninjakiwi_api-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjakiwi-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Skeleton project created by Python Project Wizard (ppw).
 Home-page: https://github.com/GustavoSchip/ninjakiwi_api
 License: MIT
 Author: Gustavo Schip
 Author-email: gustavoschip@proton.me
 Requires-Python: >=3.11,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ninjakiwi-api Version: 0.0.2 Summary: Skeleton
+Metadata-Version: 2.1 Name: ninjakiwi-api Version: 0.0.3 Summary: Skeleton
 project created by Python Project Wizard (ppw). Home-page: https://github.com/
 GustavoSchip/ninjakiwi_api License: MIT Author: Gustavo Schip Author-email:
 gustavoschip@proton.me Requires-Python: >=3.11,<4.0.0 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.11 Provides-Extra: dev Provides-Extra: doc Provides-
```

