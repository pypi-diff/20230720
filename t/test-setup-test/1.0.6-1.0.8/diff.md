# Comparing `tmp/test_setup_test-1.0.6.tar.gz` & `tmp/test_setup_test-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_setup_test-1.0.6.tar", last modified: Thu Jul 20 06:13:42 2023, max compression
+gzip compressed data, was "test_setup_test-1.0.8.tar", last modified: Thu Jul 20 06:21:48 2023, max compression
```

## Comparing `test_setup_test-1.0.6.tar` & `test_setup_test-1.0.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-20 06:13:42.299928 test_setup_test-1.0.6/
--rw-rw-r--   0 divy      (1000) divy      (1000)     1009 2023-07-20 06:13:42.299928 test_setup_test-1.0.6/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)       95 2023-07-05 11:00:27.000000 test_setup_test-1.0.6/README.md
--rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-20 06:13:42.299928 test_setup_test-1.0.6/setup.cfg
--rw-rw-r--   0 divy      (1000) divy      (1000)      999 2023-07-20 06:08:29.000000 test_setup_test-1.0.6/setup.py
-drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-20 06:13:42.299928 test_setup_test-1.0.6/test_setup_test.egg-info/
--rw-rw-r--   0 divy      (1000) divy      (1000)     1009 2023-07-20 06:13:42.000000 test_setup_test-1.0.6/test_setup_test.egg-info/PKG-INFO
--rw-rw-r--   0 divy      (1000) divy      (1000)      174 2023-07-20 06:13:42.000000 test_setup_test-1.0.6/test_setup_test.egg-info/SOURCES.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-20 06:13:42.000000 test_setup_test-1.0.6/test_setup_test.egg-info/dependency_links.txt
--rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-20 06:13:42.000000 test_setup_test-1.0.6/test_setup_test.egg-info/top_level.txt
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-20 06:21:48.886737 test_setup_test-1.0.8/
+-rw-rw-r--   0 divy      (1000) divy      (1000)     1009 2023-07-20 06:21:48.886737 test_setup_test-1.0.8/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)       95 2023-07-05 11:00:27.000000 test_setup_test-1.0.8/README.md
+-rw-rw-r--   0 divy      (1000) divy      (1000)       38 2023-07-20 06:21:48.886737 test_setup_test-1.0.8/setup.cfg
+-rw-rw-r--   0 divy      (1000) divy      (1000)      999 2023-07-20 06:21:32.000000 test_setup_test-1.0.8/setup.py
+drwxrwxr-x   0 divy      (1000) divy      (1000)        0 2023-07-20 06:21:48.886737 test_setup_test-1.0.8/test_setup_test.egg-info/
+-rw-rw-r--   0 divy      (1000) divy      (1000)     1009 2023-07-20 06:21:48.000000 test_setup_test-1.0.8/test_setup_test.egg-info/PKG-INFO
+-rw-rw-r--   0 divy      (1000) divy      (1000)      174 2023-07-20 06:21:48.000000 test_setup_test-1.0.8/test_setup_test.egg-info/SOURCES.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-20 06:21:48.000000 test_setup_test-1.0.8/test_setup_test.egg-info/dependency_links.txt
+-rw-rw-r--   0 divy      (1000) divy      (1000)        1 2023-07-20 06:21:48.000000 test_setup_test-1.0.8/test_setup_test.egg-info/top_level.txt
```

### Comparing `test_setup_test-1.0.6/PKG-INFO` & `test_setup_test-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_setup_test
-Version: 1.0.6
+Version: 1.0.8
 Summary: utils_bs_test
 Home-page: UNKNOWN
 Author: Divy TEST
 Author-email: divy.jain@bombaysoftwares.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/utils-bs-test
 Project-URL: Source Code, https://github.com/abc
```

### Comparing `test_setup_test-1.0.6/setup.py` & `test_setup_test-1.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 from setuptools import setup
 
 setup(
     name='test_setup_test',
-    version='1.0.6',
+    version='1.0.8',
     author='Divy TEST',
     author_email='divy.jain@bombaysoftwares.com',
     description='utils_bs_test',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     maintainers=['Maintainer 1', 'Maintainer 2'],
```

### Comparing `test_setup_test-1.0.6/test_setup_test.egg-info/PKG-INFO` & `test_setup_test-1.0.8/test_setup_test.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-setup-test
-Version: 1.0.6
+Version: 1.0.8
 Summary: utils_bs_test
 Home-page: UNKNOWN
 Author: Divy TEST
 Author-email: divy.jain@bombaysoftwares.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/utils-bs-test
 Project-URL: Source Code, https://github.com/abc
```

