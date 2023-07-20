# Comparing `tmp/pt_names-0.1.0.tar.gz` & `tmp/pt_names-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_names-0.1.0.tar", max compression
+gzip compressed data, was "pt_names-0.1.1.tar", max compression
```

## Comparing `pt_names-0.1.0.tar` & `pt_names-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.0/pt_names/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.0/pt_names/data_files/__init__.py
--rw-r--r--   0        0        0  5439608 2023-07-20 10:56:10.103392 pt_names-0.1.0/pt_names/data_files/first_names.csv
--rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.0/pt_names/data_files/last_names.csv
--rw-r--r--   0        0        0     1587 2023-07-20 11:44:01.407417 pt_names-0.1.0/pt_names/name_match.py
--rw-r--r--   0        0        0     2444 2023-07-20 10:56:10.129467 pt_names-0.1.0/pt_names/pt_name_gen.py
--rw-r--r--   0        0        0      387 2023-07-20 11:45:00.840188 pt_names-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.1/pt_names/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.1/pt_names/data_files/__init__.py
+-rw-r--r--   0        0        0  5439608 2023-07-20 10:56:10.103392 pt_names-0.1.1/pt_names/data_files/first_names.csv
+-rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.1/pt_names/data_files/last_names.csv
+-rw-r--r--   0        0        0     1587 2023-07-20 11:44:01.407417 pt_names-0.1.1/pt_names/name_match.py
+-rw-r--r--   0        0        0     2471 2023-07-20 11:52:12.132711 pt_names-0.1.1/pt_names/pt_name_gen.py
+-rw-r--r--   0        0        0      387 2023-07-20 11:53:45.561415 pt_names-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.1/PKG-INFO
```

### Comparing `pt_names-0.1.0/pt_names/data_files/first_names.csv` & `pt_names-0.1.1/pt_names/data_files/first_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.0/pt_names/data_files/last_names.csv` & `pt_names-0.1.1/pt_names/data_files/last_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.0/pt_names/name_match.py` & `pt_names-0.1.1/pt_names/name_match.py`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.0/pt_names/pt_name_gen.py` & `pt_names-0.1.1/pt_names/pt_name_gen.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module contains a function for generating random names in Portuguese.
 """
 import csv
 import random
 from unidecode import unidecode
 from typing import Optional
+import importlib.resources
 
 class Person:
     def __init__(self, first_name: str, last_name: str, gender: int) -> None:
         self.first_name = first_name
         self.last_name = last_name
         self.gender = gender
         self.email = self.get_email()
```

### Comparing `pt_names-0.1.0/PKG-INFO` & `pt_names-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-names
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

