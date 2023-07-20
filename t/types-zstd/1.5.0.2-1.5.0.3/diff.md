# Comparing `tmp/types-zstd-1.5.0.2.tar.gz` & `tmp/types-zstd-1.5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-zstd-1.5.0.2.tar", last modified: Fri Mar 24 12:29:08 2023, max compression
+gzip compressed data, was "types-zstd-1.5.0.3.tar", last modified: Thu Jul 20 15:17:54 2023, max compression
```

## Comparing `types-zstd-1.5.0.2.tar` & `types-zstd-1.5.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:29:08.448746 types-zstd-1.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-24 12:29:07.000000 types-zstd-1.5.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-24 12:29:07.000000 types-zstd-1.5.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-24 12:29:08.448746 types-zstd-1.5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 12:29:08.448746 types-zstd-1.5.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-24 12:29:07.000000 types-zstd-1.5.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:29:08.448746 types-zstd-1.5.0.2/types_zstd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-03-24 12:29:08.000000 types-zstd-1.5.0.2/types_zstd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-24 12:29:08.000000 types-zstd-1.5.0.2/types_zstd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 12:29:08.000000 types-zstd-1.5.0.2/types_zstd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-24 12:29:08.000000 types-zstd-1.5.0.2/types_zstd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:29:08.448746 types-zstd-1.5.0.2/zstd-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-24 12:29:07.000000 types-zstd-1.5.0.2/zstd-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-03-24 12:29:07.000000 types-zstd-1.5.0.2/zstd-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:54.306335 types-zstd-1.5.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-20 15:17:53.000000 types-zstd-1.5.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:53.000000 types-zstd-1.5.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 15:17:54.306335 types-zstd-1.5.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:54.306335 types-zstd-1.5.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-07-20 15:17:53.000000 types-zstd-1.5.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:54.306335 types-zstd-1.5.0.3/types_zstd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 15:17:54.000000 types-zstd-1.5.0.3/types_zstd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-20 15:17:54.000000 types-zstd-1.5.0.3/types_zstd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:54.000000 types-zstd-1.5.0.3/types_zstd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 15:17:54.000000 types-zstd-1.5.0.3/types_zstd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:54.306335 types-zstd-1.5.0.3/zstd-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 15:17:53.000000 types-zstd-1.5.0.3/zstd-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 15:17:53.000000 types-zstd-1.5.0.3/zstd-stubs/__init__.pyi
```

### Comparing `types-zstd-1.5.0.2/PKG-INFO` & `types-zstd-1.5.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-zstd
-Version: 1.5.0.2
+Version: 1.5.0.3
 Summary: Typing stubs for zstd
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/zstd.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `zstd`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/zstd. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0bb57fcbc63a4e2f15b70e7321b79abd76391d92`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-zstd-1.5.0.2/setup.py` & `types-zstd-1.5.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `zstd`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/zstd. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0bb57fcbc63a4e2f15b70e7321b79abd76391d92`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.5.0.2",
+      version="1.5.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/zstd.md",
```

### Comparing `types-zstd-1.5.0.2/types_zstd.egg-info/PKG-INFO` & `types-zstd-1.5.0.3/types_zstd.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-zstd
-Version: 1.5.0.2
+Version: 1.5.0.3
 Summary: Typing stubs for zstd
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/zstd.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `zstd`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/zstd. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0bb57fcbc63a4e2f15b70e7321b79abd76391d92`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-zstd-1.5.0.2/zstd-stubs/__init__.pyi` & `types-zstd-1.5.0.3/zstd-stubs/__init__.pyi`

 * *Files identical despite different names*

