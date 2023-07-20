# Comparing `tmp/types-passpy-1.0.2.3.tar.gz` & `tmp/types-passpy-1.0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-passpy-1.0.2.3.tar", last modified: Mon Mar 27 18:24:47 2023, max compression
+gzip compressed data, was "types-passpy-1.0.2.4.tar", last modified: Thu Jul 20 15:17:22 2023, max compression
```

## Comparing `types-passpy-1.0.2.3.tar` & `types-passpy-1.0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:47.359423 types-passpy-1.0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-27 18:24:46.000000 types-passpy-1.0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:46.000000 types-passpy-1.0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:24:47.359423 types-passpy-1.0.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:47.359423 types-passpy-1.0.2.3/passpy-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:24:46.000000 types-passpy-1.0.2.3/passpy-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-27 18:21:24.000000 types-passpy-1.0.2.3/passpy-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 18:21:24.000000 types-passpy-1.0.2.3/passpy-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-03-27 18:21:24.000000 types-passpy-1.0.2.3/passpy-stubs/store.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-03-27 18:21:24.000000 types-passpy-1.0.2.3/passpy-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:47.359423 types-passpy-1.0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-03-27 18:24:46.000000 types-passpy-1.0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:47.359423 types-passpy-1.0.2.3/types_passpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:24:47.000000 types-passpy-1.0.2.3/types_passpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-27 18:24:47.000000 types-passpy-1.0.2.3/types_passpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:47.000000 types-passpy-1.0.2.3/types_passpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:24:47.000000 types-passpy-1.0.2.3/types_passpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:22.377943 types-passpy-1.0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 15:17:21.000000 types-passpy-1.0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:21.000000 types-passpy-1.0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:17:22.377943 types-passpy-1.0.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:22.377943 types-passpy-1.0.2.4/passpy-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 15:17:21.000000 types-passpy-1.0.2.4/passpy-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-20 15:15:13.000000 types-passpy-1.0.2.4/passpy-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 15:15:13.000000 types-passpy-1.0.2.4/passpy-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-07-20 15:15:13.000000 types-passpy-1.0.2.4/passpy-stubs/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-20 15:15:13.000000 types-passpy-1.0.2.4/passpy-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:22.377943 types-passpy-1.0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-07-20 15:17:21.000000 types-passpy-1.0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:22.377943 types-passpy-1.0.2.4/types_passpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:17:22.000000 types-passpy-1.0.2.4/types_passpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-20 15:17:22.000000 types-passpy-1.0.2.4/types_passpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:22.000000 types-passpy-1.0.2.4/types_passpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:17:22.000000 types-passpy-1.0.2.4/types_passpy.egg-info/top_level.txt
```

### Comparing `types-passpy-1.0.2.3/CHANGELOG.md` & `types-passpy-1.0.2.4/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.0.2.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.0.2.3 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 1.0.2.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-passpy-1.0.2.3/PKG-INFO` & `types-passpy-1.0.2.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-passpy
-Version: 1.0.2.3
+Version: 1.0.2.4
 Summary: Typing stubs for passpy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/passpy.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `passpy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/passpy. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-passpy-1.0.2.3/passpy-stubs/store.pyi` & `types-passpy-1.0.2.4/passpy-stubs/store.pyi`

 * *Files identical despite different names*

### Comparing `types-passpy-1.0.2.3/passpy-stubs/util.pyi` & `types-passpy-1.0.2.4/passpy-stubs/util.pyi`

 * *Files identical despite different names*

### Comparing `types-passpy-1.0.2.3/setup.py` & `types-passpy-1.0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `passpy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/passpy. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.0.2.3",
+      version="1.0.2.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/passpy.md",
```

### Comparing `types-passpy-1.0.2.3/types_passpy.egg-info/PKG-INFO` & `types-passpy-1.0.2.4/types_passpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-passpy
-Version: 1.0.2.3
+Version: 1.0.2.4
 Summary: Typing stubs for passpy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/passpy.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `passpy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/passpy. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

