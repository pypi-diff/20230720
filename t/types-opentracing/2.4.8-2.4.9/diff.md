# Comparing `tmp/types-opentracing-2.4.8.tar.gz` & `tmp/types-opentracing-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-opentracing-2.4.8.tar", last modified: Sat Apr 16 15:20:17 2022, max compression
+gzip compressed data, was "types-opentracing-2.4.9.tar", last modified: Sat May 21 15:20:01 2022, max compression
```

## Comparing `types-opentracing-2.4.8.tar` & `types-opentracing-2.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.126777 types-opentracing-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1748 2022-04-16 15:20:16.000000 types-opentracing-2.4.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-16 15:20:16.000000 types-opentracing-2.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-04-16 15:20:17.126777 types-opentracing-2.4.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.122777 types-opentracing-2.4.8/opentracing-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-16 15:20:16.000000 types-opentracing-2.4.8/opentracing-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (121)      774 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.122777 types-opentracing-2.4.8/opentracing-stubs/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/ext/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/ext/tags.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.122777 types-opentracing-2.4.8/opentracing-stubs/harness/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/harness/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/harness/api_check.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/harness/scope_check.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/logs.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.126777 types-opentracing-2.4.8/opentracing-stubs/mocktracer/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/binary_propagator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      402 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/context.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/propagator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/span.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      392 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/text_propagator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/mocktracer/tracer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/propagation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_manager.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.126777 types-opentracing-2.4.8/opentracing-stubs/scope_managers/
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_managers/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      277 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_managers/asyncio.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_managers/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_managers/contextvars.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_managers/gevent.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/scope_managers/tornado.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/span.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/tags.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-04-16 15:18:34.000000 types-opentracing-2.4.8/opentracing-stubs/tracer.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-16 15:20:17.126777 types-opentracing-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-04-16 15:20:16.000000 types-opentracing-2.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-16 15:20:17.126777 types-opentracing-2.4.8/types_opentracing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1174 2022-04-16 15:20:17.000000 types-opentracing-2.4.8/types_opentracing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-04-16 15:20:17.000000 types-opentracing-2.4.8/types_opentracing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-16 15:20:17.000000 types-opentracing-2.4.8/types_opentracing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-16 15:20:17.000000 types-opentracing-2.4.8/types_opentracing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.089708 types-opentracing-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-05-21 15:20:00.000000 types-opentracing-2.4.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-21 15:20:00.000000 types-opentracing-2.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-05-21 15:20:01.089708 types-opentracing-2.4.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.085708 types-opentracing-2.4.9/opentracing-stubs/
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-21 15:20:00.000000 types-opentracing-2.4.9/opentracing-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      774 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.085708 types-opentracing-2.4.9/opentracing-stubs/ext/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/ext/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/ext/tags.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.085708 types-opentracing-2.4.9/opentracing-stubs/harness/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/harness/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1665 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/harness/api_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/harness/scope_check.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/logs.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.085708 types-opentracing-2.4.9/opentracing-stubs/mocktracer/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/binary_propagator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      402 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/context.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/propagator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/span.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      392 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/text_propagator.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/mocktracer/tracer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      218 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/propagation.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      233 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_manager.pyi
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.085708 types-opentracing-2.4.9/opentracing-stubs/scope_managers/
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_managers/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      277 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_managers/asyncio.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_managers/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_managers/contextvars.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_managers/gevent.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/scope_managers/tornado.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/span.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)      454 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/tags.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)     1657 2022-05-21 15:19:47.000000 types-opentracing-2.4.9/opentracing-stubs/tracer.pyi
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-21 15:20:01.089708 types-opentracing-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-05-21 15:20:00.000000 types-opentracing-2.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-21 15:20:01.089708 types-opentracing-2.4.9/types_opentracing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1222 2022-05-21 15:20:01.000000 types-opentracing-2.4.9/types_opentracing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-05-21 15:20:01.000000 types-opentracing-2.4.9/types_opentracing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-21 15:20:01.000000 types-opentracing-2.4.9/types_opentracing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-05-21 15:20:01.000000 types-opentracing-2.4.9/types_opentracing.egg-info/top_level.txt
```

### Comparing `types-opentracing-2.4.8/CHANGELOG.md` & `types-opentracing-2.4.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.4.9 (2022-05-21)
+
+Simplify and correct many numeric unions (#7906)
+
+Unblocks PyCQA/flake8-pyi#222
+
 ## 2.4.8 (2022-04-16)
 
 Third-party stubs: import from `collections.abc` where possible (#7637)
 
 ## 2.4.7 (2022-01-10)
 
 Always use `_typeshed.Self`, where applicable (#6880)
```

### Comparing `types-opentracing-2.4.8/PKG-INFO` & `types-opentracing-2.4.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-opentracing
-Version: 2.4.8
+Version: 2.4.9
 Summary: Typing stubs for opentracing
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/opentracing.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for opentracing
 
 This is a PEP 561 type stub package for the `opentracing` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `opentracing`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/opentracing. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `7a3eb5a4818664d7619ea6ec664c280d0a64c7ee`.
+This package was generated from typeshed commit `8b58371278078d50c85128d74b1fc10c24029d21`.
```

### Comparing `types-opentracing-2.4.8/opentracing-stubs/__init__.pyi` & `types-opentracing-2.4.9/opentracing-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-opentracing-2.4.8/opentracing-stubs/harness/api_check.pyi` & `types-opentracing-2.4.9/opentracing-stubs/harness/api_check.pyi`

 * *Files identical despite different names*

### Comparing `types-opentracing-2.4.8/opentracing-stubs/harness/scope_check.pyi` & `types-opentracing-2.4.9/opentracing-stubs/harness/scope_check.pyi`

 * *Files identical despite different names*

### Comparing `types-opentracing-2.4.8/opentracing-stubs/mocktracer/span.pyi` & `types-opentracing-2.4.9/opentracing-stubs/mocktracer/span.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         start_time: float | None = ...,
     ) -> None: ...
     @property
     def tracer(self) -> MockTracer: ...
     @property
     def context(self) -> SpanContext: ...
     def set_operation_name(self: Self, operation_name: str) -> Self: ...
-    def set_tag(self: Self, key: str, value: str | bool | int | float) -> Self: ...
+    def set_tag(self: Self, key: str, value: str | bool | float) -> Self: ...
     def log_kv(self: Self, key_values: dict[str, Any], timestamp: float | None = ...) -> Self: ...
     def set_baggage_item(self: Self, key: str, value: str) -> Self: ...
 
 class LogData:
     key_values: dict[str, Any]
     timestamp: float | None
     def __init__(self, key_values: dict[str, Any], timestamp: float | None = ...) -> None: ...
```

### Comparing `types-opentracing-2.4.8/opentracing-stubs/mocktracer/tracer.pyi` & `types-opentracing-2.4.9/opentracing-stubs/mocktracer/tracer.pyi`

 * *Files identical despite different names*

### Comparing `types-opentracing-2.4.8/opentracing-stubs/scope.pyi` & `types-opentracing-2.4.9/opentracing-stubs/scope.pyi`

 * *Files identical despite different names*

### Comparing `types-opentracing-2.4.8/opentracing-stubs/span.pyi` & `types-opentracing-2.4.9/opentracing-stubs/span.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self, tracer: Tracer, context: SpanContext) -> None: ...
     @property
     def context(self) -> SpanContext: ...
     @property
     def tracer(self) -> Tracer: ...
     def set_operation_name(self: Self, operation_name: str) -> Self: ...
     def finish(self, finish_time: float | None = ...) -> None: ...
-    def set_tag(self: Self, key: str, value: str | bool | int | float) -> Self: ...
+    def set_tag(self: Self, key: str, value: str | bool | float) -> Self: ...
     def log_kv(self: Self, key_values: dict[str, Any], timestamp: float | None = ...) -> Self: ...
     def set_baggage_item(self: Self, key: str, value: str) -> Self: ...
     def get_baggage_item(self, key: str) -> str | None: ...
     def __enter__(self: Self) -> Self: ...
     def __exit__(
         self, exc_type: type[BaseException] | None, exc_val: BaseException | None, exc_tb: TracebackType | None
     ) -> None: ...
```

### Comparing `types-opentracing-2.4.8/opentracing-stubs/tracer.pyi` & `types-opentracing-2.4.9/opentracing-stubs/tracer.pyi`

 * *Files identical despite different names*

### Comparing `types-opentracing-2.4.8/setup.py` & `types-opentracing-2.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 This is a PEP 561 type stub package for the `opentracing` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `opentracing`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/opentracing. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `7a3eb5a4818664d7619ea6ec664c280d0a64c7ee`.
+This package was generated from typeshed commit `8b58371278078d50c85128d74b1fc10c24029d21`.
 '''.lstrip()
 
 setup(name=name,
-      version="2.4.8",
+      version="2.4.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/opentracing.md",
@@ -29,10 +29,11 @@
       },
       install_requires=[],
       packages=['opentracing-stubs'],
       package_data={'opentracing-stubs': ['__init__.pyi', 'ext/__init__.pyi', 'ext/tags.pyi', 'harness/__init__.pyi', 'harness/api_check.pyi', 'harness/scope_check.pyi', 'logs.pyi', 'mocktracer/__init__.pyi', 'mocktracer/binary_propagator.pyi', 'mocktracer/context.pyi', 'mocktracer/propagator.pyi', 'mocktracer/span.pyi', 'mocktracer/text_propagator.pyi', 'mocktracer/tracer.pyi', 'propagation.pyi', 'scope.pyi', 'scope_manager.pyi', 'scope_managers/__init__.pyi', 'scope_managers/asyncio.pyi', 'scope_managers/constants.pyi', 'scope_managers/contextvars.pyi', 'scope_managers/gevent.pyi', 'scope_managers/tornado.pyi', 'span.pyi', 'tags.pyi', 'tracer.pyi', 'METADATA.toml']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
+          "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-opentracing-2.4.8/types_opentracing.egg-info/PKG-INFO` & `types-opentracing-2.4.9/types_opentracing.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: types-opentracing
-Version: 2.4.8
+Version: 2.4.9
 Summary: Typing stubs for opentracing
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/opentracing.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Description-Content-Type: text/markdown
 
 ## Typing stubs for opentracing
 
 This is a PEP 561 type stub package for the `opentracing` package.
 It can be used by type-checking tools like mypy, PyCharm, pytype etc. to check code
 that uses `opentracing`. The source for this package can be found at
 https://github.com/python/typeshed/tree/master/stubs/opentracing. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/master/README.md for more details.
-This package was generated from typeshed commit `7a3eb5a4818664d7619ea6ec664c280d0a64c7ee`.
+This package was generated from typeshed commit `8b58371278078d50c85128d74b1fc10c24029d21`.
```

### Comparing `types-opentracing-2.4.8/types_opentracing.egg-info/SOURCES.txt` & `types-opentracing-2.4.9/types_opentracing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

