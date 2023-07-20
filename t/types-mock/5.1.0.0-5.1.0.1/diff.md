# Comparing `tmp/types-mock-5.1.0.0.tar.gz` & `tmp/types-mock-5.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-mock-5.1.0.0.tar", last modified: Wed Jul 19 12:29:46 2023, max compression
+gzip compressed data, was "types-mock-5.1.0.1.tar", last modified: Thu Jul 20 15:18:47 2023, max compression
```

## Comparing `types-mock-5.1.0.0.tar` & `types-mock-5.1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:46.787357 types-mock-5.1.0.0/mock-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/mock-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-19 12:29:24.000000 types-mock-5.1.0.0/mock-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-19 12:29:24.000000 types-mock-5.1.0.0/mock-stubs/backports.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-07-19 12:29:24.000000 types-mock-5.1.0.0/mock-stubs/mock.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:29:46.791357 types-mock-5.1.0.0/types_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-19 12:29:46.000000 types-mock-5.1.0.0/types_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:47.743022 types-mock-5.1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-20 15:18:46.000000 types-mock-5.1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:46.000000 types-mock-5.1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 15:18:47.739022 types-mock-5.1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:47.739022 types-mock-5.1.0.1/mock-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 15:18:46.000000 types-mock-5.1.0.1/mock-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-20 15:15:13.000000 types-mock-5.1.0.1/mock-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-20 15:15:13.000000 types-mock-5.1.0.1/mock-stubs/backports.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13541 2023-07-20 15:15:13.000000 types-mock-5.1.0.1/mock-stubs/mock.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:47.743022 types-mock-5.1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-07-20 15:18:46.000000 types-mock-5.1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:47.739022 types-mock-5.1.0.1/types_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 15:18:47.000000 types-mock-5.1.0.1/types_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 15:18:47.000000 types-mock-5.1.0.1/types_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:47.000000 types-mock-5.1.0.1/types_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 15:18:47.000000 types-mock-5.1.0.1/types_mock.egg-info/top_level.txt
```

### Comparing `types-mock-5.1.0.0/CHANGELOG.md` & `types-mock-5.1.0.1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 5.1.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 5.1.0.0 (2023-07-19)
 
 Add a more precise signature for `AsyncMock.reset_mock()` (#10481)
 
 Update `mock` to `5.1.*` (#10472)
 
 ## 5.0.0.7 (2023-06-21)
```

### Comparing `types-mock-5.1.0.0/PKG-INFO` & `types-mock-5.1.0.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mock
-Version: 5.1.0.0
+Version: 5.1.0.1
 Summary: Typing stubs for mock
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mock`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

### Comparing `types-mock-5.1.0.0/mock-stubs/mock.pyi` & `types-mock-5.1.0.1/mock-stubs/mock.pyi`

 * *Files identical despite different names*

### Comparing `types-mock-5.1.0.0/setup.py` & `types-mock-5.1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mock`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="5.1.0.0",
+      version="5.1.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md",
```

### Comparing `types-mock-5.1.0.0/types_mock.egg-info/PKG-INFO` & `types-mock-5.1.0.1/types_mock.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mock
-Version: 5.1.0.0
+Version: 5.1.0.1
 Summary: Typing stubs for mock
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mock.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mock`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mock. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `032f9195f9e3788a6e5c7ecb086f173a3ac92a95` and was tested
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
 with mypy 1.4.1, pyright 1.1.318, and
 pytype 2023.6.16.
```

