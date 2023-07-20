# Comparing `tmp/tooey-0.3.0.tar.gz` & `tmp/tooey-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooey-0.3.0.tar", last modified: Thu Jul  6 21:49:29 2023, max compression
+gzip compressed data, was "tooey-0.4.0.tar", last modified: Thu Jul 20 17:40:23 2023, max compression
```

## Comparing `tooey-0.3.0.tar` & `tooey-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 21:49:29.000000 tooey-0.3.0/
--rw-r--r--   0 simon      (501) staff       (20)    11357 2023-06-29 07:36:21.000000 tooey-0.3.0/LICENSE
--rw-r--r--   0 simon      (501) staff       (20)     3754 2023-07-06 21:49:29.000000 tooey-0.3.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     2859 2023-07-02 19:14:03.000000 tooey-0.3.0/README.md
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-06 21:49:29.000000 tooey-0.3.0/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)     1023 2023-07-03 18:45:40.000000 tooey-0.3.0/setup.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey/
--rw-r--r--   0 simon      (501) staff       (20)       30 2023-06-29 08:16:41.000000 tooey-0.3.0/tooey/__init__.py
--rwxr-xr-x   0 simon      (501) staff       (20)      787 2023-07-05 19:07:13.000000 tooey-0.3.0/tooey/__version__.py
--rw-r--r--   0 simon      (501) staff       (20)    13219 2023-07-06 21:23:56.000000 tooey-0.3.0/tooey/tooey.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     3754 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      196 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)        6 2023-07-06 21:49:29.000000 tooey-0.3.0/tooey.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-20 17:40:23.000000 tooey-0.4.0/
+-rw-r--r--   0 simon      (501) staff       (20)    11357 2023-06-29 07:36:21.000000 tooey-0.4.0/LICENSE
+-rw-r--r--   0 simon      (501) staff       (20)     5808 2023-07-20 17:40:23.000000 tooey-0.4.0/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     4913 2023-07-20 17:38:12.000000 tooey-0.4.0/README.md
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-07-20 17:40:23.000000 tooey-0.4.0/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)     1023 2023-07-18 18:16:25.000000 tooey-0.4.0/setup.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-20 17:40:23.000000 tooey-0.4.0/tooey/
+-rw-r--r--   0 simon      (501) staff       (20)       30 2023-06-29 08:16:41.000000 tooey-0.4.0/tooey/__init__.py
+-rwxr-xr-x   0 simon      (501) staff       (20)      787 2023-07-18 16:31:45.000000 tooey-0.4.0/tooey/__version__.py
+-rw-r--r--   0 simon      (501) staff       (20)    16979 2023-07-20 17:33:27.000000 tooey-0.4.0/tooey/tooey.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-07-20 17:40:23.000000 tooey-0.4.0/tooey.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     5808 2023-07-20 17:40:23.000000 tooey-0.4.0/tooey.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      196 2023-07-20 17:40:23.000000 tooey-0.4.0/tooey.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-07-20 17:40:23.000000 tooey-0.4.0/tooey.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)        6 2023-07-20 17:40:23.000000 tooey-0.4.0/tooey.egg-info/top_level.txt
```

### Comparing `tooey-0.3.0/LICENSE` & `tooey-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooey-0.3.0/setup.py` & `tooey-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tooey-0.3.0/tooey/__version__.py` & `tooey-0.4.0/tooey/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __title__ = 'tooey'
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 __description__ = 'Automatically turn script arguments into an interactive terminal interface'
 __author__ = 'Simon Robinson'
 __author_email__ = 'simon@robinson.ac'
 __url__ = 'https://github.com/simonrob/tooey'
 __copyright__ = 'Copyright (c) 2023 Simon Robinson'
 __license__ = 'Apache 2.0'
 __classifiers__ = [  # https://pypi.org/classifiers/
```

