# Comparing `tmp/tortoise-api-0.0.6.tar.gz` & `tmp/tortoise-api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise-api-0.0.6.tar", last modified: Thu Jul 20 15:51:35 2023, max compression
+gzip compressed data, was "tortoise-api-0.0.7.tar", last modified: Thu Jul 20 16:28:24 2023, max compression
```

## Comparing `tortoise-api-0.0.6.tar` & `tortoise-api-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 15:51:35.222554 tortoise-api-0.0.6/
--rw-r--r--   0 sol        (501) staff       (20)      259 2023-07-20 15:51:35.222359 tortoise-api-0.0.6/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)     1687 2023-07-20 15:47:15.000000 tortoise-api-0.0.6/README.md
--rw-r--r--   0 sol        (501) staff       (20)      487 2023-07-15 15:10:57.000000 tortoise-api-0.0.6/pyproject.toml
--rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 15:51:35.222605 tortoise-api-0.0.6/setup.cfg
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 15:51:35.221092 tortoise-api-0.0.6/tortoise_api/
--rw-r--r--   0 sol        (501) staff       (20)       51 2023-07-20 15:50:36.000000 tortoise-api-0.0.6/tortoise_api/__init__.py
--rw-r--r--   0 sol        (501) staff       (20)     2717 2023-07-20 15:31:46.000000 tortoise-api-0.0.6/tortoise_api/api.py
--rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.6/tortoise_api/util.py
-drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 15:51:35.222152 tortoise-api-0.0.6/tortoise_api.egg-info/
--rw-r--r--   0 sol        (501) staff       (20)      259 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/PKG-INFO
--rw-r--r--   0 sol        (501) staff       (20)      269 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/SOURCES.txt
--rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/dependency_links.txt
--rw-r--r--   0 sol        (501) staff       (20)       46 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/requires.txt
--rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 15:51:35.000000 tortoise-api-0.0.6/tortoise_api.egg-info/top_level.txt
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 16:28:24.722657 tortoise-api-0.0.7/
+-rw-r--r--   0 sol        (501) staff       (20)     1069 2023-07-20 16:06:42.000000 tortoise-api-0.0.7/LICENSE
+-rw-r--r--   0 sol        (501) staff       (20)     3556 2023-07-20 16:28:24.722480 tortoise-api-0.0.7/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)     1911 2023-07-20 16:15:02.000000 tortoise-api-0.0.7/README.md
+-rw-r--r--   0 sol        (501) staff       (20)      584 2023-07-20 16:28:16.000000 tortoise-api-0.0.7/pyproject.toml
+-rw-r--r--   0 sol        (501) staff       (20)       38 2023-07-20 16:28:24.722706 tortoise-api-0.0.7/setup.cfg
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 16:28:24.721133 tortoise-api-0.0.7/tortoise_api/
+-rw-r--r--   0 sol        (501) staff       (20)       28 2023-07-20 15:57:11.000000 tortoise-api-0.0.7/tortoise_api/__init__.py
+-rw-r--r--   0 sol        (501) staff       (20)     2717 2023-07-20 15:31:46.000000 tortoise-api-0.0.7/tortoise_api/api.py
+-rw-r--r--   0 sol        (501) staff       (20)      691 2023-07-19 21:44:31.000000 tortoise-api-0.0.7/tortoise_api/util.py
+drwxr-xr-x   0 sol        (501) staff       (20)        0 2023-07-20 16:28:24.722185 tortoise-api-0.0.7/tortoise_api.egg-info/
+-rw-r--r--   0 sol        (501) staff       (20)     3556 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/PKG-INFO
+-rw-r--r--   0 sol        (501) staff       (20)      277 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/SOURCES.txt
+-rw-r--r--   0 sol        (501) staff       (20)        1 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/dependency_links.txt
+-rw-r--r--   0 sol        (501) staff       (20)       54 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/requires.txt
+-rw-r--r--   0 sol        (501) staff       (20)       13 2023-07-20 16:28:24.000000 tortoise-api-0.0.7/tortoise_api.egg-info/top_level.txt
```

### Comparing `tortoise-api-0.0.6/README.md` & `tortoise-api-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 uvicorn main:app
 ```
 Or you can just fork Completed minimal runnable example from [sample apps](https://github.com/mixartemev/tortoise-api/blob/master/sample_apps/minimal/).
 
 #### And voila:
 You have menu with all your models at root app route: http://127.0.0.1:8000
 
-<img width="246" alt="Home menu" src="https://github.com/mixartemev/tortoise-api/assets/5181924/80373cd8-1597-4fce-9664-09997bc9e53e">
+<img width="245" alt="Home - Models list" src="https://github.com/mixartemev/tortoise-api/assets/5181924/0ddaa015-2193-43e1-a6d1-2dbad09bfc7b">
+
 
 And JSON resources for each db Entity at [/{modelName}]() routes:
 
-<img width="284" alt="User JSON resources" src="https://github.com/mixartemev/tortoise-api/assets/5181924/4168b82d-0f6a-4be2-8cc7-2ca364b22b30">
+<img width="450" alt="User JSON resources" src="https://github.com/mixartemev/tortoise-api/assets/5181924/d4497aa5-1f10-45f3-82e8-f5145b72572e">
+
+
+And one separate Entity at [/{modelName}/{entity_id}]() routes:
+
+<img width="362" alt="User 1 JSON resource" src="https://github.com/mixartemev/tortoise-api/assets/5181924/f1fed04c-8bf2-462c-ad71-fbee35652b1a">
+
 
 ---
 Made with ❤ on top of the Starlette and Tortoise ORM.
```

### Comparing `tortoise-api-0.0.6/tortoise_api/api.py` & `tortoise-api-0.0.7/tortoise_api/api.py`

 * *Files identical despite different names*

### Comparing `tortoise-api-0.0.6/tortoise_api/util.py` & `tortoise-api-0.0.7/tortoise_api/util.py`

 * *Files identical despite different names*

