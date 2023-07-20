# Comparing `tmp/tortoise-api-0.0.5.tar.gz` & `tmp/tortoise-api-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.0.5.tar", last modified: Thu Jul 20 11:04:21 2023, max compression
+gzip compressed data, was "tortoise-api-0.0.6.tar", last modified: Thu Jul 20 15:51:35 2023, max compression
```

## Comparing `tortoise-api-0.0.5.tar` & `tortoise-api-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 11:04:21.767397 tortoise-api-0.0.5/
--rw-r--r--   0 sol        (501) staff       (20)      259 2023-07-20 11:04:21.767178 tortoise-api-0.0.5/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1237 2023-07-18 09:24:02.000000 tortoise-api-0.0.5/README.md
--rw-r--r--   0 sol        (501) staff       (20)      487 2023-07-15 15:10:57.000000 tortoise-api-0.0.5/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 11:04:21.767459 tortoise-api-0.0.5/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 11:04:21.765488 tortoise-api-0.0.5/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       51 2023-07-19 21:48:58.000000 tortoise-api-0.0.5/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     2773 2023-07-19 21:46:01.000000 tortoise-api-0.0.5/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.5/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 11:04:21.766942 tortoise-api-0.0.5/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      259 2023-07-20 11:04:21.000000 tortoise-api-0.0.5/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      269 2023-07-20 11:04:21.000000 tortoise-api-0.0.5/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 11:04:21.000000 tortoise-api-0.0.5/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       46 2023-07-20 11:04:21.000000 tortoise-api-0.0.5/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 11:04:21.000000 tortoise-api-0.0.5/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 15:51:35.222554 tortoise-api-0.0.6/
+-rw-r--r--   0 sol        (501) staff       (20)      259 2023-07-20 15:51:35.222359 tortoise-api-0.0.6/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1687 2023-07-20 15:47:15.000000 tortoise-api-0.0.6/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      487 2023-07-15 15:10:57.000000 tortoise-api-0.0.6/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 15:51:35.222605 tortoise-api-0.0.6/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 15:51:35.221092 tortoise-api-0.0.6/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       51 2023-07-20 15:50:36.000000 tortoise-api-0.0.6/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     2717 2023-07-20 15:31:46.000000 tortoise-api-0.0.6/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.6/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 15:51:35.222152 tortoise-api-0.0.6/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)      259 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      269 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       46 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.0.5/tortoise_api/api.py` & `tortoise-api-0.0.6/tortoise_api/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from inspect import getmembers
 from os import getenv as env
 from dotenv import load_dotenv
 from starlette.applications import Starlette
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response
 from starlette.routing import Route
 from starlette.templating import Jinja2Templates
@@ -19,53 +18,52 @@
         if self._name in self._meta.db_fields:
             return getattr(self, self._name)
         return self.__repr__()
 
 
 class Api:
     app: Starlette
+    models: {str: Model}
+
     def __init__(
         self,
-        models_module,
         debug: bool = False,
         # auth_provider: AuthProvider = None, # todo: add auth
     ):
         """
         Parameters:
-            models_module: Admin title.
+            debug: Debug SQL queries, api requests
             # auth_provider: Authentication Provider
         """
-        models = getmembers(models_module)
-        self.models: {str: Model} = {k: v for k, v in models if isinstance(v, type(Model)) and v.mro()[0] != Model}
         self.templates = Jinja2Templates("templates")
         self.routes: [Route] = [
             Route('/{model}/{oid}', self.api_one, methods=['GET', 'POST']),
             Route('/favicon.ico', lambda req: Response(), methods=['GET']),  # avoid chrome auto favicon load
             Route('/{model}', self.api_all, methods=['GET', 'POST']),
             Route('/', self.api_menu, methods=['GET']),
         ]
         self.debug = debug
-        self.models_module = models_module
 
-    def start(self):
+    def start(self, models_module):
+        self.models = {key: model for key in dir(models_module) if isinstance(model := getattr(models_module, key), type(Model)) and model.mro()[1]==Model}
         if self.debug:
             logging.basicConfig(level=logging.DEBUG)
         self.app = Starlette(debug=self.debug, routes=self.routes)
         load_dotenv()
-        register_tortoise(self.app, db_url=env("DB_URL"), modules={"models": [self.models_module]}, generate_schemas=self.debug)
+        register_tortoise(self.app, db_url=env("DB_URL"), modules={"models": [models_module]}, generate_schemas=self.debug)
         return self.app
 
     # ROUTES
     async def api_menu(self, _: Request):
         return JSONResponse(list(self.models))
 
     async def api_all(self, request: Request):
         model: Model = self._get_model(request)
-        objects: [{str: Model}] = await model.all().prefetch_related(*model._meta.fetch_fields)
-        data = [jsonify(d) for d in objects]
+        objects: [Model] = await model.all().prefetch_related(*model._meta.fetch_fields)
+        data = [jsonify(obj) for obj in objects]
         return JSONResponse({'data': data})
 
     async def api_one(self, request: Request):
         model: Model = self._get_model(request)
         obj = await self._get_model(request).get(id=request.path_params['oid']).prefetch_related(*model._meta.fetch_fields)
         return JSONResponse(jsonify(obj))
```

### Comparing `tortoise-api-0.0.5/tortoise_api/util.py` & `tortoise-api-0.0.6/tortoise_api/util.py`

 * *Files identical despite different names*

