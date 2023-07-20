# Comparing `tmp/llamaapi-0.1.5.tar.gz` & `tmp/llamaapi-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamaapi-0.1.5.tar", max compression
+gzip compressed data, was "llamaapi-0.1.6.tar", max compression
```

## Comparing `llamaapi-0.1.5.tar` & `llamaapi-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.5/LICENSE
--rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.5/README.md
--rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.5/llamaapi/__init__.py
--rw-r--r--   0        0        0     1385 2023-07-20 18:05:40.153925 llamaapi-0.1.5/llamaapi/llamaapi.py
--rw-r--r--   0        0        0      368 2023-07-20 18:05:49.342925 llamaapi-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.6/README.md
+-rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.6/llamaapi/__init__.py
+-rw-r--r--   0        0        0     1282 2023-07-20 20:35:21.052778 llamaapi-0.1.6/llamaapi/llamaapi.py
+-rw-r--r--   0        0        0      368 2023-07-20 20:35:29.372779 llamaapi-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.6/PKG-INFO
```

### Comparing `llamaapi-0.1.5/LICENSE` & `llamaapi-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.5/README.md` & `llamaapi-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.5/PKG-INFO` & `llamaapi-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamaapi
-Version: 0.1.5
+Version: 0.1.6
 Summary: Llama API python SDK
 License: MIT
 Author: Eduardo Reis
 Author-email: edu.pontes@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

