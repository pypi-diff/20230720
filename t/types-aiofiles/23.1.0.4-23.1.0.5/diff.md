# Comparing `tmp/types-aiofiles-23.1.0.4.tar.gz` & `tmp/types-aiofiles-23.1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiofiles-23.1.0.4.tar", last modified: Wed Jun  7 15:15:35 2023, max compression
+gzip compressed data, was "types-aiofiles-23.1.0.5.tar", last modified: Thu Jul 20 15:16:14 2023, max compression
```

## Comparing `types-aiofiles-23.1.0.4.tar` & `types-aiofiles-23.1.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-07 15:15:32.000000 types-aiofiles-23.1.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 15:15:32.000000 types-aiofiles-23.1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/aiofiles-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-07 15:15:32.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/os.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/ospath.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/aiofiles-stubs/tempfile/
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/tempfile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/tempfile/temptypes.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/binary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/text.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-07 15:15:14.000000 types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-07 15:15:32.000000 types-aiofiles-23.1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 15:15:35.199396 types-aiofiles-23.1.0.4/types_aiofiles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-07 15:15:35.000000 types-aiofiles-23.1.0.4/types_aiofiles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-07 15:15:35.000000 types-aiofiles-23.1.0.4/types_aiofiles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 15:15:35.000000 types-aiofiles-23.1.0.4/types_aiofiles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 15:15:35.000000 types-aiofiles-23.1.0.4/types_aiofiles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-07-20 15:16:13.000000 types-aiofiles-23.1.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:13.000000 types-aiofiles-23.1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/aiofiles-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 15:16:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/os.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/ospath.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/aiofiles-stubs/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/tempfile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/tempfile/temptypes.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/binary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/text.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 15:15:13.000000 types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-20 15:16:13.000000 types-aiofiles-23.1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:14.077120 types-aiofiles-23.1.0.5/types_aiofiles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-07-20 15:16:14.000000 types-aiofiles-23.1.0.5/types_aiofiles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 15:16:14.000000 types-aiofiles-23.1.0.5/types_aiofiles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:14.000000 types-aiofiles-23.1.0.5/types_aiofiles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:16:14.000000 types-aiofiles-23.1.0.5/types_aiofiles.egg-info/top_level.txt
```

### Comparing `types-aiofiles-23.1.0.4/CHANGELOG.md` & `types-aiofiles-23.1.0.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 23.1.0.5 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 23.1.0.4 (2023-06-07)
 
 [aiofiles] Use file mode alias from _typeshed (#10233)
 
 ## 23.1.0.3 (2023-05-22)
 
 add typing support to more aiofiles wrapped functions (#10175)
```

### Comparing `types-aiofiles-23.1.0.4/PKG-INFO` & `types-aiofiles-23.1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiofiles
-Version: 23.1.0.4
+Version: 23.1.0.5
 Summary: Typing stubs for aiofiles
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `aiofiles`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `786bd22343a66ecdb0eeb3fe053dfb81365608c5`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/base.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/base.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/os.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/os.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/ospath.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/ospath.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/tempfile/__init__.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/tempfile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/tempfile/temptypes.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/tempfile/temptypes.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/__init__.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/binary.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/binary.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/aiofiles-stubs/threadpool/text.pyi` & `types-aiofiles-23.1.0.5/aiofiles-stubs/threadpool/text.pyi`

 * *Files identical despite different names*

### Comparing `types-aiofiles-23.1.0.4/setup.py` & `types-aiofiles-23.1.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `aiofiles`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `786bd22343a66ecdb0eeb3fe053dfb81365608c5`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="23.1.0.4",
+      version="23.1.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md",
```

### Comparing `types-aiofiles-23.1.0.4/types_aiofiles.egg-info/PKG-INFO` & `types-aiofiles-23.1.0.5/types_aiofiles.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-aiofiles
-Version: 23.1.0.4
+Version: 23.1.0.5
 Summary: Typing stubs for aiofiles
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/aiofiles.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `aiofiles`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/aiofiles. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `786bd22343a66ecdb0eeb3fe053dfb81365608c5`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-aiofiles-23.1.0.4/types_aiofiles.egg-info/SOURCES.txt` & `types-aiofiles-23.1.0.5/types_aiofiles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

