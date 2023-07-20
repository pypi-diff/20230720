# Comparing `tmp/svc_reg-23.2.0.tar.gz` & `tmp/svc_reg-23.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Jul 13 11:01:31 2023, max compression
+gzip compressed data, last modified: Thu Jul 20 12:15:28 2023, max compression
```

## Comparing `svc_reg-23.2.0.tar` & `svc_reg-23.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      472 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        5 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.python-version-default
--rw-r--r--   0        0        0     1504 2023-07-13 11:01:31.000000 svc_reg-23.2.0/CHANGELOG.md
--rw-r--r--   0        0        0    11229 2023-07-13 11:01:31.000000 svc_reg-23.2.0/README.md
--rw-r--r--   0        0        0      294 2023-07-13 11:01:31.000000 svc_reg-23.2.0/conftest.py
--rw-r--r--   0        0        0      840 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tox.ini
--rw-r--r--   0        0        0     5482 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      291 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0       18 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      865 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/SECURITY.md
--rw-r--r--   0        0        0      117 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     3925 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      749 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1642 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.github/workflows/pypi-package.yml
--rw-r--r--   0        0        0      367 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/__init__.py
--rw-r--r--   0        0        0     5611 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/_core.py
--rw-r--r--   0        0        0     2893 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/flask.py
--rw-r--r--   0        0        0        0 2023-07-13 11:01:31.000000 svc_reg-23.2.0/src/svc_reg/py.typed
--rw-r--r--   0        0        0        0 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/__init__.py
--rw-r--r--   0        0        0     1103 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/test_async.py
--rw-r--r--   0        0        0     8819 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/test_core.py
--rw-r--r--   0        0        0     6182 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/test_flask.py
--rw-r--r--   0        0        0      684 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/typing/core.py
--rw-r--r--   0        0        0      947 2023-07-13 11:01:31.000000 svc_reg-23.2.0/tests/typing/flask_.py
--rw-r--r--   0        0        0      108 2023-07-13 11:01:31.000000 svc_reg-23.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2023-07-13 11:01:31.000000 svc_reg-23.2.0/LICENSE
--rw-r--r--   0        0        0     4143 2023-07-13 11:01:31.000000 svc_reg-23.2.0/pyproject.toml
--rw-r--r--   0        0        0     4658 2023-07-13 11:01:31.000000 svc_reg-23.2.0/PKG-INFO
+-rw-r--r--   0        0        0      472 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        5 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.python-version-default
+-rw-r--r--   0        0        0     2195 2023-07-20 12:15:28.000000 svc_reg-23.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    12930 2023-07-20 12:15:28.000000 svc_reg-23.3.0/README.md
+-rw-r--r--   0        0        0      600 2023-07-20 12:15:28.000000 svc_reg-23.3.0/conftest.py
+-rw-r--r--   0        0        0      840 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tox.ini
+-rw-r--r--   0        0        0     5482 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      291 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0       18 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      865 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/SECURITY.md
+-rw-r--r--   0        0        0      117 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3925 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      749 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1642 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.github/workflows/pypi-package.yml
+-rw-r--r--   0        0        0      476 2023-07-20 12:15:28.000000 svc_reg-23.3.0/src/svc_reg/__init__.py
+-rw-r--r--   0        0        0     6879 2023-07-20 12:15:28.000000 svc_reg-23.3.0/src/svc_reg/_core.py
+-rw-r--r--   0        0        0      234 2023-07-20 12:15:28.000000 svc_reg-23.3.0/src/svc_reg/exceptions.py
+-rw-r--r--   0        0        0     2377 2023-07-20 12:15:28.000000 svc_reg-23.3.0/src/svc_reg/flask.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:15:28.000000 svc_reg-23.3.0/src/svc_reg/py.typed
+-rw-r--r--   0        0        0       91 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     4324 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tests/test_async.py
+-rw-r--r--   0        0        0     7033 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tests/test_core.py
+-rw-r--r--   0        0        0     6053 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tests/test_flask.py
+-rw-r--r--   0        0        0     1150 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tests/typing/core.py
+-rw-r--r--   0        0        0      948 2023-07-20 12:15:28.000000 svc_reg-23.3.0/tests/typing/flask_.py
+-rw-r--r--   0        0        0      108 2023-07-20 12:15:28.000000 svc_reg-23.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2023-07-20 12:15:28.000000 svc_reg-23.3.0/LICENSE
+-rw-r--r--   0        0        0     4221 2023-07-20 12:15:28.000000 svc_reg-23.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5654 2023-07-20 12:15:28.000000 svc_reg-23.3.0/PKG-INFO
```

### Comparing `svc_reg-23.2.0/CHANGELOG.md` & `svc_reg-23.3.0/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,19 +9,38 @@
 The **third number** is for emergencies when we need to start branches for older releases.
 
 You can find our backwards-compatibility policy [here](https://github.com/hynek/svc-reg/blob/main/.github/SECURITY.md).
 
 <!-- changelog follows -->
 
 
- ## [23.2.0](https://github.com/hynek/svc-reg/compare/23.1.0...23.2.0) - 2023-07-13
+## [23.3.0](https://github.com/hynek/svc-reg/compare/23.2.0...23.3.0) - 2023-07-20
+
+### Added
+
+- Async method `Container.aget()`.
+  This was necessary for generator-based cleanups.
+  It works with sync factories too, so you can use it universally in async code.
+- Async method `ServicePing.aping()`.
+  It works with sync factories and pings too, so you can use it universally in async code.
+  [#4](https://github.com/hynek/svc-reg/pull/4)
+
+
+### Changed
+
+- Switched the cleanup mechanism from passing a function to allowing the factory to be a generator that yields the resource and can clean up after the `yield`.
+  Just like Pytest fixtures.
+  [#3](https://github.com/hynek/svc-reg/pull/3)
+
+
+## [23.2.0](https://github.com/hynek/svc-reg/compare/23.1.0...23.2.0) - 2023-07-13
 
 ### Changed
 
-- `Container.cleanup()` and `Container.acleanup` have been renamed to `close()` and `aclose*()` respectively.
+- `Container.cleanup()` and `Container.acleanup` have been renamed to `close()` and `aclose()` respectively.
 - The clean up methods are now more resilient by catching and logging exceptions at `warning` level.
   That means that if the first clean up method fails, the second one will still be called.
 - `svc_reg.flask.register_(factory|value)` now take the current Flask application as first argument.
   The old behavior moved to `svc_reg.flask.replace_(factory|value)`.
 
   The former requires no application context (and thusly be used in `init_app()`-style initializers) while the latter *does* require an application context and can be used to "monkey-patch" an existing application in tests.
```

### Comparing `svc_reg-23.2.0/README.md` & `svc_reg-23.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 > This project is only public to [gather feedback](https://github.com/hynek/svc-reg/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
-*svc-reg* is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python that lets you register factories for types/interfaces and then create instances of those types with unified life-cycle management and health checks.
+*svc-reg* is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python that lets you register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
-**This allows you to configure and manage resources in *one central place* and access them in a *consistent* way.**
+**This allows you to configure and manage resources in *one central place* and access them all in a *consistent* way.**
+
+In practice that means that at runtime, you say, for example, "*Give me a database connection*!", and *svc-reg* will give you whatever you've configured it to return when asked for a database connection.
+This can be an actual database connection or it can be a mock object for testing.
 
-The idea is that at runtime, you say, for example, "*Give me a database connection*!", and *svc-reg* will give you one, depending on how you configured it.
 If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces[^abstract].
 
 [^abstract]: In Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
 
 That:
 
 - enables **dependency injection**,
@@ -31,25 +33,46 @@
 No global mutable state is necessary – but possible for extra comfort.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
     db = request.services.get(Database)
+    api = request.services.get(WebAPIClient)
 ```
 
 or even:
 
 ```python
 def view():
     db = services.get(Database)
+    api = services.get(WebAPIClient)
 ```
 
 The latter already works with [Flask](#flask).
 
+And you set it up like this:
+
+```python
+engine = create_engine("postgresql://localhost")
+
+def engine_factory():
+    with engine.connect() as conn:
+        yield Database(conn)
+
+registry = svc_reg.Registry()
+registry.register_factory(Database, create_database)
+```
+
+The generator-based setup and cleanup may remind you of [Pytest fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
+
+Unlike typical dependency injection that passes your dependencies as arguments, the active obtainment of resources by calling `get()` when you *know* you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool -- which also puts the onus of cleanup on you), or eagerly creating resources that are never used.
+
+*svc-reg* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
+
 <!-- end-pypi -->
 
 
 ## Low-Level Core API
 
 You're unlikely to use the core API directly, but knowing what's happening underneath is good to dispel any concerns about magic.
 
@@ -91,27 +114,31 @@
 True
 >>> container.get(str)
 'Hello World'
 
 ```
 
 A container lives as long as you want the instances to live -- e.g., as long as a request lives.
-At the end, you run `container.close()` to clean up all instances that the container has created.
+
+If a factory is a generator and yields the instance, the generator will be remembered.
+At the end, you run `container.close()` and all generators will be finished (i.e. called `next(factory)` again).
 You can use this to return database connections to a pool, et cetera.
 
-If you have async cleanup functions, use `await container.aclose()` instead.
-It will run both sync and async cleanup functions.
+If you have async generators, use `await container.aclose()` instead which calls `await anext(factory)` on all async generators (and `next(factory)` on sync ones).
 
 Failing cleanups are logged at `warning` level but otherwise ignored.
 
 ---
 
 Additionally, each registered service may have a `ping` callable that you can use for health checks.
 You can request all pingable registered services with `container.get_pings()`.
 This returns a list of `ServicePing` objects that currently have a name property to identify the ping and a `ping` method that instantiates the service, adds it to the cleanup list, and runs the ping.
+If you have async resources (either factory or ping callable), you can use `aping()` instead.
+`aping()` works with sync resources too, so you can use it universally in async code.
+You can look at the `is_async` property to check whether you *need* to use `aget()`, though.
 
 Importantly: It is possible to overwrite registered service factories later -- e.g., for testing -- **without monkey-patching**.
 You have to remove possibly cached instances from the container if you're using nested dependencies (`Container.forget_service_type()`).
 The Flask integration takes care of this for you.
 
 How to achieve this in other frameworks elegantly is TBD.
 
@@ -156,32 +183,37 @@
     app.config.from_pyfile(config_filename)
 
     ##########################################################################
     # Set up the registry using Flask integration.
     app = svc_reg.flask.init_app(app)
 
     # Now, register a factory that calls `engine.connect()` if you ask for a
-    # Connections and `connection.close()` on cleanup.
+    # Connections. Since we use yield inside of a context manager, the
+    # connection gets cleaned up when the container is closed.
     # If you ask for a ping, it will run `SELECT 1` on a new connection and
     # clean up the connection behind itself.
     engine = create_engine("postgresql://localhost")
+    def engine_factory():
+        with engine.connect() as conn:
+            yield conn
+
     ping = text("SELECT 1")
     svc_reg_flask.register_factory(
         # The app argument makes it good for custom init_app() functions.
         app,
         Connection,
-        engine.connect,
-        cleanup=lambda conn: conn.close(),
+        engine_factory,
         ping=lambda conn: conn.execute(ping)
     )
 
     # You also use svc_reg WITHIN factories:
     svc_reg_flask.register_factory(
         app, # <---
         AbstractRepository,
+        # No cleanup, so we just return an object using a lambda
         lambda: Repository.from_connection(
             svc_reg.flask.get(Connection)
         ),
     )
     ##########################################################################
 
     from yourapplication.views.admin import admin
```

### Comparing `svc_reg-23.2.0/tox.ini` & `svc_reg-23.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/.github/CODE_OF_CONDUCT.md` & `svc_reg-23.3.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/.github/SECURITY.md` & `svc_reg-23.3.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/.github/workflows/ci.yml` & `svc_reg-23.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/.github/workflows/codeql-analysis.yml` & `svc_reg-23.3.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/.github/workflows/pypi-package.yml` & `svc_reg-23.3.0/.github/workflows/pypi-package.yml`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/src/svc_reg/flask.py` & `svc_reg-23.3.0/src/svc_reg/flask.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from __future__ import annotations
+# SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
 
-import warnings
+from __future__ import annotations
 
 from collections.abc import Callable
 from typing import Any
 
 from flask import Flask, current_app, g, has_app_context
 
 from ._core import Container, Registry, ServicePing
@@ -32,59 +34,51 @@
 
 
 def register_factory(
     app: Flask,
     svc_type: type,
     factory: Callable,
     *,
-    cleanup: Callable | None = None,
     ping: Callable | None = None,
 ) -> None:
-    app.config["svc_registry"].register_factory(
-        svc_type, factory, cleanup=cleanup, ping=ping
-    )
+    app.config["svc_registry"].register_factory(svc_type, factory, ping=ping)
 
 
 def register_value(
     app: Flask,
     svc_type: type,
     instance: object,
     *,
-    cleanup: Callable | None = None,
     ping: Callable | None = None,
 ) -> None:
-    app.config["svc_registry"].register_value(
-        svc_type, instance, cleanup=cleanup, ping=ping
-    )
+    app.config["svc_registry"].register_value(svc_type, instance, ping=ping)
 
 
 def replace_factory(
     svc_type: type,
     factory: Callable,
     *,
-    cleanup: Callable | None = None,
     ping: Callable | None = None,
 ) -> None:
     registry, container = _ensure_req_data()
 
     container.forget_service_type(svc_type)
-    registry.register_factory(svc_type, factory, cleanup=cleanup, ping=ping)
+    registry.register_factory(svc_type, factory, ping=ping)
 
 
 def replace_value(
     svc_type: type,
     instance: object,
     *,
-    cleanup: Callable | None = None,
     ping: Callable | None = None,
 ) -> None:
     registry, container = _ensure_req_data()
 
     container.forget_service_type(svc_type)
-    registry.register_value(svc_type, instance, cleanup=cleanup, ping=ping)
+    registry.register_value(svc_type, instance, ping=ping)
 
 
 def get_pings() -> list[ServicePing]:
     _, container = _ensure_req_data()
 
     return container.get_pings()
 
@@ -94,21 +88,14 @@
     To be used with Flask.teardown_appcontext that requires to take an
     exception.
 
     The app context is torn down after the response is sent.
     """
     if has_app_context() and (container := g.pop("svc_container", None)):
         container.close()
-        if container.async_cleanups:
-            warnings.warn(
-                f"{len(container.async_cleanups)} async cleanup(s) left, but "
-                "svc-reg's Flask support does not support them automatically.",
-                # stacklevel doesn't matter here; it's coming from a framework.
-                stacklevel=1,
-            )
 
 
 def _ensure_req_data() -> tuple[Registry, Container]:
     registry: Registry = current_app.config["svc_registry"]
     if "svc_container" not in g:
         g.svc_container = Container(registry)
```

### Comparing `svc_reg-23.2.0/tests/test_flask.py` & `svc_reg-23.3.0/tests/test_flask.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
+
 from unittest.mock import Mock
 
 import pytest
 
 import svc_reg
 
 
@@ -21,19 +25,14 @@
 @pytest.fixture(name="clean_app_ctx")
 def _clean_app_ctx(registry, app):
     svc_reg.flask.init_app(app, registry)
     with app.app_context() as ctx:
         yield ctx
 
 
-@pytest.fixture(name="registry")
-def _registry():
-    return svc_reg.Registry()
-
-
 @pytest.fixture(name="container")
 def _container(clean_app_ctx):
     return svc_reg.flask._ensure_req_data()[1]
 
 
 class Interface:
     pass
@@ -50,60 +49,62 @@
 @pytest.mark.usefixtures("clean_app_ctx")
 class TestFlask:
     def test_cleanup_added(self, registry):
         """
         get() handles the case where there is already a cleanup registered.
         """
 
-        cleanup1 = Mock(return_value=None)
-        cleanup2 = Mock(return_value=None)
+        cleanup1 = Mock()
+        cleanup2 = Mock()
+
+        def factory1():
+            yield Service1()
+            cleanup1()
+
+        def factory2():
+            yield Service2()
+            cleanup2()
 
-        registry.register_factory(Service1, Service1, cleanup=cleanup1)
-        svc_reg.flask.replace_factory(Service2, Service2, cleanup=cleanup2)
+        registry.register_factory(Service1, factory1)
+        svc_reg.flask.replace_factory(Service2, factory2)
 
         svc1 = svc_reg.flask.get(Service1)
         svc2 = svc_reg.flask.get(Service2)
 
         assert isinstance(svc1, Service1)
         assert isinstance(svc2, Service2)
+        assert 2 == len(flask.g.svc_container.cleanups)
 
         teardown(None)
 
-        cleanup1.assert_called_once_with(svc1)
-        cleanup2.assert_called_once_with(svc2)
+        cleanup1.assert_called_once_with()
+        cleanup2.assert_called_once_with()
 
-    def test_overwrite_value(self, registry, container):
+    def test_overwrite_value(self, registry):
         """
-        It's possible to overwrite an already registered type. That type's
-        cleanup is removed.
+        It's possible to overwrite an already registered type.
         """
-
-        registry.register_value(
-            Interface, Interface(), cleanup=lambda _: None, ping=lambda _: None
-        )
+        registry.register_value(Interface, Interface(), ping=lambda _: None)
 
         assert isinstance(svc_reg.flask.get(Interface), Interface)
-        assert [] != container.cleanups
 
         svc_reg.flask.replace_value(Interface, Service2())
 
         assert isinstance(svc_reg.flask.get(Interface), Service2)
         assert [] == svc_reg.flask.get_pings()
 
     def test_overwrite_factory(self, container):
         """
         It's possible to overwrite an already registered type using a factory.
         """
-
         svc_reg.flask.replace_value(
-            Interface, Interface(), cleanup=lambda _: None, ping=lambda _: None
+            Interface, Interface(), ping=lambda _: None
         )
 
         assert isinstance(svc_reg.flask.get(Interface), Interface)
-        assert [] != container.cleanups
 
         svc_reg.flask.replace_factory(Interface, Service2)
 
         assert isinstance(svc_reg.flask.get(Interface), Service2)
         assert [] == svc_reg.flask.get_pings()
 
     def test_cache(self):
@@ -116,15 +117,15 @@
         assert svc_reg.flask.get(Interface) is svc_reg.flask.get(Interface)
 
     def test_not_found(self):
         """
         Trying to get a service that hasn't been registered raises a
         ServiceNotFoundError.
         """
-        with pytest.raises(svc_reg.ServiceNotFoundError):
+        with pytest.raises(svc_reg.exceptions.ServiceNotFoundError):
             svc_reg.flask.get(Interface)
 
     def test_get_pingeable(self):
         """
         get_pingable returns only pingable svc_reg.
         """
         svc_reg.flask.replace_factory(Service1, Service1)
@@ -135,59 +136,59 @@
         ]
 
     def test_cleanup_purge_tolerant(self, container):
         """
         If other svc_reg are registered, they are ignored by the cleanup
         purge.
         """
-        svc_reg.flask.replace_factory(
-            Service1, Service1, cleanup=lambda _: None
-        )
-        svc_reg.flask.replace_factory(
-            Service2, Service2, cleanup=lambda _: None
-        )
+
+        def factory1():
+            yield Service1()
+
+        def factory2():
+            yield Service2()
+
+        svc_reg.flask.replace_factory(Service1, factory1)
+        svc_reg.flask.replace_factory(Service2, factory2)
 
         svc_reg.flask.get(Service1)
         svc_reg.flask.get(Service2)
 
         assert 2 == len(container.cleanups)
-        assert 0 == len(container.async_cleanups)
 
         svc_reg.flask.replace_factory(Service1, Interface)
 
         svc_reg.flask.get(Service1)
         svc_reg.flask.get(Service2)
 
         assert 2 == len(container.cleanups)
-        assert 0 == len(container.async_cleanups)
 
-    def test_teardown_warns_on_async_cleanups(self, container):
+    @pytest.mark.asyncio()
+    async def test_teardown_warns_on_async_cleanups(self, container):
         """
         teardown() warns if there are async cleanups.
         """
 
-        async def cleanup(svc):
-            pass
+        async def factory():
+            yield Service1()
 
-        rs = svc_reg.RegisteredService(
-            Interface, lambda: Service1(), cleanup=cleanup, ping=None
-        )
+        svc_reg.flask.replace_factory(Service1, factory)
 
-        container.add_cleanup(rs, rs.factory())
+        await container.aget(Service1)
 
         with pytest.warns(UserWarning) as wi:
             teardown(None)
 
         w = wi.pop()
 
         assert 0 == len(wi.list)
         assert (
-            "1 async cleanup(s) left, "
-            "but svc-reg's Flask support does not support them automatically."
-            == w.message.args[0]
+            "Skipped async cleanup for "
+            "<RegisteredService(svc_type=tests.test_flask.Service1, "
+            "has_ping=False)>. Use aclose() instead." == w.message.args[0]
         )
 
 
 class TestNonContextHelpers:
     def test_register_factory_helper(self, registry, app):
         """
         register_factory() registers a factory to the app that is passed.
```

### Comparing `svc_reg-23.2.0/tests/typing/flask_.py` & `svc_reg-23.3.0/tests/typing/flask_.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,37 @@
+# SPDX-FileCopyrightText: 2023 Hynek Schlawack <hs@ox.cx>
+#
+# SPDX-License-Identifier: MIT
+
+from typing import Generator
+
 from flask import Flask
 
 import svc_reg
 
 
+def factory_with_cleanup() -> Generator[int, None, None]:
+    yield 1
+
+
 reg = svc_reg.Registry()
 
 app = Flask("tests")
 app = svc_reg.flask.init_app(app, reg)
 app = svc_reg.flask.init_app(app)
 
 svc_reg.flask.replace_value(int, 1)
 svc_reg.flask.replace_value(int, 1, ping=lambda: None)
-svc_reg.flask.replace_value(int, 1, cleanup=lambda _: None)
 
 svc_reg.flask.register_value(app, int, 1)
 svc_reg.flask.register_value(app, int, 1, ping=lambda: None)
-svc_reg.flask.register_value(app, int, 1, cleanup=lambda _: None)
 
 svc_reg.flask.replace_factory(str, str)
 svc_reg.flask.replace_value(str, str, ping=lambda: None)
-svc_reg.flask.replace_value(str, str, cleanup=lambda _: None)
 
 svc_reg.flask.register_factory(app, str, str)
+svc_reg.flask.register_factory(app, int, factory_with_cleanup)
 svc_reg.flask.register_value(app, str, str, ping=lambda: None)
-svc_reg.flask.register_value(app, str, str, cleanup=lambda _: None)
 
 # The type checker believes whatever we tell it.
 o1: object = svc_reg.flask.get(object)
 o2: int = svc_reg.flask.get(object)
```

### Comparing `svc_reg-23.2.0/LICENSE` & `svc_reg-23.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `svc_reg-23.2.0/pyproject.toml` & `svc_reg-23.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -153,11 +153,15 @@
   "SIM300", # Yoda rocks in asserts
   "PT005",  # we always add underscores and explicit name
   "PT011",  # broad is fine
   "TRY002", # stock exceptions are fine in tests
   "EM101",  # no need for exception msg hygiene in tests
 ]
 
+"conftest.py" = [
+  "PT005", # we always add underscores and explicit name
+]
+
 
 [tool.ruff.isort]
 lines-between-types = 1
 lines-after-imports = 2
```

### Comparing `svc_reg-23.2.0/PKG-INFO` & `svc_reg-23.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svc-reg
-Version: 23.2.0
+Version: 23.3.0
 Summary: A Service Registry for Dependency Injection
 Project-URL: Changelog, https://github.com/hynek/svc-reg/blob/main/CHANGELOG.md
 Project-URL: Documentation, https://github.com/hynek/svc-reg/blob/main/README.md
 Project-URL: Source, https://github.com/hynek/svc-reg
 Project-URL: Funding, https://github.com/sponsors/hynek
 Author-email: Hynek Schlawack <hs@ox.cx>
 License-Expression: MIT
@@ -42,19 +42,21 @@
 > This project is only public to [gather feedback](https://github.com/hynek/svc-reg/discussions), and everything can and will change until the project is proclaimed stable.
 >
 > Currently only [**Flask** support](#flask) is production-ready, but API details can still change.
 >
 > At this point, it's unclear whether this project will become a "proper Hynek project".
 > I will keep using it for my work projects, but whether this will grow beyond my personal needs depends on community interest.
 
-*svc-reg* is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python that lets you register factories for types/interfaces and then create instances of those types with unified life-cycle management and health checks.
+*svc-reg* is a [service locator](https://en.wikipedia.org/wiki/Service_locator_pattern) for Python that lets you register factories for types/interfaces and then imperatively request instances of those types with **automatic cleanup** and **health checks**.
 
-**This allows you to configure and manage resources in *one central place* and access them in a *consistent* way.**
+**This allows you to configure and manage resources in *one central place* and access them all in a *consistent* way.**
+
+In practice that means that at runtime, you say, for example, "*Give me a database connection*!", and *svc-reg* will give you whatever you've configured it to return when asked for a database connection.
+This can be an actual database connection or it can be a mock object for testing.
 
-The idea is that at runtime, you say, for example, "*Give me a database connection*!", and *svc-reg* will give you one, depending on how you configured it.
 If you like the [*Dependency Inversion Principle*](https://en.wikipedia.org/wiki/Dependency_inversion_principle) (aka "*program against interfaces, not implementations*"), you would register concrete factories for abstract interfaces[^abstract].
 
 [^abstract]: In Python usually a [`Protocol`](https://docs.python.org/3/library/typing.html#typing.Protocol) or an [Abstract Base Class](https://docs.python.org/3.11/library/abc.html).
 
 That:
 
 - enables **dependency injection**,
@@ -65,41 +67,68 @@
 No global mutable state is necessary – but possible for extra comfort.
 
 The goal is to minimize your business code to:
 
 ```python
 def view(request):
     db = request.services.get(Database)
+    api = request.services.get(WebAPIClient)
 ```
 
 or even:
 
 ```python
 def view():
     db = services.get(Database)
+    api = services.get(WebAPIClient)
 ```
 
 The latter already works with [Flask](#flask).
 
+And you set it up like this:
+
+```python
+engine = create_engine("postgresql://localhost")
+
+def engine_factory():
+    with engine.connect() as conn:
+        yield Database(conn)
+
+registry = svc_reg.Registry()
+registry.register_factory(Database, create_database)
+```
+
+The generator-based setup and cleanup may remind you of [Pytest fixtures](https://docs.pytest.org/en/stable/explanation/fixtures.html).
+
+Unlike typical dependency injection that passes your dependencies as arguments, the active obtainment of resources by calling `get()` when you *know* you're going to need it avoids the conundrum of either having to pass a factory (e.g., a connection pool -- which also puts the onus of cleanup on you), or eagerly creating resources that are never used.
+
+*svc-reg* comes with **full async** support via a-prefixed methods (i.e. `aget()` instead of `get()`, et cetera).
+
 ---
 
 For now, please refer to the [GitHub README](https://github.com/hynek/svc-reg/blob/main/README.md) for latest documentation.
 
 
 ## Release Information
 
-### Changed
+### Added
 
-- `Container.cleanup()` and `Container.acleanup` have been renamed to `close()` and `aclose*()` respectively.
-- The clean up methods are now more resilient by catching and logging exceptions at `warning` level.
-  That means that if the first clean up method fails, the second one will still be called.
-- `svc_reg.flask.register_(factory|value)` now take the current Flask application as first argument.
-  The old behavior moved to `svc_reg.flask.replace_(factory|value)`.
+- Async method `Container.aget()`.
+  This was necessary for generator-based cleanups.
+  It works with sync factories too, so you can use it universally in async code.
+- Async method `ServicePing.aping()`.
+  It works with sync factories and pings too, so you can use it universally in async code.
+  [#4](https://github.com/hynek/svc-reg/pull/4)
+
+
+### Changed
 
-  The former requires no application context (and thusly be used in `init_app()`-style initializers) while the latter *does* require an application context and can be used to "monkey-patch" an existing application in tests.
+- Switched the cleanup mechanism from passing a function to allowing the factory to be a generator that yields the resource and can clean up after the `yield`.
+  Just like Pytest fixtures.
+  [#3](https://github.com/hynek/svc-reg/pull/3)
 
 
 ---
 
 [→ Full Changelog](https://github.com/hynek/svc-reg/blob/main/CHANGELOG.md)
```

