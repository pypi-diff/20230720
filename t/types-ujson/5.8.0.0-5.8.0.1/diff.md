# Comparing `tmp/types-ujson-5.8.0.0.tar.gz` & `tmp/types-ujson-5.8.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ujson-5.8.0.0.tar", last modified: Mon Jun 12 01:37:12 2023, max compression
+gzip compressed data, was "types-ujson-5.8.0.1.tar", last modified: Thu Jul 20 15:19:23 2023, max compression
```

## Comparing `types-ujson-5.8.0.0.tar` & `types-ujson-5.8.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/types_ujson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-12 01:37:12.000000 types-ujson-5.8.0.0/types_ujson.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 01:37:12.409065 types-ujson-5.8.0.0/ujson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/ujson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-12 01:37:09.000000 types-ujson-5.8.0.0/ujson-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:23.959476 types-ujson-5.8.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:19:23.955476 types-ujson-5.8.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:23.959476 types-ujson-5.8.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:23.955476 types-ujson-5.8.0.1/types_ujson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/types_ujson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:23.955476 types-ujson-5.8.0.1/ujson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/ujson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 15:19:23.000000 types-ujson-5.8.0.1/ujson-stubs/__init__.pyi
```

### Comparing `types-ujson-5.8.0.0/CHANGELOG.md` & `types-ujson-5.8.0.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 5.8.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 5.8.0.0 (2023-06-12)
 
 [stubsabot] Bump ujson to 5.8.* (#10302)
 
 Release: https://pypi.org/pypi/ujson/5.8.0
 Homepage: https://github.com/ultrajson/ultrajson
 Diff: https://github.com/ultrajson/ultrajson/compare/5.7.0...5.8.0
```

### Comparing `types-ujson-5.8.0.0/PKG-INFO` & `types-ujson-5.8.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.8.0.0
+Version: 5.8.0.1
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6a94c9d677db9e9f85d764cc46294fd5c5e2a4b8`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-ujson-5.8.0.0/setup.py` & `types-ujson-5.8.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6a94c9d677db9e9f85d764cc46294fd5c5e2a4b8`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="5.8.0.0",
+      version="5.8.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md",
```

### Comparing `types-ujson-5.8.0.0/types_ujson.egg-info/PKG-INFO` & `types-ujson-5.8.0.1/types_ujson.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ujson
-Version: 5.8.0.0
+Version: 5.8.0.1
 Summary: Typing stubs for ujson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ujson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ujson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ujson. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6a94c9d677db9e9f85d764cc46294fd5c5e2a4b8`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-ujson-5.8.0.0/ujson-stubs/__init__.pyi` & `types-ujson-5.8.0.1/ujson-stubs/__init__.pyi`

 * *Files identical despite different names*

