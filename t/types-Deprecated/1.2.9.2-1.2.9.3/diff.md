# Comparing `tmp/types-Deprecated-1.2.9.2.tar.gz` & `tmp/types-Deprecated-1.2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-Deprecated-1.2.9.2.tar", last modified: Mon Mar 27 18:22:30 2023, max compression
+gzip compressed data, was "types-Deprecated-1.2.9.3.tar", last modified: Thu Jul 20 15:19:58 2023, max compression
```

## Comparing `types-Deprecated-1.2.9.2.tar` & `types-Deprecated-1.2.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:30.753987 types-Deprecated-1.2.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:22:30.753987 types-Deprecated-1.2.9.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:30.753987 types-Deprecated-1.2.9.2/deprecated-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/deprecated-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-27 18:21:24.000000 types-Deprecated-1.2.9.2/deprecated-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-03-27 18:21:24.000000 types-Deprecated-1.2.9.2/deprecated-stubs/classic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-03-27 18:21:24.000000 types-Deprecated-1.2.9.2/deprecated-stubs/sphinx.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:22:30.753987 types-Deprecated-1.2.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:22:30.753987 types-Deprecated-1.2.9.2/types_Deprecated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/types_Deprecated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/types_Deprecated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/types_Deprecated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 18:22:30.000000 types-Deprecated-1.2.9.2/types_Deprecated.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:58.227905 types-Deprecated-1.2.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-07-20 15:19:57.000000 types-Deprecated-1.2.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:19:57.000000 types-Deprecated-1.2.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 15:19:58.227905 types-Deprecated-1.2.9.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:58.227905 types-Deprecated-1.2.9.3/deprecated-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 15:19:57.000000 types-Deprecated-1.2.9.3/deprecated-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 15:15:13.000000 types-Deprecated-1.2.9.3/deprecated-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-20 15:15:13.000000 types-Deprecated-1.2.9.3/deprecated-stubs/classic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-20 15:15:13.000000 types-Deprecated-1.2.9.3/deprecated-stubs/sphinx.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:19:58.227905 types-Deprecated-1.2.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-07-20 15:19:57.000000 types-Deprecated-1.2.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:19:58.227905 types-Deprecated-1.2.9.3/types_Deprecated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-20 15:19:58.000000 types-Deprecated-1.2.9.3/types_Deprecated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 15:19:58.000000 types-Deprecated-1.2.9.3/types_Deprecated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:19:58.000000 types-Deprecated-1.2.9.3/types_Deprecated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-20 15:19:58.000000 types-Deprecated-1.2.9.3/types_Deprecated.egg-info/top_level.txt
```

### Comparing `types-Deprecated-1.2.9.2/deprecated-stubs/classic.pyi` & `types-Deprecated-1.2.9.3/deprecated-stubs/classic.pyi`

 * *Files identical despite different names*

### Comparing `types-Deprecated-1.2.9.2/deprecated-stubs/sphinx.pyi` & `types-Deprecated-1.2.9.3/deprecated-stubs/sphinx.pyi`

 * *Files identical despite different names*

### Comparing `types-Deprecated-1.2.9.2/setup.py` & `types-Deprecated-1.2.9.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `Deprecated`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/Deprecated. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.2.9.2",
+      version="1.2.9.3",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/Deprecated.md",
```

