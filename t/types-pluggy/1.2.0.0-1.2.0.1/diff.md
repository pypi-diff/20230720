# Comparing `tmp/types-pluggy-1.2.0.0.tar.gz` & `tmp/types-pluggy-1.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pluggy-1.2.0.0.tar", last modified: Thu Jul 20 12:31:18 2023, max compression
+gzip compressed data, was "types-pluggy-1.2.0.1.tar", last modified: Thu Jul 20 15:18:03 2023, max compression
```

## Comparing `types-pluggy-1.2.0.0.tar` & `types-pluggy-1.2.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:31:18.219599 types-pluggy-1.2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-20 12:31:15.000000 types-pluggy-1.2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 12:31:15.000000 types-pluggy-1.2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 12:31:18.215599 types-pluggy-1.2.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:31:18.215599 types-pluggy-1.2.0.0/pluggy-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 12:31:15.000000 types-pluggy-1.2.0.0/pluggy-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 12:31:03.000000 types-pluggy-1.2.0.0/pluggy-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-20 12:31:03.000000 types-pluggy-1.2.0.0/pluggy-stubs/_hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-20 12:31:03.000000 types-pluggy-1.2.0.0/pluggy-stubs/_manager.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 12:31:03.000000 types-pluggy-1.2.0.0/pluggy-stubs/_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-20 12:31:03.000000 types-pluggy-1.2.0.0/pluggy-stubs/_tracing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 12:31:18.219599 types-pluggy-1.2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-20 12:31:15.000000 types-pluggy-1.2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:31:18.215599 types-pluggy-1.2.0.0/types_pluggy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 12:31:18.000000 types-pluggy-1.2.0.0/types_pluggy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 12:31:18.000000 types-pluggy-1.2.0.0/types_pluggy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:31:18.000000 types-pluggy-1.2.0.0/types_pluggy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 12:31:18.000000 types-pluggy-1.2.0.0/types_pluggy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:03.386453 types-pluggy-1.2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 15:18:02.000000 types-pluggy-1.2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:02.000000 types-pluggy-1.2.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:03.386453 types-pluggy-1.2.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:03.382454 types-pluggy-1.2.0.1/pluggy-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 15:18:02.000000 types-pluggy-1.2.0.1/pluggy-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 15:15:13.000000 types-pluggy-1.2.0.1/pluggy-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-07-20 15:15:13.000000 types-pluggy-1.2.0.1/pluggy-stubs/_hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-07-20 15:15:13.000000 types-pluggy-1.2.0.1/pluggy-stubs/_manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 15:15:13.000000 types-pluggy-1.2.0.1/pluggy-stubs/_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-20 15:15:13.000000 types-pluggy-1.2.0.1/pluggy-stubs/_tracing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:03.386453 types-pluggy-1.2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-20 15:18:02.000000 types-pluggy-1.2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:03.386453 types-pluggy-1.2.0.1/types_pluggy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-20 15:18:03.000000 types-pluggy-1.2.0.1/types_pluggy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 15:18:03.000000 types-pluggy-1.2.0.1/types_pluggy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:03.000000 types-pluggy-1.2.0.1/types_pluggy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:18:03.000000 types-pluggy-1.2.0.1/types_pluggy.egg-info/top_level.txt
```

### Comparing `types-pluggy-1.2.0.0/PKG-INFO` & `types-pluggy-1.2.0.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pluggy
-Version: 1.2.0.0
+Version: 1.2.0.1
 Summary: Typing stubs for pluggy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pluggy.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pluggy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pluggy. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4f56889f237da15bac1a570ad703a665bef983d9` and was tested
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-pluggy-1.2.0.0/pluggy-stubs/_hooks.pyi` & `types-pluggy-1.2.0.1/pluggy-stubs/_hooks.pyi`

 * *Files identical despite different names*

### Comparing `types-pluggy-1.2.0.0/pluggy-stubs/_manager.pyi` & `types-pluggy-1.2.0.1/pluggy-stubs/_manager.pyi`

 * *Files identical despite different names*

### Comparing `types-pluggy-1.2.0.0/pluggy-stubs/_result.pyi` & `types-pluggy-1.2.0.1/pluggy-stubs/_result.pyi`

 * *Files identical despite different names*

### Comparing `types-pluggy-1.2.0.0/pluggy-stubs/_tracing.pyi` & `types-pluggy-1.2.0.1/pluggy-stubs/_tracing.pyi`

 * *Files identical despite different names*

### Comparing `types-pluggy-1.2.0.0/setup.py` & `types-pluggy-1.2.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pluggy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pluggy. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4f56889f237da15bac1a570ad703a665bef983d9` and was tested
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.2.0.0",
+      version="1.2.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pluggy.md",
```

### Comparing `types-pluggy-1.2.0.0/types_pluggy.egg-info/PKG-INFO` & `types-pluggy-1.2.0.1/types_pluggy.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pluggy
-Version: 1.2.0.0
+Version: 1.2.0.1
 Summary: Typing stubs for pluggy
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pluggy.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pluggy`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pluggy. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `4f56889f237da15bac1a570ad703a665bef983d9` and was tested
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

