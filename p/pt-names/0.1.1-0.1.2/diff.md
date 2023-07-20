# Comparing `tmp/pt_names-0.1.1.tar.gz` & `tmp/pt_names-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_names-0.1.1.tar", max compression
+gzip compressed data, was "pt_names-0.1.2.tar", max compression
```

## Comparing `pt_names-0.1.1.tar` & `pt_names-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.1/pt_names/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.1/pt_names/data_files/__init__.py
--rw-r--r--   0        0        0  5439608 2023-07-20 10:56:10.103392 pt_names-0.1.1/pt_names/data_files/first_names.csv
--rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.1/pt_names/data_files/last_names.csv
--rw-r--r--   0        0        0     1587 2023-07-20 11:44:01.407417 pt_names-0.1.1/pt_names/name_match.py
--rw-r--r--   0        0        0     2471 2023-07-20 11:52:12.132711 pt_names-0.1.1/pt_names/pt_name_gen.py
--rw-r--r--   0        0        0      387 2023-07-20 11:53:45.561415 pt_names-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.2/pt_names/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.2/pt_names/data_files/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-20 15:10:11.853164 pt_names-0.1.2/pt_names/data_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0  5439608 2023-03-29 14:11:41.000000 pt_names-0.1.2/pt_names/data_files/first_names.csv
+-rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.2/pt_names/data_files/last_names.csv
+-rw-r--r--   0        0        0     1587 2023-07-20 15:41:51.127333 pt_names-0.1.2/pt_names/name_match.py
+-rw-r--r--   0        0        0     2497 2023-07-20 15:41:37.599761 pt_names-0.1.2/pt_names/pt_name_gen.py
+-rw-r--r--   0        0        0      386 2023-07-20 15:42:26.768649 pt_names-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.2/PKG-INFO
```

### Comparing `pt_names-0.1.1/pt_names/data_files/first_names.csv` & `pt_names-0.1.2/pt_names/data_files/first_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.1/pt_names/data_files/last_names.csv` & `pt_names-0.1.2/pt_names/data_files/last_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.1/pt_names/name_match.py` & `pt_names-0.1.2/pt_names/name_match.py`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.1/pt_names/pt_name_gen.py` & `pt_names-0.1.2/pt_names/pt_name_gen.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 This module contains a function for generating random names in Portuguese.
 """
 import csv
 import random
 from unidecode import unidecode
 from typing import Optional
 import importlib.resources
+from pt_names import data_files
 
 class Person:
     def __init__(self, first_name: str, last_name: str, gender: int) -> None:
         self.first_name = first_name
         self.last_name = last_name
         self.gender = gender
         self.email = self.get_email()
@@ -24,15 +25,15 @@
         # Convert last name to lowercase and remove special characters
         last_name = unidecode(self.last_name.replace(" ", ".").lower())
         return f"{first_name}.{last_name}@example.com"
 
 def read_names_from_csv(file_name: str) -> dict:
     names = {"M": [], "F": []}
 
-    with importlib.resources.open_text("pt_name_gen", file_name) as csvfile:
+    with importlib.resources.open_text(data_files, file_name) as csvfile:
         csv_reader = csv.DictReader(csvfile)
     
         for row in csv_reader:
             name = row["name"]
             classification = row["classification"]
             names[classification].append(name)
 
@@ -49,15 +50,15 @@
         Name: An object containing the generated name.
     """
     names = read_names_from_csv("first_names.csv")
     
     men_names = names["M"]
     women_names = names["F"]
 
-    with importlib.resources.open_text("pt_name_gen", "last_names.csv") as csvfile:
+    with importlib.resources.open_text(data_files, "last_names.csv") as csvfile:
         surnames = [row["last_name"] for row in csv.DictReader(csvfile)]
 
     try:
         if gender is None:
             gender = random.randint(0, 1)
         first_name = random.choices(men_names if gender == 0 else women_names, k=1)[0]
         last_name = random.choices(surnames, k=1)[0]
```

### Comparing `pt_names-0.1.1/PKG-INFO` & `pt_names-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-names
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

