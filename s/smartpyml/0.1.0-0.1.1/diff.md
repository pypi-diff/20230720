# Comparing `tmp/smartpyml-0.1.0.tar.gz` & `tmp/smartpyml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartpyml-0.1.0.tar", last modified: Wed Jul 19 19:06:14 2023, max compression
+gzip compressed data, was "smartpyml-0.1.1.tar", last modified: Thu Jul 20 08:12:20 2023, max compression
```

## Comparing `smartpyml-0.1.0.tar` & `smartpyml-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:14.852241 smartpyml-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-07-19 16:56:10.000000 smartpyml-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1642 2023-07-19 19:06:14.849023 smartpyml-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:14.773645 smartpyml-0.1.0/ml_utils/
--rw-rw-rw-   0        0        0       23 2023-07-19 17:26:54.000000 smartpyml-0.1.0/ml_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:14.781909 smartpyml-0.1.0/ml_utils/analysis/
--rw-rw-rw-   0        0        0     4071 2023-07-19 18:36:42.000000 smartpyml-0.1.0/ml_utils/analysis/Overview.py
--rw-rw-rw-   0        0        0    15986 2023-07-19 17:47:18.000000 smartpyml-0.1.0/ml_utils/analysis/Plot.py
--rw-rw-rw-   0        0        0       88 2023-07-19 16:34:03.000000 smartpyml-0.1.0/ml_utils/analysis/__init__.py
--rw-rw-rw-   0        0        0       42 2023-07-19 19:06:14.853297 smartpyml-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1943 2023-07-19 19:03:38.000000 smartpyml-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:14.843756 smartpyml-0.1.0/smartpyml.egg-info/
--rw-rw-rw-   0        0        0     1642 2023-07-19 19:06:14.000000 smartpyml-0.1.0/smartpyml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-19 19:06:14.000000 smartpyml-0.1.0/smartpyml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-19 19:06:14.000000 smartpyml-0.1.0/smartpyml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      254 2023-07-19 19:06:14.000000 smartpyml-0.1.0/smartpyml.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-07-19 19:06:14.000000 smartpyml-0.1.0/smartpyml.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-19 19:06:14.848014 smartpyml-0.1.0/ts_utils/
--rw-rw-rw-   0        0        0        0 2023-07-19 17:38:55.000000 smartpyml-0.1.0/ts_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:12:20.375733 smartpyml-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2023-07-19 16:56:10.000000 smartpyml-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1642 2023-07-20 08:12:20.374736 smartpyml-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1732 2023-07-20 07:51:08.000000 smartpyml-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 08:12:20.269409 smartpyml-0.1.1/ml_utils/
+-rw-rw-rw-   0        0        0       23 2023-07-19 17:26:54.000000 smartpyml-0.1.1/ml_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:12:20.279347 smartpyml-0.1.1/ml_utils/analysis/
+-rw-rw-rw-   0        0        0     4071 2023-07-19 18:36:42.000000 smartpyml-0.1.1/ml_utils/analysis/Overview.py
+-rw-rw-rw-   0        0        0    15986 2023-07-19 17:47:18.000000 smartpyml-0.1.1/ml_utils/analysis/Plot.py
+-rw-rw-rw-   0        0        0       88 2023-07-19 16:34:03.000000 smartpyml-0.1.1/ml_utils/analysis/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:12:20.375733 smartpyml-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1943 2023-07-20 07:25:49.000000 smartpyml-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:12:20.363469 smartpyml-0.1.1/smartpyml.egg-info/
+-rw-rw-rw-   0        0        0     1642 2023-07-20 08:12:19.000000 smartpyml-0.1.1/smartpyml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-07-20 08:12:19.000000 smartpyml-0.1.1/smartpyml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:12:19.000000 smartpyml-0.1.1/smartpyml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      254 2023-07-20 08:12:19.000000 smartpyml-0.1.1/smartpyml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-07-20 08:12:19.000000 smartpyml-0.1.1/smartpyml.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 08:12:20.370838 smartpyml-0.1.1/ts_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-19 17:38:55.000000 smartpyml-0.1.1/ts_utils/__init__.py
```

### Comparing `smartpyml-0.1.0/LICENSE` & `smartpyml-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `smartpyml-0.1.0/PKG-INFO` & `smartpyml-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpyml
-Version: 0.1.0
+Version: 0.1.1
 Summary: smartpyml: A Comprehensive Machine Learning Library
 Home-page: https://github.com/srikresna/smartpyml
 Author: srikresna
 Author-email: srikresna383@gmail.com
 Keywords: machine learning,data science,automl,ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `smartpyml-0.1.0/ml_utils/analysis/Overview.py` & `smartpyml-0.1.1/ml_utils/analysis/Overview.py`

 * *Files identical despite different names*

### Comparing `smartpyml-0.1.0/ml_utils/analysis/Plot.py` & `smartpyml-0.1.1/ml_utils/analysis/Plot.py`

 * *Files identical despite different names*

### Comparing `smartpyml-0.1.0/setup.py` & `smartpyml-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     required_packages = f.read().splitlines()
 
 setup(
     name='smartpyml',          
-    version='0.1.0',              
+    version='0.1.1',              
     author='srikresna',
     author_email='srikresna383@gmail.com',
     description='smartpyml: A Comprehensive Machine Learning Library',
     long_description='''smartpyml is a comprehensive machine learning library that empowers developers and data scientists to easily apply classical machine learning algorithms and time series analysis techniques. It provides a collection of user-friendly functions and tools for data preprocessing, model training, evaluation, and prediction, making it suitable for both beginners and experienced practitioners in the field of data science and artificial intelligence.
 
 Main Features:
 - A wide range of classical machine learning algorithms
```

### Comparing `smartpyml-0.1.0/smartpyml.egg-info/PKG-INFO` & `smartpyml-0.1.1/smartpyml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartpyml
-Version: 0.1.0
+Version: 0.1.1
 Summary: smartpyml: A Comprehensive Machine Learning Library
 Home-page: https://github.com/srikresna/smartpyml
 Author: srikresna
 Author-email: srikresna383@gmail.com
 Keywords: machine learning,data science,automl,ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

