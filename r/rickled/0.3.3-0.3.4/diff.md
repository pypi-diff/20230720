# Comparing `tmp/rickled-0.3.3.tar.gz` & `tmp/rickled-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rickled-0.3.3.tar", last modified: Thu Jul 20 20:51:45 2023, max compression
+gzip compressed data, was "dist\rickled-0.3.4.tar", last modified: Thu Jul 20 21:34:12 2023, max compression
```

## Comparing `rickled-0.3.3.tar` & `rickled-0.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 20:51:45.000000 rickled-0.3.3/
--rw-rw-rw-   0        0        0    11357 2021-12-06 14:18:08.000000 rickled-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     6475 2023-07-20 20:51:45.000000 rickled-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     7051 2022-08-15 15:51:56.000000 rickled-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled/
--rw-rw-rw-   0        0        0    50289 2023-04-06 21:36:35.000000 rickled-0.3.3/rickled/__init__.py
--rw-rw-rw-   0        0        0       48 2023-07-20 20:51:44.000000 rickled-0.3.3/rickled/__version__.py
--rw-rw-rw-   0        0        0     2049 2023-04-29 09:20:08.000000 rickled-0.3.3/rickled/net.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/
--rw-rw-rw-   0        0        0     6475 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-20 20:51:45.000000 rickled-0.3.3/rickled.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2023-07-20 20:51:45.000000 rickled-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2074 2023-07-20 20:48:40.000000 rickled-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:51:45.000000 rickled-0.3.3/tests/
-drwxrwxrwx   0        0        0        0 2023-07-20 20:51:45.000000 rickled-0.3.3/tests/integration/
--rw-rw-rw-   0        0        0        0 2021-12-06 14:18:08.000000 rickled-0.3.3/tests/integration/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 20:51:45.000000 rickled-0.3.3/tests/unittest/
--rw-rw-rw-   0        0        0        0 2022-03-13 15:27:46.000000 rickled-0.3.3/tests/unittest/__init__.py
--rw-rw-rw-   0        0        0     7819 2023-04-06 21:55:53.000000 rickled-0.3.3/tests/unittest/test_advanced.py
--rw-rw-rw-   0        0        0      630 2023-07-20 20:51:27.000000 rickled-0.3.3/tests/unittest/test_net.py
--rw-rw-rw-   0        0        0     1717 2023-01-18 22:01:25.000000 rickled-0.3.3/tests/unittest/test_object_rickler.py
--rw-rw-rw-   0        0        0    10648 2023-04-02 21:25:40.000000 rickled-0.3.3/tests/unittest/test_rickle.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:34:12.000000 rickled-0.3.4/
+-rw-rw-rw-   0        0        0    11357 2021-12-06 14:18:08.000000 rickled-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     6504 2023-07-20 21:34:12.000000 rickled-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7051 2022-08-15 15:51:56.000000 rickled-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled/
+-rw-rw-rw-   0        0        0    50289 2023-04-06 21:36:35.000000 rickled-0.3.4/rickled/__init__.py
+-rw-rw-rw-   0        0        0       48 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled/__version__.py
+-rw-rw-rw-   0        0        0     2285 2023-07-20 21:22:06.000000 rickled-0.3.4/rickled/net.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/
+-rw-rw-rw-   0        0        0     6504 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-20 21:34:12.000000 rickled-0.3.4/rickled.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2023-07-20 21:34:12.000000 rickled-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2124 2023-07-20 21:32:11.000000 rickled-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:34:12.000000 rickled-0.3.4/tests/
+drwxrwxrwx   0        0        0        0 2023-07-20 21:34:12.000000 rickled-0.3.4/tests/integration/
+-rw-rw-rw-   0        0        0        0 2021-12-06 14:18:08.000000 rickled-0.3.4/tests/integration/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-20 21:34:12.000000 rickled-0.3.4/tests/unittest/
+-rw-rw-rw-   0        0        0        0 2022-03-13 15:27:46.000000 rickled-0.3.4/tests/unittest/__init__.py
+-rw-rw-rw-   0        0        0     7819 2023-04-06 21:55:53.000000 rickled-0.3.4/tests/unittest/test_advanced.py
+-rw-rw-rw-   0        0        0      630 2023-07-20 20:51:27.000000 rickled-0.3.4/tests/unittest/test_net.py
+-rw-rw-rw-   0        0        0     1717 2023-01-18 22:01:25.000000 rickled-0.3.4/tests/unittest/test_object_rickler.py
+-rw-rw-rw-   0        0        0    10648 2023-04-02 21:25:40.000000 rickled-0.3.4/tests/unittest/test_rickle.py
```

### Comparing `rickled-0.3.3/LICENSE` & `rickled-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rickled-0.3.3/PKG-INFO` & `rickled-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rickled
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools for pickling Python objects in a completely different way
 Home-page: https://github.com/Zipfian-Science/rickled
 Author: Zipfian Science
 Author-email: about@zipfian.science
 License: Apache 2.0
 Download-URL: https://github.com/Zipfian-Science/rickled/archive/v_01.tar.gz
 Keywords: Pickle,Python
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: twisted
+Provides-Extra: twisted,ssl
 License-File: LICENSE
 
 # Rickled
 ```
                                       ....                                      
                                 &((((((((((((((%,                               
                               #(*,*((//(((((((((((%.                            
@@ -155,11 +156,11 @@
 >> config.BASIC.callable_lambda()
 'hell world!'
 ```
 
 ## Release
 
 - Date: 2023-07-20
-- Version: 0.3.3
+- Version: 0.3.4
```

### Comparing `rickled-0.3.3/README.md` & `rickled-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `rickled-0.3.3/rickled/__init__.py` & `rickled-0.3.4/rickled/__init__.py`

 * *Files identical despite different names*

### Comparing `rickled-0.3.3/rickled/net.py` & `rickled-0.3.4/rickled/net.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 from rickled import Rickle
 
 try:
     from twisted.web import server, resource
     from twisted.internet import reactor, endpoints, ssl
 except ModuleNotFoundError as exc:
     warnings.warn('Required Python package not found.', ImportWarning)
-    raise exc
 except ImportError as exc:
     warnings.warn('Required Python package "twisted" not found.', ImportWarning)
-    raise exc
+
+try:
+    from twisted.internet import ssl
+except ModuleNotFoundError as exc:
+    warnings.warn('Required Python package not found.', ImportWarning)
+except ImportError as exc:
+    warnings.warn('Required Python package "pyopenssl" not found.', ImportWarning)
 
 
 class HttpResource(resource.Resource):
     isLeaf = True
     numberRequests = 0
 
     def __init__(self, rickle):
```

### Comparing `rickled-0.3.3/rickled.egg-info/PKG-INFO` & `rickled-0.3.4/rickled.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rickled
-Version: 0.3.3
+Version: 0.3.4
 Summary: Tools for pickling Python objects in a completely different way
 Home-page: https://github.com/Zipfian-Science/rickled
 Author: Zipfian Science
 Author-email: about@zipfian.science
 License: Apache 2.0
 Download-URL: https://github.com/Zipfian-Science/rickled/archive/v_01.tar.gz
 Keywords: Pickle,Python
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 Provides-Extra: twisted
+Provides-Extra: twisted,ssl
 License-File: LICENSE
 
 # Rickled
 ```
                                       ....                                      
                                 &((((((((((((((%,                               
                               #(*,*((//(((((((((((%.                            
@@ -155,11 +156,11 @@
 >> config.BASIC.callable_lambda()
 'hell world!'
 ```
 
 ## Release
 
 - Date: 2023-07-20
-- Version: 0.3.3
+- Version: 0.3.4
```

### Comparing `rickled-0.3.3/setup.py` & `rickled-0.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,16 @@
     url='https://github.com/Zipfian-Science/rickled',
     download_url='https://github.com/Zipfian-Science/rickled/archive/v_01.tar.gz',
     packages=find_packages(".", exclude=("tests", "dist", "deploy", "egg-info")),
     include_package_data=True,
     install_requires=pipreq,
     package_dir={'.': 'rickled'},
     extras_require = {
-        'twisted':  ['twisted']
+        'twisted':  ['twisted'],
+        'twisted,ssl':  ['twisted', 'pyopenssl']
     },
     classifiers=[
             'Intended Audience :: Science/Research',
             'Operating System :: OS Independent',
             'Programming Language :: Python :: 3',
             'Topic :: Scientific/Engineering :: Artificial Intelligence']
 )
```

### Comparing `rickled-0.3.3/tests/unittest/test_advanced.py` & `rickled-0.3.4/tests/unittest/test_advanced.py`

 * *Files identical despite different names*

### Comparing `rickled-0.3.3/tests/unittest/test_net.py` & `rickled-0.3.4/tests/unittest/test_net.py`

 * *Files identical despite different names*

### Comparing `rickled-0.3.3/tests/unittest/test_object_rickler.py` & `rickled-0.3.4/tests/unittest/test_object_rickler.py`

 * *Files identical despite different names*

### Comparing `rickled-0.3.3/tests/unittest/test_rickle.py` & `rickled-0.3.4/tests/unittest/test_rickle.py`

 * *Files identical despite different names*

