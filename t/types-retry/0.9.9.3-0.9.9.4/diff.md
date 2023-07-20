# Comparing `tmp/types-retry-0.9.9.3.tar.gz` & `tmp/types-retry-0.9.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-retry-0.9.9.3.tar", last modified: Tue Mar 28 12:33:06 2023, max compression
+gzip compressed data, was "types-retry-0.9.9.4.tar", last modified: Thu Jul 20 15:18:00 2023, max compression
```

## Comparing `types-retry-0.9.9.3.tar` & `types-retry-0.9.9.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:06.129248 types-retry-0.9.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-28 12:33:05.000000 types-retry-0.9.9.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:05.000000 types-retry-0.9.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-28 12:33:06.125249 types-retry-0.9.9.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:06.125249 types-retry-0.9.9.3/retry-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 12:33:05.000000 types-retry-0.9.9.3/retry-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-28 12:32:25.000000 types-retry-0.9.9.3/retry-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-28 12:32:25.000000 types-retry-0.9.9.3/retry-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:06.129248 types-retry-0.9.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-28 12:33:05.000000 types-retry-0.9.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:06.125249 types-retry-0.9.9.3/types_retry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-03-28 12:33:06.000000 types-retry-0.9.9.3/types_retry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-28 12:33:06.000000 types-retry-0.9.9.3/types_retry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:06.000000 types-retry-0.9.9.3/types_retry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-28 12:33:06.000000 types-retry-0.9.9.3/types_retry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:00.026410 types-retry-0.9.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:18:00.026410 types-retry-0.9.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:00.026410 types-retry-0.9.9.4/retry-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/retry-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 15:15:13.000000 types-retry-0.9.9.4/retry-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 15:15:13.000000 types-retry-0.9.9.4/retry-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:00.026410 types-retry-0.9.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:00.026410 types-retry-0.9.9.4/types_retry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/types_retry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/types_retry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/types_retry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 15:17:59.000000 types-retry-0.9.9.4/types_retry.egg-info/top_level.txt
```

### Comparing `types-retry-0.9.9.3/CHANGELOG.md` & `types-retry-0.9.9.4/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.9.9.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.9.9.3 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 0.9.9.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-retry-0.9.9.3/PKG-INFO` & `types-retry-0.9.9.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-retry
-Version: 0.9.9.3
+Version: 0.9.9.4
 Summary: Typing stubs for retry
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/retry.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `retry`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/retry. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-retry-0.9.9.3/retry-stubs/api.pyi` & `types-retry-0.9.9.4/retry-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-retry-0.9.9.3/setup.py` & `types-retry-0.9.9.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `retry`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/retry. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.9.3",
+      version="0.9.9.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/retry.md",
```

### Comparing `types-retry-0.9.9.3/types_retry.egg-info/PKG-INFO` & `types-retry-0.9.9.4/types_retry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-retry
-Version: 0.9.9.3
+Version: 0.9.9.4
 Summary: Typing stubs for retry
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/retry.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `retry`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/retry. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

