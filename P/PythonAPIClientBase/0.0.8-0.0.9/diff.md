# Comparing `tmp/PythonAPIClientBase-0.0.8.tar.gz` & `tmp/PythonAPIClientBase-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonAPIClientBase-0.0.8.tar", last modified: Thu Jul 13 12:31:05 2023, max compression
+gzip compressed data, was "PythonAPIClientBase-0.0.9.tar", last modified: Thu Jul 20 10:05:27 2023, max compression
```

## Comparing `PythonAPIClientBase-0.0.8.tar` & `PythonAPIClientBase-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/
--rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/LICENSE
--rw-rw-r--   0 robert    (1000) robert    (1000)       62 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/MANIFEST.in
--rw-rw-r--   0 robert    (1000) robert    (1000)      343 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PKG-INFO
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PythonAPIClientBase/
--rw-rw-r--   0 robert    (1000) robert    (1000)     4567 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/APIClientBase.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      503 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/LoginSession.py
--rw-rw-r--   0 robert    (1000) robert    (1000)     5911 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/Mock.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      271 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase/__init__.py
--rw-rw-r--   0 robert    (1000) robert    (1000)      497 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PythonAPIClientBase/_version.py
-drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/
--rw-rw-r--   0 robert    (1000) robert    (1000)      343 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/PKG-INFO
--rw-rw-r--   0 robert    (1000) robert    (1000)      483 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/SOURCES.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/dependency_links.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/not-zip-safe
--rw-rw-r--   0 robert    (1000) robert    (1000)       53 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/requires.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       20 2023-07-13 12:31:05.000000 PythonAPIClientBase-0.0.8/PythonAPIClientBase.egg-info/top_level.txt
--rw-rw-r--   0 robert    (1000) robert    (1000)       25 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/README.md
--rw-rw-r--   0 robert    (1000) robert    (1000)      313 2023-07-13 12:31:05.120293 PythonAPIClientBase-0.0.8/setup.cfg
--rw-rw-r--   0 robert    (1000) robert    (1000)      987 2023-07-13 12:30:44.000000 PythonAPIClientBase-0.0.8/setup.py
--rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.8/versioneer.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 10:05:27.613909 PythonAPIClientBase-0.0.9/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     1071 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/LICENSE
+-rw-rw-r--   0 robert    (1000) robert    (1000)       62 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/MANIFEST.in
+-rw-rw-r--   0 robert    (1000) robert    (1000)      343 2023-07-20 10:05:27.613909 PythonAPIClientBase-0.0.9/PKG-INFO
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 10:05:27.613909 PythonAPIClientBase-0.0.9/PythonAPIClientBase/
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5107 2023-07-20 10:04:10.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase/APIClientBase.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      503 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase/LoginSession.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)     5911 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase/Mock.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      271 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase/__init__.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)      497 2023-07-20 10:05:27.613909 PythonAPIClientBase-0.0.9/PythonAPIClientBase/_version.py
+drwxrwxr-x   0 robert    (1000) robert    (1000)        0 2023-07-20 10:05:27.613909 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/
+-rw-rw-r--   0 robert    (1000) robert    (1000)      343 2023-07-20 10:05:27.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/PKG-INFO
+-rw-rw-r--   0 robert    (1000) robert    (1000)      483 2023-07-20 10:05:27.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/SOURCES.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2023-07-20 10:05:27.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/dependency_links.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)        1 2022-07-30 20:28:34.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/not-zip-safe
+-rw-rw-r--   0 robert    (1000) robert    (1000)       53 2023-07-20 10:05:27.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/requires.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       20 2023-07-20 10:05:27.000000 PythonAPIClientBase-0.0.9/PythonAPIClientBase.egg-info/top_level.txt
+-rw-rw-r--   0 robert    (1000) robert    (1000)       25 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/README.md
+-rw-rw-r--   0 robert    (1000) robert    (1000)      313 2023-07-20 10:05:27.613909 PythonAPIClientBase-0.0.9/setup.cfg
+-rw-rw-r--   0 robert    (1000) robert    (1000)      987 2023-07-13 12:30:44.000000 PythonAPIClientBase-0.0.9/setup.py
+-rw-rw-r--   0 robert    (1000) robert    (1000)    68611 2022-07-30 20:25:46.000000 PythonAPIClientBase-0.0.9/versioneer.py
```

### Comparing `PythonAPIClientBase-0.0.8/LICENSE` & `PythonAPIClientBase-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PythonAPIClientBase-0.0.8/PythonAPIClientBase/APIClientBase.py` & `PythonAPIClientBase-0.0.9/PythonAPIClientBase/APIClientBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -119,7 +119,13 @@
     return self.sendRequest(reqFn=requests.post, url=url, loginSession=loginSession, data=data, origin=origin, injectHeadersFn=injectHeadersFn, params=params)
 
   def sendPutRequest(self, url, loginSession, data, origin=None, injectHeadersFn=None, params=None):
     return self.sendRequest(reqFn=requests.put, url=url, loginSession=loginSession, data=data, origin=origin, injectHeadersFn=injectHeadersFn, params=params)
 
   def sendDeleteRequest(self, url, loginSession, data=None, origin=None, injectHeadersFn=None, params=None):
     return self.sendRequest(reqFn=requests.delete, url=url, loginSession=loginSession, data=data, origin=origin, injectHeadersFn=injectHeadersFn, params=params)
+
+  def sendHeadRequest(self, url, loginSession, data=None, origin=None, injectHeadersFn=None, params=None):
+    return self.sendRequest(reqFn=requests.head, url=url, loginSession=loginSession, data=data, origin=origin, injectHeadersFn=injectHeadersFn, params=params)
+
+  def sendOptionsRequest(self, url, loginSession, data=None, origin=None, injectHeadersFn=None, params=None):
+    return self.sendRequest(reqFn=requests.options, url=url, loginSession=loginSession, data=data, origin=origin, injectHeadersFn=injectHeadersFn, params=params)
```

### Comparing `PythonAPIClientBase-0.0.8/PythonAPIClientBase/Mock.py` & `PythonAPIClientBase-0.0.9/PythonAPIClientBase/Mock.py`

 * *Files identical despite different names*

### Comparing `PythonAPIClientBase-0.0.8/setup.py` & `PythonAPIClientBase-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `PythonAPIClientBase-0.0.8/versioneer.py` & `PythonAPIClientBase-0.0.9/versioneer.py`

 * *Files identical despite different names*

