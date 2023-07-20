# Comparing `tmp/cachetoolz-0.2.0.tar.gz` & `tmp/cachetoolz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetoolz-0.2.0.tar", max compression
+gzip compressed data, was "cachetoolz-0.3.0.tar", max compression
```

## Comparing `cachetoolz-0.2.0.tar` & `cachetoolz-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/LICENSE
--rw-r--r--   0        0        0    11097 2023-07-19 13:12:21.864253 cachetoolz-0.2.0/README.md
--rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/__init__.py
--rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/__init__.py
--rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/backend.py
--rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/coder.py
--rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/abc/serializer.py
--rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/__init__.py
--rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/inmemory.py
--rw-r--r--   0        0        0     6595 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/mongo.py
--rw-r--r--   0        0        0     4212 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/backend/redis.py
--rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/coder/__init__.py
--rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/coder/decoder.py
--rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/coder/encoder.py
--rw-r--r--   0        0        0     4260 2023-07-19 13:28:48.375536 cachetoolz-0.2.0/cachetoolz/decorator.py
--rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/exceptions.py
--rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/log.py
--rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.2.0/cachetoolz/types.py
--rw-r--r--   0        0        0     3194 2023-07-19 13:24:39.070373 cachetoolz-0.2.0/cachetoolz/utils.py
--rw-r--r--   0        0        0     3063 2023-07-19 13:46:29.211552 cachetoolz-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    12638 1970-01-01 00:00:00.000000 cachetoolz-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/LICENSE
+-rw-r--r--   0        0        0    11097 2023-07-19 13:12:21.864253 cachetoolz-0.3.0/README.md
+-rw-r--r--   0        0        0      394 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/__init__.py
+-rw-r--r--   0        0        0      223 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/__init__.py
+-rw-r--r--   0        0        0     2181 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/backend.py
+-rw-r--r--   0        0        0      618 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/coder.py
+-rw-r--r--   0        0        0      623 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/abc/serializer.py
+-rw-r--r--   0        0        0      315 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/backend/__init__.py
+-rw-r--r--   0        0        0     4619 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/backend/inmemory.py
+-rw-r--r--   0        0        0     7162 2023-07-20 13:38:56.376102 cachetoolz-0.3.0/cachetoolz/backend/mongo.py
+-rw-r--r--   0        0        0     4797 2023-07-20 13:38:56.384102 cachetoolz-0.3.0/cachetoolz/backend/redis.py
+-rw-r--r--   0        0        0     2151 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/coder/__init__.py
+-rw-r--r--   0        0        0     2413 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/coder/decoder.py
+-rw-r--r--   0        0        0     3733 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/coder/encoder.py
+-rw-r--r--   0        0        0     4259 2023-07-19 13:56:43.867298 cachetoolz-0.3.0/cachetoolz/decorator.py
+-rw-r--r--   0        0        0      250 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/exceptions.py
+-rw-r--r--   0        0        0      702 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/log.py
+-rw-r--r--   0        0        0      633 2023-07-19 02:08:29.819918 cachetoolz-0.3.0/cachetoolz/types.py
+-rw-r--r--   0        0        0     3194 2023-07-19 13:24:39.070373 cachetoolz-0.3.0/cachetoolz/utils.py
+-rw-r--r--   0        0        0     3063 2023-07-20 13:39:21.839935 cachetoolz-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12638 1970-01-01 00:00:00.000000 cachetoolz-0.3.0/PKG-INFO
```

### Comparing `cachetoolz-0.2.0/LICENSE` & `cachetoolz-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/README.md` & `cachetoolz-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/abc/backend.py` & `cachetoolz-0.3.0/cachetoolz/abc/backend.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/abc/coder.py` & `cachetoolz-0.3.0/cachetoolz/abc/coder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/abc/serializer.py` & `cachetoolz-0.3.0/cachetoolz/abc/serializer.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/backend/inmemory.py` & `cachetoolz-0.3.0/cachetoolz/backend/inmemory.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/backend/mongo.py` & `cachetoolz-0.3.0/cachetoolz/backend/mongo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 """Mongo backend."""
 
 from contextlib import contextmanager
 from datetime import datetime, timedelta
-from typing import Any
+from typing import Any, Dict
 
 from ..abc import AsyncBackendABC, BackendABC
 
 
 class MongoBackend(BackendABC):
     """MongoDB cache."""
 
-    def __init__(self, url: str, database: str = '.cachetoolz'):
+    def __init__(
+        self,
+        host: str = 'localhost',
+        database: str = '.cachetoolz',
+        **kwargs: Dict[str, Any],
+    ):
         """Initialize the instance.
 
         Parameters
         ----------
-        url
-            Mongo url
+        host
+            MongoDB URI
         database
             Cache database name
+        kwargs
+            Takes the same constructor arguments as
+            :class:`~pymongo.mongo_client.MongoClient`
 
         """
         try:
             from pymongo import MongoClient
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'mongo' extra in order "
                 "to use mongo backend."
             ) from exc
 
         self._client_cls = MongoClient
+        self._kwargs = kwargs
 
-        self._url = url
+        self._kwargs['host'] = host
+
+        self._host = host
         self._database = database
 
     def __repr__(self):
         """Creates a visual representation of the instance."""
         _cls = self.__class__.__name__
-        return f'{_cls}(url="{self._url}", database="{self._database}")'
+        return f'{_cls}(host="{self._host}", database="{self._database}")'
 
     @contextmanager
     def _get_database_or_collection(self, collection=None):
-        with self._client_cls(self._url) as client:
+        with self._client_cls(**self._kwargs) as client:
             if collection:
                 yield client[self._database][collection]
             else:
                 yield client[self._database]
 
     def get(self, key: str) -> Any:
         """Get a value if not expired.
@@ -123,46 +134,56 @@
         with self._get_database_or_collection() as database:
             database.drop_collection(namespace)
 
 
 class AsyncMongoBackend(AsyncBackendABC):
     """Async MongoDB cache."""
 
-    def __init__(self, url: str, database: str = '.cachetoolz'):
+    def __init__(
+        self,
+        host: str = 'localhost',
+        database: str = '.cachetoolz',
+        **kwargs: Dict[str, Any],
+    ):
         """Initialize the instance.
 
         Parameters
         ----------
-        url
-            Mongo url
+        host
+            MongoDB URI
         database
             Cache database name
+        kwargs
+            Takes the same constructor arguments as
+            :class:`~pymongo.mongo_client.MongoClient`
 
         """
         try:
             from motor.motor_asyncio import AsyncIOMotorClient
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'mongo' extra in order "
                 "to use mongo backend."
             ) from exc
 
         self._client_cls = AsyncIOMotorClient
+        self._kwargs = kwargs
+        self._kwargs['host'] = host
 
-        self._url = url
+        self._host = host
         self._database = database
 
     def __repr__(self):
         """Creates a visual representation of the instance."""
         _cls = self.__class__.__name__
-        return f'{_cls}(url="{self._url}", database="{self._database}")'
+        return f'{_cls}(host="{self._host}", database="{self._database}")'
 
     @contextmanager
     def _get_database_or_collection(self, collection=None):
-        client = self._client_cls(self._url)
+        client = self._client_cls(**self._kwargs)
         try:
             if collection:
                 yield client[self._database][collection]
             else:
                 yield client[self._database]
         finally:
             client.close()
```

### Comparing `cachetoolz-0.2.0/cachetoolz/backend/redis.py` & `cachetoolz-0.3.0/cachetoolz/backend/redis.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,44 @@
 """Redis memory."""
 
 from datetime import timedelta
-from typing import Any
+from typing import Any, Dict
 
 from ..abc import AsyncBackendABC, BackendABC
 
 
 class RedisBackend(BackendABC):
     """Redis cache."""
 
-    def __init__(self, url: str):
+    def __init__(self, url: str, **kwargs: Dict[str, Any]):
         """Initialize the instance.
 
+        The ``decode_responses`` parameter will always be True
+        as the result needs to be returned as a string.
+
         Parameters
         ----------
         url
             Redis url
+        kwargs
+            Takes the same constructor arguments as
+            :method:`~redis.client.Redis.from_url`
 
         """
         try:
             from redis import Redis
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'redis' extra in order "
                 "to use redis backend."
             ) from exc
 
         self._url = url
-        self._backend = Redis.from_url(self._url, decode_responses=True)
+        kwargs['decode_responses'] = True
+        self._backend = Redis.from_url(self._url, **kwargs)
 
     def __repr__(self):
         """Creates a visual representation of the instance."""
         return f'{self.__class__.__name__}(url="{self._url}")'
 
     def get(self, key: str) -> Any:
         """Get a value if not expired.
@@ -89,33 +96,40 @@
         for key in self._backend.scan_iter(f'{namespace}:*'):
             self._backend.delete(key)
 
 
 class AsyncRedisBackend(AsyncBackendABC):
     """Async Redis backend."""
 
-    def __init__(self, url: str):
+    def __init__(self, url: str, **kwargs):
         """Initialize the instance.
 
+        The ``decode_responses`` parameter will always be True
+        as the result needs to be returned as a string.
+
         Parameters
         ----------
         url
             Redis url
+        kwargs
+            Takes the same constructor arguments as
+            :method:`~redis.asyncio. client.Redis.from_url`
 
         """
         try:
             from redis.asyncio import Redis
         except ImportError as exc:
             raise RuntimeError(
                 "Install cachetoolz with the 'redis' extra in order "
                 "to use redis backend."
             ) from exc
 
         self._url = url
-        self._backend = Redis.from_url(self._url, decode_responses=True)
+        kwargs['decode_responses'] = True
+        self._backend = Redis.from_url(self._url, **kwargs)
 
     def __repr__(self):
         """Creates a visual representation of the instance."""
         return f'{self.__class__.__name__}(url="{self._url}")'
 
     async def get(self, key: str) -> Any:
         """Get a value if not expired.
```

### Comparing `cachetoolz-0.2.0/cachetoolz/coder/__init__.py` & `cachetoolz-0.3.0/cachetoolz/coder/__init__.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/coder/decoder.py` & `cachetoolz-0.3.0/cachetoolz/coder/decoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/coder/encoder.py` & `cachetoolz-0.3.0/cachetoolz/coder/encoder.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/decorator.py` & `cachetoolz-0.3.0/cachetoolz/decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,14 @@
         *args,
         ttl: Union[int, float, timedelta] = inf,
         namespace: str = 'default',
         typed: bool = False,
         keygen: Optional[KeyGenerator] = None,
     ) -> Decorator:
         """Caches a function call and stores it in the namespace."""
-
         if isinf(ttl):
             ttl = timedelta(weeks=20e3)
         elif not isinstance(ttl, timedelta):
             ttl = timedelta(seconds=ttl)
 
         keygen = curry(make_key)(namespace, keygen, typed)
         manipulator = manipulate(curry(Cache._cache)(self, ttl, keygen))
```

### Comparing `cachetoolz-0.2.0/cachetoolz/log.py` & `cachetoolz-0.3.0/cachetoolz/log.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/types.py` & `cachetoolz-0.3.0/cachetoolz/types.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/cachetoolz/utils.py` & `cachetoolz-0.3.0/cachetoolz/utils.py`

 * *Files identical despite different names*

### Comparing `cachetoolz-0.2.0/pyproject.toml` & `cachetoolz-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cachetoolz"
-version = "0.2.0"
+version = "0.3.0"
 description = "This library provides a decorator for caching functions"
 license = "MIT"
 authors = ["Igor Taconi <igor.taconi@protonmail.com>"]
 maintainers = ["Igor Taconi <igor.taconi@protonmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/taconi/cachetoolz/#readme"
 repository = "https://github.com/taconi/cachetoolz/"
```

### Comparing `cachetoolz-0.2.0/PKG-INFO` & `cachetoolz-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetoolz
-Version: 0.2.0
+Version: 0.3.0
 Summary: This library provides a decorator for caching functions
 Home-page: https://github.com/taconi/cachetoolz/#readme
 License: MIT
 Keywords: python,cache,async,redis,mongo
 Author: Igor Taconi
 Author-email: igor.taconi@protonmail.com
 Maintainer: Igor Taconi
```

