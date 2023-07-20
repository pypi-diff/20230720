# Comparing `tmp/types-bleach-6.0.0.3.tar.gz` & `tmp/types-bleach-6.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-bleach-6.0.0.3.tar", last modified: Wed May 10 15:21:33 2023, max compression
+gzip compressed data, was "types-bleach-6.0.0.4.tar", last modified: Thu Jul 20 15:16:32 2023, max compression
```

## Comparing `types-bleach-6.0.0.3.tar` & `types-bleach-6.0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/bleach-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/bleach-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/callbacks.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/css_sanitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/html5lib_shim.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/linkifier.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-10 15:19:44.000000 types-bleach-6.0.0.3/bleach-stubs/sanitizer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-10 15:21:32.000000 types-bleach-6.0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:33.551614 types-bleach-6.0.0.3/types_bleach.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:21:33.000000 types-bleach-6.0.0.3/types_bleach.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:32.201339 types-bleach-6.0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-20 15:16:31.000000 types-bleach-6.0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:31.000000 types-bleach-6.0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-20 15:16:32.197338 types-bleach-6.0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:32.197338 types-bleach-6.0.0.4/bleach-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 15:16:31.000000 types-bleach-6.0.0.4/bleach-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-20 15:15:13.000000 types-bleach-6.0.0.4/bleach-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-20 15:15:13.000000 types-bleach-6.0.0.4/bleach-stubs/callbacks.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 15:15:13.000000 types-bleach-6.0.0.4/bleach-stubs/css_sanitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-20 15:15:13.000000 types-bleach-6.0.0.4/bleach-stubs/html5lib_shim.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-20 15:15:13.000000 types-bleach-6.0.0.4/bleach-stubs/linkifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-07-20 15:15:13.000000 types-bleach-6.0.0.4/bleach-stubs/sanitizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:32.201339 types-bleach-6.0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-20 15:16:31.000000 types-bleach-6.0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:32.197338 types-bleach-6.0.0.4/types_bleach.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-20 15:16:32.000000 types-bleach-6.0.0.4/types_bleach.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 15:16:32.000000 types-bleach-6.0.0.4/types_bleach.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:32.000000 types-bleach-6.0.0.4/types_bleach.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:16:32.000000 types-bleach-6.0.0.4/types_bleach.egg-info/top_level.txt
```

### Comparing `types-bleach-6.0.0.3/CHANGELOG.md` & `types-bleach-6.0.0.4/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 6.0.0.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 6.0.0.3 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 6.0.0.2 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
```

### Comparing `types-bleach-6.0.0.3/PKG-INFO` & `types-bleach-6.0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-bleach
-Version: 6.0.0.3
+Version: 6.0.0.4
 Summary: Typing stubs for bleach
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/bleach.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `bleach`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/bleach. All fixes for
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

### Comparing `types-bleach-6.0.0.3/bleach-stubs/__init__.pyi` & `types-bleach-6.0.0.4/bleach-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.3/bleach-stubs/html5lib_shim.pyi` & `types-bleach-6.0.0.4/bleach-stubs/html5lib_shim.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.3/bleach-stubs/linkifier.pyi` & `types-bleach-6.0.0.4/bleach-stubs/linkifier.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.3/bleach-stubs/sanitizer.pyi` & `types-bleach-6.0.0.4/bleach-stubs/sanitizer.pyi`

 * *Files identical despite different names*

### Comparing `types-bleach-6.0.0.3/setup.py` & `types-bleach-6.0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `bleach`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/bleach. All fixes for
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
-      version="6.0.0.3",
+      version="6.0.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/bleach.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['bleach-stubs'],
-      package_data={'bleach-stubs': ['__init__.pyi', 'callbacks.pyi', 'css_sanitizer.pyi', 'html5lib_shim.pyi', 'linkifier.pyi', 'sanitizer.pyi', 'METADATA.toml']},
+      package_data={'bleach-stubs': ['__init__.pyi', 'callbacks.pyi', 'css_sanitizer.pyi', 'html5lib_shim.pyi', 'linkifier.pyi', 'sanitizer.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-bleach-6.0.0.3/types_bleach.egg-info/PKG-INFO` & `types-bleach-6.0.0.4/types_bleach.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-bleach
-Version: 6.0.0.3
+Version: 6.0.0.4
 Summary: Typing stubs for bleach
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/bleach.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `bleach`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/bleach. All fixes for
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

