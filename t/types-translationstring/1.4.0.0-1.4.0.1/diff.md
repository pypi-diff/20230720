# Comparing `tmp/types-translationstring-1.4.0.0.tar.gz` & `tmp/types-translationstring-1.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-translationstring-1.4.0.0.tar", last modified: Wed Mar 22 15:17:08 2023, max compression
+gzip compressed data, was "types-translationstring-1.4.0.1.tar", last modified: Thu Jul 20 15:17:28 2023, max compression
```

## Comparing `types-translationstring-1.4.0.0.tar` & `types-translationstring-1.4.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:17:08.203895 types-translationstring-1.4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-22 15:17:06.000000 types-translationstring-1.4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-22 15:17:06.000000 types-translationstring-1.4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-22 15:17:08.203895 types-translationstring-1.4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 15:17:08.203895 types-translationstring-1.4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-22 15:17:06.000000 types-translationstring-1.4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:17:08.203895 types-translationstring-1.4.0.0/translationstring-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-22 15:17:06.000000 types-translationstring-1.4.0.0/translationstring-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-03-22 15:16:54.000000 types-translationstring-1.4.0.0/translationstring-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:17:08.203895 types-translationstring-1.4.0.0/types_translationstring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-22 15:17:08.000000 types-translationstring-1.4.0.0/types_translationstring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-03-22 15:17:08.000000 types-translationstring-1.4.0.0/types_translationstring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:17:08.000000 types-translationstring-1.4.0.0/types_translationstring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-22 15:17:08.000000 types-translationstring-1.4.0.0/types_translationstring.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:28.162014 types-translationstring-1.4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 15:17:27.000000 types-translationstring-1.4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:27.000000 types-translationstring-1.4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-20 15:17:28.162014 types-translationstring-1.4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:28.162014 types-translationstring-1.4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-20 15:17:27.000000 types-translationstring-1.4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:28.162014 types-translationstring-1.4.0.1/translationstring-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 15:17:27.000000 types-translationstring-1.4.0.1/translationstring-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-07-20 15:15:13.000000 types-translationstring-1.4.0.1/translationstring-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:28.162014 types-translationstring-1.4.0.1/types_translationstring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-07-20 15:17:28.000000 types-translationstring-1.4.0.1/types_translationstring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-20 15:17:28.000000 types-translationstring-1.4.0.1/types_translationstring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:28.000000 types-translationstring-1.4.0.1/types_translationstring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-20 15:17:28.000000 types-translationstring-1.4.0.1/types_translationstring.egg-info/top_level.txt
```

### Comparing `types-translationstring-1.4.0.0/PKG-INFO` & `types-translationstring-1.4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-translationstring
-Version: 1.4.0.0
+Version: 1.4.0.1
 Summary: Typing stubs for translationstring
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/translationstring.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `translationstring`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/translationstring. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ed466d3cc0b92f3acea04a94650b40476e51cb6`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-translationstring-1.4.0.0/setup.py` & `types-translationstring-1.4.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `translationstring`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/translationstring. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ed466d3cc0b92f3acea04a94650b40476e51cb6`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.4.0.0",
+      version="1.4.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/translationstring.md",
```

### Comparing `types-translationstring-1.4.0.0/translationstring-stubs/__init__.pyi` & `types-translationstring-1.4.0.1/translationstring-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-translationstring-1.4.0.0/types_translationstring.egg-info/PKG-INFO` & `types-translationstring-1.4.0.1/types_translationstring.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-translationstring
-Version: 1.4.0.0
+Version: 1.4.0.1
 Summary: Typing stubs for translationstring
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/translationstring.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `translationstring`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/translationstring. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `2ed466d3cc0b92f3acea04a94650b40476e51cb6`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

