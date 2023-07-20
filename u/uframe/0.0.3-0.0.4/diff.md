# Comparing `tmp/uframe-0.0.3.tar.gz` & `tmp/uframe-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.3.tar", last modified: Thu Jul 20 08:08:26 2023, max compression
+gzip compressed data, was "uframe-0.0.4.tar", last modified: Thu Jul 20 08:31:44 2023, max compression
```

## Comparing `uframe-0.0.3.tar` & `uframe-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.903653 uframe-0.0.3/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-20 08:08:26.903653 uframe-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.3/README.md
--rw-rw-rw-   0        0        0     1053 2023-07-20 08:05:14.000000 uframe-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-07-20 08:08:26.903653 uframe-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-07-11 11:16:34.000000 uframe-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.855255 uframe-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.871376 uframe-0.0.3/src/uframe/
--rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.3/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    61128 2023-07-20 08:07:55.000000 uframe-0.0.3/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     7066 2023-07-11 11:16:34.000000 uframe-0.0.3/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12408 2023-07-11 11:16:34.000000 uframe-0.0.3/src/uframe/uframe_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.890588 uframe-0.0.3/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.3/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.903653 uframe-0.0.3/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.3/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.3/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.735144 uframe-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-20 08:31:44.735144 uframe-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.4/README.md
+-rw-rw-rw-   0        0        0     1053 2023-07-20 08:30:55.000000 uframe-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-07-20 08:31:44.735144 uframe-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-07-11 11:16:34.000000 uframe-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.697028 uframe-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.719509 uframe-0.0.4/src/uframe/
+-rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.4/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    61174 2023-07-20 08:30:39.000000 uframe-0.0.4/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     7066 2023-07-11 11:16:34.000000 uframe-0.0.4/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12408 2023-07-11 11:16:34.000000 uframe-0.0.4/src/uframe/uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.735144 uframe-0.0.4/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.4/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       85 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 08:31:44.000000 uframe-0.0.4/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 08:31:44.735144 uframe-0.0.4/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.4/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.4/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.3/LICENSE` & `uframe-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.3/PKG-INFO` & `uframe-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.3/README.md` & `uframe-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.3/pyproject.toml` & `uframe-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.3/src/uframe/__init__.py` & `uframe-0.0.4/src/uframe/__init__.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.3/src/uframe/uframe.py` & `uframe-0.0.4/src/uframe/uframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 #from src.uframe import uframe_instance
 import scipy
+from .uframe_instance import uframe_instance
 from scipy import stats
 from sklearn.neighbors import KernelDensity
 import sklearn.neighbors
 from sklearn.preprocessing import OneHotEncoder, MinMaxScaler
 import miceforest as mf
 import math
 import pickle
```

### Comparing `uframe-0.0.3/src/uframe/uframe_from_mice.py` & `uframe-0.0.4/src/uframe/uframe_from_mice.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.3/src/uframe/uframe_instance.py` & `uframe-0.0.4/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.3/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.4/src/uframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.3/tests/test_uframe_instance.py` & `uframe-0.0.4/tests/test_uframe_instance.py`

 * *Files identical despite different names*

