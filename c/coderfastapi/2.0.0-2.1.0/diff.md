# Comparing `tmp/coderfastapi-2.0.0.tar.gz` & `tmp/coderfastapi-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coderfastapi-2.0.0.tar", last modified: Tue Jul 18 13:15:41 2023, max compression
+gzip compressed data, was "coderfastapi-2.1.0.tar", last modified: Thu Jul 20 09:45:22 2023, max compression
```

## Comparing `coderfastapi-2.0.0.tar` & `coderfastapi-2.1.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/handlers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/decorators/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/router.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/acl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.782530 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/coderfastapi/lib/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/query.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/coderfastapi/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:15:41.778530 coderfastapi-2.0.0/coderfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-18 13:15:41.000000 coderfastapi-2.0.0/coderfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-18 13:15:07.000000 coderfastapi-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:15:41.786531 coderfastapi-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.932566 coderfastapi-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 09:45:22.932566 coderfastapi-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.920565 coderfastapi-2.1.0/coderfastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/handlers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/lib/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/decorators/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/acl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/lib/security/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.924565 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.928566 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/expiration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.928566 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/security/policies/authorization/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.928566 coderfastapi-2.1.0/coderfastapi/lib/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.932566 coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/coderfastapi/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:22.920565 coderfastapi-2.1.0/coderfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 09:45:22.000000 coderfastapi-2.1.0/coderfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-20 09:45:22.000000 coderfastapi-2.1.0/coderfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:45:22.000000 coderfastapi-2.1.0/coderfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 09:45:22.000000 coderfastapi-2.1.0/coderfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 09:45:22.000000 coderfastapi-2.1.0/coderfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-20 09:44:51.000000 coderfastapi-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 09:45:22.932566 coderfastapi-2.1.0/setup.cfg
```

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/decorators/__init__.py` & `coderfastapi-2.1.0/coderfastapi/lib/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/decorators/pagination.py` & `coderfastapi-2.1.0/coderfastapi/lib/decorators/pagination.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from inspect import Parameter, Signature, signature
+from inspect import Parameter, Signature, isclass, signature
 from typing import Awaitable, Callable, Iterable, TypeVar
 from urllib.parse import parse_qs, urlencode, urlsplit, urlunsplit
 
 from codercore.lib.collection import Direction
 from fastapi import Request, Response
-from fastapi.params import Depends
 
 from coderfastapi.lib.signature import copy_parameters
 from coderfastapi.lib.validation.schemas.pagination import CursorSchema
 from coderfastapi.lib.validation.schemas.query import (
     OrderableQueryParameters,
     QueryParameters,
 )
@@ -58,18 +57,16 @@
     for name, parameter in func_signature.parameters.items():
         if _is_valid_query_parameter(parameter):
             return (name, parameter.annotation(**dict(request.query_params)))
     raise KeyError("QuerySchema not found")
 
 
 def _is_valid_query_parameter(parameter: Parameter) -> bool:
-    return (
-        isinstance(parameter.default, Depends)
-        and parameter.default.dependency is None
-        and issubclass(parameter.annotation, QueryParameters)
+    return isclass(parameter.annotation) and issubclass(
+        parameter.annotation, QueryParameters
     )
 
 
 def _build_links(
     id_attr: str,
     query_schema: S,
     request: Request,
```

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/router.py` & `coderfastapi-2.1.0/coderfastapi/lib/router.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py` & `coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py` & `coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/recovery.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py` & `coderfastapi-2.1.0/coderfastapi/lib/security/policies/authentication/jwt/providers/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/__init__.py` & `coderfastapi-2.1.0/coderfastapi/lib/security/policies/authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/security/policies/authorization/user.py` & `coderfastapi-2.1.0/coderfastapi/lib/security/policies/authorization/user.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/signature.py` & `coderfastapi-2.1.0/coderfastapi/lib/signature.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/pagination.py` & `coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/pagination.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi/lib/validation/schemas/query.py` & `coderfastapi-2.1.0/coderfastapi/lib/validation/schemas/query.py`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/coderfastapi.egg-info/SOURCES.txt` & `coderfastapi-2.1.0/coderfastapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coderfastapi-2.0.0/pyproject.toml` & `coderfastapi-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coderfastapi"
-version = "2.0.0"
+version = "2.1.0"
 description = "coderfastapi"
 readme = "README.md"
 authors = [{ name = "Code R", email = "hello@coderstudio.dev" }]
 dependencies = [
     'codercore ~= 3.0',
     'fastapi[all] ~= 0.89',
     'orjson ~= 3.8',
@@ -28,15 +28,15 @@
     'black ~= 22.12',
     'bumpver ~= 2022.1120',
     'flake8 ~= 6.0',
     'isort ~= 5.12',
 ]
 
 [tool.bumpver]
-current_version = "2.0.0"
+current_version = "2.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

