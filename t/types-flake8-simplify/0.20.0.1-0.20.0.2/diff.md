# Comparing `tmp/types-flake8-simplify-0.20.0.1.tar.gz` & `tmp/types-flake8-simplify-0.20.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-simplify-0.20.0.1.tar", last modified: Wed May 10 15:20:10 2023, max compression
+gzip compressed data, was "types-flake8-simplify-0.20.0.2.tar", last modified: Thu Jul 20 15:17:12 2023, max compression
```

## Comparing `types-flake8-simplify-0.20.0.1.tar` & `types-flake8-simplify-0.20.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/flake8_simplify-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/flake8_simplify-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-10 15:19:44.000000 types-flake8-simplify-0.20.0.1/flake8_simplify-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:10.753699 types-flake8-simplify-0.20.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-10 15:20:09.000000 types-flake8-simplify-0.20.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:10.749699 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 15:20:10.000000 types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:12.813827 types-flake8-simplify-0.20.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-20 15:17:12.813827 types-flake8-simplify-0.20.0.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:12.809826 types-flake8-simplify-0.20.0.2/flake8_simplify-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/flake8_simplify-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 15:15:13.000000 types-flake8-simplify-0.20.0.2/flake8_simplify-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:12.813827 types-flake8-simplify-0.20.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:12.809826 types-flake8-simplify-0.20.0.2/types_flake8_simplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/types_flake8_simplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/types_flake8_simplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/types_flake8_simplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:17:12.000000 types-flake8-simplify-0.20.0.2/types_flake8_simplify.egg-info/top_level.txt
```

### Comparing `types-flake8-simplify-0.20.0.1/CHANGELOG.md` & `types-flake8-simplify-0.20.0.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.20.0.2 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.20.0.1 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 0.20.0.0 (2023-03-31)
 
 [stubsabot] Bump flake8-simplify to 0.20.* (#9993)
```

### Comparing `types-flake8-simplify-0.20.0.1/PKG-INFO` & `types-flake8-simplify-0.20.0.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-simplify
-Version: 0.20.0.1
+Version: 0.20.0.2
 Summary: Typing stubs for flake8-simplify
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-simplify.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-simplify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-simplify. All fixes for
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

### Comparing `types-flake8-simplify-0.20.0.1/setup.py` & `types-flake8-simplify-0.20.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-simplify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-simplify. All fixes for
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
-      version="0.20.0.1",
+      version="0.20.0.2",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-simplify.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['flake8_simplify-stubs'],
-      package_data={'flake8_simplify-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'flake8_simplify-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-flake8-simplify-0.20.0.1/types_flake8_simplify.egg-info/PKG-INFO` & `types-flake8-simplify-0.20.0.2/types_flake8_simplify.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-flake8-simplify
-Version: 0.20.0.1
+Version: 0.20.0.2
 Summary: Typing stubs for flake8-simplify
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-simplify.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-simplify`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-simplify. All fixes for
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

