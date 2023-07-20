# Comparing `tmp/calibrated_explanations-0.0.6.tar.gz` & `tmp/calibrated_explanations-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrated_explanations-0.0.6.tar", last modified: Thu Jul 20 13:13:43 2023, max compression
+gzip compressed data, was "calibrated_explanations-0.0.6a0.tar", last modified: Thu Jul 20 12:54:34 2023, max compression
```

## Comparing `calibrated_explanations-0.0.6.tar` & `calibrated_explanations-0.0.6a0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 13:13:43.813020 calibrated_explanations-0.0.6/
--rw-rw-rw-   0        0        0     1085 2023-07-12 12:35:31.000000 calibrated_explanations-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2658 2023-07-20 13:13:43.811008 calibrated_explanations-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1976 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/README.md
--rw-rw-rw-   0        0        0      977 2023-07-20 13:07:59.000000 calibrated_explanations-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-20 13:13:43.813020 calibrated_explanations-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      179 2023-07-12 12:35:32.000000 calibrated_explanations-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 13:13:43.687011 calibrated_explanations-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 13:13:43.754006 calibrated_explanations-0.0.6/src/calibrated_explanations/
--rw-rw-rw-   0        0        0     2533 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/src/calibrated_explanations/VennAbers.py
--rw-rw-rw-   0        0        0      509 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/src/calibrated_explanations/__init__.py
--rw-rw-rw-   0        0        0     1957 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/src/calibrated_explanations/_discretizers.py
--rw-rw-rw-   0        0        0    38940 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/src/calibrated_explanations/_explanations.py
--rw-rw-rw-   0        0        0    36850 2023-07-20 12:36:38.000000 calibrated_explanations-0.0.6/src/calibrated_explanations/core.py
--rw-rw-rw-   0        0        0     3039 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/src/calibrated_explanations/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-07-20 13:13:43.789008 calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/
--rw-rw-rw-   0        0        0     2658 2023-07-20 13:13:43.000000 calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      596 2023-07-20 13:13:43.000000 calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 13:13:43.000000 calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-20 13:13:43.000000 calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-20 13:13:43.000000 calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 13:13:43.809007 calibrated_explanations-0.0.6/tests/
--rw-rw-rw-   0        0        0     8692 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/tests/test_classification.py
--rw-rw-rw-   0        0        0    15625 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.808170 calibrated_explanations-0.0.6a0/
+-rw-rw-rw-   0        0        0     1085 2023-07-12 12:35:31.000000 calibrated_explanations-0.0.6a0/LICENSE
+-rw-rw-rw-   0        0        0     2660 2023-07-20 12:54:34.807164 calibrated_explanations-0.0.6a0/PKG-INFO
+-rw-rw-rw-   0        0        0     1976 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/README.md
+-rw-rw-rw-   0        0        0      979 2023-07-20 12:49:04.000000 calibrated_explanations-0.0.6a0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 12:54:34.808170 calibrated_explanations-0.0.6a0/setup.cfg
+-rw-rw-rw-   0        0        0      179 2023-07-12 12:35:32.000000 calibrated_explanations-0.0.6a0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.756162 calibrated_explanations-0.0.6a0/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.781161 calibrated_explanations-0.0.6a0/src/calibrated_explanations/
+-rw-rw-rw-   0        0        0     2533 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/VennAbers.py
+-rw-rw-rw-   0        0        0      509 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/__init__.py
+-rw-rw-rw-   0        0        0     1957 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/_discretizers.py
+-rw-rw-rw-   0        0        0    38940 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/_explanations.py
+-rw-rw-rw-   0        0        0    36850 2023-07-20 12:36:38.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/core.py
+-rw-rw-rw-   0        0        0     3039 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.800161 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/
+-rw-rw-rw-   0        0        0     2660 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      596 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-20 12:54:34.000000 calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 12:54:34.804163 calibrated_explanations-0.0.6a0/tests/
+-rw-rw-rw-   0        0        0     8692 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/tests/test_classification.py
+-rw-rw-rw-   0        0        0    15625 2023-07-14 13:36:20.000000 calibrated_explanations-0.0.6a0/tests/test_regression.py
```

### Comparing `calibrated_explanations-0.0.6/LICENSE` & `calibrated_explanations-0.0.6a0/LICENSE`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/PKG-INFO` & `calibrated_explanations-0.0.6a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrated_explanations
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: Extract calibrated explanations from machine learning models.
 Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
 Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
 Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calibrated_explanations-0.0.6/README.md` & `calibrated_explanations-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/pyproject.toml` & `calibrated_explanations-0.0.6a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calibrated_explanations"
-version = "0.0.6"
+version = "0.0.6a0"
 authors = [
   { name="Helena Löfström", email="helena.lofstrom@ju.se" },
   { name="Tuwe Löfström", email="tuwe.lofstrom@ju.se" },
 ]
 description = "Extract calibrated explanations from machine learning models."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations/VennAbers.py` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations/VennAbers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations/_discretizers.py` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations/_discretizers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations/_explanations.py` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations/_explanations.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations/core.py` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations/core.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations/wrappers.py` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations/wrappers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/PKG-INFO` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrated-explanations
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: Extract calibrated explanations from machine learning models.
 Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
 Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
 Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `calibrated_explanations-0.0.6/src/calibrated_explanations.egg-info/SOURCES.txt` & `calibrated_explanations-0.0.6a0/src/calibrated_explanations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/tests/test_classification.py` & `calibrated_explanations-0.0.6a0/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.0.6/tests/test_regression.py` & `calibrated_explanations-0.0.6a0/tests/test_regression.py`

 * *Files identical despite different names*

