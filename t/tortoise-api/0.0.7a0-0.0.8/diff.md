# Comparing `tmp/tortoise-api-0.0.7a0.tar.gz` & `tmp/tortoise-api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.0.7a0.tar", last modified: Thu Jul 20 17:20:28 2023, max compression
+gzip compressed data, was "tortoise-api-0.0.8.tar", last modified: Thu Jul 20 18:36:00 2023, max compression
```

## Comparing `tortoise-api-0.0.7a0.tar` & `tortoise-api-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 17:20:28.635501 tortoise-api-0.0.7a0/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.7a0/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     3640 2023-07-20 17:20:28.635271 tortoise-api-0.0.7a0/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.7a0/README.md
--rw-r--r--   0 sol        (501) staff       (20)      674 2023-07-20 17:20:19.000000 tortoise-api-0.0.7a0/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 17:20:28.635561 tortoise-api-0.0.7a0/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 17:20:28.633858 tortoise-api-0.0.7a0/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       28 2023-07-20 15:57:11.000000 tortoise-api-0.0.7a0/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     2717 2023-07-20 15:31:46.000000 tortoise-api-0.0.7a0/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.7a0/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 17:20:28.634992 tortoise-api-0.0.7a0/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     3640 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       54 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:36:00.200544 tortoise-api-0.0.8/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.8/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2412 2023-07-20 18:36:00.200252 tortoise-api-0.0.8/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.8/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      695 2023-07-20 18:32:45.000000 tortoise-api-0.0.8/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 18:36:00.200617 tortoise-api-0.0.8/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:36:00.198330 tortoise-api-0.0.8/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.0.8/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     2521 2023-07-20 18:22:34.000000 tortoise-api-0.0.8/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.8/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:36:00.199935 tortoise-api-0.0.8/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2412 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       73 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.0.7a0/LICENSE` & `tortoise-api-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.7a0/README.md` & `tortoise-api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.7a0/pyproject.toml` & `tortoise-api-0.0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 requires-python = ">=3.9"
 authors = [
     {name = "Artemiev", email = "mixartemev@gmail.com"},
 ]
 keywords = ["starlette", "fastapi", "admin", "dashboard", "datatables", "crud", "tortoise-orm", "ASGI-admin"]
 description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
-license = {file = "LICENSE"}
+license = {text = "MIT"}
 dependencies = [
     "python-dotenv",
     "starlette",
+    "tortoise-api-model",
     "tortoise-orm[asyncpg]",
     "uvicorn"
 ]
-version = "0.0.7a"
+version = "0.0.8"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.0.7a0/tortoise_api/api.py` & `tortoise-api-0.0.8/tortoise_api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,20 @@
 from os import getenv as env
 from dotenv import load_dotenv
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
 from starlette.routing import Route
 from starlette.templating import Jinja2Templates
-from tortoise import Model as BaseModel
 from tortoise.contrib.starlette import register_tortoise
+from tortoise_api_model import Model
 
 from tortoise_api.util import jsonify
 
 
-class Model(BaseModel):
-    _name: str = 'name'
-    def repr(self):
-        if self._name in self._meta.db_fields:
-            return getattr(self, self._name)
-        return self.__repr__()
-
-
 class Api:
     app: Starlette
     models: {str: Model}
 
     def __init__(
         self,
         debug: bool = False,
```

### Comparing `tortoise-api-0.0.7a0/tortoise_api/util.py` & `tortoise-api-0.0.8/tortoise_api/util.py`

 * *Files identical despite different names*

