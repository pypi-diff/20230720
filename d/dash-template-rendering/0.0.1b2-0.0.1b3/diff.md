# Comparing `tmp/dash-template-rendering-0.0.1b2.tar.gz` & `tmp/dash-template-rendering-0.0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-template-rendering-0.0.1b2.tar", last modified: Thu Jul 20 10:18:29 2023, max compression
+gzip compressed data, was "dash-template-rendering-0.0.1b3.tar", last modified: Thu Jul 20 11:03:33 2023, max compression
```

## Comparing `dash-template-rendering-0.0.1b2.tar` & `dash-template-rendering-0.0.1b3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:18:29.727513 dash-template-rendering-0.0.1b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 10:18:29.727513 dash-template-rendering-0.0.1b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:18:29.727513 dash-template-rendering-0.0.1b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:18:29.723513 dash-template-rendering-0.0.1b2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:18:29.727513 dash-template-rendering-0.0.1b2/src/dash_template_rendering/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering/template_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering/templating.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:18:29.727513 dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 10:18:29.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 10:18:29.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:18:29.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 10:18:29.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 10:18:29.000000 dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:18:29.727513 dash-template-rendering-0.0.1b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 10:18:01.000000 dash-template-rendering-0.0.1b2/tests/test_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/src/dash_template_rendering/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering/template_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering/templating.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 11:03:33.000000 dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:03:33.215791 dash-template-rendering-0.0.1b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-20 11:03:16.000000 dash-template-rendering-0.0.1b3/tests/test_template.py
```

### Comparing `dash-template-rendering-0.0.1b2/LICENSE` & `dash-template-rendering-0.0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b2/PKG-INFO` & `dash-template-rendering-0.0.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-template-rendering
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Dash Python extention for rendering Jinja2 templates.
 Author-email: Patrick Schleiter <git.pschleiter@gmail.com>
 Project-URL: Source Code, https://github.com/pschleiter/dash-template-rendering
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dash-template-rendering-0.0.1b2/README.md` & `dash-template-rendering-0.0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b2/pyproject.toml` & `dash-template-rendering-0.0.1b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b2/src/dash_template_rendering/template_renderer.py` & `dash-template-rendering-0.0.1b3/src/dash_template_rendering/template_renderer.py`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b2/src/dash_template_rendering/templating.py` & `dash-template-rendering-0.0.1b3/src/dash_template_rendering/templating.py`

 * *Files identical despite different names*

### Comparing `dash-template-rendering-0.0.1b2/src/dash_template_rendering.egg-info/PKG-INFO` & `dash-template-rendering-0.0.1b3/src/dash_template_rendering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-template-rendering
-Version: 0.0.1b2
+Version: 0.0.1b3
 Summary: Dash Python extention for rendering Jinja2 templates.
 Author-email: Patrick Schleiter <git.pschleiter@gmail.com>
 Project-URL: Source Code, https://github.com/pschleiter/dash-template-rendering
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dash-template-rendering-0.0.1b2/tests/test_template.py` & `dash-template-rendering-0.0.1b3/tests/test_template.py`

 * *Files identical despite different names*

