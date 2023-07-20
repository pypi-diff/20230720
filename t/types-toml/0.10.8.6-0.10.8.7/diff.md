# Comparing `tmp/types-toml-0.10.8.6.tar.gz` & `tmp/types-toml-0.10.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-toml-0.10.8.6.tar", last modified: Tue Mar 28 12:33:17 2023, max compression
+gzip compressed data, was "types-toml-0.10.8.7.tar", last modified: Thu Jul 20 15:19:42 2023, max compression
```

## Comparing `types-toml-0.10.8.6.tar` & `types-toml-0.10.8.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:17.129091 types-toml-0.10.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-28 12:33:16.000000 types-toml-0.10.8.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:16.000000 types-toml-0.10.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-28 12:33:17.129091 types-toml-0.10.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:17.129091 types-toml-0.10.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-03-28 12:33:16.000000 types-toml-0.10.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:17.129091 types-toml-0.10.8.6/toml-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 12:33:16.000000 types-toml-0.10.8.6/toml-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-28 12:32:25.000000 types-toml-0.10.8.6/toml-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-03-28 12:32:25.000000 types-toml-0.10.8.6/toml-stubs/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-28 12:32:25.000000 types-toml-0.10.8.6/toml-stubs/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-28 12:32:25.000000 types-toml-0.10.8.6/toml-stubs/ordered.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-28 12:32:25.000000 types-toml-0.10.8.6/toml-stubs/tz.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:17.129091 types-toml-0.10.8.6/types_toml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-28 12:33:17.000000 types-toml-0.10.8.6/types_toml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-03-28 12:33:17.000000 types-toml-0.10.8.6/types_toml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:17.000000 types-toml-0.10.8.6/types_toml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-28 12:33:17.000000 types-toml-0.10.8.6/types_toml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:42.235703 types-toml-0.10.8.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-20 15:19:41.000000 types-toml-0.10.8.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:41.000000 types-toml-0.10.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 15:19:42.235703 types-toml-0.10.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:42.235703 types-toml-0.10.8.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-20 15:19:41.000000 types-toml-0.10.8.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:42.235703 types-toml-0.10.8.7/toml-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 15:19:41.000000 types-toml-0.10.8.7/toml-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 15:15:13.000000 types-toml-0.10.8.7/toml-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-20 15:15:13.000000 types-toml-0.10.8.7/toml-stubs/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-20 15:15:13.000000 types-toml-0.10.8.7/toml-stubs/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-20 15:15:13.000000 types-toml-0.10.8.7/toml-stubs/ordered.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-20 15:15:13.000000 types-toml-0.10.8.7/toml-stubs/tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:42.235703 types-toml-0.10.8.7/types_toml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 15:19:42.000000 types-toml-0.10.8.7/types_toml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-07-20 15:19:42.000000 types-toml-0.10.8.7/types_toml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:42.000000 types-toml-0.10.8.7/types_toml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 15:19:42.000000 types-toml-0.10.8.7/types_toml.egg-info/top_level.txt
```

### Comparing `types-toml-0.10.8.6/CHANGELOG.md` & `types-toml-0.10.8.7/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.10.8.7 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.10.8.6 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 0.10.8.5 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-toml-0.10.8.6/PKG-INFO` & `types-toml-0.10.8.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-toml
-Version: 0.10.8.6
+Version: 0.10.8.7
 Summary: Typing stubs for toml
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/toml.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `toml`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/toml. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-toml-0.10.8.6/setup.py` & `types-toml-0.10.8.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `toml`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/toml. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.10.8.6",
+      version="0.10.8.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/toml.md",
```

### Comparing `types-toml-0.10.8.6/toml-stubs/__init__.pyi` & `types-toml-0.10.8.7/toml-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-toml-0.10.8.6/toml-stubs/decoder.pyi` & `types-toml-0.10.8.7/toml-stubs/decoder.pyi`

 * *Files identical despite different names*

### Comparing `types-toml-0.10.8.6/toml-stubs/encoder.pyi` & `types-toml-0.10.8.7/toml-stubs/encoder.pyi`

 * *Files identical despite different names*

### Comparing `types-toml-0.10.8.6/types_toml.egg-info/PKG-INFO` & `types-toml-0.10.8.7/types_toml.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-toml
-Version: 0.10.8.6
+Version: 0.10.8.7
 Summary: Typing stubs for toml
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/toml.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `toml`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/toml. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

