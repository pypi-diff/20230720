# Comparing `tmp/types-cachetools-5.3.0.5.tar.gz` & `tmp/types-cachetools-5.3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-cachetools-5.3.0.5.tar", last modified: Mon Mar 27 18:23:15 2023, max compression
+gzip compressed data, was "types-cachetools-5.3.0.6.tar", last modified: Thu Jul 20 15:16:48 2023, max compression
```

## Comparing `types-cachetools-5.3.0.5.tar` & `types-cachetools-5.3.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:15.694469 types-cachetools-5.3.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:23:15.694469 types-cachetools-5.3.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:15.694469 types-cachetools-5.3.0.5/cachetools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/cachetools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-03-27 18:21:24.000000 types-cachetools-5.3.0.5/cachetools-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-27 18:21:24.000000 types-cachetools-5.3.0.5/cachetools-stubs/func.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-27 18:21:24.000000 types-cachetools-5.3.0.5/cachetools-stubs/keys.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:23:15.694469 types-cachetools-5.3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:15.694469 types-cachetools-5.3.0.5/types_cachetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/types_cachetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/types_cachetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/types_cachetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 18:23:15.000000 types-cachetools-5.3.0.5/types_cachetools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:48.273528 types-cachetools-5.3.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-07-20 15:16:47.000000 types-cachetools-5.3.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:47.000000 types-cachetools-5.3.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 15:16:48.273528 types-cachetools-5.3.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:48.273528 types-cachetools-5.3.0.6/cachetools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 15:16:47.000000 types-cachetools-5.3.0.6/cachetools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-20 15:15:13.000000 types-cachetools-5.3.0.6/cachetools-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-20 15:15:13.000000 types-cachetools-5.3.0.6/cachetools-stubs/func.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-20 15:15:13.000000 types-cachetools-5.3.0.6/cachetools-stubs/keys.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:48.273528 types-cachetools-5.3.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-20 15:16:47.000000 types-cachetools-5.3.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:48.273528 types-cachetools-5.3.0.6/types_cachetools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 15:16:48.000000 types-cachetools-5.3.0.6/types_cachetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-20 15:16:48.000000 types-cachetools-5.3.0.6/types_cachetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:48.000000 types-cachetools-5.3.0.6/types_cachetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:16:48.000000 types-cachetools-5.3.0.6/types_cachetools.egg-info/top_level.txt
```

### Comparing `types-cachetools-5.3.0.5/CHANGELOG.md` & `types-cachetools-5.3.0.6/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 5.3.0.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 5.3.0.5 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
 
 ## 5.3.0.4 (2023-02-26)
 
 Improve many `__(a)exit__` annotations (#9696)
```

### Comparing `types-cachetools-5.3.0.5/PKG-INFO` & `types-cachetools-5.3.0.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-cachetools
-Version: 5.3.0.5
+Version: 5.3.0.6
 Summary: Typing stubs for cachetools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/cachetools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `cachetools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/cachetools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-cachetools-5.3.0.5/cachetools-stubs/__init__.pyi` & `types-cachetools-5.3.0.6/cachetools-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-cachetools-5.3.0.5/cachetools-stubs/func.pyi` & `types-cachetools-5.3.0.6/cachetools-stubs/func.pyi`

 * *Files identical despite different names*

### Comparing `types-cachetools-5.3.0.5/setup.py` & `types-cachetools-5.3.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `cachetools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/cachetools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="5.3.0.5",
+      version="5.3.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/cachetools.md",
```

### Comparing `types-cachetools-5.3.0.5/types_cachetools.egg-info/PKG-INFO` & `types-cachetools-5.3.0.6/types_cachetools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-cachetools
-Version: 5.3.0.5
+Version: 5.3.0.6
 Summary: Typing stubs for cachetools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/cachetools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `cachetools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/cachetools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

