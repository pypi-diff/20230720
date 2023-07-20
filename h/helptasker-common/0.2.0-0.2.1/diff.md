# Comparing `tmp/helptasker_common-0.2.0.tar.gz` & `tmp/helptasker_common-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helptasker_common-0.2.0.tar", max compression
+gzip compressed data, was "helptasker_common-0.2.1.tar", max compression
```

## Comparing `helptasker_common-0.2.0.tar` & `helptasker_common-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1067 2023-07-20 14:50:03.195202 helptasker_common-0.2.0/LICENSE
--rw-r--r--   0        0        0      344 2023-07-20 14:50:03.195202 helptasker_common-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-07-20 14:50:03.195202 helptasker_common-0.2.0/helptasker_common/__init__.py
--rw-r--r--   0        0        0      172 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/context.py
--rw-r--r--   0        0        0       26 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/handlers/__init__.py
--rw-r--r--   0        0        0      199 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/handlers/healthcheck.py
--rw-r--r--   0        0        0     2833 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/http_base_client.py
--rw-r--r--   0        0        0     2145 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/instrumentation.py
--rw-r--r--   0        0        0     1774 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/logger.py
--rw-r--r--   0        0        0     4258 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/middlewares.py
--rw-r--r--   0        0        0        0 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/py.typed
--rw-r--r--   0        0        0     1790 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/settings.py
--rw-r--r--   0        0        0     1759 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/helptasker_common/trace.py
--rw-r--r--   0        0        0     2915 2023-07-20 14:50:03.199202 helptasker_common-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 helptasker_common-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/LICENSE
+-rw-r--r--   0        0        0      344 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/__init__.py
+-rw-r--r--   0        0        0      172 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/context.py
+-rw-r--r--   0        0        0       26 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/handlers/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/handlers/healthcheck.py
+-rw-r--r--   0        0        0     2833 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/http_base_client.py
+-rw-r--r--   0        0        0     2146 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/instrumentation.py
+-rw-r--r--   0        0        0     1774 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/logger.py
+-rw-r--r--   0        0        0     4258 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/middlewares.py
+-rw-r--r--   0        0        0        0 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/py.typed
+-rw-r--r--   0        0        0     1790 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/settings.py
+-rw-r--r--   0        0        0     1759 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/helptasker_common/trace.py
+-rw-r--r--   0        0        0     2915 2023-07-20 15:46:53.009828 helptasker_common-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2000 1970-01-01 00:00:00.000000 helptasker_common-0.2.1/PKG-INFO
```

### Comparing `helptasker_common-0.2.0/LICENSE` & `helptasker_common-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.2.0/helptasker_common/http_base_client.py` & `helptasker_common-0.2.1/helptasker_common/http_base_client.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.2.0/helptasker_common/instrumentation.py` & `helptasker_common-0.2.1/helptasker_common/instrumentation.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         logger_load: bool = True,
         cors_enable: bool = False,
         cors_allow_origins: typing.Sequence[str] = (),
         cors_allow_credentials: bool = False,
         cors_allow_methods: typing.Sequence[str] = ('GET',),
         cors_allow_headers: typing.Sequence[str] = (),
         cors_max_age: int = 600,
-        trusted_host_enable: bool = True,
+        trusted_host_enable: bool = False,
         trusted_host_allowed_hosts: typing.Sequence[str] | None = (),
         healthcheck_enable: bool = False,
     ):
         self.logger_load = logger_load
         self.cors_enable = cors_enable
         self.cors_allow_origins = cors_allow_origins
         self.cors_allow_credentials = cors_allow_credentials
```

### Comparing `helptasker_common-0.2.0/helptasker_common/logger.py` & `helptasker_common-0.2.1/helptasker_common/logger.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.2.0/helptasker_common/middlewares.py` & `helptasker_common-0.2.1/helptasker_common/middlewares.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.2.0/helptasker_common/settings.py` & `helptasker_common-0.2.1/helptasker_common/settings.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.2.0/helptasker_common/trace.py` & `helptasker_common-0.2.1/helptasker_common/trace.py`

 * *Files identical despite different names*

### Comparing `helptasker_common-0.2.0/pyproject.toml` & `helptasker_common-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "helptasker-common"
-version = "0.2.0"
+version = "0.2.1"
 description = "Shared Library"
 authors = [
     "Kostya Ten <kostya@yandex.com>"
 ]
 repository = "https://github.com/helptasker/common/"
 keywords = ["fastapi", "pydantic", "asyncio"]
 homepage = "https://github.com/helptasker/common/"
```

### Comparing `helptasker_common-0.2.0/PKG-INFO` & `helptasker_common-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helptasker-common
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shared Library
 Home-page: https://github.com/helptasker/common/
 Keywords: fastapi,pydantic,asyncio
 Author: Kostya Ten
 Author-email: kostya@yandex.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

