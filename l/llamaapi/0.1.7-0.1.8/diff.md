# Comparing `tmp/llamaapi-0.1.7.tar.gz` & `tmp/llamaapi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llamaapi-0.1.7.tar", max compression
+gzip compressed data, was "llamaapi-0.1.8.tar", max compression
```

## Comparing `llamaapi-0.1.7.tar` & `llamaapi-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.7/LICENSE
--rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.7/README.md
--rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.7/llamaapi/__init__.py
--rw-r--r--   0        0        0     1766 2023-07-20 20:40:31.490801 llamaapi-0.1.7/llamaapi/llamaapi.py
--rw-r--r--   0        0        0      368 2023-07-20 20:40:35.659802 llamaapi-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-20 16:25:58.963474 llamaapi-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1901 2023-07-20 16:44:53.762559 llamaapi-0.1.8/README.md
+-rw-r--r--   0        0        0       70 2023-07-20 17:01:27.580634 llamaapi-0.1.8/llamaapi/__init__.py
+-rw-r--r--   0        0        0     1842 2023-07-20 21:06:53.583921 llamaapi-0.1.8/llamaapi/llamaapi.py
+-rw-r--r--   0        0        0      368 2023-07-20 21:12:19.392945 llamaapi-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2500 1970-01-01 00:00:00.000000 llamaapi-0.1.8/PKG-INFO
```

### Comparing `llamaapi-0.1.7/LICENSE` & `llamaapi-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.7/README.md` & `llamaapi-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `llamaapi-0.1.7/PKG-INFO` & `llamaapi-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llamaapi
-Version: 0.1.7
+Version: 0.1.8
 Summary: Llama API python SDK
 License: MIT
 Author: Eduardo Reis
 Author-email: edu.pontes@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

