# Comparing `tmp/types-peewee-3.16.0.0.tar.gz` & `tmp/types-peewee-3.16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-peewee-3.16.0.0.tar", last modified: Tue Feb 28 01:23:49 2023, max compression
+gzip compressed data, was "types-peewee-3.16.0.1.tar", last modified: Thu Jul 20 15:18:58 2023, max compression
```

## Comparing `types-peewee-3.16.0.0.tar` & `types-peewee-3.16.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 01:23:49.533343 types-peewee-3.16.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-02-28 01:23:48.000000 types-peewee-3.16.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 01:23:48.000000 types-peewee-3.16.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-28 01:23:49.533343 types-peewee-3.16.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 01:23:49.533343 types-peewee-3.16.0.0/peewee-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-28 01:23:48.000000 types-peewee-3.16.0.0/peewee-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)    61414 2023-02-28 01:23:48.000000 types-peewee-3.16.0.0/peewee-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 01:23:49.533343 types-peewee-3.16.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-02-28 01:23:48.000000 types-peewee-3.16.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 01:23:49.533343 types-peewee-3.16.0.0/types_peewee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-02-28 01:23:49.000000 types-peewee-3.16.0.0/types_peewee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-28 01:23:49.000000 types-peewee-3.16.0.0/types_peewee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 01:23:49.000000 types-peewee-3.16.0.0/types_peewee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-28 01:23:49.000000 types-peewee-3.16.0.0/types_peewee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:58.119151 types-peewee-3.16.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-20 15:18:57.000000 types-peewee-3.16.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:57.000000 types-peewee-3.16.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-20 15:18:58.119151 types-peewee-3.16.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:58.119151 types-peewee-3.16.0.1/peewee-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 15:18:57.000000 types-peewee-3.16.0.1/peewee-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    61414 2023-07-20 15:18:57.000000 types-peewee-3.16.0.1/peewee-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:58.119151 types-peewee-3.16.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-20 15:18:57.000000 types-peewee-3.16.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:58.119151 types-peewee-3.16.0.1/types_peewee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-20 15:18:58.000000 types-peewee-3.16.0.1/types_peewee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-20 15:18:58.000000 types-peewee-3.16.0.1/types_peewee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:58.000000 types-peewee-3.16.0.1/types_peewee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:18:58.000000 types-peewee-3.16.0.1/types_peewee.egg-info/top_level.txt
```

### Comparing `types-peewee-3.16.0.0/CHANGELOG.md` & `types-peewee-3.16.0.1/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.16.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.16.0.0 (2023-02-28)
 
 Update peewee stubs to v3.16 (#9827)
 
 Bump peewee to 3.16.*
 
 Release: https://pypi.org/pypi/peewee/3.16.0
```

### Comparing `types-peewee-3.16.0.0/PKG-INFO` & `types-peewee-3.16.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-peewee
-Version: 3.16.0.0
+Version: 3.16.0.1
 Summary: Typing stubs for peewee
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `peewee`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `05b294e911b30d503d29982ac53649e012ba8424`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-peewee-3.16.0.0/peewee-stubs/__init__.pyi` & `types-peewee-3.16.0.1/peewee-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-peewee-3.16.0.0/setup.py` & `types-peewee-3.16.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `peewee`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `05b294e911b30d503d29982ac53649e012ba8424`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.16.0.0",
+      version="3.16.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md",
```

### Comparing `types-peewee-3.16.0.0/types_peewee.egg-info/PKG-INFO` & `types-peewee-3.16.0.1/types_peewee.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-peewee
-Version: 3.16.0.0
+Version: 3.16.0.1
 Summary: Typing stubs for peewee
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/peewee.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `peewee`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/peewee. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `05b294e911b30d503d29982ac53649e012ba8424`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

