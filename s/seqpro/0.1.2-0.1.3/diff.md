# Comparing `tmp/seqpro-0.1.2.tar.gz` & `tmp/seqpro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqpro-0.1.2.tar", max compression
+gzip compressed data, was "seqpro-0.1.3.tar", max compression
```

## Comparing `seqpro-0.1.2.tar` & `seqpro-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1066 2023-07-20 18:52:35.000000 seqpro-0.1.2/LICENSE
--rw-r--r--   0        0        0      543 2023-07-20 19:49:51.000000 seqpro-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      977 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/__init__.py
--rw-r--r--   0        0        0     5455 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_analyzers.py
--rw-r--r--   0        0        0     1276 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_cleaners.py
--rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.2/seqpro/_comparisons.py
--rw-r--r--   0        0        0     5098 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_encoders.py
--rw-r--r--   0        0        0     6926 2023-07-20 18:32:36.000000 seqpro-0.1.2/seqpro/_modifiers.py
--rw-r--r--   0        0        0     3535 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_numba.py
--rw-r--r--   0        0        0     3810 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/_utils.py
--rw-r--r--   0        0        0     1458 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/alphabets/__init__.py
--rw-r--r--   0        0        0     8278 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/alphabets/_alphabets.py
--rw-r--r--   0        0        0     2504 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_analyzers.py
--rw-r--r--   0        0        0     1358 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_cleaners.py
--rw-r--r--   0        0        0     4364 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_encoders.py
--rw-r--r--   0        0        0     9481 2023-07-20 18:31:57.000000 seqpro-0.1.2/seqpro/deprecated/_helpers.py
--rw-r--r--   0        0        0     6113 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_modifiers.py
--rw-r--r--   0        0        0     1419 2023-07-20 18:31:56.000000 seqpro-0.1.2/seqpro/deprecated/_utils.py
--rw-r--r--   0        0        0     2914 2023-07-20 18:52:06.000000 seqpro-0.1.2/seqpro/experimental/_experimental.py
--rw-r--r--   0        0        0      773 2023-07-20 18:31:57.000000 seqpro-0.1.2/seqpro/experimental/_visualizers.py
--rw-r--r--   0        0        0     6198 2023-07-20 18:31:57.000000 seqpro-0.1.2/seqpro/xr/__init__.py
--rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 seqpro-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-07-20 18:52:35.000000 seqpro-0.1.3/LICENSE
+-rw-r--r--   0        0        0      543 2023-07-20 19:52:15.000000 seqpro-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      977 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/__init__.py
+-rw-r--r--   0        0        0     5455 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/_analyzers.py
+-rw-r--r--   0        0        0     1276 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/_cleaners.py
+-rw-r--r--   0        0        0        0 2023-03-30 18:14:39.000000 seqpro-0.1.3/seqpro/_comparisons.py
+-rw-r--r--   0        0        0     5098 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/_encoders.py
+-rw-r--r--   0        0        0     6926 2023-07-20 18:32:36.000000 seqpro-0.1.3/seqpro/_modifiers.py
+-rw-r--r--   0        0        0     3535 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/_numba.py
+-rw-r--r--   0        0        0     3810 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/_utils.py
+-rw-r--r--   0        0        0     1458 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/alphabets/__init__.py
+-rw-r--r--   0        0        0     8278 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/alphabets/_alphabets.py
+-rw-r--r--   0        0        0     2504 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/deprecated/_analyzers.py
+-rw-r--r--   0        0        0     1358 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/deprecated/_cleaners.py
+-rw-r--r--   0        0        0     4364 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/deprecated/_encoders.py
+-rw-r--r--   0        0        0     9481 2023-07-20 18:31:57.000000 seqpro-0.1.3/seqpro/deprecated/_helpers.py
+-rw-r--r--   0        0        0     6113 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/deprecated/_modifiers.py
+-rw-r--r--   0        0        0     1419 2023-07-20 18:31:56.000000 seqpro-0.1.3/seqpro/deprecated/_utils.py
+-rw-r--r--   0        0        0     2914 2023-07-20 18:52:06.000000 seqpro-0.1.3/seqpro/experimental/_experimental.py
+-rw-r--r--   0        0        0      773 2023-07-20 18:31:57.000000 seqpro-0.1.3/seqpro/experimental/_visualizers.py
+-rw-r--r--   0        0        0     6198 2023-07-20 18:31:57.000000 seqpro-0.1.3/seqpro/xr/__init__.py
+-rw-r--r--   0        0        0      619 1970-01-01 00:00:00.000000 seqpro-0.1.3/PKG-INFO
```

### Comparing `seqpro-0.1.2/LICENSE` & `seqpro-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/pyproject.toml` & `seqpro-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seqpro"
-version = "0.1.2"
+version = "0.1.3"
 description = "Sequence processing toolkit"
 authors = ["Adam Klie <aklie@ucsd.edu>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numba = "^0.57.0"
 numpy = "~1.23.5"
```

### Comparing `seqpro-0.1.2/seqpro/__init__.py` & `seqpro-0.1.3/seqpro/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/_analyzers.py` & `seqpro-0.1.3/seqpro/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/_cleaners.py` & `seqpro-0.1.3/seqpro/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/_encoders.py` & `seqpro-0.1.3/seqpro/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/_modifiers.py` & `seqpro-0.1.3/seqpro/_modifiers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/_numba.py` & `seqpro-0.1.3/seqpro/_numba.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/_utils.py` & `seqpro-0.1.3/seqpro/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/alphabets/__init__.py` & `seqpro-0.1.3/seqpro/alphabets/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/alphabets/_alphabets.py` & `seqpro-0.1.3/seqpro/alphabets/_alphabets.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/deprecated/_analyzers.py` & `seqpro-0.1.3/seqpro/deprecated/_analyzers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/deprecated/_cleaners.py` & `seqpro-0.1.3/seqpro/deprecated/_cleaners.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/deprecated/_encoders.py` & `seqpro-0.1.3/seqpro/deprecated/_encoders.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/deprecated/_helpers.py` & `seqpro-0.1.3/seqpro/deprecated/_helpers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/deprecated/_modifiers.py` & `seqpro-0.1.3/seqpro/deprecated/_modifiers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/deprecated/_utils.py` & `seqpro-0.1.3/seqpro/deprecated/_utils.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/experimental/_experimental.py` & `seqpro-0.1.3/seqpro/experimental/_experimental.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/experimental/_visualizers.py` & `seqpro-0.1.3/seqpro/experimental/_visualizers.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/seqpro/xr/__init__.py` & `seqpro-0.1.3/seqpro/xr/__init__.py`

 * *Files identical despite different names*

### Comparing `seqpro-0.1.2/PKG-INFO` & `seqpro-0.1.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqpro
-Version: 0.1.2
+Version: 0.1.3
 Summary: Sequence processing toolkit
 Author: Adam Klie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

