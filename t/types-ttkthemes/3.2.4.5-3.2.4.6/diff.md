# Comparing `tmp/types-ttkthemes-3.2.4.5.tar.gz` & `tmp/types-ttkthemes-3.2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ttkthemes-3.2.4.5.tar", last modified: Tue Mar 28 12:33:28 2023, max compression
+gzip compressed data, was "types-ttkthemes-3.2.4.6.tar", last modified: Thu Jul 20 15:19:32 2023, max compression
```

## Comparing `types-ttkthemes-3.2.4.5.tar` & `types-ttkthemes-3.2.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:28.608924 types-ttkthemes-3.2.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-28 12:33:28.608924 types-ttkthemes-3.2.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:33:28.608924 types-ttkthemes-3.2.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:28.608924 types-ttkthemes-3.2.4.5/ttkthemes-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-28 12:32:25.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-28 12:32:25.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/_imgops.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-03-28 12:32:25.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-28 12:32:25.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/_widget.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-28 12:32:25.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/themed_style.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-28 12:32:25.000000 types-ttkthemes-3.2.4.5/ttkthemes-stubs/themed_tk.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:33:28.608924 types-ttkthemes-3.2.4.5/types_ttkthemes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/types_ttkthemes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/types_ttkthemes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/types_ttkthemes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-28 12:33:28.000000 types-ttkthemes-3.2.4.5/types_ttkthemes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:32.859586 types-ttkthemes-3.2.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:19:32.859586 types-ttkthemes-3.2.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:32.859586 types-ttkthemes-3.2.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:32.859586 types-ttkthemes-3.2.4.6/ttkthemes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 15:15:13.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 15:15:13.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/_imgops.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 15:15:13.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 15:15:13.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/_widget.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-20 15:15:13.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/themed_style.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-20 15:15:13.000000 types-ttkthemes-3.2.4.6/ttkthemes-stubs/themed_tk.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:32.859586 types-ttkthemes-3.2.4.6/types_ttkthemes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/types_ttkthemes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/types_ttkthemes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/types_ttkthemes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-20 15:19:32.000000 types-ttkthemes-3.2.4.6/types_ttkthemes.egg-info/top_level.txt
```

### Comparing `types-ttkthemes-3.2.4.5/CHANGELOG.md` & `types-ttkthemes-3.2.4.6/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.2.4.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.2.4.5 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 3.2.4.4 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-ttkthemes-3.2.4.5/PKG-INFO` & `types-ttkthemes-3.2.4.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ttkthemes
-Version: 3.2.4.5
+Version: 3.2.4.6
 Summary: Typing stubs for ttkthemes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ttkthemes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ttkthemes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ttkthemes. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-ttkthemes-3.2.4.5/setup.py` & `types-ttkthemes-3.2.4.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ttkthemes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ttkthemes. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.2.4.5",
+      version="3.2.4.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ttkthemes.md",
```

### Comparing `types-ttkthemes-3.2.4.5/ttkthemes-stubs/_widget.pyi` & `types-ttkthemes-3.2.4.6/ttkthemes-stubs/_widget.pyi`

 * *Files identical despite different names*

### Comparing `types-ttkthemes-3.2.4.5/ttkthemes-stubs/themed_tk.pyi` & `types-ttkthemes-3.2.4.6/ttkthemes-stubs/themed_tk.pyi`

 * *Files identical despite different names*

### Comparing `types-ttkthemes-3.2.4.5/types_ttkthemes.egg-info/PKG-INFO` & `types-ttkthemes-3.2.4.6/types_ttkthemes.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ttkthemes
-Version: 3.2.4.5
+Version: 3.2.4.6
 Summary: Typing stubs for ttkthemes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ttkthemes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ttkthemes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ttkthemes. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

