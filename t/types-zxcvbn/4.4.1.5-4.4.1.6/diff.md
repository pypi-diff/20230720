# Comparing `tmp/types-zxcvbn-4.4.1.5.tar.gz` & `tmp/types-zxcvbn-4.4.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-zxcvbn-4.4.1.5.tar", last modified: Tue Mar 28 18:20:12 2023, max compression
+gzip compressed data, was "types-zxcvbn-4.4.1.6.tar", last modified: Thu Jul 20 15:18:10 2023, max compression
```

## Comparing `types-zxcvbn-4.4.1.5.tar` & `types-zxcvbn-4.4.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:12.006596 types-zxcvbn-4.4.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-03-28 18:20:09.000000 types-zxcvbn-4.4.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 18:20:09.000000 types-zxcvbn-4.4.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-28 18:20:12.006596 types-zxcvbn-4.4.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 18:20:12.006596 types-zxcvbn-4.4.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-03-28 18:20:09.000000 types-zxcvbn-4.4.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:12.002596 types-zxcvbn-4.4.1.5/types_zxcvbn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-28 18:20:11.000000 types-zxcvbn-4.4.1.5/types_zxcvbn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-28 18:20:11.000000 types-zxcvbn-4.4.1.5/types_zxcvbn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 18:20:11.000000 types-zxcvbn-4.4.1.5/types_zxcvbn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-28 18:20:11.000000 types-zxcvbn-4.4.1.5/types_zxcvbn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:12.006596 types-zxcvbn-4.4.1.5/zxcvbn-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 18:20:09.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/adjacency_graphs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/feedback.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/frequency_lists.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/matching.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/scoring.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-28 18:19:54.000000 types-zxcvbn-4.4.1.5/zxcvbn-stubs/time_estimates.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:10.658546 types-zxcvbn-4.4.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-20 15:18:09.000000 types-zxcvbn-4.4.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:09.000000 types-zxcvbn-4.4.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:10.658546 types-zxcvbn-4.4.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:10.658546 types-zxcvbn-4.4.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 15:18:09.000000 types-zxcvbn-4.4.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:10.654546 types-zxcvbn-4.4.1.6/types_zxcvbn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:10.000000 types-zxcvbn-4.4.1.6/types_zxcvbn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-20 15:18:10.000000 types-zxcvbn-4.4.1.6/types_zxcvbn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:10.000000 types-zxcvbn-4.4.1.6/types_zxcvbn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:18:10.000000 types-zxcvbn-4.4.1.6/types_zxcvbn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:10.658546 types-zxcvbn-4.4.1.6/zxcvbn-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 15:18:09.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/adjacency_graphs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/feedback.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/frequency_lists.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/matching.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/scoring.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-20 15:15:13.000000 types-zxcvbn-4.4.1.6/zxcvbn-stubs/time_estimates.pyi
```

### Comparing `types-zxcvbn-4.4.1.5/CHANGELOG.md` & `types-zxcvbn-4.4.1.6/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 4.4.1.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 4.4.1.5 (2023-03-28)
 
 Add defaults to third-party stubs U-Z (#9971)
 
 ## 4.4.1.4 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-zxcvbn-4.4.1.5/PKG-INFO` & `types-zxcvbn-4.4.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-zxcvbn
-Version: 4.4.1.5
+Version: 4.4.1.6
 Summary: Typing stubs for zxcvbn
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/zxcvbn.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `zxcvbn`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/zxcvbn. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `87c1b949cdf996148e44fb913a1b689f8d337a5a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-zxcvbn-4.4.1.5/setup.py` & `types-zxcvbn-4.4.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `zxcvbn`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/zxcvbn. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `87c1b949cdf996148e44fb913a1b689f8d337a5a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.4.1.5",
+      version="4.4.1.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/zxcvbn.md",
```

### Comparing `types-zxcvbn-4.4.1.5/types_zxcvbn.egg-info/PKG-INFO` & `types-zxcvbn-4.4.1.6/types_zxcvbn.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-zxcvbn
-Version: 4.4.1.5
+Version: 4.4.1.6
 Summary: Typing stubs for zxcvbn
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/zxcvbn.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `zxcvbn`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/zxcvbn. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `87c1b949cdf996148e44fb913a1b689f8d337a5a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-zxcvbn-4.4.1.5/zxcvbn-stubs/matching.pyi` & `types-zxcvbn-4.4.1.6/zxcvbn-stubs/matching.pyi`

 * *Files identical despite different names*

### Comparing `types-zxcvbn-4.4.1.5/zxcvbn-stubs/scoring.pyi` & `types-zxcvbn-4.4.1.6/zxcvbn-stubs/scoring.pyi`

 * *Files identical despite different names*

### Comparing `types-zxcvbn-4.4.1.5/zxcvbn-stubs/time_estimates.pyi` & `types-zxcvbn-4.4.1.6/zxcvbn-stubs/time_estimates.pyi`

 * *Files identical despite different names*

