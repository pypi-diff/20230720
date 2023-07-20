# Comparing `tmp/types-jmespath-1.0.2.6.tar.gz` & `tmp/types-jmespath-1.0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-jmespath-1.0.2.6.tar", last modified: Mon Mar 27 18:24:15 2023, max compression
+gzip compressed data, was "types-jmespath-1.0.2.7.tar", last modified: Thu Jul 20 15:18:41 2023, max compression
```

## Comparing `types-jmespath-1.0.2.6.tar` & `types-jmespath-1.0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:15.583090 types-jmespath-1.0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-27 18:24:14.000000 types-jmespath-1.0.2.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:24:14.000000 types-jmespath-1.0.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:24:15.583090 types-jmespath-1.0.2.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:15.583090 types-jmespath-1.0.2.6/jmespath-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:24:14.000000 types-jmespath-1.0.2.6/jmespath-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/ast.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/functions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/lexer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-03-27 18:21:24.000000 types-jmespath-1.0.2.6/jmespath-stubs/visitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:24:15.583090 types-jmespath-1.0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-27 18:24:14.000000 types-jmespath-1.0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:24:15.583090 types-jmespath-1.0.2.6/types_jmespath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:24:15.000000 types-jmespath-1.0.2.6/types_jmespath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-03-27 18:24:15.000000 types-jmespath-1.0.2.6/types_jmespath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:24:15.000000 types-jmespath-1.0.2.6/types_jmespath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:24:15.000000 types-jmespath-1.0.2.6/types_jmespath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:41.234943 types-jmespath-1.0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-20 15:18:40.000000 types-jmespath-1.0.2.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:40.000000 types-jmespath-1.0.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:18:41.230943 types-jmespath-1.0.2.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:41.230943 types-jmespath-1.0.2.7/jmespath-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-20 15:18:40.000000 types-jmespath-1.0.2.7/jmespath-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/ast.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/lexer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-07-20 15:15:13.000000 types-jmespath-1.0.2.7/jmespath-stubs/visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:41.234943 types-jmespath-1.0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-20 15:18:40.000000 types-jmespath-1.0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:41.230943 types-jmespath-1.0.2.7/types_jmespath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:18:41.000000 types-jmespath-1.0.2.7/types_jmespath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-20 15:18:41.000000 types-jmespath-1.0.2.7/types_jmespath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:41.000000 types-jmespath-1.0.2.7/types_jmespath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:18:41.000000 types-jmespath-1.0.2.7/types_jmespath.egg-info/top_level.txt
```

### Comparing `types-jmespath-1.0.2.6/CHANGELOG.md` & `types-jmespath-1.0.2.7/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.0.2.7 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.0.2.6 (2023-03-27)
 
 Add defaults for third-party stubs I-L (#9955)
 
 ## 1.0.2.5 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-jmespath-1.0.2.6/PKG-INFO` & `types-jmespath-1.0.2.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jmespath
-Version: 1.0.2.6
+Version: 1.0.2.7
 Summary: Typing stubs for jmespath
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/jmespath.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `jmespath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/jmespath. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-jmespath-1.0.2.6/jmespath-stubs/ast.pyi` & `types-jmespath-1.0.2.7/jmespath-stubs/ast.pyi`

 * *Files identical despite different names*

### Comparing `types-jmespath-1.0.2.6/jmespath-stubs/exceptions.pyi` & `types-jmespath-1.0.2.7/jmespath-stubs/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `types-jmespath-1.0.2.6/jmespath-stubs/functions.pyi` & `types-jmespath-1.0.2.7/jmespath-stubs/functions.pyi`

 * *Files identical despite different names*

### Comparing `types-jmespath-1.0.2.6/jmespath-stubs/lexer.pyi` & `types-jmespath-1.0.2.7/jmespath-stubs/lexer.pyi`

 * *Files identical despite different names*

### Comparing `types-jmespath-1.0.2.6/jmespath-stubs/parser.pyi` & `types-jmespath-1.0.2.7/jmespath-stubs/parser.pyi`

 * *Files identical despite different names*

### Comparing `types-jmespath-1.0.2.6/jmespath-stubs/visitor.pyi` & `types-jmespath-1.0.2.7/jmespath-stubs/visitor.pyi`

 * *Files identical despite different names*

### Comparing `types-jmespath-1.0.2.6/setup.py` & `types-jmespath-1.0.2.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `jmespath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/jmespath. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.0.2.6",
+      version="1.0.2.7",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/jmespath.md",
```

### Comparing `types-jmespath-1.0.2.6/types_jmespath.egg-info/PKG-INFO` & `types-jmespath-1.0.2.7/types_jmespath.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-jmespath
-Version: 1.0.2.6
+Version: 1.0.2.7
 Summary: Typing stubs for jmespath
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/jmespath.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `jmespath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/jmespath. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

