# Comparing `tmp/olympix-test-generator-0.1.tar.gz` & `tmp/olympix-test-generator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympix-test-generator-0.1.tar", last modified: Thu Jul 20 17:57:15 2023, max compression
+gzip compressed data, was "olympix-test-generator-0.2.tar", last modified: Thu Jul 20 18:06:46 2023, max compression
```

## Comparing `olympix-test-generator-0.1.tar` & `olympix-test-generator-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:36:52.353210 olympix-test-generator-0.1/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1603 2023-07-20 18:36:52.351212 olympix-test-generator-0.1/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1081 2023-07-20 18:27:04.000000 olympix-test-generator-0.1/README.md
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:36:52.272562 olympix-test-generator-0.1/olympix-test-generator/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-0.1/olympix-test-generator/__init__.py
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2957 2023-07-20 18:32:54.000000 olympix-test-generator-0.1/olympix-test-generator/client.py
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:36:52.338717 olympix-test-generator-0.1/olympix_test_generator.egg-info/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1603 2023-07-20 18:36:51.000000 olympix-test-generator-0.1/olympix_test_generator.egg-info/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-20 18:36:51.000000 olympix-test-generator-0.1/olympix_test_generator.egg-info/SOURCES.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-20 18:36:51.000000 olympix-test-generator-0.1/olympix_test_generator.egg-info/dependency_links.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-20 18:36:51.000000 olympix-test-generator-0.1/olympix_test_generator.egg-info/entry_points.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-20 18:36:51.000000 olympix-test-generator-0.1/olympix_test_generator.egg-info/requires.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-20 18:36:51.000000 olympix-test-generator-0.1/olympix_test_generator.egg-info/top_level.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-20 18:36:52.354212 olympix-test-generator-0.1/setup.cfg
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      986 2023-07-20 18:28:07.000000 olympix-test-generator-0.1/setup.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:46:22.670911 olympix-test-generator-0.2/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1606 2023-07-20 18:46:22.668912 olympix-test-generator-0.2/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1084 2023-07-20 18:45:11.000000 olympix-test-generator-0.2/README.md
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:46:22.586398 olympix-test-generator-0.2/olympix_test_generator/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-0.2/olympix_test_generator/__init__.py
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2957 2023-07-20 18:32:54.000000 olympix-test-generator-0.2/olympix_test_generator/client.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:46:22.655383 olympix-test-generator-0.2/olympix_test_generator.egg-info/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1606 2023-07-20 18:46:21.000000 olympix-test-generator-0.2/olympix_test_generator.egg-info/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-20 18:46:21.000000 olympix-test-generator-0.2/olympix_test_generator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-20 18:46:21.000000 olympix-test-generator-0.2/olympix_test_generator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-20 18:46:21.000000 olympix-test-generator-0.2/olympix_test_generator.egg-info/entry_points.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-20 18:46:21.000000 olympix-test-generator-0.2/olympix_test_generator.egg-info/requires.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-20 18:46:21.000000 olympix-test-generator-0.2/olympix_test_generator.egg-info/top_level.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-20 18:46:22.671912 olympix-test-generator-0.2/setup.cfg
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      986 2023-07-20 18:46:16.000000 olympix-test-generator-0.2/setup.py
```

### Comparing `olympix-test-generator-0.1/PKG-INFO` & `olympix-test-generator-0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 0.1
+Version: 0.2
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
 
 ## Installation
 
 You can install Olympix Test Generator using pip:
 
 ```bash
-pip install opix-test-generator
+pip install olympix-test-generator
 ```
 
 ## Usage
 
 The package includes a command-line interface for generating tests.
 
 Before running the script, make sure to set the `OPLYMPIX_API_KEY` environment variable in a `.env` file located in the same directory.
```

### Comparing `olympix-test-generator-0.1/README.md` & `olympix-test-generator-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
 
 ## Installation
 
 You can install Olympix Test Generator using pip:
 
 ```bash
-pip install opix-test-generator
+pip install olympix-test-generator
 ```
 
 ## Usage
 
 The package includes a command-line interface for generating tests.
 
 Before running the script, make sure to set the `OPLYMPIX_API_KEY` environment variable in a `.env` file located in the same directory.
```

### Comparing `olympix-test-generator-0.1/olympix-test-generator/client.py` & `olympix-test-generator-0.2/olympix_test_generator/client.py`

 * *Files identical despite different names*

### Comparing `olympix-test-generator-0.1/olympix_test_generator.egg-info/PKG-INFO` & `olympix-test-generator-0.2/olympix_test_generator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 0.1
+Version: 0.2
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 Olympix Test Generator is a Python package designed to assist with the generation of unit tests for Solidity smart contracts. These unit tests are specifically designed to be ran through [Foundry](https://book.getfoundry.sh/), a tool for writing unit tests in Solidity. 
 
 ## Installation
 
 You can install Olympix Test Generator using pip:
 
 ```bash
-pip install opix-test-generator
+pip install olympix-test-generator
 ```
 
 ## Usage
 
 The package includes a command-line interface for generating tests.
 
 Before running the script, make sure to set the `OPLYMPIX_API_KEY` environment variable in a `.env` file located in the same directory.
```

### Comparing `olympix-test-generator-0.1/setup.py` & `olympix-test-generator-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="olympix-test-generator",
-    version="0.1",
+    version="0.2",
     packages=find_packages(),
     author="Evan Fenster",
     author_email="evan@olympix.ai",
     description="Used to auto-generate unit tests for smart contracts using the Forge framework.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/olympix/olympix-test-generator",
```

