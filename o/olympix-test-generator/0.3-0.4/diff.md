# Comparing `tmp/olympix-test-generator-0.3.tar.gz` & `tmp/olympix-test-generator-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olympix-test-generator-0.3.tar", last modified: Thu Jul 20 18:19:04 2023, max compression
+gzip compressed data, was "olympix-test-generator-0.4.tar", last modified: Thu Jul 20 18:21:32 2023, max compression
```

## Comparing `olympix-test-generator-0.3.tar` & `olympix-test-generator-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:58:40.732623 olympix-test-generator-0.3/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1606 2023-07-20 18:58:40.730614 olympix-test-generator-0.3/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1084 2023-07-20 18:45:11.000000 olympix-test-generator-0.3/README.md
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:58:40.644554 olympix-test-generator-0.3/olympix_test_generator/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-0.3/olympix_test_generator/__init__.py
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2911 2023-07-20 18:58:33.000000 olympix-test-generator-0.3/olympix_test_generator/client.py
-drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 18:58:40.718419 olympix-test-generator-0.3/olympix_test_generator.egg-info/
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1606 2023-07-20 18:58:39.000000 olympix-test-generator-0.3/olympix_test_generator.egg-info/PKG-INFO
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-20 18:58:40.000000 olympix-test-generator-0.3/olympix_test_generator.egg-info/SOURCES.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-20 18:58:39.000000 olympix-test-generator-0.3/olympix_test_generator.egg-info/dependency_links.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-20 18:58:39.000000 olympix-test-generator-0.3/olympix_test_generator.egg-info/entry_points.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-20 18:58:39.000000 olympix-test-generator-0.3/olympix_test_generator.egg-info/requires.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-20 18:58:39.000000 olympix-test-generator-0.3/olympix_test_generator.egg-info/top_level.txt
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-20 18:58:40.733622 olympix-test-generator-0.3/setup.cfg
--rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      986 2023-07-20 18:58:13.000000 olympix-test-generator-0.3/setup.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 19:01:09.079611 olympix-test-generator-0.4/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1606 2023-07-20 19:01:09.077698 olympix-test-generator-0.4/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1084 2023-07-20 18:45:11.000000 olympix-test-generator-0.4/README.md
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 19:01:08.995882 olympix-test-generator-0.4/olympix_test_generator/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 16:57:55.000000 olympix-test-generator-0.4/olympix_test_generator/__init__.py
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     2899 2023-07-20 19:00:33.000000 olympix-test-generator-0.4/olympix_test_generator/client.py
+drwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        0 2023-07-20 19:01:09.064699 olympix-test-generator-0.4/olympix_test_generator.egg-info/
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)     1606 2023-07-20 19:01:08.000000 olympix-test-generator-0.4/olympix_test_generator.egg-info/PKG-INFO
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      364 2023-07-20 19:01:08.000000 olympix-test-generator-0.4/olympix_test_generator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)        1 2023-07-20 19:01:08.000000 olympix-test-generator-0.4/olympix_test_generator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       63 2023-07-20 19:01:08.000000 olympix-test-generator-0.4/olympix_test_generator.egg-info/entry_points.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      203 2023-07-20 19:01:08.000000 olympix-test-generator-0.4/olympix_test_generator.egg-info/requires.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       23 2023-07-20 19:01:08.000000 olympix-test-generator-0.4/olympix_test_generator.egg-info/top_level.txt
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)       38 2023-07-20 19:01:09.080618 olympix-test-generator-0.4/setup.cfg
+-rwxrwxrwx   0 evanfen   (1000) evanfen   (1000)      986 2023-07-20 19:00:59.000000 olympix-test-generator-0.4/setup.py
```

### Comparing `olympix-test-generator-0.3/PKG-INFO` & `olympix-test-generator-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 0.3
+Version: 0.4
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `olympix-test-generator-0.3/README.md` & `olympix-test-generator-0.4/README.md`

 * *Files identical despite different names*

### Comparing `olympix-test-generator-0.3/olympix_test_generator/client.py` & `olympix-test-generator-0.4/olympix_test_generator/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 opix_api_key = ""
 
 def get_opix_api_key() -> bool:
     global opix_api_key  # Use global variable
 
     opix_api_key = os.getenv('OLYMPIX_API_KEY')
     if opix_api_key is None:
-        print("'OLYMPIX_API_KEY' not found in .env file")
+        print("'OLYMPIX_API_KEY' not found.")
         return False
     else:
         select_sol_file()
         return True
 
 def select_sol_file():
     global file_content, contract_name, function_name  # Use global variables
```

### Comparing `olympix-test-generator-0.3/olympix_test_generator.egg-info/PKG-INFO` & `olympix-test-generator-0.4/olympix_test_generator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olympix-test-generator
-Version: 0.3
+Version: 0.4
 Summary: Used to auto-generate unit tests for smart contracts using the Forge framework.
 Home-page: https://github.com/olympix/olympix-test-generator
 Author: Evan Fenster
 Author-email: evan@olympix.ai
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `olympix-test-generator-0.3/setup.py` & `olympix-test-generator-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="olympix-test-generator",
-    version="0.3",
+    version="0.4",
     packages=find_packages(),
     author="Evan Fenster",
     author_email="evan@olympix.ai",
     description="Used to auto-generate unit tests for smart contracts using the Forge framework.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/olympix/olympix-test-generator",
```

