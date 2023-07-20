# Comparing `tmp/types-stdlib-list-0.8.3.3.tar.gz` & `tmp/types-stdlib-list-0.8.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-stdlib-list-0.8.3.3.tar", last modified: Fri Jun 23 06:22:34 2023, max compression
+gzip compressed data, was "types-stdlib-list-0.8.3.4.tar", last modified: Thu Jul 20 15:16:27 2023, max compression
```

## Comparing `types-stdlib-list-0.8.3.3.tar` & `types-stdlib-list-0.8.3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:22:34.071557 types-stdlib-list-0.8.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-23 06:22:32.000000 types-stdlib-list-0.8.3.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 06:22:32.000000 types-stdlib-list-0.8.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-23 06:22:34.071557 types-stdlib-list-0.8.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:22:34.071557 types-stdlib-list-0.8.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-23 06:22:32.000000 types-stdlib-list-0.8.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:22:34.067557 types-stdlib-list-0.8.3.3/stdlib_list-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 06:22:32.000000 types-stdlib-list-0.8.3.3/stdlib_list-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-23 06:22:19.000000 types-stdlib-list-0.8.3.3/stdlib_list-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 06:22:19.000000 types-stdlib-list-0.8.3.3/stdlib_list-stubs/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-23 06:22:19.000000 types-stdlib-list-0.8.3.3/stdlib_list-stubs/base.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:22:34.071557 types-stdlib-list-0.8.3.3/types_stdlib_list.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-23 06:22:34.000000 types-stdlib-list-0.8.3.3/types_stdlib_list.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-23 06:22:34.000000 types-stdlib-list-0.8.3.3/types_stdlib_list.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:22:34.000000 types-stdlib-list-0.8.3.3/types_stdlib_list.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 06:22:34.000000 types-stdlib-list-0.8.3.3/types_stdlib_list.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:27.537282 types-stdlib-list-0.8.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-20 15:16:26.000000 types-stdlib-list-0.8.3.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:26.000000 types-stdlib-list-0.8.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-20 15:16:27.533282 types-stdlib-list-0.8.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:27.537282 types-stdlib-list-0.8.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 15:16:26.000000 types-stdlib-list-0.8.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:27.533282 types-stdlib-list-0.8.3.4/stdlib_list-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 15:16:26.000000 types-stdlib-list-0.8.3.4/stdlib_list-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 15:15:13.000000 types-stdlib-list-0.8.3.4/stdlib_list-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 15:15:13.000000 types-stdlib-list-0.8.3.4/stdlib_list-stubs/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-20 15:15:13.000000 types-stdlib-list-0.8.3.4/stdlib_list-stubs/base.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:27.533282 types-stdlib-list-0.8.3.4/types_stdlib_list.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-20 15:16:27.000000 types-stdlib-list-0.8.3.4/types_stdlib_list.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 15:16:27.000000 types-stdlib-list-0.8.3.4/types_stdlib_list.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:27.000000 types-stdlib-list-0.8.3.4/types_stdlib_list.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 15:16:27.000000 types-stdlib-list-0.8.3.4/types_stdlib_list.egg-info/top_level.txt
```

### Comparing `types-stdlib-list-0.8.3.3/CHANGELOG.md` & `types-stdlib-list-0.8.3.4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.8.3.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.8.3.3 (2023-06-23)
 
 [stubsabot] Mark stdlib-list as obsolete since 0.9.0 (#10348)
 
 Release: https://pypi.org/pypi/stdlib-list/0.9.0
 Homepage: https://pypi.org/project/stdlib-list/
 Diff: https://github.com/pypi/stdlib-list/compare/v0.8.0...v0.9.0
```

### Comparing `types-stdlib-list-0.8.3.3/PKG-INFO` & `types-stdlib-list-0.8.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-stdlib-list
-Version: 0.8.3.3
+Version: 0.8.3.4
 Summary: Typing stubs for stdlib-list
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/stdlib-list.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,10 +27,10 @@
 
 *Note:* The `stdlib-list` package includes type annotations or type stubs
 since version 0.9.0. Please uninstall the `types-stdlib-list`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c402107f8afd57a1916ba116e6aafb5bf7a663f3` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-stdlib-list-0.8.3.3/setup.py` & `types-stdlib-list-0.8.3.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 
 *Note:* The `stdlib-list` package includes type annotations or type stubs
 since version 0.9.0. Please uninstall the `types-stdlib-list`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c402107f8afd57a1916ba116e6aafb5bf7a663f3` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.8.3.3",
+      version="0.8.3.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/stdlib-list.md",
```

### Comparing `types-stdlib-list-0.8.3.3/types_stdlib_list.egg-info/PKG-INFO` & `types-stdlib-list-0.8.3.4/types_stdlib_list.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-stdlib-list
-Version: 0.8.3.3
+Version: 0.8.3.4
 Summary: Typing stubs for stdlib-list
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/stdlib-list.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,10 +27,10 @@
 
 *Note:* The `stdlib-list` package includes type annotations or type stubs
 since version 0.9.0. Please uninstall the `types-stdlib-list`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `c402107f8afd57a1916ba116e6aafb5bf7a663f3` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

