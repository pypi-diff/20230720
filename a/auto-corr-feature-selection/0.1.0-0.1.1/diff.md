# Comparing `tmp/auto_corr_feature_selection-0.1.0.tar.gz` & `tmp/auto_corr_feature_selection-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_corr_feature_selection-0.1.0.tar", max compression
+gzip compressed data, was "auto_corr_feature_selection-0.1.1.tar", max compression
```

## Comparing `auto_corr_feature_selection-0.1.0.tar` & `auto_corr_feature_selection-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2830 2023-07-19 13:33:14.157589 auto_corr_feature_selection-0.1.0/README.md
--rw-r--r--   0        0        0       66 2023-07-19 11:37:26.859400 auto_corr_feature_selection-0.1.0/auto_corr_feature_selection/__init__.py
--rw-r--r--   0        0        0     3088 2023-07-19 13:48:29.439086 auto_corr_feature_selection-0.1.0/auto_corr_feature_selection/auto_corr_feature_selection.py
--rw-r--r--   0        0        0      740 2023-07-19 13:53:36.928704 auto_corr_feature_selection-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 auto_corr_feature_selection-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3136 2023-07-19 14:13:50.699169 auto_corr_feature_selection-0.1.1/README.md
+-rw-r--r--   0        0        0       66 2023-07-19 11:37:26.859400 auto_corr_feature_selection-0.1.1/auto_corr_feature_selection/__init__.py
+-rw-r--r--   0        0        0     3088 2023-07-19 13:48:29.439086 auto_corr_feature_selection-0.1.1/auto_corr_feature_selection/auto_corr_feature_selection.py
+-rw-r--r--   0        0        0      740 2023-07-20 12:31:13.482452 auto_corr_feature_selection-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 auto_corr_feature_selection-0.1.1/PKG-INFO
```

### Comparing `auto_corr_feature_selection-0.1.0/README.md` & `auto_corr_feature_selection-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # AutoCorrFeatureSelection
 
 Automatically select the most relevant features based on correlation.
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/auto-corr-feature-selection.svg)](https://pypi.org/project/auto-corr-feature-selection/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/auto-corr-feature-selection.svg?label=PyPI%20downloads)](https://pypi.org/project/auto-corr-feature-selection/)
+
 
 # How it works
 
 The __AutoCorrFeatureSelection__ class utilizes correlation analysis to automatically select relevant features from a given dataset. Here's a step-by-step overview of how it works:
 
 1. Correlation Matrix:
```

### Comparing `auto_corr_feature_selection-0.1.0/auto_corr_feature_selection/auto_corr_feature_selection.py` & `auto_corr_feature_selection-0.1.1/auto_corr_feature_selection/auto_corr_feature_selection.py`

 * *Files identical despite different names*

### Comparing `auto_corr_feature_selection-0.1.0/pyproject.toml` & `auto_corr_feature_selection-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "auto_corr_feature_selection"
-version = "0.1.0"
+version = "0.1.1"
 description = "Automatically select the most relevant features based on correlation."
 authors = ["Andres Di Giovanni <andresdigiovanni@gmail.com>"]
 readme = "README.md"
 packages = [{include = "auto_corr_feature_selection"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8"
-pandas = "^2.0.3"
+python = ">=3.9"
+pandas = ">1.5.0"
 numpy = "^1.25.1"
 scikit-learn = "^1.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 pre-commit = "^2.20.0"
```

### Comparing `auto_corr_feature_selection-0.1.0/PKG-INFO` & `auto_corr_feature_selection-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: auto-corr-feature-selection
-Version: 0.1.0
+Version: 0.1.1
 Summary: Automatically select the most relevant features based on correlation.
 Author: Andres Di Giovanni
 Author-email: andresdigiovanni@gmail.com
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.25.1,<2.0.0)
-Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: pandas (>1.5.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # AutoCorrFeatureSelection
 
 Automatically select the most relevant features based on correlation.
 
+[![PyPI Latest Release](https://img.shields.io/pypi/v/auto-corr-feature-selection.svg)](https://pypi.org/project/auto-corr-feature-selection/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/auto-corr-feature-selection.svg?label=PyPI%20downloads)](https://pypi.org/project/auto-corr-feature-selection/)
+
 
 # How it works
 
 The __AutoCorrFeatureSelection__ class utilizes correlation analysis to automatically select relevant features from a given dataset. Here's a step-by-step overview of how it works:
 
 1. Correlation Matrix:
```

