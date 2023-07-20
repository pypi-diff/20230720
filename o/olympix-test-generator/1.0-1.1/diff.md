# Comparing `tmp/olympix-test-generator-1.0.tar.gz` & `tmp/olympix-test-generator-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympix-test-generator-1.0.tar", last modified: Thu Jul 20 19:55:28 2023, max compression
+gzip compressed data, was "olympix-test-generator-1.1.tar", last modified: Thu Jul 20 19:57:14 2023, max compression
```

## Comparing `olympix-test-generator-1.0.tar` & `olympix-test-generator-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 20:35:05.050644 olympix-test-generator-1.0/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1574 2023-07-20 20:35:05.049201 olympix-test-generator-1.0/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1052 2023-07-20 20:34:25.000000 olympix-test-generator-1.0/README.md
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 20:35:04.968332 olympix-test-generator-1.0/olympix_test_generator/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-1.0/olympix_test_generator/__init__.py
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2927 2023-07-20 20:07:12.000000 olympix-test-generator-1.0/olympix_test_generator/client.py
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 20:35:05.035828 olympix-test-generator-1.0/olympix_test_generator.egg-info/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1574 2023-07-20 20:35:04.000000 olympix-test-generator-1.0/olympix_test_generator.egg-info/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-20 20:35:04.000000 olympix-test-generator-1.0/olympix_test_generator.egg-info/SOURCES.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-20 20:35:04.000000 olympix-test-generator-1.0/olympix_test_generator.egg-info/dependency_links.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-20 20:35:04.000000 olympix-test-generator-1.0/olympix_test_generator.egg-info/entry_points.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-20 20:35:04.000000 olympix-test-generator-1.0/olympix_test_generator.egg-info/requires.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-20 20:35:04.000000 olympix-test-generator-1.0/olympix_test_generator.egg-info/top_level.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-20 20:35:05.051643 olympix-test-generator-1.0/setup.cfg
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      986 2023-07-20 20:34:57.000000 olympix-test-generator-1.0/setup.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 20:36:51.473928 olympix-test-generator-1.1/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1573 2023-07-20 20:36:51.470928 olympix-test-generator-1.1/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1051 2023-07-20 20:36:15.000000 olympix-test-generator-1.1/README.md
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 20:36:51.389963 olympix-test-generator-1.1/olympix_test_generator/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-1.1/olympix_test_generator/__init__.py
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2927 2023-07-20 20:07:12.000000 olympix-test-generator-1.1/olympix_test_generator/client.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 20:36:51.458418 olympix-test-generator-1.1/olympix_test_generator.egg-info/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1573 2023-07-20 20:36:50.000000 olympix-test-generator-1.1/olympix_test_generator.egg-info/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-20 20:36:50.000000 olympix-test-generator-1.1/olympix_test_generator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-20 20:36:50.000000 olympix-test-generator-1.1/olympix_test_generator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-20 20:36:50.000000 olympix-test-generator-1.1/olympix_test_generator.egg-info/entry_points.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-20 20:36:50.000000 olympix-test-generator-1.1/olympix_test_generator.egg-info/requires.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-20 20:36:50.000000 olympix-test-generator-1.1/olympix_test_generator.egg-info/top_level.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-20 20:36:51.473928 olympix-test-generator-1.1/setup.cfg
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      986 2023-07-20 20:36:43.000000 olympix-test-generator-1.1/setup.py
```

### Comparing `olympix-test-generator-1.0/PKG-INFO` & `olympix-test-generator-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 1.0
+Version: 1.1
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +24,15 @@
 pip install olympix-test-generator
 ```
 
 ## Usage
 
 The package includes a command-line interface for generating tests.
 
-Before running the script, make sure to set the `OPLYMPIX_API_KEY` environment variable in your system.
+Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
 
 To generate a test, run:
 
 ```bash
 olympix generate
 ```
```

### Comparing `olympix-test-generator-1.0/README.md` & `olympix-test-generator-1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 pip install olympix-test-generator
 ```
 
 ## Usage
 
 The package includes a command-line interface for generating tests.
 
-Before running the script, make sure to set the `OPLYMPIX_API_KEY` environment variable in your system.
+Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
 
 To generate a test, run:
 
 ```bash
 olympix generate
 ```
```

### Comparing `olympix-test-generator-1.0/olympix_test_generator/client.py` & `olympix-test-generator-1.1/olympix_test_generator/client.py`

 * *Files identical despite different names*

### Comparing `olympix-test-generator-1.0/olympix_test_generator.egg-info/PKG-INFO` & `olympix-test-generator-1.1/olympix_test_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 1.0
+Version: 1.1
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -24,15 +24,15 @@
 pip install olympix-test-generator
 ```
 
 ## Usage
 
 The package includes a command-line interface for generating tests.
 
-Before running the script, make sure to set the `OPLYMPIX_API_KEY` environment variable in your system.
+Before running the script, make sure to set the `OLYMPIX_API_KEY` environment variable in your system.
 
 To generate a test, run:
 
 ```bash
 olympix generate
 ```
```

### Comparing `olympix-test-generator-1.0/setup.py` & `olympix-test-generator-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="olympix-test-generator",
-    version="1.0",
+    version="1.1",
     packages=find_packages(),
     author="Evan Fenster",
     author_email="evan@olympix.ai",
     description="Used to auto-generate unit tests for smart contracts using the Forge framework.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/olympix/olympix-test-generator",
```

