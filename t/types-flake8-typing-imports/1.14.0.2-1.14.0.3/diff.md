# Comparing `tmp/types-flake8-typing-imports-1.14.0.2.tar.gz` & `tmp/types-flake8-typing-imports-1.14.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-flake8-typing-imports-1.14.0.2.tar", last modified: Wed May 10 15:20:23 2023, max compression
+gzip compressed data, was "types-flake8-typing-imports-1.14.0.3.tar", last modified: Thu Jul 20 15:17:37 2023, max compression
```

## Comparing `types-flake8-typing-imports-1.14.0.2.tar` & `types-flake8-typing-imports-1.14.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:23.085982 types-flake8-typing-imports-1.14.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-10 15:20:22.000000 types-flake8-typing-imports-1.14.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:20:22.000000 types-flake8-typing-imports-1.14.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-10 15:20:23.085982 types-flake8-typing-imports-1.14.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:23.085982 types-flake8-typing-imports-1.14.0.2/flake8_typing_imports-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 15:20:22.000000 types-flake8-typing-imports-1.14.0.2/flake8_typing_imports-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-10 15:20:22.000000 types-flake8-typing-imports-1.14.0.2/flake8_typing_imports-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:20:23.085982 types-flake8-typing-imports-1.14.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-10 15:20:22.000000 types-flake8-typing-imports-1.14.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:20:23.085982 types-flake8-typing-imports-1.14.0.2/types_flake8_typing_imports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-10 15:20:23.000000 types-flake8-typing-imports-1.14.0.2/types_flake8_typing_imports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-10 15:20:23.000000 types-flake8-typing-imports-1.14.0.2/types_flake8_typing_imports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:20:23.000000 types-flake8-typing-imports-1.14.0.2/types_flake8_typing_imports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-10 15:20:23.000000 types-flake8-typing-imports-1.14.0.2/types_flake8_typing_imports.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:37.310125 types-flake8-typing-imports-1.14.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-20 15:17:36.000000 types-flake8-typing-imports-1.14.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:17:36.000000 types-flake8-typing-imports-1.14.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-20 15:17:37.310125 types-flake8-typing-imports-1.14.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:37.306125 types-flake8-typing-imports-1.14.0.3/flake8_typing_imports-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-20 15:17:36.000000 types-flake8-typing-imports-1.14.0.3/flake8_typing_imports-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 15:17:36.000000 types-flake8-typing-imports-1.14.0.3/flake8_typing_imports-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:17:37.310125 types-flake8-typing-imports-1.14.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-20 15:17:36.000000 types-flake8-typing-imports-1.14.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:17:37.310125 types-flake8-typing-imports-1.14.0.3/types_flake8_typing_imports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-20 15:17:37.000000 types-flake8-typing-imports-1.14.0.3/types_flake8_typing_imports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 15:17:37.000000 types-flake8-typing-imports-1.14.0.3/types_flake8_typing_imports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:17:37.000000 types-flake8-typing-imports-1.14.0.3/types_flake8_typing_imports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 15:17:37.000000 types-flake8-typing-imports-1.14.0.3/types_flake8_typing_imports.egg-info/top_level.txt
```

### Comparing `types-flake8-typing-imports-1.14.0.2/CHANGELOG.md` & `types-flake8-typing-imports-1.14.0.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.14.0.3 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.14.0.2 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 1.14.0.1 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-flake8-typing-imports-1.14.0.2/flake8_typing_imports-stubs/__init__.pyi` & `types-flake8-typing-imports-1.14.0.3/flake8_typing_imports-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-flake8-typing-imports-1.14.0.2/setup.py` & `types-flake8-typing-imports-1.14.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `flake8-typing-imports`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/flake8-typing-imports. All fixes for
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
-      version="1.14.0.2",
+      version="1.14.0.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/flake8-typing-imports.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['flake8_typing_imports-stubs'],
-      package_data={'flake8_typing_imports-stubs': ['__init__.pyi', 'METADATA.toml']},
+      package_data={'flake8_typing_imports-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

