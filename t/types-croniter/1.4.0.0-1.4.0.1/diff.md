# Comparing `tmp/types-croniter-1.4.0.0.tar.gz` & `tmp/types-croniter-1.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-croniter-1.4.0.0.tar", last modified: Wed Jun 21 15:14:47 2023, max compression
+gzip compressed data, was "types-croniter-1.4.0.1.tar", last modified: Thu Jul 20 15:19:55 2023, max compression
```

## Comparing `types-croniter-1.4.0.0.tar` & `types-croniter-1.4.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/croniter-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/croniter-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-21 15:14:34.000000 types-croniter-1.4.0.0/croniter-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-06-21 15:14:34.000000 types-croniter-1.4.0.0/croniter-stubs/croniter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-21 15:14:45.000000 types-croniter-1.4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:14:47.982594 types-croniter-1.4.0.0/types_croniter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 15:14:47.000000 types-croniter-1.4.0.0/types_croniter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:55.215867 types-croniter-1.4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-20 15:19:54.000000 types-croniter-1.4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:54.000000 types-croniter-1.4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:19:55.215867 types-croniter-1.4.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:55.215867 types-croniter-1.4.0.1/croniter-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 15:19:54.000000 types-croniter-1.4.0.1/croniter-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-20 15:15:13.000000 types-croniter-1.4.0.1/croniter-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-20 15:15:13.000000 types-croniter-1.4.0.1/croniter-stubs/croniter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:55.215867 types-croniter-1.4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-20 15:19:54.000000 types-croniter-1.4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:55.215867 types-croniter-1.4.0.1/types_croniter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:19:55.000000 types-croniter-1.4.0.1/types_croniter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-20 15:19:55.000000 types-croniter-1.4.0.1/types_croniter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:55.000000 types-croniter-1.4.0.1/types_croniter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:19:55.000000 types-croniter-1.4.0.1/types_croniter.egg-info/top_level.txt
```

### Comparing `types-croniter-1.4.0.0/CHANGELOG.md` & `types-croniter-1.4.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.4.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.4.0.0 (2023-06-21)
 
 Bump croniter to 1.4 (#10341)
 
 Also require `bytes` for all `hash_id`s for consistency, even
 if some methods might work with other types as well. But
 using other types might hint at some inconsistent type
```

### Comparing `types-croniter-1.4.0.0/PKG-INFO` & `types-croniter-1.4.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.4.0.0
+Version: 1.4.0.1
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4a692fc54616c68d606c3ba6c93d393589663809` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-croniter-1.4.0.0/croniter-stubs/croniter.pyi` & `types-croniter-1.4.0.1/croniter-stubs/croniter.pyi`

 * *Files identical despite different names*

### Comparing `types-croniter-1.4.0.0/setup.py` & `types-croniter-1.4.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4a692fc54616c68d606c3ba6c93d393589663809` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.4.0.0",
+      version="1.4.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md",
```

### Comparing `types-croniter-1.4.0.0/types_croniter.egg-info/PKG-INFO` & `types-croniter-1.4.0.1/types_croniter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-croniter
-Version: 1.4.0.0
+Version: 1.4.0.1
 Summary: Typing stubs for croniter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/croniter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `croniter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/croniter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4a692fc54616c68d606c3ba6c93d393589663809` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

