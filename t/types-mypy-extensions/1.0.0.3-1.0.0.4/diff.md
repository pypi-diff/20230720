# Comparing `tmp/types-mypy-extensions-1.0.0.3.tar.gz` & `tmp/types-mypy-extensions-1.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-mypy-extensions-1.0.0.3.tar", last modified: Wed Feb 22 09:17:44 2023, max compression
+gzip compressed data, was "types-mypy-extensions-1.0.0.4.tar", last modified: Thu Jul 20 15:17:51 2023, max compression
```

## Comparing `types-mypy-extensions-1.0.0.3.tar` & `types-mypy-extensions-1.0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:44.334215 types-mypy-extensions-1.0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-02-22 09:17:43.000000 types-mypy-extensions-1.0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-22 09:17:43.000000 types-mypy-extensions-1.0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-22 09:17:44.330215 types-mypy-extensions-1.0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:44.330215 types-mypy-extensions-1.0.0.3/mypy_extensions-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-22 09:17:43.000000 types-mypy-extensions-1.0.0.3/mypy_extensions-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-02-22 09:17:43.000000 types-mypy-extensions-1.0.0.3/mypy_extensions-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-22 09:17:44.334215 types-mypy-extensions-1.0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-02-22 09:17:43.000000 types-mypy-extensions-1.0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-22 09:17:44.330215 types-mypy-extensions-1.0.0.3/types_mypy_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-22 09:17:44.000000 types-mypy-extensions-1.0.0.3/types_mypy_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-22 09:17:44.000000 types-mypy-extensions-1.0.0.3/types_mypy_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-22 09:17:44.000000 types-mypy-extensions-1.0.0.3/types_mypy_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-22 09:17:44.000000 types-mypy-extensions-1.0.0.3/types_mypy_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:51.458297 types-mypy-extensions-1.0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-07-20 15:17:50.000000 types-mypy-extensions-1.0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:50.000000 types-mypy-extensions-1.0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-20 15:17:51.458297 types-mypy-extensions-1.0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:51.454297 types-mypy-extensions-1.0.0.4/mypy_extensions-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 15:17:50.000000 types-mypy-extensions-1.0.0.4/mypy_extensions-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-07-20 15:17:50.000000 types-mypy-extensions-1.0.0.4/mypy_extensions-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:51.458297 types-mypy-extensions-1.0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-20 15:17:50.000000 types-mypy-extensions-1.0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:51.458297 types-mypy-extensions-1.0.0.4/types_mypy_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-07-20 15:17:51.000000 types-mypy-extensions-1.0.0.4/types_mypy_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-20 15:17:51.000000 types-mypy-extensions-1.0.0.4/types_mypy_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:51.000000 types-mypy-extensions-1.0.0.4/types_mypy_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:17:51.000000 types-mypy-extensions-1.0.0.4/types_mypy_extensions.egg-info/top_level.txt
```

### Comparing `types-mypy-extensions-1.0.0.3/CHANGELOG.md` & `types-mypy-extensions-1.0.0.4/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.0.0.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.0.0.3 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
 
 * Update _Unused TypeAlias
 
 * Update `object | None` params
```

### Comparing `types-mypy-extensions-1.0.0.3/PKG-INFO` & `types-mypy-extensions-1.0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mypy-extensions
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: Typing stubs for mypy-extensions
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mypy-extensions.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mypy-extensions`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mypy-extensions. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-mypy-extensions-1.0.0.3/mypy_extensions-stubs/__init__.pyi` & `types-mypy-extensions-1.0.0.4/mypy_extensions-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-mypy-extensions-1.0.0.3/setup.py` & `types-mypy-extensions-1.0.0.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mypy-extensions`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mypy-extensions. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.0.0.3",
+      version="1.0.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mypy-extensions.md",
```

### Comparing `types-mypy-extensions-1.0.0.3/types_mypy_extensions.egg-info/PKG-INFO` & `types-mypy-extensions-1.0.0.4/types_mypy_extensions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mypy-extensions
-Version: 1.0.0.3
+Version: 1.0.0.4
 Summary: Typing stubs for mypy-extensions
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mypy-extensions.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mypy-extensions`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mypy-extensions. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `078c6a095892e12c94462889fa43c2c2dc8280ad`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

