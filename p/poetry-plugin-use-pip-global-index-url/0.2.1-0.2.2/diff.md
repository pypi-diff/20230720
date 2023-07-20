# Comparing `tmp/poetry_plugin_use_pip_global_index_url-0.2.1.tar.gz` & `tmp/poetry_plugin_use_pip_global_index_url-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_use_pip_global_index_url-0.2.1.tar", max compression
+gzip compressed data, was "poetry_plugin_use_pip_global_index_url-0.2.2.tar", max compression
```

## Comparing `poetry_plugin_use_pip_global_index_url-0.2.1.tar` & `poetry_plugin_use_pip_global_index_url-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1457 2023-03-14 14:47:14.379982 poetry_plugin_use_pip_global_index_url-0.2.1/LICENSE
--rw-r--r--   0        0        0     1068 2023-03-14 15:34:02.219248 poetry_plugin_use_pip_global_index_url-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 14:47:14.383983 poetry_plugin_use_pip_global_index_url-0.2.1/src/poetry_plugin_use_pip_global_index_url/__init__.py
--rw-r--r--   0        0        0     4912 2023-03-14 15:36:25.355684 poetry_plugin_use_pip_global_index_url-0.2.1/src/poetry_plugin_use_pip_global_index_url/plugins.py
--rw-r--r--   0        0        0       48 2023-03-14 14:47:14.383983 poetry_plugin_use_pip_global_index_url-0.2.1/src/poetry_plugin_use_pip_global_index_url/py.typed
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 poetry_plugin_use_pip_global_index_url-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1457 2023-03-14 14:47:14.379982 poetry_plugin_use_pip_global_index_url-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1068 2023-07-20 14:01:00.839682 poetry_plugin_use_pip_global_index_url-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 14:47:14.383983 poetry_plugin_use_pip_global_index_url-0.2.2/src/poetry_plugin_use_pip_global_index_url/__init__.py
+-rw-r--r--   0        0        0     4912 2023-03-14 15:36:25.355684 poetry_plugin_use_pip_global_index_url-0.2.2/src/poetry_plugin_use_pip_global_index_url/plugins.py
+-rw-r--r--   0        0        0       48 2023-03-14 14:47:14.383983 poetry_plugin_use_pip_global_index_url-0.2.2/src/poetry_plugin_use_pip_global_index_url/py.typed
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 poetry_plugin_use_pip_global_index_url-0.2.2/PKG-INFO
```

### Comparing `poetry_plugin_use_pip_global_index_url-0.2.1/LICENSE` & `poetry_plugin_use_pip_global_index_url-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_use_pip_global_index_url-0.2.1/pyproject.toml` & `poetry_plugin_use_pip_global_index_url-0.2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "poetry-plugin-use-pip-global-index-url"
-version = "0.2.1"
+version = "0.2.2"
 description = "Poetry plugin that sets the global index with the value obtained from pip."
 authors = ["Jacob Henner <code@ventricle.us>", "Hugh Baxter <hughdbaxter@gmail.com>"]
 license = "BSD-3-Clause"
 keywords = ["packaging", "poetry", "pypi", "pip"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-poetry = ">=1.3.0,<1.5"
+poetry = ">=1.3.0,<1.6"
 
 [tool.poetry.plugins."poetry.plugin"]
 demo = "poetry_plugin_use_pip_global_index_url.plugins:UsePipGlobalIndexUrlPlugin"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 mypy = "^0.982"
```

### Comparing `poetry_plugin_use_pip_global_index_url-0.2.1/src/poetry_plugin_use_pip_global_index_url/plugins.py` & `poetry_plugin_use_pip_global_index_url-0.2.2/src/poetry_plugin_use_pip_global_index_url/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_use_pip_global_index_url-0.2.1/PKG-INFO` & `poetry_plugin_use_pip_global_index_url-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-use-pip-global-index-url
-Version: 0.2.1
+Version: 0.2.2
 Summary: Poetry plugin that sets the global index with the value obtained from pip.
 License: BSD-3-Clause
 Keywords: packaging,poetry,pypi,pip
 Author: Jacob Henner
 Author-email: code@ventricle.us
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: poetry (>=1.3.0,<1.5)
+Requires-Dist: poetry (>=1.3.0,<1.6)
```

