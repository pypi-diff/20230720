# Comparing `tmp/gncxml-0.6.8.tar.gz` & `tmp/gncxml-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gncxml-0.6.8.tar", max compression
+gzip compressed data, was "gncxml-0.6.9.tar", max compression
```

## Comparing `gncxml-0.6.8.tar` & `gncxml-0.6.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2017-12-17 01:02:32.000000 gncxml-0.6.8/LICENSE
--rw-r--r--   0        0        0     1124 2022-01-22 02:05:23.252599 gncxml-0.6.8/README.md
--rw-r--r--   0        0        0      121 2017-11-23 20:24:39.000000 gncxml-0.6.8/gncxml/__init__.py
--rw-r--r--   0        0        0       90 2021-12-27 13:53:45.410909 gncxml-0.6.8/gncxml/__main__.py
--rw-r--r--   0        0        0     2871 2022-08-24 00:28:47.978154 gncxml-0.6.8/gncxml/_cli.py
--rw-r--r--   0        0        0    10398 2023-03-24 00:18:29.115533 gncxml-0.6.8/gncxml/_iso4217.py
--rw-r--r--   0        0        0    11085 2021-12-27 13:53:45.413612 gncxml-0.6.8/gncxml/book.py
--rw-r--r--   0        0        0      618 2023-03-24 00:17:15.794424 gncxml-0.6.8/pyproject.toml
--rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 gncxml-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2017-12-17 01:02:32.000000 gncxml-0.6.9/LICENSE
+-rw-r--r--   0        0        0     1124 2022-01-22 02:05:23.252599 gncxml-0.6.9/README.md
+-rw-r--r--   0        0        0      121 2017-11-23 20:24:39.000000 gncxml-0.6.9/gncxml/__init__.py
+-rw-r--r--   0        0        0       90 2021-12-27 13:53:45.410909 gncxml-0.6.9/gncxml/__main__.py
+-rw-r--r--   0        0        0     2871 2022-08-24 00:28:47.978154 gncxml-0.6.9/gncxml/_cli.py
+-rw-r--r--   0        0        0    10398 2023-07-20 00:33:06.893294 gncxml-0.6.9/gncxml/_iso4217.py
+-rw-r--r--   0        0        0    11085 2021-12-27 13:53:45.413612 gncxml-0.6.9/gncxml/book.py
+-rw-r--r--   0        0        0      618 2023-07-20 16:09:15.147061 gncxml-0.6.9/pyproject.toml
+-rw-r--r--   0        0        0     1876 1970-01-01 00:00:00.000000 gncxml-0.6.9/PKG-INFO
```

### Comparing `gncxml-0.6.8/LICENSE` & `gncxml-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.8/README.md` & `gncxml-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.8/gncxml/_cli.py` & `gncxml-0.6.9/gncxml/_cli.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.8/gncxml/_iso4217.py` & `gncxml-0.6.9/gncxml/_iso4217.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.8/gncxml/book.py` & `gncxml-0.6.9/gncxml/book.py`

 * *Files identical despite different names*

### Comparing `gncxml-0.6.8/pyproject.toml` & `gncxml-0.6.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gncxml"
-version = "0.6.8"
+version = "0.6.9"
 description = "Extract entries from GnuCash data file to pandas.DataFrame."
 license = "Apache-2.0"
 authors = ["LiosK <contact@mail.liosk.net>"]
 readme = "README.md"
 homepage = "https://github.com/LiosK/gncxml"
 classifiers = [
   "Operating System :: OS Independent",
@@ -15,12 +15,12 @@
 gncxml = "gncxml._cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.5.3"
 
 [tool.poetry.dev-dependencies]
-jupyterlab = "^3.6.2"
+jupyterlab = "^3.6.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `gncxml-0.6.8/PKG-INFO` & `gncxml-0.6.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gncxml
-Version: 0.6.8
+Version: 0.6.9
 Summary: Extract entries from GnuCash data file to pandas.DataFrame.
 Home-page: https://github.com/LiosK/gncxml
 License: Apache-2.0
 Author: LiosK
 Author-email: contact@mail.liosk.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

