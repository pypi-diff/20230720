# Comparing `tmp/pt_names-0.1.2.tar.gz` & `tmp/pt_names-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_names-0.1.2.tar", max compression
+gzip compressed data, was "pt_names-0.1.3.tar", max compression
```

## Comparing `pt_names-0.1.2.tar` & `pt_names-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.2/pt_names/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.2/pt_names/data_files/__init__.py
--rw-r--r--   0        0        0      169 2023-07-20 15:10:11.853164 pt_names-0.1.2/pt_names/data_files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0  5439608 2023-03-29 14:11:41.000000 pt_names-0.1.2/pt_names/data_files/first_names.csv
--rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.2/pt_names/data_files/last_names.csv
--rw-r--r--   0        0        0     1587 2023-07-20 15:41:51.127333 pt_names-0.1.2/pt_names/name_match.py
--rw-r--r--   0        0        0     2497 2023-07-20 15:41:37.599761 pt_names-0.1.2/pt_names/pt_name_gen.py
--rw-r--r--   0        0        0      386 2023-07-20 15:42:26.768649 pt_names-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.3/pt_names/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.3/pt_names/data_files/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-20 15:10:11.853164 pt_names-0.1.3/pt_names/data_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0  5439608 2023-03-29 14:11:41.000000 pt_names-0.1.3/pt_names/data_files/first_names.csv
+-rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.3/pt_names/data_files/last_names.csv
+-rw-r--r--   0        0        0     1674 2023-07-20 16:38:00.808645 pt_names-0.1.3/pt_names/gender_classifier.py
+-rw-r--r--   0        0        0     2721 2023-07-20 16:43:44.487887 pt_names-0.1.3/pt_names/pt_name_gen.py
+-rw-r--r--   0        0        0      386 2023-07-20 16:43:54.371019 pt_names-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.3/PKG-INFO
```

### Comparing `pt_names-0.1.2/pt_names/data_files/first_names.csv` & `pt_names-0.1.3/pt_names/data_files/first_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.2/pt_names/data_files/last_names.csv` & `pt_names-0.1.3/pt_names/data_files/last_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.2/pt_names/name_match.py` & `pt_names-0.1.3/pt_names/gender_classifier.py`

 * *Files 11% similar despite different names*

```diff
@@ -42,15 +42,17 @@
 
         return name_data
     
     def __call__(self, name : str) -> Optional[str]:
         """
         Find the gender of the given name in the CSV file.
 
+        looks only at the first word passed in the name string.
+
         Args:
             name (str): The name to search for.
 
         Returns:
             Optional[str]: The gender of the name if found, otherwise None.
         """
-        name = name.upper()
+        name = name.upper().split(" ")[0].strip()
         return self.name_data.get(name, None)
```

### Comparing `pt_names-0.1.2/pt_names/pt_name_gen.py` & `pt_names-0.1.3/pt_names/pt_name_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 class Person:
     def __init__(self, first_name: str, last_name: str, gender: int) -> None:
         self.first_name = first_name
         self.last_name = last_name
         self.gender = gender
         self.email = self.get_email()
         self.full_name = self.get_full_name()
+    
+    def __repr__(self) -> str:
+        # show first and last names as well as gender and full name in a nice format
+        return f"Person(first_name={self.first_name},last_name={self.last_name},gender={self.gender})"
 
     def get_full_name(self) -> str:
         return f"{self.first_name} {self.last_name}"
 
     def get_email(self) -> str:
         # Replace spaces in the first name with dots, convert to lowercase, and remove special characters
         first_name = unidecode(self.first_name.replace(" ", ".").lower())
```

### Comparing `pt_names-0.1.2/PKG-INFO` & `pt_names-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pt-names
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Simao Novais
 Author-email: snovaisg.97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

