# Comparing `tmp/python_Testing_Utilities-0.1.8.tar.gz` & `tmp/python_Testing_Utilities-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_Testing_Utilities-0.1.8.tar", last modified: Thu Jul 28 12:12:00 2022, max compression
+gzip compressed data, was "python_Testing_Utilities-0.1.9.tar", last modified: Thu Jul 28 12:18:22 2022, max compression
```

## Comparing `python_Testing_Utilities-0.1.8.tar` & `python_Testing_Utilities-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-28 12:12:00.553698 python_Testing_Utilities-0.1.8/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       67 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)      301 2022-07-28 12:12:00.553698 python_Testing_Utilities-0.1.8/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)     1003 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/README.md
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-28 12:12:00.553698 python_Testing_Utilities-0.1.8/python_Testing_Utilities/
--rw-rw-r--   0 robert    (1000) robert    (1000)      696 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      497 2022-07-28 12:12:00.553698 python_Testing_Utilities-0.1.8/python_Testing_Utilities/_version.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     2994 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities/assertMultiLineStringsEqual.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3351 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities/callService.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     3186 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities/pythonObjCompare.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-28 12:12:00.553698 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)      301 2022-07-28 12:12:00.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      563 2022-07-28 12:12:00.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-28 12:12:00.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-28 12:09:05.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)       17 2022-07-28 12:12:00.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       25 2022-07-28 12:12:00.000000 python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/top_level.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)      280 2022-07-28 12:12:00.553698 python_Testing_Utilities-0.1.8/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)      790 2022-07-28 12:11:35.000000 python_Testing_Utilities-0.1.8/setup.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.8/versioneer.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-28 12:18:22.436869 python_Testing_Utilities-0.1.9/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       67 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)      301 2022-07-28 12:18:22.436869 python_Testing_Utilities-0.1.9/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1003 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/README.md
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-28 12:18:22.436869 python_Testing_Utilities-0.1.9/python_Testing_Utilities/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      696 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      497 2022-07-28 12:18:22.436869 python_Testing_Utilities-0.1.9/python_Testing_Utilities/_version.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     2994 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities/assertMultiLineStringsEqual.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3351 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities/callService.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     3186 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities/pythonObjCompare.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2022-07-28 12:18:22.436869 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      301 2022-07-28 12:18:22.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      563 2022-07-28 12:18:22.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-28 12:18:22.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-28 12:09:05.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)       17 2022-07-28 12:18:22.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       25 2022-07-28 12:18:22.000000 python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/top_level.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)      280 2022-07-28 12:18:22.436869 python_Testing_Utilities-0.1.9/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)      790 2022-07-28 12:11:35.000000 python_Testing_Utilities-0.1.9/setup.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-28 12:08:51.000000 python_Testing_Utilities-0.1.9/versioneer.py
```

### Comparing `python_Testing_Utilities-0.1.8/LICENSE` & `python_Testing_Utilities-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/README.md` & `python_Testing_Utilities-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/python_Testing_Utilities/__init__.py` & `python_Testing_Utilities-0.1.9/python_Testing_Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/python_Testing_Utilities/assertMultiLineStringsEqual.py` & `python_Testing_Utilities-0.1.9/python_Testing_Utilities/assertMultiLineStringsEqual.py`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/python_Testing_Utilities/callService.py` & `python_Testing_Utilities-0.1.9/python_Testing_Utilities/callService.py`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/python_Testing_Utilities/pythonObjCompare.py` & `python_Testing_Utilities-0.1.9/python_Testing_Utilities/pythonObjCompare.py`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/python_Testing_Utilities.egg-info/SOURCES.txt` & `python_Testing_Utilities-0.1.9/python_Testing_Utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/setup.py` & `python_Testing_Utilities-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `python_Testing_Utilities-0.1.8/versioneer.py` & `python_Testing_Utilities-0.1.9/versioneer.py`

 * *Files identical despite different names*

