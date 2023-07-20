# Comparing `tmp/types-simplejson-3.19.0.1.tar.gz` & `tmp/types-simplejson-3.19.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-simplejson-3.19.0.1.tar", last modified: Wed May 10 15:22:40 2023, max compression
+gzip compressed data, was "types-simplejson-3.19.0.2.tar", last modified: Thu Jul 20 15:15:50 2023, max compression
```

## Comparing `types-simplejson-3.19.0.1.tar` & `types-simplejson-3.19.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:40.549222 types-simplejson-3.19.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-10 15:22:39.000000 types-simplejson-3.19.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:39.000000 types-simplejson-3.19.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:22:40.549222 types-simplejson-3.19.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:40.549222 types-simplejson-3.19.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-10 15:22:39.000000 types-simplejson-3.19.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:40.549222 types-simplejson-3.19.0.1/simplejson-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:22:39.000000 types-simplejson-3.19.0.1/simplejson-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-10 15:19:44.000000 types-simplejson-3.19.0.1/simplejson-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 15:19:44.000000 types-simplejson-3.19.0.1/simplejson-stubs/decoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-10 15:19:44.000000 types-simplejson-3.19.0.1/simplejson-stubs/encoder.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-10 15:19:44.000000 types-simplejson-3.19.0.1/simplejson-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-10 15:19:44.000000 types-simplejson-3.19.0.1/simplejson-stubs/raw_json.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-10 15:19:44.000000 types-simplejson-3.19.0.1/simplejson-stubs/scanner.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:40.549222 types-simplejson-3.19.0.1/types_simplejson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-10 15:22:40.000000 types-simplejson-3.19.0.1/types_simplejson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-10 15:22:40.000000 types-simplejson-3.19.0.1/types_simplejson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:40.000000 types-simplejson-3.19.0.1/types_simplejson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:22:40.000000 types-simplejson-3.19.0.1/types_simplejson.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:50.776833 types-simplejson-3.19.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-20 15:15:50.776833 types-simplejson-3.19.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:15:50.776833 types-simplejson-3.19.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:50.776833 types-simplejson-3.19.0.2/simplejson-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/simplejson-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-20 15:15:13.000000 types-simplejson-3.19.0.2/simplejson-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-07-20 15:15:13.000000 types-simplejson-3.19.0.2/simplejson-stubs/decoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 15:15:13.000000 types-simplejson-3.19.0.2/simplejson-stubs/encoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 15:15:13.000000 types-simplejson-3.19.0.2/simplejson-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 15:15:13.000000 types-simplejson-3.19.0.2/simplejson-stubs/raw_json.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-20 15:15:13.000000 types-simplejson-3.19.0.2/simplejson-stubs/scanner.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:50.776833 types-simplejson-3.19.0.2/types_simplejson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/types_simplejson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/types_simplejson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/types_simplejson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:50.000000 types-simplejson-3.19.0.2/types_simplejson.egg-info/top_level.txt
```

### Comparing `types-simplejson-3.19.0.1/CHANGELOG.md` & `types-simplejson-3.19.0.2/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.19.0.2 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.19.0.1 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 3.19.0.0 (2023-04-15)
 
 Bump simplejson to 3.19.* (#10049)
```

### Comparing `types-simplejson-3.19.0.1/PKG-INFO` & `types-simplejson-3.19.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-simplejson
-Version: 3.19.0.1
+Version: 3.19.0.2
 Summary: Typing stubs for simplejson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/simplejson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `simplejson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/simplejson. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-simplejson-3.19.0.1/setup.py` & `types-simplejson-3.19.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `simplejson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/simplejson. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.19.0.1",
+      version="3.19.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/simplejson.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['simplejson-stubs'],
-      package_data={'simplejson-stubs': ['__init__.pyi', 'decoder.pyi', 'encoder.pyi', 'errors.pyi', 'raw_json.pyi', 'scanner.pyi', 'METADATA.toml']},
+      package_data={'simplejson-stubs': ['__init__.pyi', 'decoder.pyi', 'encoder.pyi', 'errors.pyi', 'raw_json.pyi', 'scanner.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-simplejson-3.19.0.1/simplejson-stubs/__init__.pyi` & `types-simplejson-3.19.0.2/simplejson-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-simplejson-3.19.0.1/simplejson-stubs/errors.pyi` & `types-simplejson-3.19.0.2/simplejson-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-simplejson-3.19.0.1/types_simplejson.egg-info/PKG-INFO` & `types-simplejson-3.19.0.2/types_simplejson.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-simplejson
-Version: 3.19.0.1
+Version: 3.19.0.2
 Summary: Typing stubs for simplejson
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/simplejson.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `simplejson`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/simplejson. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

