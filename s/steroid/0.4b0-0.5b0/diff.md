# Comparing `tmp/steroid-0.4b0.tar.gz` & `tmp/steroid-0.5b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steroid-0.4b0.tar", max compression
+gzip compressed data, was "steroid-0.5b0.tar", max compression
```

## Comparing `steroid-0.4b0.tar` & `steroid-0.5b0.tar`

### file list

```diff
@@ -1,7 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-07-18 18:58:31.444535 steroid-0.4b0/LICENSE
--rw-r--r--   0        0        0       69 2023-07-18 18:58:31.444535 steroid-0.4b0/README.md
--rw-r--r--   0        0        0      803 2023-07-18 18:58:57.988668 steroid-0.4b0/pyproject.toml
--rw-r--r--   0        0        0      806 2023-07-18 18:58:31.444535 steroid-0.4b0/steroid/app.py
--rw-r--r--   0        0        0     1924 2023-07-18 18:58:31.444535 steroid-0.4b0/steroid/common.py
--rw-r--r--   0        0        0      313 2023-07-18 18:58:31.444535 steroid-0.4b0/steroid/utils.py
--rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 steroid-0.4b0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-20 14:49:56.441029 steroid-0.5b0/LICENSE
+-rw-r--r--   0        0        0       69 2023-07-20 14:49:56.441029 steroid-0.5b0/README.md
+-rw-r--r--   0        0        0      803 2023-07-20 14:50:24.742405 steroid-0.5b0/pyproject.toml
+-rw-r--r--   0        0        0      164 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/__init__.py
+-rw-r--r--   0        0        0     1689 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/app.py
+-rw-r--r--   0        0        0     1112 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/controller.py
+-rw-r--r--   0        0        0      971 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/logging.py
+-rw-r--r--   0        0        0     1706 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/methods.py
+-rw-r--r--   0        0        0     1808 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/middleware.py
+-rw-r--r--   0        0        0      485 2023-07-20 14:49:56.441029 steroid-0.5b0/steroid/utils.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 steroid-0.5b0/PKG-INFO
```

### Comparing `steroid-0.4b0/LICENSE` & `steroid-0.5b0/LICENSE`

 * *Files identical despite different names*

### Comparing `steroid-0.4b0/pyproject.toml` & `steroid-0.5b0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "steroid"
-version = "v0.4b"
+version = "v0.5b"
 authors = [
   "Mohammed Al Ameen <ameenmohammed2311@gmail.com>"
 ]
 description = "Steroid"
 readme = "README.md"
 
 repository = "https://github.com/struckchure/steroid"
```

### Comparing `steroid-0.4b0/steroid/common.py` & `steroid-0.5b0/steroid/methods.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,23 @@
 import inspect
-from typing import Any
-
-from fastapi.routing import APIRouter
 
 from steroid.utils import formatPath
 
 
-class Controller:
-    def __init__(self, path: str = "", *args, **kwargs):
-        self.router = APIRouter()
-
-        self.path = formatPath(path)
-
-        self.args = args
-        self.kwargs = kwargs
-
-    def __call__(self, cls):
-        setattr(cls, "path", self.path)
-        setattr(cls, "router", self.router)
-
-        for name, method in cls.__dict__.items():
-            methodClass = getattr(method, "object", None)
-            if isinstance(methodClass, Method):
-                methodClass.register(self.router)
-
-        return cls(*self.args, **self.kwargs)
-
-
-class Method:
+class BaseMethod:
     _METHOD: str
 
     def __init__(self, path: str = "", *args, **kwargs):
         self.path = formatPath(path)
 
         self.args = args
         self.kwargs = kwargs
 
         self.route = None
 
-    def register(self, router):
-        self.__call__(self.func, router)
-
     def __call__(self, func, router=None):
         # TODO: alot feels very wrong in this method, help me!
 
         self.func = func
 
         if router:
             httpMethodDecorator = getattr(router, self._METHOD.lower())
@@ -64,20 +37,44 @@
         def wrapper(*args, **kwargs):
             return func(*args, **kwargs)
 
         setattr(wrapper, "object", self)
 
         return wrapper
 
+    def mapSelfToRouter(self, router):
+        self.__call__(self.func, router)
+
 
-class Get(Method):
+class Get(BaseMethod):
     _METHOD = "GET"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
-class Post(Method):
+class Post(BaseMethod):
     _METHOD = "POST"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
+
+
+class Put(BaseMethod):
+    _METHOD = "PUT"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class Patch(BaseMethod):
+    _METHOD = "PATCH"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class Delete(BaseMethod):
+    _METHOD = "DELETE"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
```

### Comparing `steroid-0.4b0/PKG-INFO` & `steroid-0.5b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steroid
-Version: 0.4b0
+Version: 0.5b0
 Summary: Steroid
 Home-page: https://github.com/struckchure/steroid
 Author: Mohammed Al Ameen
 Author-email: ameenmohammed2311@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -25,11 +25,11 @@
 Requires-Dist: sniffio (==1.3.0)
 Requires-Dist: starlette (==0.27.0)
 Requires-Dist: typing-extensions (==4.7.1)
 Requires-Dist: uvicorn (==0.23.0)
 Project-URL: Repository, https://github.com/struckchure/steroid
 Description-Content-Type: text/markdown
 
-# steriod
+# steroid
 
 NestJs like framework for python, built on top of FastAPI
```

