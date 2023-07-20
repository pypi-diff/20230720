# Comparing `tmp/types-Flask-Migrate-4.0.0.5.tar.gz` & `tmp/types-Flask-Migrate-4.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Flask-Migrate-4.0.0.5.tar", last modified: Sat Jul  8 12:30:40 2023, max compression
+gzip compressed data, was "types-Flask-Migrate-4.0.0.6.tar", last modified: Thu Jul 20 15:21:17 2023, max compression
```

## Comparing `types-Flask-Migrate-4.0.0.5.tar` & `types-Flask-Migrate-4.0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:30:40.709183 types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-08 12:30:21.000000 types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-08 12:30:37.000000 types-Flask-Migrate-4.0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 12:30:40.713183 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 12:30:40.000000 types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:17.048864 types-Flask-Migrate-4.0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 15:21:16.000000 types-Flask-Migrate-4.0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:16.000000 types-Flask-Migrate-4.0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-20 15:21:17.044864 types-Flask-Migrate-4.0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:17.044864 types-Flask-Migrate-4.0.0.6/flask_migrate-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 15:21:16.000000 types-Flask-Migrate-4.0.0.6/flask_migrate-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-20 15:15:13.000000 types-Flask-Migrate-4.0.0.6/flask_migrate-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:17.048864 types-Flask-Migrate-4.0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-20 15:21:16.000000 types-Flask-Migrate-4.0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:17.044864 types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-20 15:21:17.000000 types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 15:21:17.000000 types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:17.000000 types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 15:21:17.000000 types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:21:17.000000 types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/top_level.txt
```

### Comparing `types-Flask-Migrate-4.0.0.5/CHANGELOG.md` & `types-Flask-Migrate-4.0.0.6/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.0.0.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 4.0.0.5 (2023-07-08)
 
 Remove `SQLAlchemy` stubs (#10389)
 
 Co-authored-by: AlexWaygood <alex.waygood@gmail.com>
 
 ## 4.0.0.4 (2023-05-10)
```

### Comparing `types-Flask-Migrate-4.0.0.5/PKG-INFO` & `types-Flask-Migrate-4.0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Migrate
-Version: 4.0.0.5
+Version: 4.0.0.6
 Summary: Typing stubs for Flask-Migrate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `aed8c3fe1c7e8a4e720cd2cebb610d7ce186dc1b` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-Flask-Migrate-4.0.0.5/flask_migrate-stubs/__init__.pyi` & `types-Flask-Migrate-4.0.0.6/flask_migrate-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-Flask-Migrate-4.0.0.5/setup.py` & `types-Flask-Migrate-4.0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `aed8c3fe1c7e8a4e720cd2cebb610d7ce186dc1b` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.0.0.5",
+      version="4.0.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md",
```

### Comparing `types-Flask-Migrate-4.0.0.5/types_Flask_Migrate.egg-info/PKG-INFO` & `types-Flask-Migrate-4.0.0.6/types_Flask_Migrate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-Flask-Migrate
-Version: 4.0.0.5
+Version: 4.0.0.6
 Summary: Typing stubs for Flask-Migrate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Flask-Migrate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `aed8c3fe1c7e8a4e720cd2cebb610d7ce186dc1b` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

