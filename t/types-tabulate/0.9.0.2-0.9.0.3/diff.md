# Comparing `tmp/types-tabulate-0.9.0.2.tar.gz` & `tmp/types-tabulate-0.9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tabulate-0.9.0.2.tar", last modified: Tue Mar 28 12:32:53 2023, max compression
+gzip compressed data, was "types-tabulate-0.9.0.3.tar", last modified: Thu Jul 20 15:18:38 2023, max compression
```

## Comparing `types-tabulate-0.9.0.2.tar` & `types-tabulate-0.9.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:53.781422 types-tabulate-0.9.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-28 12:32:53.781422 types-tabulate-0.9.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:32:53.785422 types-tabulate-0.9.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:53.781422 types-tabulate-0.9.0.2/tabulate-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/tabulate-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-03-28 12:32:25.000000 types-tabulate-0.9.0.2/tabulate-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-28 12:32:25.000000 types-tabulate-0.9.0.2/tabulate-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:53.781422 types-tabulate-0.9.0.2/types_tabulate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/types_tabulate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/types_tabulate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/types_tabulate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 12:32:53.000000 types-tabulate-0.9.0.2/types_tabulate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:38.122904 types-tabulate-0.9.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-20 15:18:37.000000 types-tabulate-0.9.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:37.000000 types-tabulate-0.9.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:18:38.122904 types-tabulate-0.9.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:38.122904 types-tabulate-0.9.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-20 15:18:37.000000 types-tabulate-0.9.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:38.122904 types-tabulate-0.9.0.3/tabulate-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 15:18:37.000000 types-tabulate-0.9.0.3/tabulate-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-20 15:15:13.000000 types-tabulate-0.9.0.3/tabulate-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-20 15:15:13.000000 types-tabulate-0.9.0.3/tabulate-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:38.122904 types-tabulate-0.9.0.3/types_tabulate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:18:38.000000 types-tabulate-0.9.0.3/types_tabulate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-20 15:18:38.000000 types-tabulate-0.9.0.3/types_tabulate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:38.000000 types-tabulate-0.9.0.3/types_tabulate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:18:38.000000 types-tabulate-0.9.0.3/types_tabulate.egg-info/top_level.txt
```

### Comparing `types-tabulate-0.9.0.2/CHANGELOG.md` & `types-tabulate-0.9.0.3/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.9.0.3 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.9.0.2 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 0.9.0.1 (2023-02-21)
 
 Add missing symbols to `tabulate` (#9781)
```

### Comparing `types-tabulate-0.9.0.2/PKG-INFO` & `types-tabulate-0.9.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tabulate
-Version: 0.9.0.2
+Version: 0.9.0.3
 Summary: Typing stubs for tabulate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tabulate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tabulate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tabulate. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-tabulate-0.9.0.2/setup.py` & `types-tabulate-0.9.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tabulate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tabulate. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.0.2",
+      version="0.9.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tabulate.md",
```

### Comparing `types-tabulate-0.9.0.2/tabulate-stubs/__init__.pyi` & `types-tabulate-0.9.0.3/tabulate-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tabulate-0.9.0.2/types_tabulate.egg-info/PKG-INFO` & `types-tabulate-0.9.0.3/types_tabulate.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tabulate
-Version: 0.9.0.2
+Version: 0.9.0.3
 Summary: Typing stubs for tabulate
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tabulate.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tabulate`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tabulate. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

