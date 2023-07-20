# Comparing `tmp/orbit_component_dbshell-1.0.5.tar.gz` & `tmp/orbit_component_dbshell-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_dbshell-1.0.5.tar", max compression
+gzip compressed data, was "orbit_component_dbshell-1.0.6.tar", max compression
```

## Comparing `orbit_component_dbshell-1.0.5.tar` & `orbit_component_dbshell-1.0.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-17 16:50:03.098236 orbit_component_dbshell-1.0.5/LICENSE.md
--rw-r--r--   0        0        0        0 2023-06-21 15:30:58.376561 orbit_component_dbshell-1.0.5/README.md
--rw-r--r--   0        0        0       82 2023-06-21 12:41:11.901965 orbit_component_dbshell-1.0.5/orbit_component_dbshell/__init__.py
--rw-r--r--   0        0        0      515 2023-07-06 17:21:12.797206 orbit_component_dbshell-1.0.5/orbit_component_dbshell/plugin.py
--rw-r--r--   0        0        0     1254 2023-07-07 16:32:02.621578 orbit_component_dbshell-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 orbit_component_dbshell-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-17 16:50:03.098236 orbit_component_dbshell-1.0.6/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-06-21 15:30:58.376561 orbit_component_dbshell-1.0.6/README.md
+-rw-r--r--   0        0        0       82 2023-06-21 12:41:11.901965 orbit_component_dbshell-1.0.6/orbit_component_dbshell/__init__.py
+-rw-r--r--   0        0        0      515 2023-07-06 17:21:12.797206 orbit_component_dbshell-1.0.6/orbit_component_dbshell/plugin.py
+-rw-r--r--   0        0        0     1254 2023-07-20 17:09:51.986572 orbit_component_dbshell-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 orbit_component_dbshell-1.0.6/PKG-INFO
```

### Comparing `orbit_component_dbshell-1.0.5/orbit_component_dbshell/plugin.py` & `orbit_component_dbshell-1.0.6/orbit_component_dbshell/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_dbshell-1.0.5/pyproject.toml` & `orbit_component_dbshell-1.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orbit-component-dbshell"
-version = "1.0.5"
+version = "1.0.6"
 description = "Orbit Database shell component"
 authors = ["Gareth Bult <gareth@madpenguin.uk>"]
 license = "MIT"
 readme = "README.md"
 include = ['README.md', 'LICENSE.md']
 packages = [{include = "orbit_component_dbshell"}]
 classifiers = [
```

### Comparing `orbit_component_dbshell-1.0.5/PKG-INFO` & `orbit_component_dbshell-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orbit-component-dbshell
-Version: 1.0.5
+Version: 1.0.6
 Summary: Orbit Database shell component
 Home-page: https://gitlab.com/madpenguin/orbit-component-dbshell
 License: MIT
 Author: Gareth Bult
 Author-email: gareth@madpenguin.uk
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 4 - Beta
```

