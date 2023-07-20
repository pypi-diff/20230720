# Comparing `tmp/types-pyflakes-3.0.0.4.tar.gz` & `tmp/types-pyflakes-3.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyflakes-3.0.0.4.tar", last modified: Wed May 10 15:22:14 2023, max compression
+gzip compressed data, was "types-pyflakes-3.0.0.5.tar", last modified: Thu Jul 20 15:20:35 2023, max compression
```

## Comparing `types-pyflakes-3.0.0.4.tar` & `types-pyflakes-3.0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:14.688607 types-pyflakes-3.0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:22:14.684607 types-pyflakes-3.0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:14.684607 types-pyflakes-3.0.0.4/pyflakes-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/checker.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/messages.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-10 15:19:44.000000 types-pyflakes-3.0.0.4/pyflakes-stubs/reporter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:22:14.688607 types-pyflakes-3.0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-10 15:22:13.000000 types-pyflakes-3.0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:22:14.684607 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 15:22:14.000000 types-pyflakes-3.0.0.4/types_pyflakes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/pyflakes-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14441 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/checker.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/messages.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 15:15:13.000000 types-pyflakes-3.0.0.5/pyflakes-stubs/reporter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:35.856363 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:20:35.000000 types-pyflakes-3.0.0.5/types_pyflakes.egg-info/top_level.txt
```

### Comparing `types-pyflakes-3.0.0.4/CHANGELOG.md` & `types-pyflakes-3.0.0.5/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.0.0.5 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.0.0.4 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 3.0.0.3 (2023-03-27)
 
 Add default values for third-party stubs beginning with 'P' (#9957)
```

### Comparing `types-pyflakes-3.0.0.4/PKG-INFO` & `types-pyflakes-3.0.0.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyflakes
-Version: 3.0.0.4
+Version: 3.0.0.5
 Summary: Typing stubs for pyflakes
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyflakes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyflakes. All fixes for
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

### Comparing `types-pyflakes-3.0.0.4/pyflakes-stubs/api.pyi` & `types-pyflakes-3.0.0.5/pyflakes-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.4/pyflakes-stubs/checker.pyi` & `types-pyflakes-3.0.0.5/pyflakes-stubs/checker.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.4/pyflakes-stubs/messages.pyi` & `types-pyflakes-3.0.0.5/pyflakes-stubs/messages.pyi`

 * *Files identical despite different names*

### Comparing `types-pyflakes-3.0.0.4/setup.py` & `types-pyflakes-3.0.0.5/types_pyflakes.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-from setuptools import setup
+Metadata-Version: 2.1
+Name: types-pyflakes
+Version: 3.0.0.5
+Summary: Typing stubs for pyflakes
+Home-page: https://github.com/python/typeshed
+License: Apache-2.0 license
+Project-URL: GitHub, https://github.com/python/typeshed
+Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md
+Project-URL: Issue tracker, https://github.com/python/typeshed/issues
+Project-URL: Chat, https://gitter.im/python/typing
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Typing :: Stubs Only
+Description-Content-Type: text/markdown
 
-name = "types-pyflakes"
-description = "Typing stubs for pyflakes"
-long_description = '''
 ## Typing stubs for pyflakes
 
 This is a PEP 561 type stub package for the `pyflakes` package. It
 can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyflakes`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyflakes. All fixes for
 types and metadata should be contributed there.
 
-See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
-'''.lstrip()
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
 
-setup(name=name,
-      version="3.0.0.4",
-      description=description,
-      long_description=long_description,
-      long_description_content_type="text/markdown",
-      url="https://github.com/python/typeshed",
-      project_urls={
-          "GitHub": "https://github.com/python/typeshed",
-          "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyflakes.md",
-          "Issue tracker": "https://github.com/python/typeshed/issues",
-          "Chat": "https://gitter.im/python/typing",
-      },
-      install_requires=[],
-      packages=['pyflakes-stubs'],
-      package_data={'pyflakes-stubs': ['__init__.pyi', 'api.pyi', 'checker.pyi', 'messages.pyi', 'reporter.pyi', 'METADATA.toml']},
-      license="Apache-2.0 license",
-      classifiers=[
-          "License :: OSI Approved :: Apache Software License",
-          "Programming Language :: Python :: 3",
-          "Typing :: Stubs Only",
-      ]
-)
+See https://github.com/python/typeshed/blob/main/README.md for more details.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

