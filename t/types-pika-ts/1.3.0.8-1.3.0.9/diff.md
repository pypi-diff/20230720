# Comparing `tmp/types-pika-ts-1.3.0.8.tar.gz` & `tmp/types-pika-ts-1.3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pika-ts-1.3.0.8.tar", last modified: Sat Mar 25 06:19:02 2023, max compression
+gzip compressed data, was "types-pika-ts-1.3.0.9.tar", last modified: Mon Mar 27 18:24:02 2023, max compression
```

## Comparing `types-pika-ts-1.3.0.8.tar` & `types-pika-ts-1.3.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-03-25 06:19:01.000000 types-pika-ts-1.3.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-25 06:19:01.000000 types-pika-ts-1.3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/pika-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-25 06:19:01.000000 types-pika-ts-1.3.0.8/pika-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/pika-stubs/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/asyncio_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/base_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/blocking_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/gevent_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/select_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/tornado_connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/twisted_connection.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/connection_workflow.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/io_services_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/nbio_interface.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/selector_ioloop_adapter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/amqp_object.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/callback.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/channel.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/connection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/data.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/delivery_mode.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/diagnostic_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/exchange_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/frame.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/heartbeat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28551 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/spec.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/tcp_socket_opts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-25 06:18:50.000000 types-pika-ts-1.3.0.8/pika-stubs/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-25 06:19:01.000000 types-pika-ts-1.3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 06:19:02.348506 types-pika-ts-1.3.0.8/types_pika_ts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-25 06:19:02.000000 types-pika-ts-1.3.0.8/types_pika_ts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-25 06:19:02.000000 types-pika-ts-1.3.0.8/types_pika_ts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 06:19:02.000000 types-pika-ts-1.3.0.8/types_pika_ts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-25 06:19:02.000000 types-pika-ts-1.3.0.8/types_pika_ts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:02.846961 types-pika-ts-1.3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-27 18:24:02.846961 types-pika-ts-1.3.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:02.842961 types-pika-ts-1.3.0.9/pika-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/pika-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:02.842961 types-pika-ts-1.3.0.9/pika-stubs/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/asyncio_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/base_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/blocking_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/gevent_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/select_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/tornado_connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/twisted_connection.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:02.846961 types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/connection_workflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/io_services_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/nbio_interface.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/selector_ioloop_adapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/amqp_object.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/callback.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/channel.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/connection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/data.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/delivery_mode.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/diagnostic_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/exchange_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/frame.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/heartbeat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28506 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/spec.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/tcp_socket_opts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-27 18:21:24.000000 types-pika-ts-1.3.0.9/pika-stubs/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:02.846961 types-pika-ts-1.3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:02.846961 types-pika-ts-1.3.0.9/types_pika_ts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/types_pika_ts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/types_pika_ts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/types_pika_ts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-27 18:24:02.000000 types-pika-ts-1.3.0.9/types_pika_ts.egg-info/top_level.txt
```

### Comparing `types-pika-ts-1.3.0.8/CHANGELOG.md` & `types-pika-ts-1.3.0.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.3.0.9 (2023-03-27)
+
+Add default values for third-party stubs beginning with 'P' (#9957)
+
 ## 1.3.0.8 (2023-03-25)
 
 Use of twisted in pika (#9494)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 1.3.0.7 (2023-02-28)
```

### Comparing `types-pika-ts-1.3.0.8/PKG-INFO` & `types-pika-ts-1.3.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pika-ts
-Version: 1.3.0.8
+Version: 1.3.0.9
 Summary: Typing stubs for pika
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pika.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -24,8 +24,8 @@
 `pika`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pika. All fixes for
 types and metadata should be contributed there.
 
 The `types-pika` package contains alternate, more complete type stubs, that are maintained outside of typeshed.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2e59b81ffdb36160270fbbedb7ac78f17a85f5d2`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/__init__.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/asyncio_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/asyncio_connection.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 from .utils import io_services_utils, nbio_interface
 
 LOGGER: Logger
 
 class AsyncioConnection(BaseConnection):
     def __init__(
         self,
-        parameters: Parameters | None = ...,
-        on_open_callback: Callable[[Self], object] | None = ...,
-        on_open_error_callback: Callable[[Self, BaseException], object] | None = ...,
-        on_close_callback: Callable[[Self, BaseException], object] | None = ...,
-        custom_ioloop: AbstractEventLoop | None = ...,
-        internal_connection_workflow: bool = ...,
+        parameters: Parameters | None = None,
+        on_open_callback: Callable[[Self], object] | None = None,
+        on_open_error_callback: Callable[[Self, BaseException], object] | None = None,
+        on_close_callback: Callable[[Self, BaseException], object] | None = None,
+        custom_ioloop: AbstractEventLoop | None = None,
+        internal_connection_workflow: bool = True,
     ) -> None: ...
     @classmethod
     def create_connection(
-        cls, connection_configs, on_done, custom_ioloop: AbstractEventLoop | None = ..., workflow: Incomplete | None = ...
+        cls, connection_configs, on_done, custom_ioloop: AbstractEventLoop | None = None, workflow: Incomplete | None = None
     ): ...
 
 class _AsyncioIOServicesAdapter(
     io_services_utils.SocketConnectionMixin,
     io_services_utils.StreamingConnectionMixin,
     nbio_interface.AbstractIOServices,
     nbio_interface.AbstractFileDescriptorServices,
 ):
-    def __init__(self, loop: Incomplete | None = ...) -> None: ...
+    def __init__(self, loop: Incomplete | None = None) -> None: ...
     def get_native_ioloop(self): ...
     def close(self) -> None: ...
     def run(self) -> None: ...
     def stop(self) -> None: ...
     def add_callback_threadsafe(self, callback) -> None: ...
     def call_later(self, delay, callback): ...
-    def getaddrinfo(self, host, port, on_done, family: int = ..., socktype: int = ..., proto: int = ..., flags: int = ...): ...
+    def getaddrinfo(self, host, port, on_done, family: int = 0, socktype: int = 0, proto: int = 0, flags: int = 0): ...
     def set_reader(self, fd, on_readable) -> None: ...
     def remove_reader(self, fd): ...
     def set_writer(self, fd, on_writable) -> None: ...
     def remove_writer(self, fd): ...
 
 class _TimerHandle(nbio_interface.AbstractTimerReference):
     def __init__(self, handle) -> None: ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/base_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/base_connection.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         on_close_callback: Callable[[Self, BaseException], object] | None,
         nbio,
         internal_connection_workflow: bool,
     ) -> None: ...
     @classmethod
     @abc.abstractmethod
     def create_connection(
-        cls, connection_configs, on_done, custom_ioloop: Incomplete | None = ..., workflow: Incomplete | None = ...
+        cls, connection_configs, on_done, custom_ioloop: Incomplete | None = None, workflow: Incomplete | None = None
     ): ...
     @property
     def ioloop(self): ...
 
 class _StreamingProtocolShim(nbio_interface.AbstractStreamProtocol):
     connection_made: Incomplete
     connection_lost: Incomplete
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/blocking_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/blocking_connection.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..data import _ArgumentMapping
 from ..exchange_type import ExchangeType
 from ..spec import BasicProperties
 
 LOGGER: Incomplete
 
 class _CallbackResult:
-    def __init__(self, value_class: Incomplete | None = ...) -> None: ...
+    def __init__(self, value_class: Incomplete | None = None) -> None: ...
     def reset(self) -> None: ...
     def __bool__(self) -> bool: ...
     __nonzero__: Incomplete
     def __enter__(self): ...
     def __exit__(self, *args: Unused, **kwargs: Unused) -> None: ...
     def is_ready(self): ...
     @property
@@ -51,30 +51,30 @@
     class _OnClosedArgs(NamedTuple):
         connection: Incomplete
         error: Incomplete
 
     class _OnChannelOpenedArgs(NamedTuple):
         channel: Incomplete
     def __init__(
-        self, parameters: Parameters | Sequence[Parameters] | None = ..., _impl_class: Incomplete | None = ...
+        self, parameters: Parameters | Sequence[Parameters] | None = None, _impl_class: Incomplete | None = None
     ) -> None: ...
     def __enter__(self) -> Self: ...
     def __exit__(
         self, exc_type: type[BaseException] | None, value: BaseException | None, traceback: TracebackType | None
     ) -> None: ...
     def add_on_connection_blocked_callback(self, callback) -> None: ...
     def add_on_connection_unblocked_callback(self, callback) -> None: ...
     def call_later(self, delay, callback): ...
     def add_callback_threadsafe(self, callback) -> None: ...
     def remove_timeout(self, timeout_id) -> None: ...
     def update_secret(self, new_secret, reason) -> None: ...
-    def close(self, reply_code: int = ..., reply_text: str = ...) -> None: ...
-    def process_data_events(self, time_limit: int = ...): ...
+    def close(self, reply_code: int = 200, reply_text: str = "Normal shutdown") -> None: ...
+    def process_data_events(self, time_limit: int = 0): ...
     def sleep(self, duration: float) -> None: ...
-    def channel(self, channel_number: int | None = ...) -> BlockingChannel: ...
+    def channel(self, channel_number: int | None = None) -> BlockingChannel: ...
     @property
     def is_closed(self) -> bool: ...
     @property
     def is_open(self) -> bool: ...
     @property
     def basic_nack_supported(self) -> bool: ...
     @property
@@ -124,15 +124,19 @@
     CANCELLED_BY_BROKER: int
     consumer_tag: Incomplete
     auto_ack: Incomplete
     on_message_callback: Incomplete
     alternate_event_sink: Incomplete
     state: Incomplete
     def __init__(
-        self, consumer_tag, auto_ack, on_message_callback: Incomplete | None = ..., alternate_event_sink: Incomplete | None = ...
+        self,
+        consumer_tag,
+        auto_ack,
+        on_message_callback: Incomplete | None = None,
+        alternate_event_sink: Incomplete | None = None,
     ) -> None: ...
     @property
     def setting_up(self): ...
     @property
     def active(self): ...
     @property
     def tearing_down(self): ...
@@ -172,80 +176,89 @@
     def connection(self): ...
     @property
     def is_closed(self): ...
     @property
     def is_open(self): ...
     @property
     def consumer_tags(self): ...
-    def close(self, reply_code: int = ..., reply_text: str = ...): ...
+    def close(self, reply_code: int = 0, reply_text: str = "Normal shutdown"): ...
     def flow(self, active): ...
     def add_on_cancel_callback(self, callback) -> None: ...
     def add_on_return_callback(self, callback): ...
     def basic_consume(
         self,
         queue,
         on_message_callback,
-        auto_ack: bool = ...,
-        exclusive: bool = ...,
-        consumer_tag: Incomplete | None = ...,
-        arguments: Incomplete | None = ...,
+        auto_ack: bool = False,
+        exclusive: bool = False,
+        consumer_tag: Incomplete | None = None,
+        arguments: Incomplete | None = None,
     ): ...
     def basic_cancel(self, consumer_tag): ...
     def start_consuming(self) -> None: ...
-    def stop_consuming(self, consumer_tag: Incomplete | None = ...) -> None: ...
+    def stop_consuming(self, consumer_tag: Incomplete | None = None) -> None: ...
     def consume(
         self,
         queue,
-        auto_ack: bool = ...,
-        exclusive: bool = ...,
-        arguments: Incomplete | None = ...,
-        inactivity_timeout: Incomplete | None = ...,
+        auto_ack: bool = False,
+        exclusive: bool = False,
+        arguments: Incomplete | None = None,
+        inactivity_timeout: Incomplete | None = None,
     ) -> Generator[Incomplete, None, None]: ...
     def get_waiting_message_count(self): ...
     def cancel(self): ...
-    def basic_ack(self, delivery_tag: int = ..., multiple: bool = ...) -> None: ...
-    def basic_nack(self, delivery_tag: int = ..., multiple: bool = ..., requeue: bool = ...) -> None: ...
-    def basic_get(self, queue, auto_ack: bool = ...): ...
+    def basic_ack(self, delivery_tag: int = 0, multiple: bool = False) -> None: ...
+    def basic_nack(self, delivery_tag: int = 0, multiple: bool = False, requeue: bool = True) -> None: ...
+    def basic_get(self, queue, auto_ack: bool = False): ...
     def basic_publish(
-        self, exchange: str, routing_key: str, body: str | bytes, properties: BasicProperties | None = ..., mandatory: bool = ...
+        self,
+        exchange: str,
+        routing_key: str,
+        body: str | bytes,
+        properties: BasicProperties | None = None,
+        mandatory: bool = False,
     ) -> None: ...
-    def basic_qos(self, prefetch_size: int = ..., prefetch_count: int = ..., global_qos: bool = ...) -> None: ...
-    def basic_recover(self, requeue: bool = ...) -> None: ...
-    def basic_reject(self, delivery_tag: int = ..., requeue: bool = ...) -> None: ...
+    def basic_qos(self, prefetch_size: int = 0, prefetch_count: int = 0, global_qos: bool = False) -> None: ...
+    def basic_recover(self, requeue: bool = False) -> None: ...
+    def basic_reject(self, delivery_tag: int = 0, requeue: bool = True) -> None: ...
     def confirm_delivery(self) -> None: ...
     def exchange_declare(
         self,
         exchange: str,
         exchange_type: ExchangeType | str = ...,
-        passive: bool = ...,
-        durable: bool = ...,
-        auto_delete: bool = ...,
-        internal: bool = ...,
-        arguments: _ArgumentMapping | None = ...,
+        passive: bool = False,
+        durable: bool = False,
+        auto_delete: bool = False,
+        internal: bool = False,
+        arguments: _ArgumentMapping | None = None,
     ): ...
-    def exchange_delete(self, exchange: str | None = ..., if_unused: bool = ...): ...
-    def exchange_bind(self, destination, source, routing_key: str = ..., arguments: Incomplete | None = ...): ...
+    def exchange_delete(self, exchange: str | None = None, if_unused: bool = False): ...
+    def exchange_bind(self, destination, source, routing_key: str = "", arguments: Incomplete | None = None): ...
     def exchange_unbind(
         self,
-        destination: Incomplete | None = ...,
-        source: Incomplete | None = ...,
-        routing_key: str = ...,
-        arguments: Incomplete | None = ...,
+        destination: Incomplete | None = None,
+        source: Incomplete | None = None,
+        routing_key: str = "",
+        arguments: Incomplete | None = None,
     ): ...
     def queue_declare(
         self,
         queue,
-        passive: bool = ...,
-        durable: bool = ...,
-        exclusive: bool = ...,
-        auto_delete: bool = ...,
-        arguments: Incomplete | None = ...,
+        passive: bool = False,
+        durable: bool = False,
+        exclusive: bool = False,
+        auto_delete: bool = False,
+        arguments: Incomplete | None = None,
     ): ...
-    def queue_delete(self, queue, if_unused: bool = ..., if_empty: bool = ...): ...
+    def queue_delete(self, queue, if_unused: bool = False, if_empty: bool = False): ...
     def queue_purge(self, queue): ...
-    def queue_bind(self, queue, exchange, routing_key: Incomplete | None = ..., arguments: Incomplete | None = ...): ...
+    def queue_bind(self, queue, exchange, routing_key: Incomplete | None = None, arguments: Incomplete | None = None): ...
     def queue_unbind(
-        self, queue, exchange: Incomplete | None = ..., routing_key: Incomplete | None = ..., arguments: Incomplete | None = ...
+        self,
+        queue,
+        exchange: Incomplete | None = None,
+        routing_key: Incomplete | None = None,
+        arguments: Incomplete | None = None,
     ): ...
     def tx_select(self): ...
     def tx_commit(self): ...
     def tx_rollback(self): ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/gevent_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/gevent_connection.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/select_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/select_connection.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
 LOGGER: Incomplete
 SELECT_TYPE: Incomplete
 
 class SelectConnection(BaseConnection):
     def __init__(
         self,
-        parameters: Incomplete | None = ...,
-        on_open_callback: Incomplete | None = ...,
-        on_open_error_callback: Incomplete | None = ...,
-        on_close_callback: Incomplete | None = ...,
-        custom_ioloop: Incomplete | None = ...,
-        internal_connection_workflow: bool = ...,
+        parameters: Incomplete | None = None,
+        on_open_callback: Incomplete | None = None,
+        on_open_error_callback: Incomplete | None = None,
+        on_close_callback: Incomplete | None = None,
+        custom_ioloop: Incomplete | None = None,
+        internal_connection_workflow: bool = True,
     ) -> None: ...
     @classmethod
     def create_connection(
-        cls, connection_configs, on_done, custom_ioloop: Incomplete | None = ..., workflow: Incomplete | None = ...
+        cls, connection_configs, on_done, custom_ioloop: Incomplete | None = None, workflow: Incomplete | None = None
     ): ...
 
 class _Timeout:
     deadline: Incomplete
     callback: Incomplete
     def __init__(self, deadline, callback) -> None: ...
     def __eq__(self, other): ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/tornado_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/tornado_connection.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/twisted_connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/twisted_connection.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/connection_workflow.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/connection_workflow.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,11 +27,11 @@
     def abort(self) -> None: ...
 
 class AbstractAMQPConnectionWorkflow(pika.compat.AbstractBase):
     def start(self, connection_configs, connector_factory, native_loop, on_done) -> None: ...
     def abort(self) -> None: ...
 
 class AMQPConnectionWorkflow(AbstractAMQPConnectionWorkflow):
-    def __init__(self, _until_first_amqp_attempt: bool = ...) -> None: ...
+    def __init__(self, _until_first_amqp_attempt: bool = False) -> None: ...
     def set_io_services(self, nbio) -> None: ...
     def start(self, connection_configs, connector_factory, native_loop, on_done) -> None: ...
     def abort(self) -> None: ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/io_services_utils.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/io_services_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def check_fd_arg(fd) -> None: ...
 
 class SocketConnectionMixin:
     def connect_socket(self, sock, resolved_addr, on_done): ...
 
 class StreamingConnectionMixin:
     def create_streaming_connection(
-        self, protocol_factory, sock, on_done, ssl_context: Incomplete | None = ..., server_hostname: Incomplete | None = ...
+        self, protocol_factory, sock, on_done, ssl_context: Incomplete | None = None, server_hostname: Incomplete | None = None
     ): ...
 
 class _AsyncServiceAsyncHandle(AbstractIOReference):
     def __init__(self, subject) -> None: ...
     def cancel(self): ...
 
 class _AsyncSocketConnector:
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/nbio_interface.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/nbio_interface.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     @abc.abstractmethod
     def stop(self): ...
     @abc.abstractmethod
     def add_callback_threadsafe(self, callback): ...
     @abc.abstractmethod
     def call_later(self, delay, callback): ...
     @abc.abstractmethod
-    def getaddrinfo(self, host, port, on_done, family: int = ..., socktype: int = ..., proto: int = ..., flags: int = ...): ...
+    def getaddrinfo(self, host, port, on_done, family: int = 0, socktype: int = 0, proto: int = 0, flags: int = 0): ...
     @abc.abstractmethod
     def connect_socket(self, sock, resolved_addr, on_done): ...
     @abc.abstractmethod
     def create_streaming_connection(
-        self, protocol_factory, sock, on_done, ssl_context: Incomplete | None = ..., server_hostname: Incomplete | None = ...
+        self, protocol_factory, sock, on_done, ssl_context: Incomplete | None = None, server_hostname: Incomplete | None = None
     ): ...
 
 class AbstractFileDescriptorServices(pika.compat.AbstractBase, metaclass=abc.ABCMeta):
     @abc.abstractmethod
     def set_reader(self, fd, on_readable): ...
     @abc.abstractmethod
     def remove_reader(self, fd): ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/adapters/utils/selector_ioloop_adapter.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/adapters/utils/selector_ioloop_adapter.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -43,24 +43,24 @@
     def __init__(self, native_loop) -> None: ...
     def get_native_ioloop(self): ...
     def close(self) -> None: ...
     def run(self) -> None: ...
     def stop(self) -> None: ...
     def add_callback_threadsafe(self, callback) -> None: ...
     def call_later(self, delay, callback): ...
-    def getaddrinfo(self, host, port, on_done, family: int = ..., socktype: int = ..., proto: int = ..., flags: int = ...): ...
+    def getaddrinfo(self, host, port, on_done, family: int = 0, socktype: int = 0, proto: int = 0, flags: int = 0): ...
     def set_reader(self, fd, on_readable) -> None: ...
     def remove_reader(self, fd): ...
     def set_writer(self, fd, on_writable) -> None: ...
     def remove_writer(self, fd): ...
 
 class _FileDescriptorCallbacks:
     reader: Incomplete
     writer: Incomplete
-    def __init__(self, reader: Incomplete | None = ..., writer: Incomplete | None = ...) -> None: ...
+    def __init__(self, reader: Incomplete | None = None, writer: Incomplete | None = None) -> None: ...
 
 class _TimerHandle(nbio_interface.AbstractTimerReference):
     def __init__(self, handle, loop) -> None: ...
     def cancel(self) -> None: ...
 
 class _SelectorIOLoopIOHandle(nbio_interface.AbstractIOReference):
     def __init__(self, subject) -> None: ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/amqp_object.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/amqp_object.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/callback.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/callback.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     ONLY_CALLER: str
     def __init__(self) -> None: ...
     def add(
         self,
         prefix,
         key,
         callback,
-        one_shot: bool = ...,
-        only_caller: Incomplete | None = ...,
-        arguments: Incomplete | None = ...,
+        one_shot: bool = True,
+        only_caller: Incomplete | None = None,
+        arguments: Incomplete | None = None,
     ): ...
     def clear(self) -> None: ...
     def cleanup(self, prefix): ...
     def pending(self, prefix, key): ...
     def process(self, prefix, key, caller, *args, **keywords): ...
-    def remove(self, prefix, key, callback_value: Incomplete | None = ..., arguments: Incomplete | None = ...): ...
+    def remove(self, prefix, key, callback_value: Incomplete | None = None, arguments: Incomplete | None = None): ...
     def remove_all(self, prefix, key) -> None: ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/channel.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/channel.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -23,134 +23,141 @@
     channel_number: int
     callbacks: CallbackManager
     connection: Connection
     flow_active: bool
 
     def __init__(self, connection: Connection, channel_number: int, on_open_callback: Callable[[Self], object]) -> None: ...
     def __int__(self) -> int: ...
-    def add_callback(self, callback, replies, one_shot: bool = ...) -> None: ...
+    def add_callback(self, callback, replies, one_shot: bool = True) -> None: ...
     def add_on_cancel_callback(self, callback) -> None: ...
     def add_on_close_callback(self, callback) -> None: ...
     def add_on_flow_callback(self, callback) -> None: ...
     def add_on_return_callback(self, callback) -> None: ...
-    def basic_ack(self, delivery_tag: int = ..., multiple: bool = ...) -> None: ...
+    def basic_ack(self, delivery_tag: int = 0, multiple: bool = False) -> None: ...
     def basic_cancel(
-        self, consumer_tag: str = ..., callback: Callable[[Method[Basic.CancelOk]], object] | None = ...
+        self, consumer_tag: str = "", callback: Callable[[Method[Basic.CancelOk]], object] | None = None
     ) -> None: ...
     def basic_consume(
         self,
         queue: str,
         on_message_callback: Callable[[Channel, Basic.Deliver, BasicProperties, bytes], object],
-        auto_ack: bool = ...,
-        exclusive: bool = ...,
-        consumer_tag: str | None = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Basic.ConsumeOk]], object] | None = ...,
+        auto_ack: bool = False,
+        exclusive: bool = False,
+        consumer_tag: str | None = None,
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Basic.ConsumeOk]], object] | None = None,
     ) -> str: ...
     def basic_get(
-        self, queue: str, callback: Callable[[Channel, Basic.GetOk, BasicProperties, bytes], object], auto_ack: bool = ...
+        self, queue: str, callback: Callable[[Channel, Basic.GetOk, BasicProperties, bytes], object], auto_ack: bool = False
     ) -> None: ...
-    def basic_nack(self, delivery_tag: int = ..., multiple: bool = ..., requeue: bool = ...) -> None: ...
+    def basic_nack(self, delivery_tag: int = 0, multiple: bool = False, requeue: bool = True) -> None: ...
     def basic_publish(
-        self, exchange: str, routing_key: str, body: str | bytes, properties: BasicProperties | None = ..., mandatory: bool = ...
+        self,
+        exchange: str,
+        routing_key: str,
+        body: str | bytes,
+        properties: BasicProperties | None = None,
+        mandatory: bool = False,
     ) -> None: ...
     def basic_qos(
         self,
-        prefetch_size: int = ...,
-        prefetch_count: int = ...,
-        global_qos: bool = ...,
-        callback: Callable[[Method[Basic.QosOk]], object] | None = ...,
-    ) -> None: ...
-    def basic_reject(self, delivery_tag: int = ..., requeue: bool = ...) -> None: ...
-    def basic_recover(self, requeue: bool = ..., callback: Callable[[Method[Basic.RecoverOk]], object] | None = ...) -> None: ...
-    def close(self, reply_code: int = ..., reply_text: str = ...) -> None: ...
+        prefetch_size: int = 0,
+        prefetch_count: int = 0,
+        global_qos: bool = False,
+        callback: Callable[[Method[Basic.QosOk]], object] | None = None,
+    ) -> None: ...
+    def basic_reject(self, delivery_tag: int = 0, requeue: bool = True) -> None: ...
+    def basic_recover(
+        self, requeue: bool = False, callback: Callable[[Method[Basic.RecoverOk]], object] | None = None
+    ) -> None: ...
+    def close(self, reply_code: int = 0, reply_text: str = "Normal shutdown") -> None: ...
     def confirm_delivery(
         self,
         ack_nack_callback: Callable[[Method[Basic.Ack | Basic.Nack]], object],
-        callback: Callable[[Method[Confirm.SelectOk]], object] | None = ...,
+        callback: Callable[[Method[Confirm.SelectOk]], object] | None = None,
     ) -> None: ...
     @property
     def consumer_tags(self) -> list[str]: ...
     def exchange_bind(
         self,
         destination: str,
         source: str,
-        routing_key: str = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Exchange.BindOk]], object] | None = ...,
+        routing_key: str = "",
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Exchange.BindOk]], object] | None = None,
     ) -> None: ...
     def exchange_declare(
         self,
         exchange: str,
         exchange_type: ExchangeType | str = ...,
-        passive: bool = ...,
-        durable: bool = ...,
-        auto_delete: bool = ...,
-        internal: bool = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Exchange.DeclareOk]], object] | None = ...,
+        passive: bool = False,
+        durable: bool = False,
+        auto_delete: bool = False,
+        internal: bool = False,
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Exchange.DeclareOk]], object] | None = None,
     ) -> None: ...
     def exchange_delete(
         self,
-        exchange: str | None = ...,
-        if_unused: bool = ...,
-        callback: Callable[[Method[Exchange.DeleteOk]], object] | None = ...,
+        exchange: str | None = None,
+        if_unused: bool = False,
+        callback: Callable[[Method[Exchange.DeleteOk]], object] | None = None,
     ) -> None: ...
     def exchange_unbind(
         self,
-        destination: str | None = ...,
-        source: str | None = ...,
-        routing_key: str = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Exchange.UnbindOk]], object] | None = ...,
+        destination: str | None = None,
+        source: str | None = None,
+        routing_key: str = "",
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Exchange.UnbindOk]], object] | None = None,
     ) -> None: ...
-    def flow(self, active: bool, callback: Callable[[bool], object] | None = ...) -> None: ...
+    def flow(self, active: bool, callback: Callable[[bool], object] | None = None) -> None: ...
     @property
     def is_closed(self) -> bool: ...
     @property
     def is_closing(self) -> bool: ...
     @property
     def is_open(self) -> bool: ...
     @property
     def is_opening(self) -> bool: ...
     def open(self) -> None: ...
     def queue_bind(
         self,
         queue: str,
         exchange: str,
-        routing_key: str | None = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Queue.BindOk]], object] | None = ...,
+        routing_key: str | None = None,
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Queue.BindOk]], object] | None = None,
     ) -> None: ...
     def queue_declare(
         self,
         queue: str,
-        passive: bool = ...,
-        durable: bool = ...,
-        exclusive: bool = ...,
-        auto_delete: bool = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Queue.DeclareOk]], object] | None = ...,
+        passive: bool = False,
+        durable: bool = False,
+        exclusive: bool = False,
+        auto_delete: bool = False,
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Queue.DeclareOk]], object] | None = None,
     ) -> None: ...
     def queue_delete(
         self,
         queue: str,
-        if_unused: bool = ...,
-        if_empty: bool = ...,
-        callback: Callable[[Method[Queue.DeleteOk]], object] | None = ...,
+        if_unused: bool = False,
+        if_empty: bool = False,
+        callback: Callable[[Method[Queue.DeleteOk]], object] | None = None,
     ) -> None: ...
-    def queue_purge(self, queue: str, callback: Callable[[Method[Queue.PurgeOk]], object] | None = ...) -> None: ...
+    def queue_purge(self, queue: str, callback: Callable[[Method[Queue.PurgeOk]], object] | None = None) -> None: ...
     def queue_unbind(
         self,
         queue: str,
-        exchange: str | None = ...,
-        routing_key: str | None = ...,
-        arguments: _ArgumentMapping | None = ...,
-        callback: Callable[[Method[Queue.UnbindOk]], object] | None = ...,
+        exchange: str | None = None,
+        routing_key: str | None = None,
+        arguments: _ArgumentMapping | None = None,
+        callback: Callable[[Method[Queue.UnbindOk]], object] | None = None,
     ): ...
-    def tx_commit(self, callback: Callable[[Method[Tx.CommitOk]], object] | None = ...) -> None: ...
-    def tx_rollback(self, callback: Callable[[Method[Tx.RollbackOk]], object] | None = ...) -> None: ...
-    def tx_select(self, callback: Callable[[Method[Tx.SelectOk]], object] | None = ...) -> None: ...
+    def tx_commit(self, callback: Callable[[Method[Tx.CommitOk]], object] | None = None) -> None: ...
+    def tx_rollback(self, callback: Callable[[Method[Tx.RollbackOk]], object] | None = None) -> None: ...
+    def tx_select(self, callback: Callable[[Method[Tx.SelectOk]], object] | None = None) -> None: ...
 
 class ContentFrameAssembler:
     def __init__(self) -> None: ...
     def process(self, frame_value: Method[Any] | Header | Body) -> tuple[Incomplete, Incomplete, bytes] | None: ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/compat.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/connection.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/connection.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 class URLParameters(Parameters):
     def __init__(self, url: str) -> None: ...
 
 class SSLOptions:
     context: Incomplete
     server_hostname: Incomplete
-    def __init__(self, context, server_hostname: Incomplete | None = ...) -> None: ...
+    def __init__(self, context, server_hostname: Incomplete | None = None) -> None: ...
 
 class Connection(AbstractBase, metaclass=abc.ABCMeta):
     ON_CONNECTION_CLOSED: Final[str]
     ON_CONNECTION_ERROR: Final[str]
     ON_CONNECTION_OPEN_OK: Final[str]
     CONNECTION_CLOSED: Final[int]
     CONNECTION_INIT: Final[int]
@@ -147,34 +147,34 @@
     params: Parameters
     callbacks: CallbackManager
     server_capabilities: Incomplete
     server_properties: Incomplete
     known_hosts: Incomplete
     def __init__(
         self,
-        parameters: Parameters | None = ...,
-        on_open_callback: Callable[[Self], object] | None = ...,
-        on_open_error_callback: Callable[[Self, BaseException], object] | None = ...,
-        on_close_callback: Callable[[Self, BaseException], object] | None = ...,
-        internal_connection_workflow: bool = ...,
+        parameters: Parameters | None = None,
+        on_open_callback: Callable[[Self], object] | None = None,
+        on_open_error_callback: Callable[[Self, BaseException], object] | None = None,
+        on_close_callback: Callable[[Self, BaseException], object] | None = None,
+        internal_connection_workflow: bool = True,
     ) -> None: ...
     def add_on_close_callback(self, callback: Callable[[Self, BaseException], object]) -> None: ...
     def add_on_connection_blocked_callback(self, callback: Callable[[Self, Method[SpecConnection.Blocked]], object]) -> None: ...
     def add_on_connection_unblocked_callback(
         self, callback: Callable[[Self, Method[SpecConnection.Unblocked]], object]
     ) -> None: ...
     def add_on_open_callback(self, callback: Callable[[Self], object]) -> None: ...
     def add_on_open_error_callback(
-        self, callback: Callable[[Self, BaseException], object], remove_default: bool = ...
+        self, callback: Callable[[Self, BaseException], object], remove_default: bool = True
     ) -> None: ...
     def channel(
-        self, channel_number: int | None = ..., on_open_callback: Callable[[Channel], object] | None = ...
+        self, channel_number: int | None = None, on_open_callback: Callable[[Channel], object] | None = None
     ) -> Channel: ...
-    def update_secret(self, new_secret, reason, callback: Incomplete | None = ...) -> None: ...
-    def close(self, reply_code: int = ..., reply_text: str = ...) -> None: ...
+    def update_secret(self, new_secret, reason, callback: Incomplete | None = None) -> None: ...
+    def close(self, reply_code: int = 200, reply_text: str = "Normal shutdown") -> None: ...
     @property
     def is_closed(self) -> bool: ...
     @property
     def is_closing(self) -> bool: ...
     @property
     def is_open(self) -> bool: ...
     @property
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/credentials.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/credentials.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 LOGGER: Logger
 
 class PlainCredentials:
     TYPE: ClassVar[str]
     username: str
     password: str
     erase_on_connect: bool
-    def __init__(self, username: str, password: str, erase_on_connect: bool = ...) -> None: ...
+    def __init__(self, username: str, password: str, erase_on_connect: bool = False) -> None: ...
     def __eq__(self, other: object) -> bool: ...
     def __ne__(self, other: object) -> bool: ...
     def response_for(self, start: Connection.Start) -> tuple[str | None, bytes | None]: ...
     def erase_credentials(self) -> None: ...
 
 class ExternalCredentials:
     TYPE: ClassVar[str]
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/data.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/data.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/exceptions.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/frame.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/frame.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -37,11 +37,11 @@
     def marshal(self) -> bytes: ...
 
 class ProtocolHeader(AMQPObject):
     frame_type: int
     major: int
     minor: int
     revision: int
-    def __init__(self, major: int | None = ..., minor: int | None = ..., revision: int | None = ...) -> None: ...
+    def __init__(self, major: int | None = None, minor: int | None = None, revision: int | None = None) -> None: ...
     def marshal(self) -> bytes: ...
 
 def decode_frame(data_in: bytes) -> tuple[int, Frame | None]: ...
```

### Comparing `types-pika-ts-1.3.0.8/pika-stubs/spec.pyi` & `types-pika-ts-1.3.0.9/pika-stubs/spec.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -49,228 +49,228 @@
         version_major: Incomplete
         version_minor: Incomplete
         server_properties: Incomplete
         mechanisms: Incomplete
         locales: Incomplete
         def __init__(
             self,
-            version_major: int = ...,
-            version_minor: int = ...,
-            server_properties: Incomplete | None = ...,
+            version_major: int = 0,
+            version_minor: int = 9,
+            server_properties: Incomplete | None = None,
             mechanisms: _str = ...,
             locales: _str = ...,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class StartOk(Method):
         INDEX: ClassVar[int]
         client_properties: Incomplete
         mechanism: Incomplete
         response: Incomplete
         locale: Incomplete
         def __init__(
             self,
-            client_properties: Incomplete | None = ...,
+            client_properties: Incomplete | None = None,
             mechanism: _str = ...,
-            response: Incomplete | None = ...,
+            response: Incomplete | None = None,
             locale: _str = ...,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Secure(Method):
         INDEX: ClassVar[int]
         challenge: Incomplete
-        def __init__(self, challenge: Incomplete | None = ...) -> None: ...
+        def __init__(self, challenge: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class SecureOk(Method):
         INDEX: ClassVar[int]
         response: Incomplete
-        def __init__(self, response: Incomplete | None = ...) -> None: ...
+        def __init__(self, response: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Tune(Method):
         INDEX: ClassVar[int]
         channel_max: Incomplete
         frame_max: Incomplete
         heartbeat: Incomplete
-        def __init__(self, channel_max: int = ..., frame_max: int = ..., heartbeat: int = ...) -> None: ...
+        def __init__(self, channel_max: int = 0, frame_max: int = 0, heartbeat: int = 0) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class TuneOk(Method):
         INDEX: ClassVar[int]
         channel_max: Incomplete
         frame_max: Incomplete
         heartbeat: Incomplete
-        def __init__(self, channel_max: int = ..., frame_max: int = ..., heartbeat: int = ...) -> None: ...
+        def __init__(self, channel_max: int = 0, frame_max: int = 0, heartbeat: int = 0) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Open(Method):
         INDEX: ClassVar[int]
         virtual_host: Incomplete
         capabilities: Incomplete
         insist: Incomplete
-        def __init__(self, virtual_host: _str = ..., capabilities: _str = ..., insist: bool = ...) -> None: ...
+        def __init__(self, virtual_host: _str = ..., capabilities: _str = ..., insist: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class OpenOk(Method):
         INDEX: ClassVar[int]
         known_hosts: Incomplete
         def __init__(self, known_hosts: _str = ...) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Close(Method):
         INDEX: ClassVar[int]
         reply_code: Incomplete
         reply_text: Incomplete
         class_id: Incomplete
         method_id: Incomplete
         def __init__(
             self,
-            reply_code: Incomplete | None = ...,
+            reply_code: Incomplete | None = None,
             reply_text: _str = ...,
-            class_id: Incomplete | None = ...,
-            method_id: Incomplete | None = ...,
+            class_id: Incomplete | None = None,
+            method_id: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class CloseOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Blocked(Method):
         INDEX: ClassVar[int]
         reason: Incomplete
         def __init__(self, reason: _str = ...) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Unblocked(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class UpdateSecret(Method):
         INDEX: ClassVar[int]
         new_secret: Incomplete
         reason: Incomplete
         def __init__(self, new_secret, reason) -> None: ...
         @property
         def synchronous(self): ...
         mechanisms: Incomplete
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class UpdateSecretOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Channel(Class):
     INDEX: ClassVar[int]
 
     class Open(Method):
         INDEX: ClassVar[int]
         out_of_band: Incomplete
         def __init__(self, out_of_band: _str = ...) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class OpenOk(Method):
         INDEX: ClassVar[int]
         channel_id: Incomplete
         def __init__(self, channel_id: _str = ...) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Flow(Method):
         INDEX: ClassVar[int]
         active: Incomplete
-        def __init__(self, active: Incomplete | None = ...) -> None: ...
+        def __init__(self, active: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class FlowOk(Method):
         INDEX: ClassVar[int]
         active: Incomplete
-        def __init__(self, active: Incomplete | None = ...) -> None: ...
+        def __init__(self, active: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Close(Method):
         INDEX: ClassVar[int]
         reply_code: Incomplete
         reply_text: Incomplete
         class_id: Incomplete
         method_id: Incomplete
         def __init__(
             self,
-            reply_code: Incomplete | None = ...,
+            reply_code: Incomplete | None = None,
             reply_text: _str = ...,
-            class_id: Incomplete | None = ...,
-            method_id: Incomplete | None = ...,
+            class_id: Incomplete | None = None,
+            method_id: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class CloseOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Access(Class):
     INDEX: ClassVar[int]
 
     class Request(Method):
         INDEX: ClassVar[int]
@@ -279,32 +279,32 @@
         passive: Incomplete
         active: Incomplete
         write: Incomplete
         read: Incomplete
         def __init__(
             self,
             realm: _str = ...,
-            exclusive: bool = ...,
-            passive: bool = ...,
-            active: bool = ...,
-            write: bool = ...,
-            read: bool = ...,
+            exclusive: bool = False,
+            passive: bool = True,
+            active: bool = True,
+            write: bool = True,
+            read: bool = True,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class RequestOk(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
-        def __init__(self, ticket: int = ...) -> None: ...
+        def __init__(self, ticket: int = 1) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Exchange(Class):
     INDEX: ClassVar[int]
 
     class Declare(Method):
         INDEX: ClassVar[int]
@@ -315,117 +315,117 @@
         durable: Incomplete
         auto_delete: Incomplete
         internal: Incomplete
         nowait: Incomplete
         arguments: Incomplete
         def __init__(
             self,
-            ticket: int = ...,
-            exchange: Incomplete | None = ...,
+            ticket: int = 0,
+            exchange: Incomplete | None = None,
             type=...,
-            passive: bool = ...,
-            durable: bool = ...,
-            auto_delete: bool = ...,
-            internal: bool = ...,
-            nowait: bool = ...,
-            arguments: Incomplete | None = ...,
+            passive: bool = False,
+            durable: bool = False,
+            auto_delete: bool = False,
+            internal: bool = False,
+            nowait: bool = False,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class DeclareOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self) -> Literal[False]: ...
-        def decode(self, encoded: bytes, offset: int = ...) -> Self: ...
+        def decode(self, encoded: bytes, offset: int = 0) -> Self: ...
         def encode(self) -> list[bytes]: ...
 
     class Delete(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         exchange: Incomplete
         if_unused: Incomplete
         nowait: Incomplete
         def __init__(
-            self, ticket: int = ..., exchange: Incomplete | None = ..., if_unused: bool = ..., nowait: bool = ...
+            self, ticket: int = 0, exchange: Incomplete | None = None, if_unused: bool = False, nowait: bool = False
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class DeleteOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Bind(Method):
         INDEX: ClassVar[int]
         ticket: int
         destination: Incomplete | None
         source: Incomplete | None
         routing_key: _str
         nowait: bool
         arguments: Incomplete | None
         def __init__(
             self,
-            ticket: int = ...,
-            destination: Incomplete | None = ...,
-            source: Incomplete | None = ...,
+            ticket: int = 0,
+            destination: Incomplete | None = None,
+            source: Incomplete | None = None,
             routing_key: _str = ...,
-            nowait: bool = ...,
-            arguments: Incomplete | None = ...,
+            nowait: bool = False,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class BindOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Unbind(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         destination: Incomplete
         source: Incomplete
         routing_key: Incomplete
         nowait: Incomplete
         arguments: Incomplete
         def __init__(
             self,
-            ticket: int = ...,
-            destination: Incomplete | None = ...,
-            source: Incomplete | None = ...,
+            ticket: int = 0,
+            destination: Incomplete | None = None,
+            source: Incomplete | None = None,
             routing_key: _str = ...,
-            nowait: bool = ...,
-            arguments: Incomplete | None = ...,
+            nowait: bool = False,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class UnbindOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Queue(Class):
     INDEX: ClassVar[int]
 
     class Declare(Method):
         INDEX: ClassVar[int]
@@ -435,436 +435,436 @@
         durable: Incomplete
         exclusive: Incomplete
         auto_delete: Incomplete
         nowait: Incomplete
         arguments: Incomplete
         def __init__(
             self,
-            ticket: int = ...,
+            ticket: int = 0,
             queue: _str = ...,
-            passive: bool = ...,
-            durable: bool = ...,
-            exclusive: bool = ...,
-            auto_delete: bool = ...,
-            nowait: bool = ...,
-            arguments: Incomplete | None = ...,
+            passive: bool = False,
+            durable: bool = False,
+            exclusive: bool = False,
+            auto_delete: bool = False,
+            nowait: bool = False,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self) -> Literal[True]: ...
-        def decode(self, encoded: bytes, offset: int = ...) -> Self: ...
+        def decode(self, encoded: bytes, offset: int = 0) -> Self: ...
         def encode(self) -> list[bytes]: ...
 
     class DeclareOk(Method):
         INDEX: ClassVar[int]
         queue: _str
         message_count: int
         consumer_count: int
         def __init__(self, queue: _str, message_count: int, consumer_count: int) -> None: ...
         @property
         def synchronous(self) -> Literal[False]: ...
-        def decode(self, encoded: bytes, offset: int = ...) -> Self: ...
+        def decode(self, encoded: bytes, offset: int = 0) -> Self: ...
         def encode(self) -> list[bytes]: ...
 
     class Bind(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         queue: Incomplete
         exchange: Incomplete
         routing_key: Incomplete
         nowait: Incomplete
         arguments: Incomplete
         def __init__(
             self,
-            ticket: int = ...,
+            ticket: int = 0,
             queue: _str = ...,
-            exchange: Incomplete | None = ...,
+            exchange: Incomplete | None = None,
             routing_key: _str = ...,
-            nowait: bool = ...,
-            arguments: Incomplete | None = ...,
+            nowait: bool = False,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class BindOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Purge(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         queue: Incomplete
         nowait: Incomplete
-        def __init__(self, ticket: int = ..., queue: _str = ..., nowait: bool = ...) -> None: ...
+        def __init__(self, ticket: int = 0, queue: _str = ..., nowait: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class PurgeOk(Method):
         INDEX: ClassVar[int]
         message_count: Incomplete
-        def __init__(self, message_count: Incomplete | None = ...) -> None: ...
+        def __init__(self, message_count: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Delete(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         queue: Incomplete
         if_unused: Incomplete
         if_empty: Incomplete
         nowait: Incomplete
         def __init__(
-            self, ticket: int = ..., queue: _str = ..., if_unused: bool = ..., if_empty: bool = ..., nowait: bool = ...
+            self, ticket: int = 0, queue: _str = ..., if_unused: bool = False, if_empty: bool = False, nowait: bool = False
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class DeleteOk(Method):
         INDEX: ClassVar[int]
         message_count: Incomplete
-        def __init__(self, message_count: Incomplete | None = ...) -> None: ...
+        def __init__(self, message_count: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Unbind(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         queue: Incomplete
         exchange: Incomplete
         routing_key: Incomplete
         arguments: Incomplete
         def __init__(
             self,
-            ticket: int = ...,
+            ticket: int = 0,
             queue: _str = ...,
-            exchange: Incomplete | None = ...,
+            exchange: Incomplete | None = None,
             routing_key: _str = ...,
-            arguments: Incomplete | None = ...,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class UnbindOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Basic(Class):
     INDEX: ClassVar[int]
 
     class Qos(Method):
         INDEX: ClassVar[int]
         prefetch_size: Incomplete
         prefetch_count: Incomplete
         global_qos: Incomplete
-        def __init__(self, prefetch_size: int = ..., prefetch_count: int = ..., global_qos: bool = ...) -> None: ...
+        def __init__(self, prefetch_size: int = 0, prefetch_count: int = 0, global_qos: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class QosOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Consume(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         queue: Incomplete
         consumer_tag: Incomplete
         no_local: Incomplete
         no_ack: Incomplete
         exclusive: Incomplete
         nowait: Incomplete
         arguments: Incomplete
         def __init__(
             self,
-            ticket: int = ...,
+            ticket: int = 0,
             queue: _str = ...,
             consumer_tag: _str = ...,
-            no_local: bool = ...,
-            no_ack: bool = ...,
-            exclusive: bool = ...,
-            nowait: bool = ...,
-            arguments: Incomplete | None = ...,
+            no_local: bool = False,
+            no_ack: bool = False,
+            exclusive: bool = False,
+            nowait: bool = False,
+            arguments: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class ConsumeOk(Method):
         INDEX: ClassVar[int]
         consumer_tag: Incomplete
-        def __init__(self, consumer_tag: Incomplete | None = ...) -> None: ...
+        def __init__(self, consumer_tag: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Cancel(Method):
         INDEX: ClassVar[int]
         consumer_tag: Incomplete
         nowait: Incomplete
-        def __init__(self, consumer_tag: Incomplete | None = ..., nowait: bool = ...) -> None: ...
+        def __init__(self, consumer_tag: Incomplete | None = None, nowait: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class CancelOk(Method):
         INDEX: ClassVar[int]
         consumer_tag: Incomplete
-        def __init__(self, consumer_tag: Incomplete | None = ...) -> None: ...
+        def __init__(self, consumer_tag: Incomplete | None = None) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Publish(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         exchange: Incomplete
         routing_key: Incomplete
         mandatory: Incomplete
         immediate: Incomplete
         def __init__(
-            self, ticket: int = ..., exchange: _str = ..., routing_key: _str = ..., mandatory: bool = ..., immediate: bool = ...
+            self, ticket: int = 0, exchange: _str = ..., routing_key: _str = ..., mandatory: bool = False, immediate: bool = False
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Return(Method):
         INDEX: ClassVar[int]
         reply_code: Incomplete
         reply_text: Incomplete
         exchange: Incomplete
         routing_key: Incomplete
         def __init__(
             self,
-            reply_code: Incomplete | None = ...,
+            reply_code: Incomplete | None = None,
             reply_text: _str = ...,
-            exchange: Incomplete | None = ...,
-            routing_key: Incomplete | None = ...,
+            exchange: Incomplete | None = None,
+            routing_key: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Deliver(Method):
         INDEX: ClassVar[int]
         consumer_tag: Incomplete
         delivery_tag: Incomplete
         redelivered: Incomplete
         exchange: Incomplete
         routing_key: Incomplete
         def __init__(
             self,
-            consumer_tag: Incomplete | None = ...,
-            delivery_tag: Incomplete | None = ...,
-            redelivered: bool = ...,
-            exchange: Incomplete | None = ...,
-            routing_key: Incomplete | None = ...,
+            consumer_tag: Incomplete | None = None,
+            delivery_tag: Incomplete | None = None,
+            redelivered: bool = False,
+            exchange: Incomplete | None = None,
+            routing_key: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Get(Method):
         INDEX: ClassVar[int]
         ticket: Incomplete
         queue: Incomplete
         no_ack: Incomplete
-        def __init__(self, ticket: int = ..., queue: _str = ..., no_ack: bool = ...) -> None: ...
+        def __init__(self, ticket: int = 0, queue: _str = ..., no_ack: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class GetOk(Method):
         INDEX: ClassVar[int]
         delivery_tag: Incomplete
         redelivered: Incomplete
         exchange: Incomplete
         routing_key: Incomplete
         message_count: Incomplete
         def __init__(
             self,
-            delivery_tag: Incomplete | None = ...,
-            redelivered: bool = ...,
-            exchange: Incomplete | None = ...,
-            routing_key: Incomplete | None = ...,
-            message_count: Incomplete | None = ...,
+            delivery_tag: Incomplete | None = None,
+            redelivered: bool = False,
+            exchange: Incomplete | None = None,
+            routing_key: Incomplete | None = None,
+            message_count: Incomplete | None = None,
         ) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class GetEmpty(Method):
         INDEX: ClassVar[int]
         cluster_id: Incomplete
         def __init__(self, cluster_id: _str = ...) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Ack(Method):
         INDEX: ClassVar[int]
         delivery_tag: Incomplete
         multiple: Incomplete
-        def __init__(self, delivery_tag: int = ..., multiple: bool = ...) -> None: ...
+        def __init__(self, delivery_tag: int = 0, multiple: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Reject(Method):
         INDEX: ClassVar[int]
         delivery_tag: Incomplete
         requeue: Incomplete
-        def __init__(self, delivery_tag: Incomplete | None = ..., requeue: bool = ...) -> None: ...
+        def __init__(self, delivery_tag: Incomplete | None = None, requeue: bool = True) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class RecoverAsync(Method):
         INDEX: ClassVar[int]
         requeue: Incomplete
-        def __init__(self, requeue: bool = ...) -> None: ...
+        def __init__(self, requeue: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Recover(Method):
         INDEX: ClassVar[int]
         requeue: Incomplete
-        def __init__(self, requeue: bool = ...) -> None: ...
+        def __init__(self, requeue: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class RecoverOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Nack(Method):
         INDEX: ClassVar[int]
         delivery_tag: Incomplete
         multiple: Incomplete
         requeue: Incomplete
-        def __init__(self, delivery_tag: int = ..., multiple: bool = ..., requeue: bool = ...) -> None: ...
+        def __init__(self, delivery_tag: int = 0, multiple: bool = False, requeue: bool = True) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Tx(Class):
     INDEX: ClassVar[int]
 
     class Select(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class SelectOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Commit(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class CommitOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class Rollback(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class RollbackOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class Confirm(Class):
     INDEX: ClassVar[int]
 
     class Select(Method):
         INDEX: ClassVar[int]
         nowait: Incomplete
-        def __init__(self, nowait: bool = ...) -> None: ...
+        def __init__(self, nowait: bool = False) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
     class SelectOk(Method):
         INDEX: ClassVar[int]
         def __init__(self) -> None: ...
         @property
         def synchronous(self): ...
-        def decode(self, encoded, offset: int = ...): ...
+        def decode(self, encoded, offset: int = 0): ...
         def encode(self): ...
 
 class BasicProperties(Properties):
     CLASS: Incomplete
     INDEX: ClassVar[int]
     FLAG_CONTENT_TYPE: Incomplete
     FLAG_CONTENT_ENCODING: Incomplete
@@ -892,29 +892,29 @@
     timestamp: Incomplete
     type: Incomplete
     user_id: Incomplete
     app_id: Incomplete
     cluster_id: Incomplete
     def __init__(
         self,
-        content_type: Incomplete | None = ...,
-        content_encoding: Incomplete | None = ...,
-        headers: Incomplete | None = ...,
-        delivery_mode: Incomplete | None = ...,
-        priority: Incomplete | None = ...,
-        correlation_id: Incomplete | None = ...,
-        reply_to: Incomplete | None = ...,
-        expiration: Incomplete | None = ...,
-        message_id: Incomplete | None = ...,
-        timestamp: Incomplete | None = ...,
-        type: Incomplete | None = ...,
-        user_id: Incomplete | None = ...,
-        app_id: Incomplete | None = ...,
-        cluster_id: Incomplete | None = ...,
+        content_type: Incomplete | None = None,
+        content_encoding: Incomplete | None = None,
+        headers: Incomplete | None = None,
+        delivery_mode: Incomplete | None = None,
+        priority: Incomplete | None = None,
+        correlation_id: Incomplete | None = None,
+        reply_to: Incomplete | None = None,
+        expiration: Incomplete | None = None,
+        message_id: Incomplete | None = None,
+        timestamp: Incomplete | None = None,
+        type: Incomplete | None = None,
+        user_id: Incomplete | None = None,
+        app_id: Incomplete | None = None,
+        cluster_id: Incomplete | None = None,
     ) -> None: ...
-    def decode(self, encoded, offset: int = ...): ...
+    def decode(self, encoded, offset: int = 0): ...
     def encode(self): ...
 
 methods: Incomplete
 props: Incomplete
 
 def has_content(methodNumber): ...
```

### Comparing `types-pika-ts-1.3.0.8/setup.py` & `types-pika-ts-1.3.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 `pika`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pika. All fixes for
 types and metadata should be contributed there.
 
 The `types-pika` package contains alternate, more complete type stubs, that are maintained outside of typeshed.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2e59b81ffdb36160270fbbedb7ac78f17a85f5d2`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.3.0.8",
+      version="1.3.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pika.md",
```

### Comparing `types-pika-ts-1.3.0.8/types_pika_ts.egg-info/PKG-INFO` & `types-pika-ts-1.3.0.9/types_pika_ts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pika-ts
-Version: 1.3.0.8
+Version: 1.3.0.9
 Summary: Typing stubs for pika
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pika.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -24,8 +24,8 @@
 `pika`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pika. All fixes for
 types and metadata should be contributed there.
 
 The `types-pika` package contains alternate, more complete type stubs, that are maintained outside of typeshed.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2e59b81ffdb36160270fbbedb7ac78f17a85f5d2`.
+This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
```

### Comparing `types-pika-ts-1.3.0.8/types_pika_ts.egg-info/SOURCES.txt` & `types-pika-ts-1.3.0.9/types_pika_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

