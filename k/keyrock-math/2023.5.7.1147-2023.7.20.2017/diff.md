# Comparing `tmp/keyrock-math-2023.5.7.1147.tar.gz` & `tmp/keyrock-math-2023.7.20.2017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-math-2023.5.7.1147.tar", last modified: Sun May  7 11:47:31 2023, max compression
+gzip compressed data, was "keyrock-math-2023.7.20.2017.tar", last modified: Thu Jul 20 20:17:34 2023, max compression
```

## Comparing `keyrock-math-2023.5.7.1147.tar` & `keyrock-math-2023.7.20.2017.tar`

### file list

```diff
@@ -1,39 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.802105 keyrock-math-2023.5.7.1147/keyrock_math/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.809106 keyrock-math-2023.5.7.1147/keyrock_math/distribution/
--rw-rw-rw-   0 root         (0) root         (0)      829 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/analytic.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/beta.py
--rw-rw-rw-   0 root         (0) root         (0)      600 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/constant.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      550 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/gamma.py
--rw-rw-rw-   0 root         (0) root         (0)     1601 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/log_normal.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/logistic.py
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/normal.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/skew_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     3658 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      532 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/uniform.py
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution/weibull.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/analytic.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/beta.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/constant.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/gamma.py
--rw-rw-rw-   0 root         (0) root         (0)     2232 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/log_normal.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/logistic.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/normal.py
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/skew_normal.py
--rw-rw-rw-   0 root         (0) root         (0)     2696 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/test_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/keyrock_math/distribution_old/uniform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 11:47:31.804105 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-07 11:47:31.000000 keyrock-math-2023.5.7.1147/keyrock_math.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-07 11:47:15.000000 keyrock-math-2023.5.7.1147/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      171 2023-05-07 11:47:31.814106 keyrock-math-2023.5.7.1147/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:34.493643 keyrock-math-2023.7.20.2017/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 20:17:34.493643 keyrock-math-2023.7.20.2017/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:34.489643 keyrock-math-2023.7.20.2017/keyrock_math/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:34.493643 keyrock-math-2023.7.20.2017/keyrock_math/distribution/
+-rw-rw-rw-   0 root         (0) root         (0)      829 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/analytic.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/beta.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/constant.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      550 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/gamma.py
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/log_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/logistic.py
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/normal.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/skew_normal.py
+-rw-rw-rw-   0 root         (0) root         (0)     3658 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/test_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)      532 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/uniform.py
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/keyrock_math/distribution/weibull.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:34.490643 keyrock-math-2023.7.20.2017/keyrock_math.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-07-20 20:17:34.000000 keyrock-math-2023.7.20.2017/keyrock_math.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      729 2023-07-20 20:17:34.000000 keyrock-math-2023.7.20.2017/keyrock_math.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 20:17:34.000000 keyrock-math-2023.7.20.2017/keyrock_math.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-20 20:17:34.000000 keyrock-math-2023.7.20.2017/keyrock_math.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 20:17:34.000000 keyrock-math-2023.7.20.2017/keyrock_math.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 20:17:22.000000 keyrock-math-2023.7.20.2017/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      171 2023-07-20 20:17:34.493643 keyrock-math-2023.7.20.2017/setup.cfg
```

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/__init__.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/analytic.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/analytic.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/beta.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/beta.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/constant.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/constant.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/distribution.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/distribution.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/gamma.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/gamma.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/log_normal.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/log_normal.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/test_distribution.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/test_distribution.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/uniform.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/uniform.py`

 * *Files identical despite different names*

### Comparing `keyrock-math-2023.5.7.1147/keyrock_math/distribution/weibull.py` & `keyrock-math-2023.7.20.2017/keyrock_math/distribution/weibull.py`

 * *Files identical despite different names*

