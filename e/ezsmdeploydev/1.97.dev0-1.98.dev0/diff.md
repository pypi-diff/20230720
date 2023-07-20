# Comparing `tmp/ezsmdeploydev-1.97.dev0.tar.gz` & `tmp/ezsmdeploydev-1.98.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsmdeploydev-1.97.dev0.tar", last modified: Thu Jul 20 19:00:13 2023, max compression
+gzip compressed data, was "ezsmdeploydev-1.98.dev0.tar", last modified: Thu Jul 20 19:35:17 2023, max compression
```

## Comparing `ezsmdeploydev-1.97.dev0.tar` & `ezsmdeploydev-1.98.dev0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:00:13.471760 ezsmdeploydev-1.97.dev0/
--rw-r--r--   0 chethan   (1000) chethan   (1000)       26 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/MANIFEST.in
--rw-r--r--   0 chethan   (1000) chethan   (1000)    19601 2023-07-20 19:00:13.471760 ezsmdeploydev-1.97.dev0/PKG-INFO
--rw-r--r--   0 chethan   (1000) chethan   (1000)    19108 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/README.rst
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:00:13.441760 ezsmdeploydev-1.97.dev0/ezsmdeploy/
--rw-r--r--   0 chethan   (1000) chethan   (1000)    48494 2023-07-20 18:59:01.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/__init__.py
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:00:13.451760 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/
--rw-r--r--   0 chethan   (1000) chethan   (1000)     2100 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/Dockerfile
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1934 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/Dockerfile_flask
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1390 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/build-docker.sh
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1603 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/conversation.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1361 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/cost.csv
--rw-r--r--   0 chethan   (1000) chethan   (1000)      884 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/dockerd-entrypoint.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      576 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/instancetypes.csv
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1797 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/model_handler.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      719 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/nginx.conf
--rw-r--r--   0 chethan   (1000) chethan   (1000)     2090 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/predictor.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)     2429 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/serve
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1409 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/smlocust.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      432 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/train
--rw-r--r--   0 chethan   (1000) chethan   (1000)      202 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/data/wsgi.py
--rw-r--r--   0 chethan   (1000) chethan   (1000)      733 2023-07-20 18:56:41.000000 ezsmdeploydev-1.97.dev0/ezsmdeploy/modelscript_sklearn.py
-drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:00:13.471760 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/
--rw-r--r--   0 chethan   (1000) chethan   (1000)    19601 2023-07-20 19:00:13.000000 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/PKG-INFO
--rw-r--r--   0 chethan   (1000) chethan   (1000)      714 2023-07-20 19:00:13.000000 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/SOURCES.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 19:00:13.000000 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/dependency_links.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 19:00:13.000000 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/not-zip-safe
--rw-r--r--   0 chethan   (1000) chethan   (1000)      129 2023-07-20 19:00:13.000000 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/requires.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)       11 2023-07-20 19:00:13.000000 ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/top_level.txt
--rw-r--r--   0 chethan   (1000) chethan   (1000)       38 2023-07-20 19:00:13.471760 ezsmdeploydev-1.97.dev0/setup.cfg
--rw-r--r--   0 chethan   (1000) chethan   (1000)     1277 2023-07-20 18:59:29.000000 ezsmdeploydev-1.97.dev0/setup.py
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)       26 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/MANIFEST.in
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    19601 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/PKG-INFO
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    19108 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/README.rst
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.540236 ezsmdeploydev-1.98.dev0/ezsmdeploy/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    48494 2023-07-20 19:34:03.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/__init__.py
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.540236 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     2100 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1934 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile_flask
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1390 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/build-docker.sh
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1603 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/conversation.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1361 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/cost.csv
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      884 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/dockerd-entrypoint.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      576 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/instancetypes.csv
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1797 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/model_handler.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      719 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/nginx.conf
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     2090 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/predictor.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     2429 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/serve
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1409 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/smlocust.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      432 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/train
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      202 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/data/wsgi.py
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      733 2023-07-20 18:56:41.000000 ezsmdeploydev-1.98.dev0/ezsmdeploy/modelscript_sklearn.py
+drwxr-xr-x   0 chethan   (1000) chethan   (1000)        0 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/
+-rw-r--r--   0 chethan   (1000) chethan   (1000)    19601 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/PKG-INFO
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      714 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/SOURCES.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/dependency_links.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)        1 2023-07-20 19:35:05.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/not-zip-safe
+-rw-r--r--   0 chethan   (1000) chethan   (1000)      129 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/requires.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)       11 2023-07-20 19:35:17.000000 ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/top_level.txt
+-rw-r--r--   0 chethan   (1000) chethan   (1000)       38 2023-07-20 19:35:17.550236 ezsmdeploydev-1.98.dev0/setup.cfg
+-rw-r--r--   0 chethan   (1000) chethan   (1000)     1277 2023-07-20 19:34:59.000000 ezsmdeploydev-1.98.dev0/setup.py
```

### Comparing `ezsmdeploydev-1.97.dev0/PKG-INFO` & `ezsmdeploydev-1.98.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploydev
-Version: 1.97.dev0
+Version: 1.98.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ezsmdeploydev-1.97.dev0/README.rst` & `ezsmdeploydev-1.98.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/__init__.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/__init__.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/Dockerfile` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/Dockerfile_flask` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/Dockerfile_flask`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/build-docker.sh` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/build-docker.sh`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/conversation.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/conversation.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/cost.csv` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/cost.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/dockerd-entrypoint.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/dockerd-entrypoint.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/instancetypes.csv` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/instancetypes.csv`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/model_handler.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/model_handler.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/nginx.conf` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/nginx.conf`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/predictor.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/predictor.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/serve` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/serve`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/data/smlocust.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/data/smlocust.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploy/modelscript_sklearn.py` & `ezsmdeploydev-1.98.dev0/ezsmdeploy/modelscript_sklearn.py`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/PKG-INFO` & `ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsmdeploydev
-Version: 1.97.dev0
+Version: 1.98.dev0
 Summary: SageMaker custom deployments made easy
 Home-page: https://pypi.python.org/pypi/ezsmdeploy
 Author: Shreyas Subramanian
 Author-email: subshrey@amazon.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ezsmdeploydev-1.97.dev0/ezsmdeploydev.egg-info/SOURCES.txt` & `ezsmdeploydev-1.98.dev0/ezsmdeploydev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezsmdeploydev-1.97.dev0/setup.py` & `ezsmdeploydev-1.98.dev0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 extras = {
     'locust': [
         'locustio==0.14.5'
     ]
 }
 
 setup(name='ezsmdeploydev',
-      version='1.97dev',
+      version='1.98dev',
       description='SageMaker custom deployments made easy',
       url='https://pypi.python.org/pypi/ezsmdeploy',
       #scripts=['Dockerfile','dockerd-entrypoint.py','model_handler.py','build-docker.sh'],
       author='Shreyas Subramanian',
       author_email='subshrey@amazon.com',
       license='MIT',
       packages=['ezsmdeploy'],
```

