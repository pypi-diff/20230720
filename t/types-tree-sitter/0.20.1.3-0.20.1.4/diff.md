# Comparing `tmp/types-tree-sitter-0.20.1.3.tar.gz` & `tmp/types-tree-sitter-0.20.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-tree-sitter-0.20.1.3.tar", last modified: Tue Mar 28 12:32:37 2023, max compression
+gzip compressed data, was "types-tree-sitter-0.20.1.4.tar", last modified: Thu Jul 20 15:15:47 2023, max compression
```

## Comparing `types-tree-sitter-0.20.1.3.tar` & `types-tree-sitter-0.20.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:37.845621 types-tree-sitter-0.20.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-28 12:32:36.000000 types-tree-sitter-0.20.1.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-28 12:32:36.000000 types-tree-sitter-0.20.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-28 12:32:37.845621 types-tree-sitter-0.20.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 12:32:37.845621 types-tree-sitter-0.20.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-28 12:32:36.000000 types-tree-sitter-0.20.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:37.845621 types-tree-sitter-0.20.1.3/tree_sitter-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-28 12:32:36.000000 types-tree-sitter-0.20.1.3/tree_sitter-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-03-28 12:32:25.000000 types-tree-sitter-0.20.1.3/tree_sitter-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-28 12:32:25.000000 types-tree-sitter-0.20.1.3/tree_sitter-stubs/binding.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 12:32:37.845621 types-tree-sitter-0.20.1.3/types_tree_sitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-28 12:32:37.000000 types-tree-sitter-0.20.1.3/types_tree_sitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-28 12:32:37.000000 types-tree-sitter-0.20.1.3/types_tree_sitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 12:32:37.000000 types-tree-sitter-0.20.1.3/types_tree_sitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 12:32:37.000000 types-tree-sitter-0.20.1.3/types_tree_sitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:47.848797 types-tree-sitter-0.20.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-20 15:15:47.848797 types-tree-sitter-0.20.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:47.848797 types-tree-sitter-0.20.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:47.848797 types-tree-sitter-0.20.1.4/tree_sitter-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/tree_sitter-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-20 15:15:13.000000 types-tree-sitter-0.20.1.4/tree_sitter-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-20 15:15:13.000000 types-tree-sitter-0.20.1.4/tree_sitter-stubs/binding.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:47.848797 types-tree-sitter-0.20.1.4/types_tree_sitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/types_tree_sitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/types_tree_sitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/types_tree_sitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:15:47.000000 types-tree-sitter-0.20.1.4/types_tree_sitter.egg-info/top_level.txt
```

### Comparing `types-tree-sitter-0.20.1.3/CHANGELOG.md` & `types-tree-sitter-0.20.1.4/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.20.1.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.20.1.3 (2023-03-28)
 
 Add defaults for third-party stubs Q-T (#9959)
 
 ## 0.20.1.2 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-tree-sitter-0.20.1.3/PKG-INFO` & `types-tree-sitter-0.20.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tree-sitter
-Version: 0.20.1.3
+Version: 0.20.1.4
 Summary: Typing stubs for tree-sitter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tree-sitter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tree-sitter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tree-sitter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-tree-sitter-0.20.1.3/setup.py` & `types-tree-sitter-0.20.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tree-sitter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tree-sitter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.20.1.3",
+      version="0.20.1.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tree-sitter.md",
```

### Comparing `types-tree-sitter-0.20.1.3/tree_sitter-stubs/__init__.pyi` & `types-tree-sitter-0.20.1.4/tree_sitter-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-tree-sitter-0.20.1.3/tree_sitter-stubs/binding.pyi` & `types-tree-sitter-0.20.1.4/tree_sitter-stubs/binding.pyi`

 * *Files identical despite different names*

### Comparing `types-tree-sitter-0.20.1.3/types_tree_sitter.egg-info/PKG-INFO` & `types-tree-sitter-0.20.1.4/types_tree_sitter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-tree-sitter
-Version: 0.20.1.3
+Version: 0.20.1.4
 Summary: Typing stubs for tree-sitter
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/tree-sitter.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `tree-sitter`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/tree-sitter. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6b485a882325829dcbb6dd1d59c5e54b0bcfece1`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

