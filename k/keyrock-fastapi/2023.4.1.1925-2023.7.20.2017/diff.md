# Comparing `tmp/keyrock-fastapi-2023.4.1.1925.tar.gz` & `tmp/keyrock-fastapi-2023.7.20.2017.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyrock-fastapi-2023.4.1.1925.tar", last modified: Sat Apr  1 19:25:49 2023, max compression
+gzip compressed data, was "keyrock-fastapi-2023.7.20.2017.tar", last modified: Thu Jul 20 20:17:31 2023, max compression
```

## Comparing `keyrock-fastapi-2023.4.1.1925.tar` & `keyrock-fastapi-2023.7.20.2017.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 19:25:49.359732 keyrock-fastapi-2023.4.1.1925/
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-01 19:25:49.359732 keyrock-fastapi-2023.4.1.1925/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 19:25:49.355732 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 19:25:49.357732 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/auth/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2575 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/auth/api_key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 19:25:49.358732 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/jwt/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/jwt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/jwt/jwt.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 19:25:49.359732 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/route/
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/route/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2910 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/route/standard_response_route.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 19:25:49.357732 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi.egg-info/
--rw-r--r--   0 root         (0) root         (0)       67 2023-04-01 19:25:49.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      453 2023-04-01 19:25:49.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 19:25:49.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-01 19:25:49.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-01 19:25:49.000000 keyrock-fastapi-2023.4.1.1925/keyrock_fastapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-01 19:25:33.000000 keyrock-fastapi-2023.4.1.1925/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-04-01 19:25:49.360732 keyrock-fastapi-2023.4.1.1925/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:31.719526 keyrock-fastapi-2023.7.20.2017/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 20:17:31.719526 keyrock-fastapi-2023.7.20.2017/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:31.717526 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:31.718526 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/auth/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/auth/api_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:31.719526 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/jwt/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/jwt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/jwt/jwt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:31.719526 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/route/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/route/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/route/standard_response_route.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 20:17:31.718526 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       68 2023-07-20 20:17:31.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      453 2023-07-20 20:17:31.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 20:17:31.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-20 20:17:31.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-20 20:17:31.000000 keyrock-fastapi-2023.7.20.2017/keyrock_fastapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-07-20 20:17:19.000000 keyrock-fastapi-2023.7.20.2017/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-07-20 20:17:31.720526 keyrock-fastapi-2023.7.20.2017/setup.cfg
```

### Comparing `keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/auth/api_key.py` & `keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/auth/api_key.py`

 * *Files identical despite different names*

### Comparing `keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/jwt/jwt.py` & `keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/jwt/jwt.py`

 * *Files identical despite different names*

### Comparing `keyrock-fastapi-2023.4.1.1925/keyrock_fastapi/route/standard_response_route.py` & `keyrock-fastapi-2023.7.20.2017/keyrock_fastapi/route/standard_response_route.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,20 +53,26 @@
                     "errors": exc.errors(),
                 }
                 raise HTTPException(status_code=422, detail=detail)
             except HTTPException as exc:
                 raise exc
             except Exception as exc:
                 tb = traceback.format_tb(exc.__traceback__)
+
+                try:
+                    msg = repr(exc)
+                except Exception as msgExc:
+                    msg = str(msgExc)
+
                 response_data = {
-                    'success': False,
+                    'failed': True,
                     'result': None,
                     'errors': [
                         {
-                            "msg": str(exc),
+                            "msg": msg,
                             "debug": {
                                 "loc": tb[-1],
                                 "stack": tb,
                             }
                         }
                     ]
                 }
```

