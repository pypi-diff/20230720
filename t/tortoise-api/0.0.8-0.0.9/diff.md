# Comparing `tmp/tortoise-api-0.0.8.tar.gz` & `tmp/tortoise-api-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.0.8.tar", last modified: Thu Jul 20 18:36:00 2023, max compression
+gzip compressed data, was "tortoise-api-0.0.9.tar", last modified: Thu Jul 20 18:57:06 2023, max compression
```

## Comparing `tortoise-api-0.0.8.tar` & `tortoise-api-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:36:00.200544 tortoise-api-0.0.8/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.8/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     2412 2023-07-20 18:36:00.200252 tortoise-api-0.0.8/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.8/README.md
--rw-r--r--   0 sol        (501) staff       (20)      695 2023-07-20 18:32:45.000000 tortoise-api-0.0.8/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 18:36:00.200617 tortoise-api-0.0.8/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:36:00.198330 tortoise-api-0.0.8/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.0.8/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     2521 2023-07-20 18:22:34.000000 tortoise-api-0.0.8/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.8/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:36:00.199935 tortoise-api-0.0.8/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     2412 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       73 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 18:36:00.000000 tortoise-api-0.0.8/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:57:06.007869 tortoise-api-0.0.9/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.9/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     2412 2023-07-20 18:57:06.007633 tortoise-api-0.0.9/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.9/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      681 2023-07-20 18:56:34.000000 tortoise-api-0.0.9/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 18:57:06.007928 tortoise-api-0.0.9/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:57:06.005363 tortoise-api-0.0.9/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       21 2023-07-20 18:33:16.000000 tortoise-api-0.0.9/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     2521 2023-07-20 18:22:34.000000 tortoise-api-0.0.9/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.9/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 18:57:06.007350 tortoise-api-0.0.9/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     2412 2023-07-20 18:57:05.000000 tortoise-api-0.0.9/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 18:57:06.000000 tortoise-api-0.0.9/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 18:57:05.000000 tortoise-api-0.0.9/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       59 2023-07-20 18:57:05.000000 tortoise-api-0.0.9/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 18:57:05.000000 tortoise-api-0.0.9/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.0.8/LICENSE` & `tortoise-api-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.8/PKG-INFO` & `tortoise-api-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

### Comparing `tortoise-api-0.0.8/README.md` & `tortoise-api-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.8/pyproject.toml` & `tortoise-api-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     {name = "Artemiev", email = "mixartemev@gmail.com"},
 ]
 keywords = ["starlette", "fastapi", "admin", "dashboard", "datatables", "crud", "tortoise-orm", "ASGI-admin"]
 description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
 license = {text = "MIT"}
 dependencies = [
+    "asyncpg",
     "python-dotenv",
     "starlette",
     "tortoise-api-model",
-    "tortoise-orm[asyncpg]",
     "uvicorn"
 ]
-version = "0.0.8"
+version = "0.0.9"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.0.8/tortoise_api/api.py` & `tortoise-api-0.0.9/tortoise_api/api.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.8/tortoise_api/util.py` & `tortoise-api-0.0.9/tortoise_api/util.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.8/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.0.9/tortoise_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/mixartemev/tortoise-api
 Project-URL: Repository, https://github.com/mixartemev/tortoise-api
 Keywords: starlette,fastapi,admin,dashboard,datatables,crud,tortoise-orm,ASGI-admin
 Requires-Python: >=3.9
```

