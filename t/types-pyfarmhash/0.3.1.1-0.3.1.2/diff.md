# Comparing `tmp/types-pyfarmhash-0.3.1.1.tar.gz` & `tmp/types-pyfarmhash-0.3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyfarmhash-0.3.1.1.tar", last modified: Tue Feb 21 01:29:11 2023, max compression
+gzip compressed data, was "types-pyfarmhash-0.3.1.2.tar", last modified: Thu Jul 20 15:17:57 2023, max compression
```

## Comparing `types-pyfarmhash-0.3.1.1.tar` & `types-pyfarmhash-0.3.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:11.723143 types-pyfarmhash-0.3.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:29:11.719143 types-pyfarmhash-0.3.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:11.719143 types-pyfarmhash-0.3.1.1/farmhash-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/farmhash-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/farmhash-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 01:29:11.723143 types-pyfarmhash-0.3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 01:29:11.719143 types-pyfarmhash-0.3.1.1/types_pyfarmhash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/types_pyfarmhash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/types_pyfarmhash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/types_pyfarmhash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-21 01:29:11.000000 types-pyfarmhash-0.3.1.1/types_pyfarmhash.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:57.146372 types-pyfarmhash-0.3.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-20 15:17:56.000000 types-pyfarmhash-0.3.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:56.000000 types-pyfarmhash-0.3.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 15:17:57.146372 types-pyfarmhash-0.3.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:57.146372 types-pyfarmhash-0.3.1.2/farmhash-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 15:17:56.000000 types-pyfarmhash-0.3.1.2/farmhash-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-20 15:17:56.000000 types-pyfarmhash-0.3.1.2/farmhash-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:57.146372 types-pyfarmhash-0.3.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-07-20 15:17:56.000000 types-pyfarmhash-0.3.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:57.146372 types-pyfarmhash-0.3.1.2/types_pyfarmhash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 15:17:57.000000 types-pyfarmhash-0.3.1.2/types_pyfarmhash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 15:17:57.000000 types-pyfarmhash-0.3.1.2/types_pyfarmhash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:57.000000 types-pyfarmhash-0.3.1.2/types_pyfarmhash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:17:57.000000 types-pyfarmhash-0.3.1.2/types_pyfarmhash.egg-info/top_level.txt
```

### Comparing `types-pyfarmhash-0.3.1.1/PKG-INFO` & `types-pyfarmhash-0.3.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyfarmhash
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: Typing stubs for pyfarmhash
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyfarmhash.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyfarmhash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyfarmhash. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-pyfarmhash-0.3.1.1/setup.py` & `types-pyfarmhash-0.3.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyfarmhash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyfarmhash. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="0.3.1.1",
+      version="0.3.1.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyfarmhash.md",
```

### Comparing `types-pyfarmhash-0.3.1.1/types_pyfarmhash.egg-info/PKG-INFO` & `types-pyfarmhash-0.3.1.2/types_pyfarmhash.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyfarmhash
-Version: 0.3.1.1
+Version: 0.3.1.2
 Summary: Typing stubs for pyfarmhash
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyfarmhash.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyfarmhash`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyfarmhash. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `880c0da4045cd5ff2c29b73429629adf27e49d50`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

