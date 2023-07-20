# Comparing `tmp/responsecurve-0.0.3.tar.gz` & `tmp/responsecurve-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsecurve-0.0.3.tar", last modified: Thu Jul 20 18:49:33 2023, max compression
+gzip compressed data, was "responsecurve-0.0.4.tar", last modified: Thu Jul 20 18:57:43 2023, max compression
```

## Comparing `responsecurve-0.0.3.tar` & `responsecurve-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:49:33.571893 responsecurve-0.0.3/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1163 2023-07-20 18:34:56.000000 responsecurve-0.0.3/LICENSE
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     2251 2023-07-20 18:49:33.571039 responsecurve-0.0.3/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1993 2023-07-20 18:34:49.000000 responsecurve-0.0.3/README.md
-drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:49:33.569571 responsecurve-0.0.3/responsecurve.egg-info/
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     2251 2023-07-20 18:49:33.000000 responsecurve-0.0.3/responsecurve.egg-info/PKG-INFO
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      210 2023-07-20 18:49:33.000000 responsecurve-0.0.3/responsecurve.egg-info/SOURCES.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:49:33.000000 responsecurve-0.0.3/responsecurve.egg-info/dependency_links.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 18:49:33.000000 responsecurve-0.0.3/responsecurve.egg-info/requires.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:49:33.000000 responsecurve-0.0.3/responsecurve.egg-info/top_level.txt
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 18:49:33.572337 responsecurve-0.0.3/setup.cfg
--rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      572 2023-07-20 18:49:20.000000 responsecurve-0.0.3/setup.py
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:57:43.550374 responsecurve-0.0.4/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1163 2023-07-20 18:34:56.000000 responsecurve-0.0.4/LICENSE
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     2251 2023-07-20 18:57:43.549744 responsecurve-0.0.4/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     1993 2023-07-20 18:34:49.000000 responsecurve-0.0.4/README.md
+drwxr-xr-x   0 ishanramrakhiani   (501) staff       (20)        0 2023-07-20 18:57:43.548479 responsecurve-0.0.4/responsecurve.egg-info/
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)     2251 2023-07-20 18:57:43.000000 responsecurve-0.0.4/responsecurve.egg-info/PKG-INFO
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      210 2023-07-20 18:57:43.000000 responsecurve-0.0.4/responsecurve.egg-info/SOURCES.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:57:43.000000 responsecurve-0.0.4/responsecurve.egg-info/dependency_links.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       43 2023-07-20 18:57:43.000000 responsecurve-0.0.4/responsecurve.egg-info/requires.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)        1 2023-07-20 18:57:43.000000 responsecurve-0.0.4/responsecurve.egg-info/top_level.txt
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)       38 2023-07-20 18:57:43.550560 responsecurve-0.0.4/setup.cfg
+-rw-r--r--   0 ishanramrakhiani   (501) staff       (20)      572 2023-07-20 18:57:32.000000 responsecurve-0.0.4/setup.py
```

### Comparing `responsecurve-0.0.3/LICENSE` & `responsecurve-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `responsecurve-0.0.3/PKG-INFO` & `responsecurve-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsecurve
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for detecting response curves in time series data.
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResponseCurve.py
```

### Comparing `responsecurve-0.0.3/README.md` & `responsecurve-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `responsecurve-0.0.3/responsecurve.egg-info/PKG-INFO` & `responsecurve-0.0.4/responsecurve.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsecurve
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for detecting response curves in time series data.
 Author: Ishan Ramrakhiani
 Author-email: ishanramrakhiani@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ResponseCurve.py
```

### Comparing `responsecurve-0.0.3/setup.py` & `responsecurve-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='responsecurve',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'numpy',
         'scipy',
         'matplotlib',
         'scikit-learn'
```

