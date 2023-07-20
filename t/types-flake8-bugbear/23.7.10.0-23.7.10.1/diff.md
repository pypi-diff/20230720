# Comparing `tmp/types-flake8-bugbear-23.7.10.0.tar.gz` & `tmp/types-flake8-bugbear-23.7.10.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-bugbear-23.7.10.0.tar", last modified: Tue Jul 11 09:16:17 2023, max compression
+gzip compressed data, was "types-flake8-bugbear-23.7.10.1.tar", last modified: Thu Jul 20 15:15:55 2023, max compression
```

## Comparing `types-flake8-bugbear-23.7.10.0.tar` & `types-flake8-bugbear-23.7.10.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/
--rw-r--r--   0 runner    (1001) docker     (123)     8461 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/bugbear-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/bugbear-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/bugbear-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-11 09:16:14.000000 types-flake8-bugbear-23.7.10.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:17.405564 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 09:16:17.000000 types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.584893 types-flake8-bugbear-23.7.10.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-07-20 15:15:54.000000 types-flake8-bugbear-23.7.10.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:54.000000 types-flake8-bugbear-23.7.10.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-20 15:15:55.584893 types-flake8-bugbear-23.7.10.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.580892 types-flake8-bugbear-23.7.10.1/bugbear-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 15:15:54.000000 types-flake8-bugbear-23.7.10.1/bugbear-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-20 15:15:54.000000 types-flake8-bugbear-23.7.10.1/bugbear-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:55.584893 types-flake8-bugbear-23.7.10.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-20 15:15:54.000000 types-flake8-bugbear-23.7.10.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:55.584893 types-flake8-bugbear-23.7.10.1/types_flake8_bugbear.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-20 15:15:55.000000 types-flake8-bugbear-23.7.10.1/types_flake8_bugbear.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-20 15:15:55.000000 types-flake8-bugbear-23.7.10.1/types_flake8_bugbear.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:55.000000 types-flake8-bugbear-23.7.10.1/types_flake8_bugbear.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:15:55.000000 types-flake8-bugbear-23.7.10.1/types_flake8_bugbear.egg-info/top_level.txt
```

### Comparing `types-flake8-bugbear-23.7.10.0/CHANGELOG.md` & `types-flake8-bugbear-23.7.10.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 23.7.10.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 23.7.10.0 (2023-07-11)
 
 [stubsabot] Bump flake8-bugbear to 23.7.10 (#10434)
 
 Release: https://pypi.org/pypi/flake8-bugbear/23.7.10
 Homepage: https://github.com/PyCQA/flake8-bugbear
 Changelog: https://github.com/PyCQA/flake8-bugbear#change-log
```

### Comparing `types-flake8-bugbear-23.7.10.0/PKG-INFO` & `types-flake8-bugbear-23.7.10.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.7.10.0
+Version: 23.7.10.1
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-flake8-bugbear-23.7.10.0/bugbear-stubs/__init__.pyi` & `types-flake8-bugbear-23.7.10.1/bugbear-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-bugbear-23.7.10.0/setup.py` & `types-flake8-bugbear-23.7.10.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="23.7.10.0",
+      version="23.7.10.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md",
```

### Comparing `types-flake8-bugbear-23.7.10.0/types_flake8_bugbear.egg-info/PKG-INFO` & `types-flake8-bugbear-23.7.10.1/types_flake8_bugbear.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-bugbear
-Version: 23.7.10.0
+Version: 23.7.10.1
 Summary: Typing stubs for flake8-bugbear
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-bugbear.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
-with mypy 1.4.1, pyright 1.1.316, and
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

