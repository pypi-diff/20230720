# Comparing `tmp/types-pep8-naming-0.13.0.4.tar.gz` & `tmp/types-pep8-naming-0.13.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pep8-naming-0.13.0.4.tar", last modified: Wed May 10 15:21:51 2023, max compression
+gzip compressed data, was "types-pep8-naming-0.13.0.5.tar", last modified: Thu Jul 20 15:16:54 2023, max compression
```

## Comparing `types-pep8-naming-0.13.0.4.tar` & `types-pep8-naming-0.13.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:51.732062 types-pep8-naming-0.13.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-10 15:21:51.728062 types-pep8-naming-0.13.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:51.728062 types-pep8-naming-0.13.0.4/pep8ext_naming-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/pep8ext_naming-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/pep8ext_naming-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:21:51.732062 types-pep8-naming-0.13.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:21:51.728062 types-pep8-naming-0.13.0.4/types_pep8_naming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/types_pep8_naming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/types_pep8_naming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/types_pep8_naming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:21:51.000000 types-pep8-naming-0.13.0.4/types_pep8_naming.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/top_level.txt
```

### Comparing `types-pep8-naming-0.13.0.4/CHANGELOG.md` & `types-pep8-naming-0.13.0.5/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.13.0.5 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 0.13.0.4 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 0.13.0.3 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-pep8-naming-0.13.0.4/PKG-INFO` & `types-pep8-naming-0.13.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pep8-naming
-Version: 0.13.0.4
+Version: 0.13.0.5
 Summary: Typing stubs for pep8-naming
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pep8-naming.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pep8-naming`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pep8-naming. All fixes for
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

### Comparing `types-pep8-naming-0.13.0.4/pep8ext_naming-stubs/__init__.pyi` & `types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pep8-naming-0.13.0.4/setup.py` & `types-pep8-naming-0.13.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pep8-naming`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pep8-naming. All fixes for
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
-      version="0.13.0.4",
+      version="0.13.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pep8-naming.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pep8ext_naming-stubs'],
-      package_data={'pep8ext_naming-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'pep8ext_naming-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pep8-naming-0.13.0.4/types_pep8_naming.egg-info/PKG-INFO` & `types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pep8-naming
-Version: 0.13.0.4
+Version: 0.13.0.5
 Summary: Typing stubs for pep8-naming
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pep8-naming.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pep8-naming`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pep8-naming. All fixes for
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

