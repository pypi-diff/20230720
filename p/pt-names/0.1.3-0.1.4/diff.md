# Comparing `tmp/pt_names-0.1.3.tar.gz` & `tmp/pt_names-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pt_names-0.1.3.tar", max compression
+gzip compressed data, was "pt_names-0.1.4.tar", max compression
```

## Comparing `pt_names-0.1.3.tar` & `pt_names-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      254 2023-07-20 11:47:49.846327 pt_names-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.3/pt_names/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.3/pt_names/data_files/__init__.py
--rw-r--r--   0        0        0      169 2023-07-20 15:10:11.853164 pt_names-0.1.3/pt_names/data_files/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0  5439608 2023-03-29 14:11:41.000000 pt_names-0.1.3/pt_names/data_files/first_names.csv
--rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.3/pt_names/data_files/last_names.csv
--rw-r--r--   0        0        0     1674 2023-07-20 16:38:00.808645 pt_names-0.1.3/pt_names/gender_classifier.py
--rw-r--r--   0        0        0     2721 2023-07-20 16:43:44.487887 pt_names-0.1.3/pt_names/pt_name_gen.py
--rw-r--r--   0        0        0      386 2023-07-20 16:43:54.371019 pt_names-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 pt_names-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      422 2023-07-20 16:54:46.798031 pt_names-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 10:56:10.050418 pt_names-0.1.4/pt_names/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:06:21.746037 pt_names-0.1.4/pt_names/data_files/__init__.py
+-rw-r--r--   0        0        0      169 2023-07-20 15:10:11.853164 pt_names-0.1.4/pt_names/data_files/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0  5439608 2023-03-29 14:11:41.000000 pt_names-0.1.4/pt_names/data_files/first_names.csv
+-rw-r--r--   0        0        0     6773 2023-07-20 10:56:10.114078 pt_names-0.1.4/pt_names/data_files/last_names.csv
+-rw-r--r--   0        0        0     1674 2023-07-20 16:38:00.808645 pt_names-0.1.4/pt_names/gender_classifier.py
+-rw-r--r--   0        0        0     2721 2023-07-20 16:43:44.487887 pt_names-0.1.4/pt_names/pt_name_gen.py
+-rw-r--r--   0        0        0      386 2023-07-20 17:18:44.335968 pt_names-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 pt_names-0.1.4/PKG-INFO
```

### Comparing `pt_names-0.1.3/pt_names/data_files/first_names.csv` & `pt_names-0.1.4/pt_names/data_files/first_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.3/pt_names/data_files/last_names.csv` & `pt_names-0.1.4/pt_names/data_files/last_names.csv`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.3/pt_names/gender_classifier.py` & `pt_names-0.1.4/pt_names/gender_classifier.py`

 * *Files identical despite different names*

### Comparing `pt_names-0.1.3/pt_names/pt_name_gen.py` & `pt_names-0.1.4/pt_names/pt_name_gen.py`

 * *Files identical despite different names*

