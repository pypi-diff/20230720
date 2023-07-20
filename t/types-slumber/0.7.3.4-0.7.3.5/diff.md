# Comparing `tmp/types-slumber-0.7.3.4.tar.gz` & `tmp/types-slumber-0.7.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-slumber-0.7.3.4.tar", last modified: Tue Mar 28 12:33:36 2023, max compression
+gzip compressed data, was "types-slumber-0.7.3.5.tar", last modified: Thu Jul 20 15:21:55 2023, max compression
```

## Comparing `types-slumber-0.7.3.4.tar` & `types-slumber-0.7.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:36.196810 types-slumber-0.7.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-28 12:33:35.000000 types-slumber-0.7.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:35.000000 types-slumber-0.7.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-28 12:33:36.196810 types-slumber-0.7.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:36.196810 types-slumber-0.7.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-03-28 12:33:35.000000 types-slumber-0.7.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:36.196810 types-slumber-0.7.3.4/slumber-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-28 12:33:35.000000 types-slumber-0.7.3.4/slumber-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-03-28 12:32:25.000000 types-slumber-0.7.3.4/slumber-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-28 12:32:25.000000 types-slumber-0.7.3.4/slumber-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-03-28 12:32:25.000000 types-slumber-0.7.3.4/slumber-stubs/serialize.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-28 12:32:25.000000 types-slumber-0.7.3.4/slumber-stubs/utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:36.196810 types-slumber-0.7.3.4/types_slumber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-03-28 12:33:36.000000 types-slumber-0.7.3.4/types_slumber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-28 12:33:36.000000 types-slumber-0.7.3.4/types_slumber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:36.000000 types-slumber-0.7.3.4/types_slumber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 12:33:36.000000 types-slumber-0.7.3.4/types_slumber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-28 12:33:36.000000 types-slumber-0.7.3.4/types_slumber.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:55.493314 types-slumber-0.7.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-20 15:21:54.000000 types-slumber-0.7.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:54.000000 types-slumber-0.7.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 15:21:55.493314 types-slumber-0.7.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:55.493314 types-slumber-0.7.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-07-20 15:21:54.000000 types-slumber-0.7.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:55.493314 types-slumber-0.7.3.5/slumber-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-20 15:21:54.000000 types-slumber-0.7.3.5/slumber-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-20 15:15:13.000000 types-slumber-0.7.3.5/slumber-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-20 15:15:13.000000 types-slumber-0.7.3.5/slumber-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-20 15:15:13.000000 types-slumber-0.7.3.5/slumber-stubs/serialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 15:15:13.000000 types-slumber-0.7.3.5/slumber-stubs/utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:55.493314 types-slumber-0.7.3.5/types_slumber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 15:21:55.000000 types-slumber-0.7.3.5/types_slumber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-20 15:21:55.000000 types-slumber-0.7.3.5/types_slumber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:55.000000 types-slumber-0.7.3.5/types_slumber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:21:55.000000 types-slumber-0.7.3.5/types_slumber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:21:55.000000 types-slumber-0.7.3.5/types_slumber.egg-info/top_level.txt
```

### Comparing `types-slumber-0.7.3.4/CHANGELOG.md` & `types-slumber-0.7.3.5/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.7.3.5 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.7.3.4 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 0.7.3.3 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-slumber-0.7.3.4/PKG-INFO` & `types-slumber-0.7.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-slumber
-Version: 0.7.3.4
+Version: 0.7.3.5
 Summary: Typing stubs for slumber
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/slumber.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `slumber`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/slumber. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-slumber-0.7.3.4/setup.py` & `types-slumber-0.7.3.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `slumber`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/slumber. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.7.3.4",
+      version="0.7.3.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/slumber.md",
```

### Comparing `types-slumber-0.7.3.4/slumber-stubs/__init__.pyi` & `types-slumber-0.7.3.5/slumber-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-slumber-0.7.3.4/slumber-stubs/serialize.pyi` & `types-slumber-0.7.3.5/slumber-stubs/serialize.pyi`

 * *Files identical despite different names*

### Comparing `types-slumber-0.7.3.4/types_slumber.egg-info/PKG-INFO` & `types-slumber-0.7.3.5/types_slumber.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-slumber
-Version: 0.7.3.4
+Version: 0.7.3.5
 Summary: Typing stubs for slumber
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/slumber.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `slumber`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/slumber. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

