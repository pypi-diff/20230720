# Comparing `tmp/simpleutilz-1.0.5.tar.gz` & `tmp/simpleutilz-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleutilz-1.0.5.tar", last modified: Thu Jul 20 18:26:25 2023, max compression
+gzip compressed data, was "simpleutilz-1.0.7.tar", last modified: Thu Jul 20 18:31:38 2023, max compression
```

## Comparing `simpleutilz-1.0.5.tar` & `simpleutilz-1.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:26:25.696123 simpleutilz-1.0.5/
--rw-rw-rw-   0        0        0     1089 2023-07-20 14:51:21.000000 simpleutilz-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     9368 2023-07-20 18:26:25.692125 simpleutilz-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-20 18:26:25.696123 simpleutilz-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-07-20 18:26:20.000000 simpleutilz-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:26:25.632127 simpleutilz-1.0.5/simpleutilz/
--rw-rw-rw-   0        0        0       65 2023-07-20 18:17:26.000000 simpleutilz-1.0.5/simpleutilz/__init__.py
--rw-rw-rw-   0        0        0     6353 2023-07-20 18:25:58.000000 simpleutilz-1.0.5/simpleutilz/simpleutilz.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:26:25.688123 simpleutilz-1.0.5/simpleutilz.egg-info/
--rw-rw-rw-   0        0        0     9368 2023-07-20 18:26:25.000000 simpleutilz-1.0.5/simpleutilz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-20 18:26:25.000000 simpleutilz-1.0.5/simpleutilz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:26:25.000000 simpleutilz-1.0.5/simpleutilz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 18:26:25.000000 simpleutilz-1.0.5/simpleutilz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-20 18:26:25.000000 simpleutilz-1.0.5/simpleutilz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 18:31:38.468047 simpleutilz-1.0.7/
+-rw-rw-rw-   0        0        0     1089 2023-07-20 14:51:21.000000 simpleutilz-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     9368 2023-07-20 18:31:38.468047 simpleutilz-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-20 18:31:38.468047 simpleutilz-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1755 2023-07-20 18:31:10.000000 simpleutilz-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:31:38.416037 simpleutilz-1.0.7/simpleutilz/
+-rw-rw-rw-   0        0        0       34 2023-07-20 18:30:48.000000 simpleutilz-1.0.7/simpleutilz/__init__.py
+-rw-rw-rw-   0        0        0     6351 2023-07-20 18:30:06.000000 simpleutilz-1.0.7/simpleutilz/simpleutilz.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:31:38.464036 simpleutilz-1.0.7/simpleutilz.egg-info/
+-rw-rw-rw-   0        0        0     9368 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/top_level.txt
```

### Comparing `simpleutilz-1.0.5/LICENSE` & `simpleutilz-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleutilz-1.0.5/PKG-INFO` & `simpleutilz-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleutilz
-Version: 1.0.5
+Version: 1.0.7
 Summary: A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations
 Home-page: https://github.com/ItzSimplyJoe/SimpleUtilz
 Author: ItzSimplyJoe
 Author-email: joebostock30@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `simpleutilz-1.0.5/setup.py` & `simpleutilz-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'simpleutilz'
-VERSION = '1.0.5'
+VERSION = '1.0.7'
 DESCRIPTION = 'A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations'
 URL = 'https://github.com/ItzSimplyJoe/SimpleUtilz'
 AUTHOR = 'ItzSimplyJoe'
 EMAIL = 'joebostock30@gmail.com'
 
 # Package dependencies (if any)
 INSTALL_REQUIRES = [
```

### Comparing `simpleutilz-1.0.5/simpleutilz/simpleutilz.py` & `simpleutilz-1.0.7/simpleutilz/simpleutilz.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -183,8 +183,8 @@
     '''Convert a PDF file to plain text.'''
     with open(pdf_file_path, 'rb') as pdf_file:
         pdf_reader = PyPDF2.PdfFileReader(pdf_file)
         text = ''
         for page_num in range(pdf_reader.getNumPages()):
             page = pdf_reader.getPage(page_num)
             text += page.extract_text()
-        return text
+        return text
```

### Comparing `simpleutilz-1.0.5/simpleutilz.egg-info/PKG-INFO` & `simpleutilz-1.0.7/simpleutilz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleutilz
-Version: 1.0.5
+Version: 1.0.7
 Summary: A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations
 Home-page: https://github.com/ItzSimplyJoe/SimpleUtilz
 Author: ItzSimplyJoe
 Author-email: joebostock30@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

