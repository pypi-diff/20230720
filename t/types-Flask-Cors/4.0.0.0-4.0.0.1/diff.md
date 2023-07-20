# Comparing `tmp/types-Flask-Cors-4.0.0.0.tar.gz` & `tmp/types-Flask-Cors-4.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Cors-4.0.0.0.tar", last modified: Tue Jun 27 01:42:56 2023, max compression
+gzip compressed data, was "types-Flask-Cors-4.0.0.1.tar", last modified: Thu Jul 20 15:21:12 2023, max compression
```

## Comparing `types-Flask-Cors-4.0.0.0.tar` & `types-Flask-Cors-4.0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/flask_cors-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/extension.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 01:42:44.000000 types-Flask-Cors-4.0.0.0/flask_cors-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-27 01:42:55.000000 types-Flask-Cors-4.0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 01:42:56.813929 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-27 01:42:56.000000 types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:12.880816 types-Flask-Cors-4.0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 15:21:12.876816 types-Flask-Cors-4.0.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:12.876816 types-Flask-Cors-4.0.0.1/flask_cors-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/flask_cors-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 15:15:13.000000 types-Flask-Cors-4.0.0.1/flask_cors-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-07-20 15:15:13.000000 types-Flask-Cors-4.0.0.1/flask_cors-stubs/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-20 15:15:13.000000 types-Flask-Cors-4.0.0.1/flask_cors-stubs/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-20 15:15:13.000000 types-Flask-Cors-4.0.0.1/flask_cors-stubs/extension.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:13.000000 types-Flask-Cors-4.0.0.1/flask_cors-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:12.880816 types-Flask-Cors-4.0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:12.876816 types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:21:12.000000 types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/top_level.txt
```

### Comparing `types-Flask-Cors-4.0.0.0/CHANGELOG.md` & `types-Flask-Cors-4.0.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.0.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 4.0.0.0 (2023-06-27)
 
 [stubsabot] Bump Flask-Cors to 4.0.* (#10363)
 
 Release: https://pypi.org/pypi/Flask-Cors/4.0.0
 Homepage: https://github.com/corydolphin/flask-cors
 Diff: https://github.com/corydolphin/flask-cors/compare/3.0.10...v4.0.0
```

### Comparing `types-Flask-Cors-4.0.0.0/PKG-INFO` & `types-Flask-Cors-4.0.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 4.0.0.0
+Version: 4.0.0.1
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
-with mypy 1.4.1, pyright 1.1.315, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-Flask-Cors-4.0.0.0/flask_cors-stubs/core.pyi` & `types-Flask-Cors-4.0.0.1/flask_cors-stubs/core.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-4.0.0.0/flask_cors-stubs/decorator.pyi` & `types-Flask-Cors-4.0.0.1/flask_cors-stubs/decorator.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-4.0.0.0/flask_cors-stubs/extension.pyi` & `types-Flask-Cors-4.0.0.1/flask_cors-stubs/extension.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Cors-4.0.0.0/setup.py` & `types-Flask-Cors-4.0.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
-with mypy 1.4.1, pyright 1.1.315, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.0.0.0",
+      version="4.0.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md",
```

### Comparing `types-Flask-Cors-4.0.0.0/types_Flask_Cors.egg-info/PKG-INFO` & `types-Flask-Cors-4.0.0.1/types_Flask_Cors.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Cors
-Version: 4.0.0.0
+Version: 4.0.0.1
 Summary: Typing stubs for Flask-Cors
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Cors.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b8ab395d4bafd6352560e74b636744d49a9bcd6e` and was tested
-with mypy 1.4.1, pyright 1.1.315, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

