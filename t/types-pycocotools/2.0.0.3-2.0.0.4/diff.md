# Comparing `tmp/types-pycocotools-2.0.0.3.tar.gz` & `tmp/types-pycocotools-2.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pycocotools-2.0.0.3.tar", last modified: Mon Mar 27 18:22:11 2023, max compression
+gzip compressed data, was "types-pycocotools-2.0.0.4.tar", last modified: Thu Jul 20 15:16:17 2023, max compression
```

## Comparing `types-pycocotools-2.0.0.3.tar` & `types-pycocotools-2.0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:11.457803 types-pycocotools-2.0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-27 18:22:10.000000 types-pycocotools-2.0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:10.000000 types-pycocotools-2.0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:22:11.457803 types-pycocotools-2.0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:11.457803 types-pycocotools-2.0.0.3/pycocotools-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:22:10.000000 types-pycocotools-2.0.0.3/pycocotools-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-27 18:21:24.000000 types-pycocotools-2.0.0.3/pycocotools-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-27 18:21:24.000000 types-pycocotools-2.0.0.3/pycocotools-stubs/coco.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-27 18:21:24.000000 types-pycocotools-2.0.0.3/pycocotools-stubs/cocoeval.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-03-27 18:21:24.000000 types-pycocotools-2.0.0.3/pycocotools-stubs/mask.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:11.457803 types-pycocotools-2.0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-03-27 18:22:10.000000 types-pycocotools-2.0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:11.457803 types-pycocotools-2.0.0.3/types_pycocotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-03-27 18:22:11.000000 types-pycocotools-2.0.0.3/types_pycocotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-27 18:22:11.000000 types-pycocotools-2.0.0.3/types_pycocotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:11.000000 types-pycocotools-2.0.0.3/types_pycocotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:22:11.000000 types-pycocotools-2.0.0.3/types_pycocotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:17.489161 types-pycocotools-2.0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-20 15:16:16.000000 types-pycocotools-2.0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:16.000000 types-pycocotools-2.0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:16:17.489161 types-pycocotools-2.0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:17.489161 types-pycocotools-2.0.0.4/pycocotools-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 15:16:16.000000 types-pycocotools-2.0.0.4/pycocotools-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 15:15:13.000000 types-pycocotools-2.0.0.4/pycocotools-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-20 15:15:13.000000 types-pycocotools-2.0.0.4/pycocotools-stubs/coco.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-20 15:15:13.000000 types-pycocotools-2.0.0.4/pycocotools-stubs/cocoeval.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-20 15:15:13.000000 types-pycocotools-2.0.0.4/pycocotools-stubs/mask.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:17.489161 types-pycocotools-2.0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-20 15:16:16.000000 types-pycocotools-2.0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:17.489161 types-pycocotools-2.0.0.4/types_pycocotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:16:17.000000 types-pycocotools-2.0.0.4/types_pycocotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-20 15:16:17.000000 types-pycocotools-2.0.0.4/types_pycocotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:17.000000 types-pycocotools-2.0.0.4/types_pycocotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:16:17.000000 types-pycocotools-2.0.0.4/types_pycocotools.egg-info/top_level.txt
```

### Comparing `types-pycocotools-2.0.0.3/PKG-INFO` & `types-pycocotools-2.0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pycocotools
-Version: 2.0.0.3
+Version: 2.0.0.4
 Summary: Typing stubs for pycocotools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycocotools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pycocotools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycocotools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pycocotools-2.0.0.3/pycocotools-stubs/coco.pyi` & `types-pycocotools-2.0.0.4/pycocotools-stubs/coco.pyi`

 * *Files identical despite different names*

### Comparing `types-pycocotools-2.0.0.3/pycocotools-stubs/cocoeval.pyi` & `types-pycocotools-2.0.0.4/pycocotools-stubs/cocoeval.pyi`

 * *Files identical despite different names*

### Comparing `types-pycocotools-2.0.0.3/pycocotools-stubs/mask.pyi` & `types-pycocotools-2.0.0.4/pycocotools-stubs/mask.pyi`

 * *Files identical despite different names*

### Comparing `types-pycocotools-2.0.0.3/setup.py` & `types-pycocotools-2.0.0.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pycocotools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycocotools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.3",
+      version="2.0.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycocotools.md",
```

### Comparing `types-pycocotools-2.0.0.3/types_pycocotools.egg-info/PKG-INFO` & `types-pycocotools-2.0.0.4/types_pycocotools.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pycocotools
-Version: 2.0.0.3
+Version: 2.0.0.4
 Summary: Typing stubs for pycocotools
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pycocotools.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pycocotools`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pycocotools. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

