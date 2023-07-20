# Comparing `tmp/types-python-slugify-8.0.0.2.tar.gz` & `tmp/types-python-slugify-8.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-slugify-8.0.0.2.tar", last modified: Mon Mar 27 18:22:58 2023, max compression
+gzip compressed data, was "types-python-slugify-8.0.0.3.tar", last modified: Thu Jul 20 15:20:19 2023, max compression
```

## Comparing `types-python-slugify-8.0.0.2.tar` & `types-python-slugify-8.0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:58.202278 types-python-slugify-8.0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-03-27 18:22:57.000000 types-python-slugify-8.0.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:57.000000 types-python-slugify-8.0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-27 18:22:58.202278 types-python-slugify-8.0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:58.202278 types-python-slugify-8.0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-27 18:22:57.000000 types-python-slugify-8.0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:58.202278 types-python-slugify-8.0.0.2/slugify-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:22:57.000000 types-python-slugify-8.0.0.2/slugify-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-27 18:21:24.000000 types-python-slugify-8.0.0.2/slugify-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-27 18:21:24.000000 types-python-slugify-8.0.0.2/slugify-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-27 18:21:24.000000 types-python-slugify-8.0.0.2/slugify-stubs/slugify.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-27 18:21:24.000000 types-python-slugify-8.0.0.2/slugify-stubs/special.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:58.202278 types-python-slugify-8.0.0.2/types_python_slugify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-03-27 18:22:58.000000 types-python-slugify-8.0.0.2/types_python_slugify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-27 18:22:58.000000 types-python-slugify-8.0.0.2/types_python_slugify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:58.000000 types-python-slugify-8.0.0.2/types_python_slugify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-27 18:22:58.000000 types-python-slugify-8.0.0.2/types_python_slugify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:19.304160 types-python-slugify-8.0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-07-20 15:20:18.000000 types-python-slugify-8.0.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:18.000000 types-python-slugify-8.0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-20 15:20:19.304160 types-python-slugify-8.0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:19.304160 types-python-slugify-8.0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-20 15:20:18.000000 types-python-slugify-8.0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:19.304160 types-python-slugify-8.0.0.3/slugify-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 15:20:18.000000 types-python-slugify-8.0.0.3/slugify-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-20 15:15:13.000000 types-python-slugify-8.0.0.3/slugify-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 15:15:13.000000 types-python-slugify-8.0.0.3/slugify-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-20 15:15:13.000000 types-python-slugify-8.0.0.3/slugify-stubs/slugify.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-20 15:15:13.000000 types-python-slugify-8.0.0.3/slugify-stubs/special.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:19.304160 types-python-slugify-8.0.0.3/types_python_slugify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-20 15:20:19.000000 types-python-slugify-8.0.0.3/types_python_slugify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-20 15:20:19.000000 types-python-slugify-8.0.0.3/types_python_slugify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:19.000000 types-python-slugify-8.0.0.3/types_python_slugify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:20:19.000000 types-python-slugify-8.0.0.3/types_python_slugify.egg-info/top_level.txt
```

### Comparing `types-python-slugify-8.0.0.2/CHANGELOG.md` & `types-python-slugify-8.0.0.3/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 8.0.0.3 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 8.0.0.2 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 8.0.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-python-slugify-8.0.0.2/PKG-INFO` & `types-python-slugify-8.0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-slugify
-Version: 8.0.0.2
+Version: 8.0.0.3
 Summary: Typing stubs for python-slugify
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-slugify.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-slugify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-slugify. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-python-slugify-8.0.0.2/setup.py` & `types-python-slugify-8.0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-slugify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-slugify. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="8.0.0.2",
+      version="8.0.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-slugify.md",
```

### Comparing `types-python-slugify-8.0.0.2/slugify-stubs/slugify.pyi` & `types-python-slugify-8.0.0.3/slugify-stubs/slugify.pyi`

 * *Files identical despite different names*

### Comparing `types-python-slugify-8.0.0.2/types_python_slugify.egg-info/PKG-INFO` & `types-python-slugify-8.0.0.3/types_python_slugify.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-slugify
-Version: 8.0.0.2
+Version: 8.0.0.3
 Summary: Typing stubs for python-slugify
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-slugify.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-slugify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-slugify. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

