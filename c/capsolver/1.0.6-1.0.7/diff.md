# Comparing `tmp/capsolver-1.0.6.tar.gz` & `tmp/capsolver-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capsolver-1.0.6.tar", last modified: Mon Jul 10 10:34:26 2023, max compression
+gzip compressed data, was "capsolver-1.0.7.tar", last modified: Thu Jul 20 09:28:09 2023, max compression
```

## Comparing `capsolver-1.0.6.tar` & `capsolver-1.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 10:34:26.348438 capsolver-1.0.6/
--rw-r--r--   0 root         (0) staff       (20)     1075 2023-02-22 02:47:40.000000 capsolver-1.0.6/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     1073 2023-02-22 02:47:24.000000 capsolver-1.0.6/LICENSE.rst
--rw-r--r--   0 root         (0) staff       (20)        0 2023-02-22 02:38:57.000000 capsolver-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)     1892 2023-07-10 10:34:26.348513 capsolver-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1354 2023-02-28 09:18:56.000000 capsolver-1.0.6/README.md
--rw-r--r--   0 root         (0) staff       (20)      106 2023-03-17 11:54:06.000000 capsolver-1.0.6/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)      635 2023-07-10 10:34:26.348828 capsolver-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      904 2023-07-10 10:22:13.000000 capsolver-1.0.6/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 10:34:26.343464 capsolver-1.0.6/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 10:34:26.347472 capsolver-1.0.6/src/capsolver/
--rw-r--r--   0 root         (0) staff       (20)      745 2023-02-28 09:03:32.000000 capsolver-1.0.6/src/capsolver/__init__.py
--rw-r--r--   0 root         (0) staff       (20)       16 2023-02-27 10:53:15.000000 capsolver-1.0.6/src/capsolver/__main__.py
--rw-r--r--   0 root         (0) staff       (20)     5542 2023-04-11 02:58:04.000000 capsolver-1.0.6/src/capsolver/api_requestor.py
--rw-r--r--   0 root         (0) staff       (20)     1492 2023-07-10 10:22:23.000000 capsolver-1.0.6/src/capsolver/capsolver.py
--rw-r--r--   0 root         (0) staff       (20)     3232 2023-02-27 10:23:08.000000 capsolver-1.0.6/src/capsolver/capsolver_object.py
--rw-r--r--   0 root         (0) staff       (20)     3908 2023-06-16 10:03:49.000000 capsolver-1.0.6/src/capsolver/check.py
--rw-r--r--   0 root         (0) staff       (20)      927 2023-02-27 10:13:34.000000 capsolver-1.0.6/src/capsolver/error.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-10 10:34:26.348325 capsolver-1.0.6/src/capsolver.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     1892 2023-07-10 10:34:26.000000 capsolver-1.0.6/src/capsolver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      449 2023-07-10 10:34:26.000000 capsolver-1.0.6/src/capsolver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-10 10:34:26.000000 capsolver-1.0.6/src/capsolver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       17 2023-07-10 10:34:26.000000 capsolver-1.0.6/src/capsolver.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       10 2023-07-10 10:34:26.000000 capsolver-1.0.6/src/capsolver.egg-info/top_level.txt
+drwxr-xr-x   0 lrabbit    (501) staff       (20)        0 2023-07-20 09:28:09.143451 capsolver-1.0.7/
+-rw-r--r--   0 lrabbit    (501) staff       (20)     1075 2023-02-22 02:47:40.000000 capsolver-1.0.7/LICENSE
+-rw-r--r--   0 lrabbit    (501) staff       (20)     1073 2023-02-22 02:47:24.000000 capsolver-1.0.7/LICENSE.rst
+-rw-r--r--   0 lrabbit    (501) staff       (20)        0 2023-02-22 02:38:57.000000 capsolver-1.0.7/MANIFEST.in
+-rw-r--r--   0 lrabbit    (501) staff       (20)     1892 2023-07-20 09:28:09.143519 capsolver-1.0.7/PKG-INFO
+-rw-r--r--   0 lrabbit    (501) staff       (20)     1354 2023-02-28 09:18:56.000000 capsolver-1.0.7/README.md
+-rw-r--r--   0 lrabbit    (501) staff       (20)      106 2023-03-17 11:54:06.000000 capsolver-1.0.7/pyproject.toml
+-rw-r--r--   0 lrabbit    (501) staff       (20)      635 2023-07-20 09:28:09.143832 capsolver-1.0.7/setup.cfg
+-rw-r--r--   0 lrabbit    (501) staff       (20)      904 2023-07-20 09:23:22.000000 capsolver-1.0.7/setup.py
+drwxr-xr-x   0 lrabbit    (501) staff       (20)        0 2023-07-20 09:28:09.138355 capsolver-1.0.7/src/
+drwxr-xr-x   0 lrabbit    (501) staff       (20)        0 2023-07-20 09:28:09.142610 capsolver-1.0.7/src/capsolver/
+-rw-r--r--   0 lrabbit    (501) staff       (20)      745 2023-02-28 09:03:32.000000 capsolver-1.0.7/src/capsolver/__init__.py
+-rw-r--r--   0 lrabbit    (501) staff       (20)       16 2023-02-27 10:53:15.000000 capsolver-1.0.7/src/capsolver/__main__.py
+-rw-r--r--   0 lrabbit    (501) staff       (20)     5511 2023-07-20 09:22:19.000000 capsolver-1.0.7/src/capsolver/api_requestor.py
+-rw-r--r--   0 lrabbit    (501) staff       (20)     1433 2023-07-20 09:22:19.000000 capsolver-1.0.7/src/capsolver/capsolver.py
+-rw-r--r--   0 lrabbit    (501) staff       (20)     3232 2023-02-27 10:23:08.000000 capsolver-1.0.7/src/capsolver/capsolver_object.py
+-rw-r--r--   0 lrabbit    (501) staff       (20)     3908 2023-06-16 10:03:49.000000 capsolver-1.0.7/src/capsolver/check.py
+-rw-r--r--   0 lrabbit    (501) staff       (20)      927 2023-02-27 10:13:34.000000 capsolver-1.0.7/src/capsolver/error.py
+drwxr-xr-x   0 lrabbit    (501) staff       (20)        0 2023-07-20 09:28:09.143341 capsolver-1.0.7/src/capsolver.egg-info/
+-rw-r--r--   0 lrabbit    (501) staff       (20)     1892 2023-07-20 09:28:09.000000 capsolver-1.0.7/src/capsolver.egg-info/PKG-INFO
+-rw-r--r--   0 lrabbit    (501) staff       (20)      449 2023-07-20 09:28:09.000000 capsolver-1.0.7/src/capsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 lrabbit    (501) staff       (20)        1 2023-07-20 09:28:09.000000 capsolver-1.0.7/src/capsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 lrabbit    (501) staff       (20)       17 2023-07-20 09:28:09.000000 capsolver-1.0.7/src/capsolver.egg-info/requires.txt
+-rw-r--r--   0 lrabbit    (501) staff       (20)       10 2023-07-20 09:28:09.000000 capsolver-1.0.7/src/capsolver.egg-info/top_level.txt
```

### Comparing `capsolver-1.0.6/LICENSE` & `capsolver-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/LICENSE.rst` & `capsolver-1.0.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/PKG-INFO` & `capsolver-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver
-Version: 1.0.6
+Version: 1.0.7
 Summary: capsolver python libary
 Home-page: https://github.com/capsolver/capsolver-python
 Author: capsolver
 Author-email: capsolver.com@gmail.com
 Project-URL: Bug Tracker, https://github.com/capsovler/capsovler-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `capsolver-1.0.6/README.md` & `capsolver-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/setup.cfg` & `capsolver-1.0.7/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capsolver
-version = 1.0.6
+version = 1.0.7
 author = capsolver
 author_email = capsolver.com@gmail.com
 description = capsolver python libary
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/capsolver/capsolver-python
 project_urls =
```

### Comparing `capsolver-1.0.6/setup.py` & `capsolver-1.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="capsolver",
-    version="1.0.6",
+    version="1.0.7",
     author="capsolver",
     author_email="capsolver.com@gmail.com",
     description="capsolver python libary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/capsolver/capsolver-python",
     project_urls={
```

### Comparing `capsolver-1.0.6/src/capsolver/__init__.py` & `capsolver-1.0.7/src/capsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/src/capsolver/api_requestor.py` & `capsolver-1.0.7/src/capsolver/api_requestor.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,14 @@
         }
         json_data.update(params)
         headers = self.request_headers(headers)
         if not hasattr(_thread_context, "session"):
             _thread_context.session = _make_session()
         try:
             result = _thread_context.session.request(method, abs_url, headers=headers, json=json_data, timeout=request_timeout if request_timeout else TIMEOUT_SECS)
-            print(result.text)
         except requests.exceptions.Timeout as e:
             raise error.Timeout("Request timed out") from e
         except requests.exceptions.RequestException as e:
             raise error.APIError("Error communicating with capsolver") from e
         return result
 
     def _interpret_response(self, result):
```

### Comparing `capsolver-1.0.6/src/capsolver/capsolver.py` & `capsolver-1.0.7/src/capsolver/capsolver.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     def postTask(cls, params:dict):
         return cls().request("post", "/createTask", {"task":params})
 
     @classmethod
     def getTask(cls, **params):
         for _ in range(_DEFAULT_RETRIES):
             time.sleep(_DEFAULT_INTERVAL)
+            t = time.time()
             r = cls().request("post", "/getTaskResult", params)
-            print("get Task",r)
             if isinstance(r,capsolver.error.CapsolverError):
                 raise r
             if r["status"]=="processing":
                 continue
             if r["status"] =="idle":
                 continue
             return r
@@ -34,20 +34,18 @@
 
     @classmethod
     def solve(cls,params:dict):
         r = cls.postTask(params)
         if isinstance(r, capsolver.error.CapsolverError):
             raise r
         if r['status']=="ready":
-            print("test2",r)
             return r['solution']
         r = cls.getTask(taskId=r['taskId'])
         if isinstance(r, capsolver.error.CapsolverError):
             raise r
-        print("teset1",r)
         return r['solution']
 
 
     @classmethod
     def balance(cls):
         r = cls().request("post", "/getBalance",{})
         return r
```

### Comparing `capsolver-1.0.6/src/capsolver/capsolver_object.py` & `capsolver-1.0.7/src/capsolver/capsolver_object.py`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/src/capsolver/check.py` & `capsolver-1.0.7/src/capsolver/check.py`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/src/capsolver/error.py` & `capsolver-1.0.7/src/capsolver/error.py`

 * *Files identical despite different names*

### Comparing `capsolver-1.0.6/src/capsolver.egg-info/PKG-INFO` & `capsolver-1.0.7/src/capsolver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capsolver
-Version: 1.0.6
+Version: 1.0.7
 Summary: capsolver python libary
 Home-page: https://github.com/capsolver/capsolver-python
 Author: capsolver
 Author-email: capsolver.com@gmail.com
 Project-URL: Bug Tracker, https://github.com/capsovler/capsovler-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

