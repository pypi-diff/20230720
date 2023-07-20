# Comparing `tmp/types-pynput-1.7.5.6.tar.gz` & `tmp/types-pynput-1.7.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pynput-1.7.5.6.tar", last modified: Mon Mar 27 18:22:04 2023, max compression
+gzip compressed data, was "types-pynput-1.7.5.7.tar", last modified: Thu Jul 20 15:18:55 2023, max compression
```

## Comparing `types-pynput-1.7.5.6.tar` & `types-pynput-1.7.5.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:04.017723 types-pynput-1.7.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:22:04.017723 types-pynput-1.7.5.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:04.013723 types-pynput-1.7.5.6/pynput-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/pynput-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:04.013723 types-pynput-1.7.5.6/pynput-stubs/keyboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/keyboard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/keyboard/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/keyboard/_dummy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:04.013723 types-pynput-1.7.5.6/pynput-stubs/mouse/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/mouse/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/mouse/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-27 18:21:24.000000 types-pynput-1.7.5.6/pynput-stubs/mouse/_dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:04.017723 types-pynput-1.7.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:04.013723 types-pynput-1.7.5.6/types_pynput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/types_pynput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/types_pynput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/types_pynput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-27 18:22:03.000000 types-pynput-1.7.5.6/types_pynput.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.147114 types-pynput-1.7.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/pynput-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/pynput-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/pynput-stubs/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/keyboard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/keyboard/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/keyboard/_dummy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/pynput-stubs/mouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/mouse/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/mouse/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-20 15:15:13.000000 types-pynput-1.7.5.7/pynput-stubs/mouse/_dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:55.147114 types-pynput-1.7.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 15:18:54.000000 types-pynput-1.7.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:55.143114 types-pynput-1.7.5.7/types_pynput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:18:55.000000 types-pynput-1.7.5.7/types_pynput.egg-info/top_level.txt
```

### Comparing `types-pynput-1.7.5.6/CHANGELOG.md` & `types-pynput-1.7.5.7/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.7.5.7 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.7.5.6 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
 
 ## 1.7.5.5 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-pynput-1.7.5.6/PKG-INFO` & `types-pynput-1.7.5.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pynput
-Version: 1.7.5.6
+Version: 1.7.5.7
 Summary: Typing stubs for pynput
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pynput`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pynput-1.7.5.6/pynput-stubs/_util.pyi` & `types-pynput-1.7.5.7/pynput-stubs/_util.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.6/pynput-stubs/keyboard/__init__.pyi` & `types-pynput-1.7.5.7/pynput-stubs/keyboard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.6/pynput-stubs/keyboard/_base.pyi` & `types-pynput-1.7.5.7/pynput-stubs/keyboard/_base.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.6/pynput-stubs/mouse/__init__.pyi` & `types-pynput-1.7.5.7/pynput-stubs/mouse/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.6/pynput-stubs/mouse/_base.pyi` & `types-pynput-1.7.5.7/pynput-stubs/mouse/_base.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.5.6/setup.py` & `types-pynput-1.7.5.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pynput`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.7.5.6",
+      version="1.7.5.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md",
```

### Comparing `types-pynput-1.7.5.6/types_pynput.egg-info/PKG-INFO` & `types-pynput-1.7.5.7/types_pynput.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pynput
-Version: 1.7.5.6
+Version: 1.7.5.7
 Summary: Typing stubs for pynput
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pynput`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

