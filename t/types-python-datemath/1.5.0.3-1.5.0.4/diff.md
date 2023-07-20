# Comparing `tmp/types-python-datemath-1.5.0.3.tar.gz` & `tmp/types-python-datemath-1.5.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-python-datemath-1.5.0.3.tar", last modified: Wed May 10 15:23:44 2023, max compression
+gzip compressed data, was "types-python-datemath-1.5.0.4.tar", last modified: Thu Jul 20 15:21:42 2023, max compression
```

## Comparing `types-python-datemath-1.5.0.3.tar` & `types-python-datemath-1.5.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/datemath-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/datemath-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-10 15:19:44.000000 types-python-datemath-1.5.0.3/datemath-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-10 15:19:44.000000 types-python-datemath-1.5.0.3/datemath-stubs/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:44.738738 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:23:44.000000 types-python-datemath-1.5.0.3/types_python_datemath.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:42.453151 types-python-datemath-1.5.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 15:21:41.000000 types-python-datemath-1.5.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:41.000000 types-python-datemath-1.5.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-20 15:21:42.453151 types-python-datemath-1.5.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:42.449151 types-python-datemath-1.5.0.4/datemath-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 15:21:41.000000 types-python-datemath-1.5.0.4/datemath-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-07-20 15:15:13.000000 types-python-datemath-1.5.0.4/datemath-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 15:15:13.000000 types-python-datemath-1.5.0.4/datemath-stubs/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:42.453151 types-python-datemath-1.5.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-20 15:21:41.000000 types-python-datemath-1.5.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:42.453151 types-python-datemath-1.5.0.4/types_python_datemath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-20 15:21:42.000000 types-python-datemath-1.5.0.4/types_python_datemath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 15:21:42.000000 types-python-datemath-1.5.0.4/types_python_datemath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:42.000000 types-python-datemath-1.5.0.4/types_python_datemath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:21:42.000000 types-python-datemath-1.5.0.4/types_python_datemath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:21:42.000000 types-python-datemath-1.5.0.4/types_python_datemath.egg-info/top_level.txt
```

### Comparing `types-python-datemath-1.5.0.3/CHANGELOG.md` & `types-python-datemath-1.5.0.4/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.5.0.4 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.5.0.3 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 1.5.0.2 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
```

### Comparing `types-python-datemath-1.5.0.3/PKG-INFO` & `types-python-datemath-1.5.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-datemath
-Version: 1.5.0.3
+Version: 1.5.0.4
 Summary: Typing stubs for python-datemath
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-datemath.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-datemath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-datemath. All fixes for
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

### Comparing `types-python-datemath-1.5.0.3/setup.py` & `types-python-datemath-1.5.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-datemath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-datemath. All fixes for
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
-      version="1.5.0.3",
+      version="1.5.0.4",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-datemath.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['arrow>=1.0.1'],
       packages=['datemath-stubs'],
-      package_data={'datemath-stubs': ['__init__.pyi', 'helpers.pyi', 'METADATA.toml']},
+      package_data={'datemath-stubs': ['__init__.pyi', 'helpers.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-python-datemath-1.5.0.3/types_python_datemath.egg-info/PKG-INFO` & `types-python-datemath-1.5.0.4/types_python_datemath.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-python-datemath
-Version: 1.5.0.3
+Version: 1.5.0.4
 Summary: Typing stubs for python-datemath
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/python-datemath.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `python-datemath`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/python-datemath. All fixes for
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

