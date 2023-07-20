# Comparing `tmp/llamaapi-0.1.3.tar.gz` & `tmp/llamaapi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamaapi-0.1.3.tar", max compression
+gzip compressed data, was "llamaapi-0.1.4.tar", max compression
```

## Comparing `llamaapi-0.1.3.tar` & `llamaapi-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.3/LICENSE
--rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.3/README.md
--rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.3/llamaapi/__init__.py
--rw-r--r--   0        0        0     1624 2023-07-20 17:36:40.114793 llamaapi-0.1.3/llamaapi/llamaapi.py
--rw-r--r--   0        0        0      344 2023-07-20 17:36:44.344794 llamaapi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 llamaapi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.4/README.md
+-rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.4/llamaapi/__init__.py
+-rw-r--r--   0        0        0     1430 2023-07-20 17:40:49.263812 llamaapi-0.1.4/llamaapi/llamaapi.py
+-rw-r--r--   0        0        0      368 2023-07-20 17:41:02.679813 llamaapi-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.4/PKG-INFO
```

### Comparing `llamaapi-0.1.3/LICENSE` & `llamaapi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.3/README.md` & `llamaapi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.3/PKG-INFO` & `llamaapi-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: llamaapi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Llama API python SDK
 License: MIT
 Author: Eduardo Reis
 Author-email: edu.pontes@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.5,<4.0.0)
+Requires-Dist: nest-asyncio (>=1.5.6,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaAPI SDK
 
 LlamaAPI is a Python SDK for interacting with the Llama API. It abstracts away the handling of aiohttp sessions and headers, allowing for a simplified interaction with the API.
```

