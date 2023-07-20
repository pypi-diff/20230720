# Comparing `tmp/types-chevron-0.14.2.4.tar.gz` & `tmp/types-chevron-0.14.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-chevron-0.14.2.4.tar", last modified: Mon Mar 27 18:22:18 2023, max compression
+gzip compressed data, was "types-chevron-0.14.2.5.tar", last modified: Thu Jul 20 15:20:08 2023, max compression
```

## Comparing `types-chevron-0.14.2.4.tar` & `types-chevron-0.14.2.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:18.625878 types-chevron-0.14.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-27 18:22:17.000000 types-chevron-0.14.2.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:17.000000 types-chevron-0.14.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-27 18:22:18.625878 types-chevron-0.14.2.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:18.625878 types-chevron-0.14.2.4/chevron-stubs/
--rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-03-27 18:22:17.000000 types-chevron-0.14.2.4/chevron-stubs/METADATA.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-03-27 18:21:24.000000 types-chevron-0.14.2.4/chevron-stubs/__init__.pyi
--rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-03-27 18:21:24.000000 types-chevron-0.14.2.4/chevron-stubs/main.pyi
--rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-03-27 18:21:24.000000 types-chevron-0.14.2.4/chevron-stubs/metadata.pyi
--rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-03-27 18:21:24.000000 types-chevron-0.14.2.4/chevron-stubs/renderer.pyi
--rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-03-27 18:21:24.000000 types-chevron-0.14.2.4/chevron-stubs/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:18.625878 types-chevron-0.14.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-03-27 18:22:17.000000 types-chevron-0.14.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:18.625878 types-chevron-0.14.2.4/types_chevron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-03-27 18:22:18.000000 types-chevron-0.14.2.4/types_chevron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-03-27 18:22:18.000000 types-chevron-0.14.2.4/types_chevron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:18.000000 types-chevron-0.14.2.4/types_chevron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:22:18.000000 types-chevron-0.14.2.4/types_chevron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:08.968033 types-chevron-0.14.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-20 15:20:08.964033 types-chevron-0.14.2.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:08.964033 types-chevron-0.14.2.5/chevron-stubs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      100 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/chevron-stubs/METADATA.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      202 2023-07-20 15:15:13.000000 types-chevron-0.14.2.5/chevron-stubs/__init__.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-07-20 15:15:13.000000 types-chevron-0.14.2.5/chevron-stubs/main.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (123)       13 2023-07-20 15:15:13.000000 types-chevron-0.14.2.5/chevron-stubs/metadata.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (123)      695 2023-07-20 15:15:13.000000 types-chevron-0.14.2.5/chevron-stubs/renderer.pyi
+-rwxr-xr-x   0 runner    (1001) docker     (123)      624 2023-07-20 15:15:13.000000 types-chevron-0.14.2.5/chevron-stubs/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:08.968033 types-chevron-0.14.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:08.964033 types-chevron-0.14.2.5/types_chevron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/types_chevron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/types_chevron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/types_chevron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:20:08.000000 types-chevron-0.14.2.5/types_chevron.egg-info/top_level.txt
```

### Comparing `types-chevron-0.14.2.4/CHANGELOG.md` & `types-chevron-0.14.2.5/CHANGELOG.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.14.2.5 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.14.2.4 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 0.14.2.3 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-chevron-0.14.2.4/PKG-INFO` & `types-chevron-0.14.2.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-chevron
-Version: 0.14.2.4
+Version: 0.14.2.5
 Summary: Typing stubs for chevron
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chevron.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `chevron`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/chevron. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-chevron-0.14.2.4/chevron-stubs/renderer.pyi` & `types-chevron-0.14.2.5/chevron-stubs/renderer.pyi`

 * *Files identical despite different names*

### Comparing `types-chevron-0.14.2.4/chevron-stubs/tokenizer.pyi` & `types-chevron-0.14.2.5/chevron-stubs/tokenizer.pyi`

 * *Files identical despite different names*

### Comparing `types-chevron-0.14.2.4/setup.py` & `types-chevron-0.14.2.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `chevron`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/chevron. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.14.2.4",
+      version="0.14.2.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chevron.md",
```

### Comparing `types-chevron-0.14.2.4/types_chevron.egg-info/PKG-INFO` & `types-chevron-0.14.2.5/types_chevron.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-chevron
-Version: 0.14.2.4
+Version: 0.14.2.5
 Summary: Typing stubs for chevron
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/chevron.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `chevron`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/chevron. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

