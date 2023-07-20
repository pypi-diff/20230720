# Comparing `tmp/busrt_worker-0.1.0.tar.gz` & `tmp/busrt_worker-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "busrt_worker-0.1.0.tar", max compression
+gzip compressed data, was "busrt_worker-0.1.1.tar", max compression
```

## Comparing `busrt_worker-0.1.0.tar` & `busrt_worker-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       39 2023-07-18 02:59:48.051098 busrt_worker-0.1.0/busrtworker/__init__.py
--rw-r--r--   0        0        0     8700 2023-07-18 03:10:10.352938 busrt_worker-0.1.0/busrtworker/app.py
--rw-r--r--   0        0        0     4066 2023-07-18 03:10:10.357938 busrt_worker-0.1.0/busrtworker/boostrap.py
--rw-r--r--   0        0        0      117 2023-07-18 02:59:55.837311 busrt_worker-0.1.0/busrtworker/busrt/__init__.py
--rw-r--r--   0        0        0    10317 2023-07-18 02:40:18.995051 busrt_worker-0.1.0/busrtworker/busrt/busrt_client.py
--rw-r--r--   0        0        0     9010 2023-07-18 02:46:57.526113 busrt_worker-0.1.0/busrtworker/busrt/busrt_rpc.py
--rw-r--r--   0        0        0      263 2023-07-18 03:12:04.012287 busrt_worker-0.1.0/busrtworker/busrt/msgutils.py
--rw-r--r--   0        0        0       47 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/__init__.py
--rw-r--r--   0        0        0       22 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/__verstion__.py
--rw-r--r--   0        0        0     3229 2023-07-18 02:23:29.228345 busrt_worker-0.1.0/busrtworker/kink/container.py
--rw-r--r--   0        0        0      169 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/errors/__init__.py
--rw-r--r--   0        0        0       45 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/errors/conainer_error.py
--rw-r--r--   0        0        0       92 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/errors/execution_error.py
--rw-r--r--   0        0        0       91 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/errors/resolver_error.py
--rw-r--r--   0        0        0      100 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/errors/service_error.py
--rw-r--r--   0        0        0     7639 2023-07-17 00:23:25.187332 busrt_worker-0.1.0/busrtworker/kink/inject.py
--rw-r--r--   0        0        0        0 2023-07-15 20:20:34.000000 busrt_worker-0.1.0/busrtworker/kink/py.typed
--rw-r--r--   0        0        0     4097 2023-07-18 02:27:55.216504 busrt_worker-0.1.0/busrtworker/scheduler/__init__.py
--rw-r--r--   0        0        0     5783 2023-07-15 06:24:47.677691 busrt_worker-0.1.0/busrtworker/tree.py
--rw-r--r--   0        0        0     1131 2023-07-18 05:37:11.393552 busrt_worker-0.1.0/LICENSE
--rw-r--r--   0        0        0      897 2023-07-18 06:12:44.330749 busrt_worker-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-07-18 05:35:24.058761 busrt_worker-0.1.0/README.md
--rw-r--r--   0        0        0     2651 1970-01-01 00:00:00.000000 busrt_worker-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       39 2023-07-18 02:59:48.051098 busrt_worker-0.1.1/busrtworker/__init__.py
+-rw-r--r--   0        0        0     8986 2023-07-20 10:00:54.825132 busrt_worker-0.1.1/busrtworker/app.py
+-rw-r--r--   0        0        0     4066 2023-07-18 03:10:10.357938 busrt_worker-0.1.1/busrtworker/boostrap.py
+-rw-r--r--   0        0        0      117 2023-07-18 02:59:55.837311 busrt_worker-0.1.1/busrtworker/busrt/__init__.py
+-rw-r--r--   0        0        0    10317 2023-07-18 02:40:18.995051 busrt_worker-0.1.1/busrtworker/busrt/busrt_client.py
+-rw-r--r--   0        0        0     9010 2023-07-18 02:46:57.526113 busrt_worker-0.1.1/busrtworker/busrt/busrt_rpc.py
+-rw-r--r--   0        0        0      315 2023-07-19 08:08:55.838990 busrt_worker-0.1.1/busrtworker/busrt/msgutils.py
+-rw-r--r--   0        0        0       47 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/__verstion__.py
+-rw-r--r--   0        0        0     3229 2023-07-18 02:23:29.228345 busrt_worker-0.1.1/busrtworker/kink/container.py
+-rw-r--r--   0        0        0      169 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/errors/__init__.py
+-rw-r--r--   0        0        0       45 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/errors/conainer_error.py
+-rw-r--r--   0        0        0       92 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/errors/execution_error.py
+-rw-r--r--   0        0        0       91 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/errors/resolver_error.py
+-rw-r--r--   0        0        0      100 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/errors/service_error.py
+-rw-r--r--   0        0        0     7639 2023-07-17 00:23:25.187332 busrt_worker-0.1.1/busrtworker/kink/inject.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:20:34.000000 busrt_worker-0.1.1/busrtworker/kink/py.typed
+-rw-r--r--   0        0        0     4097 2023-07-18 02:27:55.216504 busrt_worker-0.1.1/busrtworker/scheduler/__init__.py
+-rw-r--r--   0        0        0     5783 2023-07-15 06:24:47.677691 busrt_worker-0.1.1/busrtworker/tree.py
+-rw-r--r--   0        0        0     1131 2023-07-18 05:37:11.393552 busrt_worker-0.1.1/LICENSE
+-rw-r--r--   0        0        0      858 2023-07-20 10:00:54.833130 busrt_worker-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1982 2023-07-18 05:35:24.058761 busrt_worker-0.1.1/README.md
+-rw-r--r--   0        0        0     2650 1970-01-01 00:00:00.000000 busrt_worker-0.1.1/PKG-INFO
```

### Comparing `busrt_worker-0.1.0/busrtworker/app.py` & `busrt_worker-0.1.1/busrtworker/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 import signal
 from collections import UserList
 from enum import Enum, auto
 from typing import Callable, Coroutine, Dict, List, Optional
 
 from loguru import logger
 
+from busrtworker import kink
 from busrtworker.boostrap import RpcBoot
 from busrtworker.busrt import OP_PUBLISH, Client, Frame, Rpc, serialize
+from busrtworker.kink import di
 from busrtworker.scheduler import ScheduledTaskRunner
 from busrtworker.tree import RadixTree
 
 
 @dataclasses.dataclass
 class ConnectionInfo:
     name: str = dataclasses.field()
@@ -60,24 +62,24 @@
         self.name = connection.name
         self.app = app
         if self.name not in self.app.callers:
             self.app.callers[self.name] = {}
         if self.name not in self.app.subscribes:
             self.app.subscribes[self.name] = Router()
 
-    def on_call(self, method=None, auto_decode=True, raw=False):
+    def on_call(self, method=None, auto_decode: bool = True, raw: bool = False):
         def _warp(f):
             target = method or (f.func.__name__ if isinstance(f, functools.partial) else f.__name__)
             self.app.callers[self.name][target] = (f, auto_decode, asyncio.iscoroutinefunction(f), raw)
             return f
 
         return _warp
 
-    def subscribe(self, topic, auto_decode=True, raw=False):
-        assert isinstance(topic, str), 'topic must be str or callable'
+    def subscribe(self, topic: str, auto_decode: bool = True, raw: bool = False):
+        assert isinstance(topic, str), 'topic must be str'
 
         def _warp(f):
             self.app.subscribes[self.name].insert(topic, (f, auto_decode, asyncio.iscoroutinefunction(f), raw),
                                                   '/:' in topic)
             return f
 
         return _warp
@@ -172,14 +174,16 @@
     callers: dict[str, callable] = {}
     subscribes: dict[str, Router] = {}
     connections: Dict[str, ConnectionInfo] = {}
     closeable = []
     on_frame_default: callable = on_frame_default
     on_call_default: callable = on_call_default
     task_runners = []
+    provider = kink.provider
+    inject = kink.inject
 
     def __init__(self):
         Freezable.__init__(self)
         self.boot = RpcBoot()
         self._on_startup: Signal = Signal(self)
         self._on_shutdown: Signal = Signal(self)
         self._on_startup.append(self.boot.startup)
@@ -241,14 +245,20 @@
         Registers a coroutine to be awaited for during app shutdown
         """
         self._on_shutdown.append(coro)
 
     def __getattr__(self, name):
         return self.connections[name]
 
+    def __getitem__(self, name):
+        return self.connections[name]
+
+    def __setitem__(self, key, value):
+        di[key] = value
+
     def run_every(self, seconds: int, options: Optional[Dict] = None):
         """
         Registers a coroutine to be called with a given interval
         """
         if options is None:
             options = {}
```

### Comparing `busrt_worker-0.1.0/busrtworker/boostrap.py` & `busrt_worker-0.1.1/busrtworker/boostrap.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/busrtworker/busrt/busrt_client.py` & `busrt_worker-0.1.1/busrtworker/busrt/busrt_client.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/busrtworker/busrt/busrt_rpc.py` & `busrt_worker-0.1.1/busrtworker/busrt/busrt_rpc.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/busrtworker/kink/container.py` & `busrt_worker-0.1.1/busrtworker/kink/container.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/busrtworker/kink/inject.py` & `busrt_worker-0.1.1/busrtworker/kink/inject.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/busrtworker/scheduler/__init__.py` & `busrt_worker-0.1.1/busrtworker/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/busrtworker/tree.py` & `busrt_worker-0.1.1/busrtworker/tree.py`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/LICENSE` & `busrt_worker-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/pyproject.toml` & `busrt_worker-0.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [tool.poetry]
 name = "busrt-worker"
-version = "0.1.0"
+version = "0.1.1"
 description = "busrt-worker is a Python-based async busrt message handle framework"
 authors = ["JimZhang <zzl22100048@gmail.com>"]
 repository = "https://git.loom.run/Coder/amqp-worker"
 readme = "README.md"
 packages = [{include = "busrtworker"}]
 keywords = ["busrt", "message", "rpc"]
 license = "MIT"
 [tool.poetry.dependencies]
 python = "^3.10"
 msgpack = "^1.0.5"
-zstd = "^1.5.5.1"
 loguru = "^0.7.0"
+cramjam = "^2.6.2"
 
 
-[tool.poetry.group.dev.dependencies]
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [[tool.poetry.source]]
 name = "baidu"
```

### Comparing `busrt_worker-0.1.0/README.md` & `busrt_worker-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `busrt_worker-0.1.0/PKG-INFO` & `busrt_worker-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: busrt-worker
-Version: 0.1.0
+Version: 0.1.1
 Summary: busrt-worker is a Python-based async busrt message handle framework
 Home-page: https://git.loom.run/Coder/amqp-worker
 License: MIT
 Keywords: busrt,message,rpc
 Author: JimZhang
 Author-email: zzl22100048@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cramjam (>=2.6.2,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: msgpack (>=1.0.5,<2.0.0)
-Requires-Dist: zstd (>=1.5.5.1,<2.0.0.0)
 Project-URL: Repository, https://git.loom.run/Coder/amqp-worker
 Description-Content-Type: text/markdown
 
 # Busrt Worker
 > `BUS/RT`是一个快速、灵活且非常易于使用的框架，它使用Rust/Tokio编写，受到NATS、ZeroMQ和Nanomsg的启发。
 
 Busrt Worker是一个基于busrt消息中间件的异步框架，它对Python库进行了封装，使其更易于使用。
```

