# Comparing `tmp/async_wrapper-0.1.3.tar.gz` & `tmp/async_wrapper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.1.3.tar", max compression
+gzip compressed data, was "async_wrapper-0.1.4.tar", max compression
```

## Comparing `async_wrapper-0.1.3.tar` & `async_wrapper-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1070 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/LICENSE
--rw-r--r--   0        0        0     1610 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/README.md
--rw-r--r--   0        0        0     3648 2023-06-27 12:37:49.717504 async_wrapper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      354 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-06-27 12:37:49.749504 async_wrapper-0.1.3/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0      896 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      706 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1217 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1581 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      165 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0     2561 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/_anyio.py
--rw-r--r--   0        0        0     2253 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/_asyncio.py
--rw-r--r--   0        0        0     2123 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/base.py
--rw-r--r--   0        0        0     1966 2023-06-27 12:37:36.365415 async_wrapper-0.1.3/src/async_wrapper/task_group/main.py
--rw-r--r--   0        0        0     2723 1970-01-01 00:00:00.000000 async_wrapper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-07-20 11:12:04.820027 async_wrapper-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1892 2023-07-20 11:12:04.820027 async_wrapper-0.1.4/README.md
+-rw-r--r--   0        0        0     3648 2023-07-20 11:12:20.764335 async_wrapper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      419 2023-07-20 11:12:04.820027 async_wrapper-0.1.4/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-20 11:12:20.804336 async_wrapper-0.1.4/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0      896 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      706 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1217 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1581 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      209 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0     3495 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/_anyio.py
+-rw-r--r--   0        0        0     2960 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/_asyncio.py
+-rw-r--r--   0        0        0     2491 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/base.py
+-rw-r--r--   0        0        0     2735 2023-07-20 11:12:04.824027 async_wrapper-0.1.4/src/async_wrapper/task_group/main.py
+-rw-r--r--   0        0        0     3005 1970-01-01 00:00:00.000000 async_wrapper-0.1.4/PKG-INFO
```

### Comparing `async_wrapper-0.1.3/LICENSE` & `async_wrapper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/README.md` & `async_wrapper-0.1.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
 
 import asyncio
+import time
 
-# or(>=py311)
-# from asyncio.taskgroups import TaskGroup
-from async_wrapper import async_to_sync, get_task_group_factory, get_task_group_wrapper
+from async_wrapper import (
+    async_to_sync,
+    get_semaphore_class,
+    get_task_group_factory,
+    get_task_group_wrapper,
+)
 
 
 @async_to_sync("thread")
 async def sample_func() -> int:
     await asyncio.sleep(1)
     return 1
 
@@ -42,20 +46,30 @@
     await asyncio.sleep(1)
     return x
 
 
 async def main():
     wrapper = get_task_group_wrapper("asyncio")
     factory = get_task_group_factory("asyncio")
+    Semaphore = get_semaphore_class("asyncio")
+    semaphore = Semaphore(2)
+
+    start = time.perf_counter()
     async with factory() as task_group:
-        value_1 = wrapper(sample_func_2, task_group)(1)
-        value_2 = wrapper(sample_func_2, task_group)(2)
+        wrapped = wrapper(sample_func_2, task_group, semaphore)
+        value_1 = wrapped(1)
+        value_2 = wrapped(2)
+        value_3 = wrapped(3)
+    end = time.perf_counter()
 
     assert isinstance(value_1.value, int)
     assert isinstance(value_2.value, int)
+    assert isinstance(value_3.value, int)
     assert value_1.value == 1
     assert value_2.value == 2
+    assert value_3.value == 3
+    assert 1.5 < end - start < 2.5
 ```
 
 ## License
 
 MIT, see [LICENSE](https://github.com/phi-friday/async-wrapper/blob/main/LICENSE).
```

### Comparing `async_wrapper-0.1.3/pyproject.toml` & `async_wrapper-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.1.3"
+version = "0.1.4"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
```

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/main.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.1.4/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.1.3/src/async_wrapper/task_group/_anyio.py` & `async_wrapper-0.1.4/src/async_wrapper/task_group/_asyncio.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,76 @@
 from __future__ import annotations
 
+import sys
+from asyncio import Semaphore as AsyncioSemaphore
+from contextlib import AsyncExitStack
 from functools import partial, wraps
 from typing import (
+    TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
     Coroutine,
     Generic,
     TypeVar,
     final,
 )
 
-from typing_extensions import ParamSpec, override
+from typing_extensions import ParamSpec, Self, override
 
-from async_wrapper.task_group.base import BaseSoonWrapper, SoonValue
+from async_wrapper.task_group.base import BaseSoonWrapper, Semaphore, SoonValue
 
-try:
-    from anyio.abc import TaskGroup  # type: ignore
-except ImportError:
-    from typing import Any as TaskGroup
+if sys.version_info < (3, 11):
+    from aiotools.taskgroup import TaskGroup  # type: ignore
+else:
+    from asyncio.taskgroups import TaskGroup  # type: ignore
 
 
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
-__all__ = ["SoonWrapper", "wrap_soon", "get_task_group"]
+__all__ = ["SoonWrapper", "wrap_soon", "get_task_group", "get_semaphore_class"]
 
 
 @final
 class SoonWrapper(
     BaseSoonWrapper[TaskGroup, ParamT, ValueT_co],
     Generic[ParamT, ValueT_co],
 ):
-    @override
-    def __new__(
-        cls,
-        func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
-        task_group: TaskGroup,
-    ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
-        try:
-            import anyio  # type: ignore # noqa: F401
-        except ImportError as exc:
-            raise ImportError("install extas anyio first") from exc
+    if TYPE_CHECKING:
 
-        return super().__new__(cls, func, task_group)  # type: ignore
+        @override
+        def __new__(
+            cls,
+            func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
+            task_group: TaskGroup,
+            semaphore: Semaphore | None = None,
+        ) -> SoonWrapper[OtherParamT, OtherValueT_co]:
+            ...
 
     @override
     def __init__(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: TaskGroup,
+        semaphore: Semaphore | None = None,
     ) -> None:
-        super().__init__(func, task_group)
+        super().__init__(func, task_group, semaphore)
 
         def outer(
             result: SoonValue[ValueT_co],
         ) -> Callable[ParamT, None]:
             @wraps(self.func)
             def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> None:
                 partial_func = partial(self.func, *args, **kwargs)
-                set_value_func = partial(_set_value, partial_func, result)
-                task_group.start_soon(set_value_func)
+                set_value_func = partial(_set_value, partial_func, result, semaphore)
+                task_group.create_task(set_value_func())
 
             return inner
 
         self._func = outer
 
     @override
     def __call__(
@@ -75,25 +78,32 @@
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
         result: SoonValue[ValueT_co] = SoonValue()
         self._func(result)(*args, **kwargs)
         return result
 
+    @override
+    def copy(self, semaphore: Semaphore | None = None) -> Self:
+        if semaphore is None:
+            semaphore = self.semaphore
+        return SoonWrapper(self.func, self.task_group, semaphore)
+
 
-def get_task_group() -> TaskGroup:
-    try:
-        from anyio import create_task_group  # type: ignore
-    except ImportError as exc:
-        raise ImportError("install extas anyio first") from exc
-    return create_task_group()
+def get_semaphore_class() -> type[AsyncioSemaphore]:
+    return AsyncioSemaphore
 
 
 async def _set_value(
     func: Callable[[], Coroutine[Any, Any, ValueT]],
     value: SoonValue[ValueT],
+    semaphore: Semaphore | None,
 ) -> None:
-    result = await func()
+    async with AsyncExitStack() as stack:
+        if semaphore is not None:
+            await stack.enter_async_context(semaphore)
+        result = await func()
     value.value = result
 
 
 wrap_soon = SoonWrapper
+get_task_group = TaskGroup
```

### Comparing `async_wrapper-0.1.3/src/async_wrapper/task_group/base.py` & `async_wrapper-0.1.4/src/async_wrapper/task_group/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
+from contextlib import AbstractAsyncContextManager
 from threading import local
-from typing import (
-    Any,
-    Awaitable,
-    Callable,
-    Generic,
-    Protocol,
-    TypeVar,
-)
+from typing import Any, Awaitable, Callable, Generic, Protocol, TypeVar
 
-from typing_extensions import ParamSpec, override
+from typing_extensions import ParamSpec, Self, override
 
 from async_wrapper.convert.synclib.base import as_coro_func
 
 TaskGroupT = TypeVar("TaskGroupT")
 TaskGroupT_co = TypeVar("TaskGroupT_co", covariant=True)
 ValueT = TypeVar("ValueT")
 ValueT_co = TypeVar("ValueT_co", covariant=True)
@@ -27,39 +21,51 @@
 __all__ = ["PendingError", "BaseSoonWrapper", "SoonValue", "TaskGroupFactory"]
 
 
 class PendingError(Exception):
     ...
 
 
+class Semaphore(AbstractAsyncContextManager, Protocol):
+    async def acquire(self) -> Any:
+        ...
+
+
 class BaseSoonWrapper(ABC, Generic[TaskGroupT, ParamT, ValueT_co]):
     def __init__(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: TaskGroupT,
+        semaphore: Semaphore | None = None,
     ) -> None:
         self.func = as_coro_func(func)
         self.task_group = task_group
+        self.semaphore = semaphore
 
     @override
     def __new__(
         cls,
         func: Callable[OtherParamT, Awaitable[OtherValueT_co]],
         task_group: TaskGroupT,
+        semaphore: Semaphore | None = None,
     ) -> BaseSoonWrapper[TaskGroupT, OtherParamT, OtherValueT_co]:
         return super().__new__(cls)  # type: ignore
 
     @abstractmethod
     def __call__(  # noqa: D102
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
         ...
 
+    @abstractmethod
+    def copy(self, semaphore: Semaphore | None = None) -> Self:  # noqa: D102
+        ...
+
 
 class SoonValue(Generic[ValueT_co]):
     def __init__(self) -> None:
         self._value = Pending
 
     @property
     def value(self) -> ValueT_co:  # noqa: D102
```

### Comparing `async_wrapper-0.1.3/src/async_wrapper/task_group/main.py` & `async_wrapper-0.1.4/src/async_wrapper/task_group/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING, Literal, overload
 
 if TYPE_CHECKING:
     from async_wrapper.task_group import _anyio as anyio_task_group
     from async_wrapper.task_group import _asyncio as asyncio_task_group
     from async_wrapper.task_group.base import TaskGroupFactory
 
-__all__ = ["get_task_group_wrapper", "get_task_group_factory"]
+__all__ = ["get_task_group_wrapper", "get_task_group_factory", "get_semaphore_class"]
 
 DEFAULT_BACKEND = "asyncio"
 TaskGroupBackendType = Literal["asyncio", "anyio"]
 
 
 @overload
 def get_task_group_wrapper(
@@ -75,7 +75,39 @@
         task group factory
     """
     if not backend:
         backend = DEFAULT_BACKEND
 
     module = importlib.import_module(f"._{backend}", __package__)
     return module.get_task_group
+
+
+@overload
+def get_semaphore_class(
+    backend: Literal["asyncio"] | None = ...,
+) -> type[asyncio_task_group.AsyncioSemaphore]:
+    ...
+
+
+@overload
+def get_semaphore_class(
+    backend: Literal["anyio"] = ...,
+) -> type[anyio_task_group.AnyioSemaphore]:
+    ...
+
+
+def get_semaphore_class(
+    backend: TaskGroupBackendType | None = None,
+) -> type[asyncio_task_group.AsyncioSemaphore] | type[anyio_task_group.AnyioSemaphore]:
+    """get semaphore class using in wrap func
+
+    Args:
+        backend: asyncio or anyio. Defaults to None.
+
+    Returns:
+        semaphore class
+    """
+    if not backend:
+        backend = DEFAULT_BACKEND
+
+    module = importlib.import_module(f"._{backend}", __package__)
+    return module.get_semaphore_class()
```

### Comparing `async_wrapper-0.1.3/PKG-INFO` & `async_wrapper-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.1.3
+Version: 0.1.4
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -44,18 +44,22 @@
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
 
 import asyncio
+import time
 
-# or(>=py311)
-# from asyncio.taskgroups import TaskGroup
-from async_wrapper import async_to_sync, get_task_group_factory, get_task_group_wrapper
+from async_wrapper import (
+    async_to_sync,
+    get_semaphore_class,
+    get_task_group_factory,
+    get_task_group_wrapper,
+)
 
 
 @async_to_sync("thread")
 async def sample_func() -> int:
     await asyncio.sleep(1)
     return 1
 
@@ -69,21 +73,31 @@
     await asyncio.sleep(1)
     return x
 
 
 async def main():
     wrapper = get_task_group_wrapper("asyncio")
     factory = get_task_group_factory("asyncio")
+    Semaphore = get_semaphore_class("asyncio")
+    semaphore = Semaphore(2)
+
+    start = time.perf_counter()
     async with factory() as task_group:
-        value_1 = wrapper(sample_func_2, task_group)(1)
-        value_2 = wrapper(sample_func_2, task_group)(2)
+        wrapped = wrapper(sample_func_2, task_group, semaphore)
+        value_1 = wrapped(1)
+        value_2 = wrapped(2)
+        value_3 = wrapped(3)
+    end = time.perf_counter()
 
     assert isinstance(value_1.value, int)
     assert isinstance(value_2.value, int)
+    assert isinstance(value_3.value, int)
     assert value_1.value == 1
     assert value_2.value == 2
+    assert value_3.value == 3
+    assert 1.5 < end - start < 2.5
 ```
 
 ## License
 
 MIT, see [LICENSE](https://github.com/phi-friday/async-wrapper/blob/main/LICENSE).
```

