# Comparing `tmp/types-tzlocal-5.0.1.0.tar.gz` & `tmp/types-tzlocal-5.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tzlocal-5.0.1.0.tar", last modified: Tue May 16 09:14:33 2023, max compression
+gzip compressed data, was "types-tzlocal-5.0.1.1.tar", last modified: Thu Jul 20 15:21:00 2023, max compression
```

## Comparing `types-tzlocal-5.0.1.0.tar` & `types-tzlocal-5.0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:33.713845 types-tzlocal-5.0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 09:14:33.713845 types-tzlocal-5.0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:14:33.713845 types-tzlocal-5.0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:33.713845 types-tzlocal-5.0.1.0/types_tzlocal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/types_tzlocal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/types_tzlocal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/types_tzlocal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/types_tzlocal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/types_tzlocal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:14:33.713845 types-tzlocal-5.0.1.0/tzlocal-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 09:14:33.000000 types-tzlocal-5.0.1.0/tzlocal-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-16 09:14:13.000000 types-tzlocal-5.0.1.0/tzlocal-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-16 09:14:13.000000 types-tzlocal-5.0.1.0/tzlocal-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-16 09:14:13.000000 types-tzlocal-5.0.1.0/tzlocal-stubs/windows_tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:00.452665 types-tzlocal-5.0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-20 15:20:59.000000 types-tzlocal-5.0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:59.000000 types-tzlocal-5.0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 15:21:00.452665 types-tzlocal-5.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:00.452665 types-tzlocal-5.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-20 15:20:59.000000 types-tzlocal-5.0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:00.452665 types-tzlocal-5.0.1.1/types_tzlocal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-20 15:21:00.000000 types-tzlocal-5.0.1.1/types_tzlocal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 15:21:00.000000 types-tzlocal-5.0.1.1/types_tzlocal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:00.000000 types-tzlocal-5.0.1.1/types_tzlocal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 15:21:00.000000 types-tzlocal-5.0.1.1/types_tzlocal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:21:00.000000 types-tzlocal-5.0.1.1/types_tzlocal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:00.452665 types-tzlocal-5.0.1.1/tzlocal-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 15:20:59.000000 types-tzlocal-5.0.1.1/tzlocal-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-20 15:15:13.000000 types-tzlocal-5.0.1.1/tzlocal-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 15:15:13.000000 types-tzlocal-5.0.1.1/tzlocal-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-20 15:15:13.000000 types-tzlocal-5.0.1.1/tzlocal-stubs/windows_tz.pyi
```

### Comparing `types-tzlocal-5.0.1.0/CHANGELOG.md` & `types-tzlocal-5.0.1.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 5.0.1.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 5.0.1.0 (2023-05-16)
 
 Bump `tzlocal` to `5.0.1` (#10188)
 
 ## 5.0.0.0 (2023-05-15)
 
 Bump `tzlocal` to `5.0` (#10183)
```

### Comparing `types-tzlocal-5.0.1.0/PKG-INFO` & `types-tzlocal-5.0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tzlocal
-Version: 5.0.1.0
+Version: 5.0.1.1
 Summary: Typing stubs for tzlocal
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tzlocal.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tzlocal`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tzlocal. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f143f47b111b4a26ccc29c05b866dbb246987d6e`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-tzlocal-5.0.1.0/setup.py` & `types-tzlocal-5.0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tzlocal`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tzlocal. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f143f47b111b4a26ccc29c05b866dbb246987d6e`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="5.0.1.0",
+      version="5.0.1.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tzlocal.md",
```

### Comparing `types-tzlocal-5.0.1.0/types_tzlocal.egg-info/PKG-INFO` & `types-tzlocal-5.0.1.1/types_tzlocal.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tzlocal
-Version: 5.0.1.0
+Version: 5.0.1.1
 Summary: Typing stubs for tzlocal
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tzlocal.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tzlocal`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tzlocal. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `f143f47b111b4a26ccc29c05b866dbb246987d6e`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

