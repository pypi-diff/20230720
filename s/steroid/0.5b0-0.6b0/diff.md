# Comparing `tmp/steroid-0.5b0.tar.gz` & `tmp/steroid-0.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steroid-0.5b0.tar", max compression
+gzip compressed data, was "steroid-0.6b0.tar", max compression
```

## Comparing `steroid-0.5b0.tar` & `steroid-0.6b0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-07-20 14:49:56.441029 steroid-0.5b0/LICENSE
--rw-r--r--   0        0        0       69 2023-07-20 14:49:56.441029 steroid-0.5b0/README.md
--rw-r--r--   0        0        0      803 2023-07-20 14:50:24.742405 steroid-0.5b0/pyproject.toml
--rw-r--r--   0        0        0      164 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/__init__.py
--rw-r--r--   0        0        0     1689 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/app.py
--rw-r--r--   0        0        0     1112 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/controller.py
--rw-r--r--   0        0        0      971 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/logging.py
--rw-r--r--   0        0        0     1706 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/methods.py
--rw-r--r--   0        0        0     1808 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/middleware.py
--rw-r--r--   0        0        0      485 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/utils.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 steroid-0.5b0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-20 15:00:50.985429 steroid-0.6b0/LICENSE
+-rw-r--r--   0        0        0      199 2023-07-20 15:00:50.985429 steroid-0.6b0/README.md
+-rw-r--r--   0        0        0      803 2023-07-20 15:01:21.993691 steroid-0.6b0/pyproject.toml
+-rw-r--r--   0        0        0      164 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/__init__.py
+-rw-r--r--   0        0        0     1689 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/app.py
+-rw-r--r--   0        0        0     1112 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/controller.py
+-rw-r--r--   0        0        0      971 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/logging.py
+-rw-r--r--   0        0        0     1706 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/methods.py
+-rw-r--r--   0        0        0     1808 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/middleware.py
+-rw-r--r--   0        0        0      485 2023-07-20 15:00:50.985429 steroid-0.6b0/steroid/utils.py
+-rw-r--r--   0        0        0     1322 1970-01-01 00:00:00.000000 steroid-0.6b0/PKG-INFO
```

### Comparing `steroid-0.5b0/LICENSE` & `steroid-0.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `steroid-0.5b0/pyproject.toml` & `steroid-0.6b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "steroid"
-version = "v0.5b"
+version = "v0.6b"
 authors = [
   "Mohammed Al Ameen <ameenmohammed2311@gmail.com>"
 ]
 description = "Steroid"
 readme = "README.md"
 
 repository = "https://github.com/struckchure/steroid"
```

### Comparing `steroid-0.5b0/steroid/app.py` & `steroid-0.6b0/steroid/app.py`

 * *Files identical despite different names*

### Comparing `steroid-0.5b0/steroid/controller.py` & `steroid-0.6b0/steroid/controller.py`

 * *Files identical despite different names*

### Comparing `steroid-0.5b0/steroid/logging.py` & `steroid-0.6b0/steroid/logging.py`

 * *Files identical despite different names*

### Comparing `steroid-0.5b0/steroid/methods.py` & `steroid-0.6b0/steroid/methods.py`

 * *Files identical despite different names*

### Comparing `steroid-0.5b0/steroid/middleware.py` & `steroid-0.6b0/steroid/middleware.py`

 * *Files identical despite different names*

### Comparing `steroid-0.5b0/PKG-INFO` & `steroid-0.6b0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steroid
-Version: 0.5b0
+Version: 0.6b0
 Summary: Steroid
 Home-page: https://github.com/struckchure/steroid
 Author: Mohammed Al Ameen
 Author-email: ameenmohammed2311@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,9 +27,9 @@
 Requires-Dist: typing-extensions (==4.7.1)
 Requires-Dist: uvicorn (==0.23.0)
 Project-URL: Repository, https://github.com/struckchure/steroid
 Description-Content-Type: text/markdown
 
 # steroid
 
-NestJs like framework for python, built on top of FastAPI
+Steroid is a Python library built on top of FastAPI, designed to provide developers with a framework for building high-performance APIs using a structured architecture inspired by NestJs.
```

