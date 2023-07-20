# Comparing `tmp/fast_depends-2.1.2.tar.gz` & `tmp/fast_depends-2.1.3.tar.gz`

## Comparing `fast_depends-2.1.2.tar` & `fast_depends-2.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.2/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.2/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.2/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/_compat.py
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/use.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/core/build.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.2/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.1.2/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.2/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.2/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.2/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.2/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.2/LICENSE
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.2/README.md
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 fast_depends-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.3/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.3/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.3/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/__init__.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/_compat.py
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/use.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/core/build.py
+-rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.3/fast_depends/library/model.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.1.3/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.3/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.3/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.3/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.3/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.3/LICENSE
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.3/README.md
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 fast_depends-2.1.3/PKG-INFO
```

### Comparing `fast_depends-2.1.2/CONTRIBUTING.md` & `fast_depends-2.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/.github/workflows/documentation.yml` & `fast_depends-2.1.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/.github/workflows/publish_coverage.yml` & `fast_depends-2.1.3/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/.github/workflows/publish_pypi.yml` & `fast_depends-2.1.3/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/.github/workflows/tests.yml` & `fast_depends-2.1.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/fast_depends/_compat.py` & `fast_depends-2.1.3/fast_depends/_compat.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/fast_depends/use.py` & `fast_depends-2.1.3/fast_depends/use.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,18 @@
 def inject(  # pragma: no covers
     func: None,
     *,
     dependency_overrides_provider: Optional[Any] = dependency_provider,
     extra_dependencies: Sequence[model.Depends] = (),
     wrap_model: Callable[[CallModel[P, T]], CallModel[P, T]] = lambda x: x,
 ) -> Callable[
-    [Union[Callable[P, T], Callable[P, Awaitable[T]]]],
+    [
+        Union[Callable[P, T], Callable[P, Awaitable[T]]],
+        Optional[CallModel[P, T]],
+    ],
     Union[Callable[P, T], Callable[P, Awaitable[T]]],
 ]:
     ...
 
 
 @overload
 def inject(  # pragma: no covers
@@ -57,15 +60,18 @@
     *,
     dependency_overrides_provider: Optional[Any] = dependency_provider,
     extra_dependencies: Sequence[model.Depends] = (),
     wrap_model: Callable[[CallModel[P, T]], CallModel[P, T]] = lambda x: x,
 ) -> Union[
     Union[Callable[P, T], Callable[P, Awaitable[T]]],
     Callable[
-        [Union[Callable[P, T], Callable[P, Awaitable[T]]]],
+        [
+            Union[Callable[P, T], Callable[P, Awaitable[T]]],
+            Optional[CallModel[P, T]],
+        ],
         Union[Callable[P, T], Callable[P, Awaitable[T]]],
     ],
 ]:
     decorator = _wrap_inject(
         dependency_overrides_provider=dependency_overrides_provider,
         wrap_model=wrap_model,
         extra_dependencies=extra_dependencies,
@@ -82,35 +88,40 @@
     dependency_overrides_provider: Optional[Any],
     wrap_model: Callable[
         [CallModel[P, T]],
         CallModel[P, T],
     ],
     extra_dependencies: Sequence[model.Depends],
 ) -> Callable[
-    [Union[Callable[P, T], Callable[P, Awaitable[T]]]],
+    [
+        Union[Callable[P, T], Callable[P, Awaitable[T]]],
+        Optional[CallModel[P, T]],
+    ],
     Union[Callable[P, T], Callable[P, Awaitable[T]]],
 ]:
     if (
         dependency_overrides_provider
         and getattr(dependency_overrides_provider, "dependency_overrides", None)
         is not None
     ):
         overrides = dependency_overrides_provider.dependency_overrides
     else:
         overrides = None
 
     def func_wrapper(
-        func: Union[Callable[P, T], Callable[P, Awaitable[T]]]
+        func: Union[Callable[P, T], Callable[P, Awaitable[T]]],
+        model: Optional[CallModel[P, T]] = None,
     ) -> Union[Callable[P, T], Callable[P, Awaitable[T]]]:
-        model = wrap_model(
-            build_call_model(
-                func,
-                extra_dependencies=extra_dependencies,
+        if model is None:
+            model = wrap_model(
+                build_call_model(
+                    func,
+                    extra_dependencies=extra_dependencies,
+                )
             )
-        )
 
         if model.is_async:
 
             @wraps(func)
             async def injected_wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
                 async with AsyncExitStack() as stack:
                     r = await model.asolve(
```

### Comparing `fast_depends-2.1.2/fast_depends/utils.py` & `fast_depends-2.1.3/fast_depends/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
     Any,
     AsyncGenerator,
     Awaitable,
     Callable,
     ContextManager,
     Dict,
     ForwardRef,
-    Iterable,
     List,
     Tuple,
     Union,
     cast,
 )
 
 import anyio
```

### Comparing `fast_depends-2.1.2/fast_depends/core/build.py` & `fast_depends-2.1.3/fast_depends/core/build.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/fast_depends/core/model.py` & `fast_depends-2.1.3/fast_depends/core/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from contextlib import AsyncExitStack, ExitStack
 import inspect
+from contextlib import AsyncExitStack, ExitStack
 from typing import (
     Any,
     Awaitable,
     Callable,
     Dict,
     Generator,
     Generic,
@@ -200,15 +200,17 @@
         solved_kw = yield kw
 
         casted_model = self.model(**solved_kw)
 
         kwargs_ = {
             arg: getattr(casted_model, arg, solved_kw.get(arg))
             for arg in (
-                self.keyword_args + self.positional_args if not has_args else self.keyword_args
+                self.keyword_args + self.positional_args
+                if not has_args
+                else self.keyword_args
             )
         }
         kwargs_.update(getattr(casted_model, "kwargs", {}))
 
         if has_args:
             args_ = [
                 getattr(casted_model, arg, solved_kw.get(arg))
```

### Comparing `fast_depends-2.1.2/fast_depends/dependencies/model.py` & `fast_depends-2.1.3/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/fast_depends/library/model.py` & `fast_depends-2.1.3/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/LICENSE` & `fast_depends-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/README.md` & `fast_depends-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/pyproject.toml` & `fast_depends-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.2/PKG-INFO` & `fast_depends-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.1.2
+Version: 2.1.3
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
```

