# Comparing `tmp/setuplog-0.3.1.tar.gz` & `tmp/setuplog-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuplog-0.3.1.tar", max compression
+gzip compressed data, was "setuplog-0.4.1.tar", max compression
```

## Comparing `setuplog-0.3.1.tar` & `setuplog-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1053 2022-01-11 15:00:56.828150 setuplog-0.3.1/LICENSE
--rw-r--r--   0        0        0      902 2022-01-11 15:00:56.829656 setuplog-0.3.1/README.md
--rw-r--r--   0        0        0     1142 2022-03-14 20:28:50.514059 setuplog-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      343 2022-03-14 16:35:25.666061 setuplog-0.3.1/src/setuplog/__init__.py
--rw-r--r--   0        0        0      997 2022-03-14 17:01:09.720919 setuplog-0.3.1/src/setuplog/adaptors.py
--rw-r--r--   0        0        0     1329 2022-03-14 16:50:34.867339 setuplog-0.3.1/src/setuplog/decorator.py
--rw-r--r--   0        0        0      461 2022-01-11 15:00:56.841784 setuplog-0.3.1/src/setuplog/formatters.py
--rw-r--r--   0        0        0     2481 2022-03-14 20:22:22.523139 setuplog-0.3.1/src/setuplog/logger.py
--rw-r--r--   0        0        0        0 2022-01-11 17:39:49.281259 setuplog-0.3.1/src/setuplog/py.typed
--rw-r--r--   0        0        0     3751 2022-01-11 15:00:56.843212 setuplog-0.3.1/src/setuplog/setup.py
--rw-r--r--   0        0        0     1506 2022-03-14 20:30:13.031288 setuplog-0.3.1/setup.py
--rw-r--r--   0        0        0     1538 2022-03-14 20:30:13.031638 setuplog-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-07-20 15:56:55.207905 setuplog-0.4.1/LICENSE
+-rw-r--r--   0        0        0      902 2023-07-20 15:56:55.207905 setuplog-0.4.1/README.md
+-rw-r--r--   0        0        0     1142 2023-07-20 15:56:55.211905 setuplog-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      343 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/__init__.py
+-rw-r--r--   0        0        0      997 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/adaptors.py
+-rw-r--r--   0        0        0     1329 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/decorator.py
+-rw-r--r--   0        0        0      461 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/formatters.py
+-rw-r--r--   0        0        0     2495 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/logger.py
+-rw-r--r--   0        0        0        0 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/py.typed
+-rw-r--r--   0        0        0     3652 2023-07-20 15:56:55.211905 setuplog-0.4.1/src/setuplog/setup.py
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 setuplog-0.4.1/setup.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 setuplog-0.4.1/PKG-INFO
```

### Comparing `setuplog-0.3.1/LICENSE` & `setuplog-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `setuplog-0.3.1/README.md` & `setuplog-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `setuplog-0.3.1/pyproject.toml` & `setuplog-0.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "setuplog"
-version = "0.3.1"
+version = "0.4.1"
 description = ""
 authors = []
 license = "MIT"
 keywords = [ "logging", "logger", "log" ]
 repository = "https://github.com/schireson/setuplog"
 packages = [
     { from = "src", include = "setuplog" },
```

### Comparing `setuplog-0.3.1/src/setuplog/adaptors.py` & `setuplog-0.4.1/src/setuplog/adaptors.py`

 * *Files identical despite different names*

### Comparing `setuplog-0.3.1/src/setuplog/decorator.py` & `setuplog-0.4.1/src/setuplog/decorator.py`

 * *Files identical despite different names*

### Comparing `setuplog-0.3.1/src/setuplog/logger.py` & `setuplog-0.4.1/src/setuplog/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,16 @@
     segments = []
     namespace = getattr(logging.config, "namespace", "")
     if namespace:
         segments.append(namespace)
 
     style_adaptor = getattr(logging.config, "style_adaptor", None)
 
-    # Ensure the logger name is pulled from 2 frames up rather than from the local frame. One frame for this function, and one for the
-    # `_Logging` function calls.
+    # Ensure the logger name is pulled from 2 frames up rather than from the local frame.
+    # One frame for this function, and one for the `_Logging` function calls.
     frame_name = sys._getframe(2).f_globals["__name__"]
     segments.append(frame_name)
 
     name = ".".join(segments)
     return _cached_logger(name, style_adaptor=style_adaptor)
 
 
@@ -62,15 +62,17 @@
         logger = get_logger()
         logger.warning(msg, *args, **kwargs)
 
     def error(self, msg: Union[object, str, M], *args: Any, **kwargs: Any) -> None:
         logger = get_logger()
         logger.error(msg, *args, **kwargs)
 
-    def exception(self, msg: Union[object, str, M], *args: Any, exc_info=True, **kwargs: Any) -> None:
+    def exception(
+        self, msg: Union[object, str, M], *args: Any, exc_info=True, **kwargs: Any
+    ) -> None:
         logger = get_logger()
         logger.exception(msg, *args, exc_info=exc_info, **kwargs)
 
     def critical(self, msg: Union[object, str, M], *args: Any, **kwargs: Any) -> None:
         logger = get_logger()
         logger.critical(msg, *args, **kwargs)
```

### Comparing `setuplog-0.3.1/src/setuplog/setup.py` & `setuplog-0.4.1/src/setuplog/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from setuplog.adaptors import StyleAdapter
 from setuplog.formatters import UnicodeEscapeFormatter
 
 _DEFAULT_FORMAT = "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
 _DEFAULT_DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 _DEFAULT_LOG_LEVEL_OVERRIDES = {"requests": "INFO"}
-_FILE_HANDLER_MAX_BYTES = 1048576
 
 
 def generate_loggers(*, log_level_overrides):
     loggers = {}
     for logger, new_level in log_level_overrides.items():
         loggers[logger] = {"level": new_level}
     return loggers
@@ -27,20 +26,20 @@
             "formatter": formatter,
             "stream": "ext://sys.stdout",
             "level": level,
         }
     }
     if log_file:
         handlers["file_handler"] = {
-            "class": "logging.handlers.RotatingFileHandler",
+            "class": "logging.FileHandler",
             "formatter": formatter,
             "filename": log_file,
-            "maxBytes": _FILE_HANDLER_MAX_BYTES,
             "level": level,
         }
+
     return handlers
 
 
 def generate_logging_config(
     level,
     formatter,
     format_=_DEFAULT_FORMAT,
```

### Comparing `setuplog-0.3.1/setup.py` & `setuplog-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 ['setuplog']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'setuplog',
-    'version': '0.3.1',
+    'version': '0.4.1',
     'description': '',
     'long_description': '![CircleCI](https://img.shields.io/circleci/build/gh/schireson/setuplog/master) [![codecov](https://codecov.io/gh/schireson/setuplog/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/setuplog) [![Documentation Status](https://readthedocs.org/projects/setuplog/badge/?version=latest)](https://setuplog.readthedocs.io/en/latest/?badge=latest)\n\n## The pitch\n\nLogging setup is one of those annoying things that one finds themselves relearning\nevery time a new project is started.\n\n`setuplog` attempts to centralize, and simplify the set of decisions one needs to make\nwhen bootstrapping a project.\n\n```python\n# app.py\nfrom setuplog import setup_logging\n\nsetup_logging(\n    log_level=\'INFO\',\n    namespace=\'project_name\',\n\n    # opt into {}-style formatting!\n    style=\'format\',\n)\n\n# elsewhere\nfrom setuplog import log\n\nlog.info(\'Info!\')\n```\n\n## Installing\n\n```bash\npip install "setuplog"\n```\n',
-    'author': None,
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
+    'author': 'None',
+    'author_email': 'None',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/schireson/setuplog',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.6.0,<4',
 }
```

### Comparing `setuplog-0.3.1/PKG-INFO` & `setuplog-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: setuplog
-Version: 0.3.1
+Version: 0.4.1
 Summary: 
 Home-page: https://github.com/schireson/setuplog
 License: MIT
 Keywords: logging,logger,log
 Requires-Python: >=3.6.0,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/schireson/setuplog
 Description-Content-Type: text/markdown
 
 ![CircleCI](https://img.shields.io/circleci/build/gh/schireson/setuplog/master) [![codecov](https://codecov.io/gh/schireson/setuplog/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/setuplog) [![Documentation Status](https://readthedocs.org/projects/setuplog/badge/?version=latest)](https://setuplog.readthedocs.io/en/latest/?badge=latest)
 
 ## The pitch
```

