# Comparing `tmp/simpleutilz-1.0.7.tar.gz` & `tmp/simpleutilz-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleutilz-1.0.7.tar", last modified: Thu Jul 20 18:31:38 2023, max compression
+gzip compressed data, was "simpleutilz-1.0.8.tar", last modified: Thu Jul 20 18:36:08 2023, max compression
```

## Comparing `simpleutilz-1.0.7.tar` & `simpleutilz-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 18:31:38.468047 simpleutilz-1.0.7/
--rw-rw-rw-   0        0        0     1089 2023-07-20 14:51:21.000000 simpleutilz-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     9368 2023-07-20 18:31:38.468047 simpleutilz-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-20 18:31:38.468047 simpleutilz-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-07-20 18:31:10.000000 simpleutilz-1.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:31:38.416037 simpleutilz-1.0.7/simpleutilz/
--rw-rw-rw-   0        0        0       34 2023-07-20 18:30:48.000000 simpleutilz-1.0.7/simpleutilz/__init__.py
--rw-rw-rw-   0        0        0     6351 2023-07-20 18:30:06.000000 simpleutilz-1.0.7/simpleutilz/simpleutilz.py
-drwxrwxrwx   0        0        0        0 2023-07-20 18:31:38.464036 simpleutilz-1.0.7/simpleutilz.egg-info/
--rw-rw-rw-   0        0        0     9368 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-20 18:31:38.000000 simpleutilz-1.0.7/simpleutilz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 18:36:08.241877 simpleutilz-1.0.8/
+-rw-rw-rw-   0        0        0     1089 2023-07-20 14:51:21.000000 simpleutilz-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     9692 2023-07-20 18:36:08.237876 simpleutilz-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-20 18:36:08.241877 simpleutilz-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1755 2023-07-20 18:35:50.000000 simpleutilz-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:36:08.193889 simpleutilz-1.0.8/simpleutilz/
+-rw-rw-rw-   0        0        0       34 2023-07-20 18:30:48.000000 simpleutilz-1.0.8/simpleutilz/__init__.py
+-rw-rw-rw-   0        0        0     6351 2023-07-20 18:30:06.000000 simpleutilz-1.0.8/simpleutilz/simpleutilz.py
+drwxrwxrwx   0        0        0        0 2023-07-20 18:36:08.233877 simpleutilz-1.0.8/simpleutilz.egg-info/
+-rw-rw-rw-   0        0        0     9692 2023-07-20 18:36:07.000000 simpleutilz-1.0.8/simpleutilz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-07-20 18:36:08.000000 simpleutilz-1.0.8/simpleutilz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 18:36:07.000000 simpleutilz-1.0.8/simpleutilz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 18:36:07.000000 simpleutilz-1.0.8/simpleutilz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-20 18:36:07.000000 simpleutilz-1.0.8/simpleutilz.egg-info/top_level.txt
```

### Comparing `simpleutilz-1.0.7/LICENSE` & `simpleutilz-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleutilz-1.0.7/setup.py` & `simpleutilz-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'simpleutilz'
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 DESCRIPTION = 'A versatile Python utility library that offers a wide range of helper functions, classes, and modules to expedite development tasks and simplify common operations'
 URL = 'https://github.com/ItzSimplyJoe/SimpleUtilz'
 AUTHOR = 'ItzSimplyJoe'
 EMAIL = 'joebostock30@gmail.com'
 
 # Package dependencies (if any)
 INSTALL_REQUIRES = [
```

### Comparing `simpleutilz-1.0.7/simpleutilz/simpleutilz.py` & `simpleutilz-1.0.8/simpleutilz/simpleutilz.py`

 * *Files identical despite different names*

