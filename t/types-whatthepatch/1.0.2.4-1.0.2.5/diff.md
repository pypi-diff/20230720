# Comparing `tmp/types-whatthepatch-1.0.2.4.tar.gz` & `tmp/types-whatthepatch-1.0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-whatthepatch-1.0.2.4.tar", last modified: Tue Mar 28 18:20:32 2023, max compression
+gzip compressed data, was "types-whatthepatch-1.0.2.5.tar", last modified: Thu Jul 20 15:15:44 2023, max compression
```

## Comparing `types-whatthepatch-1.0.2.4.tar` & `types-whatthepatch-1.0.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:32.138747 types-whatthepatch-1.0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-03-28 18:20:31.000000 types-whatthepatch-1.0.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 18:20:31.000000 types-whatthepatch-1.0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-28 18:20:32.138747 types-whatthepatch-1.0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 18:20:32.138747 types-whatthepatch-1.0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-28 18:20:31.000000 types-whatthepatch-1.0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:32.134747 types-whatthepatch-1.0.2.4/types_whatthepatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-03-28 18:20:32.000000 types-whatthepatch-1.0.2.4/types_whatthepatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-28 18:20:32.000000 types-whatthepatch-1.0.2.4/types_whatthepatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 18:20:32.000000 types-whatthepatch-1.0.2.4/types_whatthepatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 18:20:32.000000 types-whatthepatch-1.0.2.4/types_whatthepatch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 18:20:32.134747 types-whatthepatch-1.0.2.4/whatthepatch-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 18:20:31.000000 types-whatthepatch-1.0.2.4/whatthepatch-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-28 18:19:54.000000 types-whatthepatch-1.0.2.4/whatthepatch-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-28 18:19:54.000000 types-whatthepatch-1.0.2.4/whatthepatch-stubs/apply.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-03-28 18:19:54.000000 types-whatthepatch-1.0.2.4/whatthepatch-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-03-28 18:19:54.000000 types-whatthepatch-1.0.2.4/whatthepatch-stubs/patch.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-28 18:19:54.000000 types-whatthepatch-1.0.2.4/whatthepatch-stubs/snippets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:44.936761 types-whatthepatch-1.0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-20 15:15:44.936761 types-whatthepatch-1.0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:44.936761 types-whatthepatch-1.0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:44.936761 types-whatthepatch-1.0.2.5/types_whatthepatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/types_whatthepatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/types_whatthepatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/types_whatthepatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/types_whatthepatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:44.936761 types-whatthepatch-1.0.2.5/whatthepatch-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 15:15:44.000000 types-whatthepatch-1.0.2.5/whatthepatch-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 15:15:13.000000 types-whatthepatch-1.0.2.5/whatthepatch-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 15:15:13.000000 types-whatthepatch-1.0.2.5/whatthepatch-stubs/apply.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-20 15:15:13.000000 types-whatthepatch-1.0.2.5/whatthepatch-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-07-20 15:15:13.000000 types-whatthepatch-1.0.2.5/whatthepatch-stubs/patch.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 15:15:13.000000 types-whatthepatch-1.0.2.5/whatthepatch-stubs/snippets.pyi
```

### Comparing `types-whatthepatch-1.0.2.4/CHANGELOG.md` & `types-whatthepatch-1.0.2.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.0.2.5 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.0.2.4 (2023-03-28)
 
 Add defaults to third-party stubs U-Z (#9971)
 
 ## 1.0.2.3 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-whatthepatch-1.0.2.4/PKG-INFO` & `types-whatthepatch-1.0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-whatthepatch
-Version: 1.0.2.4
+Version: 1.0.2.5
 Summary: Typing stubs for whatthepatch
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/whatthepatch.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `whatthepatch`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/whatthepatch. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `87c1b949cdf996148e44fb913a1b689f8d337a5a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-whatthepatch-1.0.2.4/setup.py` & `types-whatthepatch-1.0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `whatthepatch`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/whatthepatch. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `87c1b949cdf996148e44fb913a1b689f8d337a5a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.0.2.4",
+      version="1.0.2.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/whatthepatch.md",
```

### Comparing `types-whatthepatch-1.0.2.4/types_whatthepatch.egg-info/PKG-INFO` & `types-whatthepatch-1.0.2.5/types_whatthepatch.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-whatthepatch
-Version: 1.0.2.4
+Version: 1.0.2.5
 Summary: Typing stubs for whatthepatch
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/whatthepatch.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `whatthepatch`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/whatthepatch. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `87c1b949cdf996148e44fb913a1b689f8d337a5a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-whatthepatch-1.0.2.4/whatthepatch-stubs/patch.pyi` & `types-whatthepatch-1.0.2.5/whatthepatch-stubs/patch.pyi`

 * *Files identical despite different names*

