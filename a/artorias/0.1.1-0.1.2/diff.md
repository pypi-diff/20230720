# Comparing `tmp/artorias-0.1.1.tar.gz` & `tmp/artorias-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "artorias-0.1.1.tar", max compression
+gzip compressed data, was "artorias-0.1.2.tar", max compression
```

## Comparing `artorias-0.1.1.tar` & `artorias-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-07-13 08:31:07.627451 artorias-0.1.1/artorias/__init__.py
--rw-r--r--   0        0        0      822 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.1/artorias/web/__init__.py
--rw-r--r--   0        0        0       23 2023-06-21 05:31:04.248093 artorias-0.1.1/artorias/web/flask/__init__.py
--rw-r--r--   0        0        0     2906 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/app.py
--rw-r--r--   0        0        0      496 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/celery.py
--rw-r--r--   0        0        0      208 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/exts.py
--rw-r--r--   0        0        0      120 2023-06-21 05:30:20.191515 artorias-0.1.1/artorias/web/flask/json.py
--rw-r--r--   0        0        0      429 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/settings.py
--rw-r--r--   0        0        0      657 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/sqlalchemy.py
--rw-r--r--   0        0        0      416 2023-07-13 07:40:04.671720 artorias-0.1.1/artorias/web/flask/utils.py
--rw-r--r--   0        0        0      611 2023-07-13 08:30:42.235315 artorias-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 artorias-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-20 03:04:50.205504 artorias-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-07-20 08:08:46.411409 artorias-0.1.2/artorias/__init__.py
+-rw-r--r--   0        0        0      822 2023-07-13 07:40:04.671720 artorias-0.1.2/artorias/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 01:30:41.560188 artorias-0.1.2/artorias/web/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-21 05:31:04.248093 artorias-0.1.2/artorias/web/flask/__init__.py
+-rw-r--r--   0        0        0     3457 2023-07-20 08:08:37.415292 artorias-0.1.2/artorias/web/flask/app.py
+-rw-r--r--   0        0        0      489 2023-07-20 07:45:51.225609 artorias-0.1.2/artorias/web/flask/celery.py
+-rw-r--r--   0        0        0      208 2023-07-13 07:40:04.671720 artorias-0.1.2/artorias/web/flask/exts.py
+-rw-r--r--   0        0        0      120 2023-06-21 05:30:20.191515 artorias-0.1.2/artorias/web/flask/json.py
+-rw-r--r--   0        0        0      445 2023-07-20 07:45:47.861566 artorias-0.1.2/artorias/web/flask/settings.py
+-rw-r--r--   0        0        0      657 2023-07-13 07:40:04.671720 artorias-0.1.2/artorias/web/flask/sqlalchemy.py
+-rw-r--r--   0        0        0      773 2023-07-20 07:45:51.225609 artorias-0.1.2/artorias/web/flask/utils.py
+-rw-r--r--   0        0        0      611 2023-07-20 08:08:49.459448 artorias-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      826 1970-01-01 00:00:00.000000 artorias-0.1.2/PKG-INFO
```

### Comparing `artorias-0.1.1/artorias/utils/__init__.py` & `artorias-0.1.2/artorias/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `artorias-0.1.1/artorias/web/flask/app.py` & `artorias-0.1.2/artorias/web/flask/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import logging
 import os
 
+from celery import Celery
 from flask import Flask as BaseFlask
 from flask.logging import default_handler
 
 from artorias.web.flask.json import JSONProvider
-from artorias.web.flask.utils import find_blueprints
+from artorias.web.flask.utils import find_blueprints, find_commands
 
 
 class Flask(BaseFlask):
     json_provider_class = JSONProvider
 
     def __init__(
         self,
@@ -42,24 +43,29 @@
 
         self.source_path = os.path.join(self.root_path, os.path.basename(self.root_path))
 
         self.load_settings(settings)
         self.init_logger()
         self.load_exts()
         self.load_blueprints()
+        self.load_commands()
         self.load_error_handlers()
 
     def load_exts(self):
+        from artorias.web.flask import celery
         from artorias.web.flask.exts import cache, cors, db, migrate
 
         db.init_app(self)
         migrate.init_app(self)
         cors.init_app(self)
         cache.init_app(self)
 
+        if self.config.get("CELERY"):
+            celery.init_app(self)
+
         if self.debug:
             with self.app_context():
                 db.create_all()
 
         @self.shell_context_processor
         def make_shell_context():
             return {"cache": cache}
@@ -74,18 +80,28 @@
 
     def load_blueprints(self):
         blueprints_package = f"{os.path.basename(self.source_path)}.apis"
         for blueprint in find_blueprints(blueprints_package):
             self.logger.debug(f"Find blueprint '{blueprint}'")
             self.register_blueprint(blueprint)
 
+    def load_commands(self):
+        commands_package = f"{os.path.basename(self.source_path)}.commands"
+        for command in find_commands(commands_package):
+            self.logger.debug(f"Find command '{command}'")
+            self.cli.add_command(command)
+
     def init_logger(self):
         self.logger.handlers.clear()
         self.logger.setLevel(logging.DEBUG if self.debug else logging.INFO)
         default_handler.setFormatter(logging.Formatter(self.config["LOGGER_FORMAT_STRING"]))
         self.logger.addHandler(default_handler)
 
     def load_error_handlers(self):
         @self.errorhandler(Exception)
         def unknown_exception(exp: Exception):
             self.logger.exception(str(exp))
             return {"error": self.config["UNKNOWN_EXCEPTION_MESSAGE"]}, 500
+
+    @property
+    def celery(self) -> Celery | None:
+        return self.extensions.get("celery")
```

### Comparing `artorias-0.1.1/artorias/web/flask/sqlalchemy.py` & `artorias-0.1.2/artorias/web/flask/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `artorias-0.1.1/pyproject.toml` & `artorias-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "artorias"
-version = "0.1.1"
+version = "0.1.2"
 description = "My web utilities"
 authors = ["Abyssknight <501835725@qq.com>"]
 readme = "README.md"
 include = ["artorias/*"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `artorias-0.1.1/PKG-INFO` & `artorias-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artorias
-Version: 0.1.1
+Version: 0.1.2
 Summary: My web utilities
 Author: Abyssknight
 Author-email: 501835725@qq.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.3.0,<24.0.0)
```

