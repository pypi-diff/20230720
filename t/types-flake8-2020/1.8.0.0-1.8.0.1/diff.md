# Comparing `tmp/types-flake8-2020-1.8.0.0.tar.gz` & `tmp/types-flake8-2020-1.8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-2020-1.8.0.0.tar", last modified: Sun May  7 09:13:48 2023, max compression
+gzip compressed data, was "types-flake8-2020-1.8.0.1.tar", last modified: Thu Jul 20 15:15:34 2023, max compression
```

## Comparing `types-flake8-2020-1.8.0.0.tar` & `types-flake8-2020-1.8.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/flake8_2020-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/flake8_2020-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/flake8_2020-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-07 09:13:46.000000 types-flake8-2020-1.8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:13:48.901269 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 09:13:48.000000 types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:34.484633 types-flake8-2020-1.8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-20 15:15:31.000000 types-flake8-2020-1.8.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:31.000000 types-flake8-2020-1.8.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:15:34.484633 types-flake8-2020-1.8.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:34.484633 types-flake8-2020-1.8.0.1/flake8_2020-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 15:15:31.000000 types-flake8-2020-1.8.0.1/flake8_2020-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-20 15:15:31.000000 types-flake8-2020-1.8.0.1/flake8_2020-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:34.484633 types-flake8-2020-1.8.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-20 15:15:31.000000 types-flake8-2020-1.8.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:34.484633 types-flake8-2020-1.8.0.1/types_flake8_2020.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:15:34.000000 types-flake8-2020-1.8.0.1/types_flake8_2020.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 15:15:34.000000 types-flake8-2020-1.8.0.1/types_flake8_2020.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:34.000000 types-flake8-2020-1.8.0.1/types_flake8_2020.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:15:34.000000 types-flake8-2020-1.8.0.1/types_flake8_2020.egg-info/top_level.txt
```

### Comparing `types-flake8-2020-1.8.0.0/CHANGELOG.md` & `types-flake8-2020-1.8.0.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.8.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.8.0.0 (2023-05-07)
 
 [stubsabot] Bump flake8-2020 to 1.8.* (#10153)
 
 Release: https://pypi.org/pypi/flake8-2020/1.8.0
 Homepage: https://github.com/asottile/flake8-2020
 Diff: https://github.com/asottile/flake8-2020/compare/v1.7.0...v1.8.0
```

### Comparing `types-flake8-2020-1.8.0.0/PKG-INFO` & `types-flake8-2020-1.8.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-2020
-Version: 1.8.0.0
+Version: 1.8.0.1
 Summary: Typing stubs for flake8-2020
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-2020.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-2020`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-2020. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `38a11b2f06f455bad02ea91a76cb40cf521105d9`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-flake8-2020-1.8.0.0/flake8_2020-stubs/__init__.pyi` & `types-flake8-2020-1.8.0.1/flake8_2020-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-2020-1.8.0.0/setup.py` & `types-flake8-2020-1.8.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-2020`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-2020. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `38a11b2f06f455bad02ea91a76cb40cf521105d9`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.8.0.0",
+      version="1.8.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-2020.md",
```

### Comparing `types-flake8-2020-1.8.0.0/types_flake8_2020.egg-info/PKG-INFO` & `types-flake8-2020-1.8.0.1/types_flake8_2020.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-2020
-Version: 1.8.0.0
+Version: 1.8.0.1
 Summary: Typing stubs for flake8-2020
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-2020.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-2020`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-2020. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `38a11b2f06f455bad02ea91a76cb40cf521105d9`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

