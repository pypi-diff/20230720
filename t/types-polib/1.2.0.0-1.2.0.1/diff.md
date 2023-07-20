# Comparing `tmp/types-polib-1.2.0.0.tar.gz` & `tmp/types-polib-1.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-polib-1.2.0.0.tar", last modified: Fri Feb 24 01:23:19 2023, max compression
+gzip compressed data, was "types-polib-1.2.0.1.tar", last modified: Thu Jul 20 15:20:15 2023, max compression
```

## Comparing `types-polib-1.2.0.0.tar` & `types-polib-1.2.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:19.899357 types-polib-1.2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-24 01:23:18.000000 types-polib-1.2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-24 01:23:18.000000 types-polib-1.2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-24 01:23:19.895357 types-polib-1.2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:19.895357 types-polib-1.2.0.0/polib-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-24 01:23:18.000000 types-polib-1.2.0.0/polib-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-02-24 01:23:18.000000 types-polib-1.2.0.0/polib-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 01:23:19.899357 types-polib-1.2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-24 01:23:18.000000 types-polib-1.2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 01:23:19.895357 types-polib-1.2.0.0/types_polib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-02-24 01:23:19.000000 types-polib-1.2.0.0/types_polib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-24 01:23:19.000000 types-polib-1.2.0.0/types_polib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 01:23:19.000000 types-polib-1.2.0.0/types_polib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-24 01:23:19.000000 types-polib-1.2.0.0/types_polib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:15.616116 types-polib-1.2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 15:20:14.000000 types-polib-1.2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:14.000000 types-polib-1.2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:20:15.616116 types-polib-1.2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:15.616116 types-polib-1.2.0.1/polib-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 15:20:14.000000 types-polib-1.2.0.1/polib-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-20 15:20:14.000000 types-polib-1.2.0.1/polib-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:15.616116 types-polib-1.2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-20 15:20:14.000000 types-polib-1.2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:15.616116 types-polib-1.2.0.1/types_polib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:20:15.000000 types-polib-1.2.0.1/types_polib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 15:20:15.000000 types-polib-1.2.0.1/types_polib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:15.000000 types-polib-1.2.0.1/types_polib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 15:20:15.000000 types-polib-1.2.0.1/types_polib.egg-info/top_level.txt
```

### Comparing `types-polib-1.2.0.0/CHANGELOG.md` & `types-polib-1.2.0.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.2.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.2.0.0 (2023-02-24)
 
 [stubsabot] Bump polib to 1.2.* (#9804)
 
 Release: https://pypi.org/pypi/polib/1.2.0
 Homepage: https://github.com/izimobil/polib/
 Diff: https://github.com/izimobil/polib/compare/1.1.1...1.2.0
```

### Comparing `types-polib-1.2.0.0/PKG-INFO` & `types-polib-1.2.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-polib
-Version: 1.2.0.0
+Version: 1.2.0.1
 Summary: Typing stubs for polib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/polib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `polib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/polib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4ca5ee98df5654d0db7f5b24cd2bd3b3fe54f313`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-polib-1.2.0.0/polib-stubs/__init__.pyi` & `types-polib-1.2.0.1/polib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-polib-1.2.0.0/setup.py` & `types-polib-1.2.0.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `polib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/polib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4ca5ee98df5654d0db7f5b24cd2bd3b3fe54f313`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.2.0.0",
+      version="1.2.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/polib.md",
```

### Comparing `types-polib-1.2.0.0/types_polib.egg-info/PKG-INFO` & `types-polib-1.2.0.1/types_polib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-polib
-Version: 1.2.0.0
+Version: 1.2.0.1
 Summary: Typing stubs for polib
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/polib.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `polib`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/polib. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4ca5ee98df5654d0db7f5b24cd2bd3b3fe54f313`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

