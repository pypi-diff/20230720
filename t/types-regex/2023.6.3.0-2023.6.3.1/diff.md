# Comparing `tmp/types-regex-2023.6.3.0.tar.gz` & `tmp/types-regex-2023.6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-regex-2023.6.3.0.tar", last modified: Sun Jun  4 01:50:03 2023, max compression
+gzip compressed data, was "types-regex-2023.6.3.1.tar", last modified: Thu Jul 20 15:18:32 2023, max compression
```

## Comparing `types-regex-2023.6.3.0.tar` & `types-regex-2023.6.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:50:03.584844 types-regex-2023.6.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4881 2023-06-04 01:50:02.000000 types-regex-2023.6.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 01:50:02.000000 types-regex-2023.6.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-04 01:50:03.584844 types-regex-2023.6.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:50:03.584844 types-regex-2023.6.3.0/regex-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 01:50:02.000000 types-regex-2023.6.3.0/regex-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-04 01:49:49.000000 types-regex-2023.6.3.0/regex-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-04 01:49:49.000000 types-regex-2023.6.3.0/regex-stubs/_regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-04 01:49:49.000000 types-regex-2023.6.3.0/regex-stubs/_regex_core.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-06-04 01:49:49.000000 types-regex-2023.6.3.0/regex-stubs/regex.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 01:50:03.584844 types-regex-2023.6.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-06-04 01:50:02.000000 types-regex-2023.6.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 01:50:03.584844 types-regex-2023.6.3.0/types_regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-04 01:50:03.000000 types-regex-2023.6.3.0/types_regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-04 01:50:03.000000 types-regex-2023.6.3.0/types_regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 01:50:03.000000 types-regex-2023.6.3.0/types_regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 01:50:03.000000 types-regex-2023.6.3.0/types_regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:32.022828 types-regex-2023.6.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-20 15:18:32.022828 types-regex-2023.6.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:32.022828 types-regex-2023.6.3.1/regex-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/regex-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:13.000000 types-regex-2023.6.3.1/regex-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 15:15:13.000000 types-regex-2023.6.3.1/regex-stubs/_regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-20 15:15:13.000000 types-regex-2023.6.3.1/regex-stubs/_regex_core.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19263 2023-07-20 15:15:13.000000 types-regex-2023.6.3.1/regex-stubs/regex.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:32.022828 types-regex-2023.6.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:32.022828 types-regex-2023.6.3.1/types_regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/types_regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/types_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/types_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 15:18:31.000000 types-regex-2023.6.3.1/types_regex.egg-info/top_level.txt
```

### Comparing `types-regex-2023.6.3.0/CHANGELOG.md` & `types-regex-2023.6.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2023.6.3.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2023.6.3.0 (2023-06-04)
 
 [stubsabot] Bump regex to 2023.6.3 (#10252)
 
 Release: https://pypi.org/pypi/regex/2023.6.3
 Homepage: https://github.com/mrabarnett/mrab-regex
 Diff: https://github.com/mrabarnett/mrab-regex/compare/2023.5.5...2023.6.3
```

### Comparing `types-regex-2023.6.3.0/PKG-INFO` & `types-regex-2023.6.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2023.6.3.0
+Version: 2023.6.3.1
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d5555b10180b8077b0fa74ba7737d2f38c96185d`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-regex-2023.6.3.0/regex-stubs/_regex.pyi` & `types-regex-2023.6.3.1/regex-stubs/_regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.6.3.0/regex-stubs/_regex_core.pyi` & `types-regex-2023.6.3.1/regex-stubs/_regex_core.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.6.3.0/regex-stubs/regex.pyi` & `types-regex-2023.6.3.1/regex-stubs/regex.pyi`

 * *Files identical despite different names*

### Comparing `types-regex-2023.6.3.0/setup.py` & `types-regex-2023.6.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d5555b10180b8077b0fa74ba7737d2f38c96185d`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2023.6.3.0",
+      version="2023.6.3.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md",
```

### Comparing `types-regex-2023.6.3.0/types_regex.egg-info/PKG-INFO` & `types-regex-2023.6.3.1/types_regex.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-regex
-Version: 2023.6.3.0
+Version: 2023.6.3.1
 Summary: Typing stubs for regex
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/regex.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `regex`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/regex. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d5555b10180b8077b0fa74ba7737d2f38c96185d`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

