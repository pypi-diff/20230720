# Comparing `tmp/types-toposort-1.9.0.0.tar.gz` & `tmp/types-toposort-1.9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-toposort-1.9.0.0.tar", last modified: Thu Jan 12 01:21:52 2023, max compression
+gzip compressed data, was "types-toposort-1.9.0.1.tar", last modified: Tue Feb 21 01:27:58 2023, max compression
```

## Comparing `types-toposort-1.9.0.0.tar` & `types-toposort-1.9.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:21:52.210402 types-toposort-1.9.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-01-12 01:21:51.000000 types-toposort-1.9.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-12 01:21:51.000000 types-toposort-1.9.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-12 01:21:52.210402 types-toposort-1.9.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 01:21:52.210402 types-toposort-1.9.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-01-12 01:21:51.000000 types-toposort-1.9.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:21:52.210402 types-toposort-1.9.0.0/toposort-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-12 01:21:51.000000 types-toposort-1.9.0.0/toposort-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-12 01:21:51.000000 types-toposort-1.9.0.0/toposort-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 01:21:52.210402 types-toposort-1.9.0.0/types_toposort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-01-12 01:21:52.000000 types-toposort-1.9.0.0/types_toposort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-12 01:21:52.000000 types-toposort-1.9.0.0/types_toposort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 01:21:52.000000 types-toposort-1.9.0.0/types_toposort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-12 01:21:52.000000 types-toposort-1.9.0.0/types_toposort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:27:58.381809 types-toposort-1.9.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-21 01:27:57.000000 types-toposort-1.9.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:27:57.000000 types-toposort-1.9.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-21 01:27:58.381809 types-toposort-1.9.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:27:58.381809 types-toposort-1.9.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-21 01:27:57.000000 types-toposort-1.9.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:27:58.381809 types-toposort-1.9.0.1/toposort-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-21 01:27:57.000000 types-toposort-1.9.0.1/toposort-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-02-21 01:27:57.000000 types-toposort-1.9.0.1/toposort-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:27:58.381809 types-toposort-1.9.0.1/types_toposort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-02-21 01:27:58.000000 types-toposort-1.9.0.1/types_toposort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-21 01:27:58.000000 types-toposort-1.9.0.1/types_toposort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:27:58.000000 types-toposort-1.9.0.1/types_toposort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-21 01:27:58.000000 types-toposort-1.9.0.1/types_toposort.egg-info/top_level.txt
```

### Comparing `types-toposort-1.9.0.0/PKG-INFO` & `types-toposort-1.9.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-toposort
-Version: 1.9.0.0
+Version: 1.9.0.1
 Summary: Typing stubs for toposort
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/toposort.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `toposort`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/toposort. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `150dc35d43383dc4ce6814aae7f927437366bd3e`.
+This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
```

### Comparing `types-toposort-1.9.0.0/setup.py` & `types-toposort-1.9.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `toposort`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/toposort. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `150dc35d43383dc4ce6814aae7f927437366bd3e`.
+This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
 '''.lstrip()
 
 setup(name=name,
-      version="1.9.0.0",
+      version="1.9.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/toposort.md",
```

### Comparing `types-toposort-1.9.0.0/toposort-stubs/__init__.pyi` & `types-toposort-1.9.0.1/toposort-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-toposort-1.9.0.0/types_toposort.egg-info/PKG-INFO` & `types-toposort-1.9.0.1/types_toposort.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-toposort
-Version: 1.9.0.0
+Version: 1.9.0.1
 Summary: Typing stubs for toposort
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/toposort.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `toposort`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/toposort. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `150dc35d43383dc4ce6814aae7f927437366bd3e`.
+This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
```

