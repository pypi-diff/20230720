# Comparing `tmp/types-PyScreeze-0.1.0.8.tar.gz` & `tmp/types-PyScreeze-0.1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyScreeze-0.1.0.8.tar", last modified: Fri May 26 15:14:25 2023, max compression
+gzip compressed data, was "types-PyScreeze-0.1.0.9.tar", last modified: Thu Jul 20 15:20:54 2023, max compression
```

## Comparing `types-PyScreeze-0.1.0.8.tar` & `types-PyScreeze-0.1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/pyscreeze-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/pyscreeze-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-05-26 15:14:05.000000 types-PyScreeze-0.1.0.8/pyscreeze-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-05-26 15:14:23.000000 types-PyScreeze-0.1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:14:25.355084 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 15:14:25.000000 types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:54.124587 types-PyScreeze-0.1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 15:20:53.000000 types-PyScreeze-0.1.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:53.000000 types-PyScreeze-0.1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:20:54.124587 types-PyScreeze-0.1.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:54.120587 types-PyScreeze-0.1.0.9/pyscreeze-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-20 15:20:53.000000 types-PyScreeze-0.1.0.9/pyscreeze-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-20 15:15:13.000000 types-PyScreeze-0.1.0.9/pyscreeze-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:54.124587 types-PyScreeze-0.1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-07-20 15:20:53.000000 types-PyScreeze-0.1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:54.124587 types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:20:54.000000 types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 15:20:54.000000 types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:54.000000 types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:20:54.000000 types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 15:20:54.000000 types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/top_level.txt
```

### Comparing `types-PyScreeze-0.1.0.8/CHANGELOG.md` & `types-PyScreeze-0.1.0.9/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.1.0.9 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.1.0.8 (2023-05-26)
 
 Update pyscreeze stubs (#10223)
 
 ## 0.1.0.7 (2023-02-22)
 
 Update `Unused` parameters in `stubs/` (#9704)
```

### Comparing `types-PyScreeze-0.1.0.8/PKG-INFO` & `types-PyScreeze-0.1.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyScreeze
-Version: 0.1.0.8
+Version: 0.1.0.9
 Summary: Typing stubs for PyScreeze
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyScreeze`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2f65ca5cd4feaa1c69953ef7681416d8d435ffa7`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-PyScreeze-0.1.0.8/pyscreeze-stubs/__init__.pyi` & `types-PyScreeze-0.1.0.9/pyscreeze-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyScreeze-0.1.0.8/setup.py` & `types-PyScreeze-0.1.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyScreeze`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2f65ca5cd4feaa1c69953ef7681416d8d435ffa7`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.1.0.8",
+      version="0.1.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md",
```

### Comparing `types-PyScreeze-0.1.0.8/types_PyScreeze.egg-info/PKG-INFO` & `types-PyScreeze-0.1.0.9/types_PyScreeze.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyScreeze
-Version: 0.1.0.8
+Version: 0.1.0.9
 Summary: Typing stubs for PyScreeze
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyScreeze.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `PyScreeze`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/PyScreeze. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2f65ca5cd4feaa1c69953ef7681416d8d435ffa7`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

