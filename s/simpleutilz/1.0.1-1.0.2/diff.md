# Comparing `tmp/simpleutilz-1.0.1.tar.gz` & `tmp/simpleutilz-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleutilz-1.0.1.tar", last modified: Thu Jul 20 15:25:28 2023, max compression
+gzip compressed data, was "simpleutilz-1.0.2.tar", last modified: Thu Jul 20 15:30:44 2023, max compression
```

## Comparing `simpleutilz-1.0.1.tar` & `simpleutilz-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 15:25:28.726107 simpleutilz-1.0.1/
--rw-rw-rw-   0        0        0     1089 2023-07-20 14:51:21.000000 simpleutilz-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     9368 2023-07-20 15:25:28.726107 simpleutilz-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-20 15:25:28.730102 simpleutilz-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-07-20 15:25:24.000000 simpleutilz-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 15:25:28.718102 simpleutilz-1.0.1/simpleutilz.egg-info/
--rw-rw-rw-   0        0        0     9368 2023-07-20 15:25:28.000000 simpleutilz-1.0.1/simpleutilz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-07-20 15:25:28.000000 simpleutilz-1.0.1/simpleutilz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 15:25:28.000000 simpleutilz-1.0.1/simpleutilz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 15:25:28.000000 simpleutilz-1.0.1/simpleutilz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 15:25:28.000000 simpleutilz-1.0.1/simpleutilz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 15:30:44.198886 simpleutilz-1.0.2/
+-rw-rw-rw-   0        0        0     1089 2023-07-20 14:51:21.000000 simpleutilz-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     9368 2023-07-20 15:30:44.198886 simpleutilz-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-20 15:30:44.198886 simpleutilz-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1755 2023-07-20 15:30:26.000000 simpleutilz-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 15:30:44.126887 simpleutilz-1.0.2/simpleutilz/
+-rw-rw-rw-   0        0        0       63 2023-07-20 15:29:42.000000 simpleutilz-1.0.2/simpleutilz/__init__.py
+-rw-rw-rw-   0        0        0     6351 2023-07-20 15:23:28.000000 simpleutilz-1.0.2/simpleutilz/simpleutilz.py
+drwxrwxrwx   0        0        0        0 2023-07-20 15:30:44.194898 simpleutilz-1.0.2/simpleutilz.egg-info/
+-rw-rw-rw-   0        0        0     9368 2023-07-20 15:30:43.000000 simpleutilz-1.0.2/simpleutilz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-20 15:30:44.000000 simpleutilz-1.0.2/simpleutilz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 15:30:43.000000 simpleutilz-1.0.2/simpleutilz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 15:30:43.000000 simpleutilz-1.0.2/simpleutilz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-20 15:30:43.000000 simpleutilz-1.0.2/simpleutilz.egg-info/top_level.txt
```

### Comparing `simpleutilz-1.0.1/LICENSE` & `simpleutilz-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleutilz-1.0.1/PKG-INFO` & `simpleutilz-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleutilz
-Version: 1.0.1
+Version: 1.0.2
 Summary: A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations
 Home-page: https://github.com/ItzSimplyJoe/SimpleUtilz
 Author: ItzSimplyJoe
 Author-email: joebostock30@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `simpleutilz-1.0.1/setup.py` & `simpleutilz-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'simpleutilz'
-VERSION = '1.0.1'
+VERSION = '1.0.2'
 DESCRIPTION = 'A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations'
 URL = 'https://github.com/ItzSimplyJoe/SimpleUtilz'
 AUTHOR = 'ItzSimplyJoe'
 EMAIL = 'joebostock30@gmail.com'
 
 # Package dependencies (if any)
 INSTALL_REQUIRES = [
```

### Comparing `simpleutilz-1.0.1/simpleutilz.egg-info/PKG-INFO` & `simpleutilz-1.0.2/simpleutilz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpleutilz
-Version: 1.0.1
+Version: 1.0.2
 Summary: A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations
 Home-page: https://github.com/ItzSimplyJoe/SimpleUtilz
 Author: ItzSimplyJoe
 Author-email: joebostock30@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

