# Comparing `tmp/tortoise-api-0.0.7.tar.gz` & `tmp/tortoise-api-0.0.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.0.7.tar", last modified: Thu Jul 20 16:28:24 2023, max compression
+gzip compressed data, was "tortoise-api-0.0.7a0.tar", last modified: Thu Jul 20 17:20:28 2023, max compression
```

## Comparing `tortoise-api-0.0.7.tar` & `tortoise-api-0.0.7a0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 16:28:24.722657 tortoise-api-0.0.7/
--rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.7/LICENSE
--rw-r--r--   0 sol        (501) staff       (20)     3556 2023-07-20 16:28:24.722480 tortoise-api-0.0.7/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.7/README.md
--rw-r--r--   0 sol        (501) staff       (20)      584 2023-07-20 16:28:16.000000 tortoise-api-0.0.7/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 16:28:24.722706 tortoise-api-0.0.7/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 16:28:24.721133 tortoise-api-0.0.7/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       28 2023-07-20 15:57:11.000000 tortoise-api-0.0.7/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     2717 2023-07-20 15:31:46.000000 tortoise-api-0.0.7/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.7/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 16:28:24.722185 tortoise-api-0.0.7/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)     3556 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       54 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 17:20:28.635501 tortoise-api-0.0.7a0/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.7a0/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     3640 2023-07-20 17:20:28.635271 tortoise-api-0.0.7a0/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.7a0/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      674 2023-07-20 17:20:19.000000 tortoise-api-0.0.7a0/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 17:20:28.635561 tortoise-api-0.0.7a0/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 17:20:28.633858 tortoise-api-0.0.7a0/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       28 2023-07-20 15:57:11.000000 tortoise-api-0.0.7a0/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     2717 2023-07-20 15:31:46.000000 tortoise-api-0.0.7a0/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.7a0/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 17:20:28.634992 tortoise-api-0.0.7a0/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     3640 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       54 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 17:20:28.000000 tortoise-api-0.0.7a0/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.0.7/LICENSE` & `tortoise-api-0.0.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.7/PKG-INFO` & `tortoise-api-0.0.7a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.0.7
+Version: 0.0.7a0
+Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mike Artemiev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `tortoise-api-0.0.7/README.md` & `tortoise-api-0.0.7a0/README.md`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.7/pyproject.toml` & `tortoise-api-0.0.7a0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "tortoise-api"
 requires-python = ">=3.9"
 authors = [
     {name = "Artemiev", email = "mixartemev@gmail.com"},
 ]
 keywords = ["starlette", "fastapi", "admin", "dashboard", "datatables", "crud", "tortoise-orm", "ASGI-admin"]
+description = "Simplest fastest minimal REST API CRUD generator for Tortoise ORM models"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "python-dotenv",
     "starlette",
     "tortoise-orm[asyncpg]",
     "uvicorn"
 ]
-version = "0.0.7"
+version = "0.0.7a"
 
 [project.urls]
 Homepage = "https://github.com/mixartemev/tortoise-api"
 Repository = "https://github.com/mixartemev/tortoise-api"
 
 [tool.setuptools]
 packages = ["tortoise_api"]
```

### Comparing `tortoise-api-0.0.7/tortoise_api/api.py` & `tortoise-api-0.0.7a0/tortoise_api/api.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.7/tortoise_api/util.py` & `tortoise-api-0.0.7a0/tortoise_api/util.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.7/tortoise_api.egg-info/PKG-INFO` & `tortoise-api-0.0.7a0/tortoise_api.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: tortoise-api
-Version: 0.0.7
+Version: 0.0.7a0
+Summary: Simplest fastest minimal REST API CRUD generator for Tortoise ORM models
 Author-email: Artemiev <mixartemev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Mike Artemiev
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

