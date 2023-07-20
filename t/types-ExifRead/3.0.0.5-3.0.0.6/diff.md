# Comparing `tmp/types-ExifRead-3.0.0.5.tar.gz` & `tmp/types-ExifRead-3.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-ExifRead-3.0.0.5.tar", last modified: Mon Mar 27 18:23:47 2023, max compression
+gzip compressed data, was "types-ExifRead-3.0.0.6.tar", last modified: Thu Jul 20 15:18:44 2023, max compression
```

## Comparing `types-ExifRead-3.0.0.5.tar` & `types-ExifRead-3.0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-27 18:23:46.000000 types-ExifRead-3.0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-27 18:23:46.000000 types-ExifRead-3.0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/exifread-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-27 18:23:46.000000 types-ExifRead-3.0.0.5/exifread-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/classes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/exif_log.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/heic.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/jpeg.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/exifread-stubs/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/exif.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/apple.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/canon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/casio.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/fujifilm.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/nikon.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/olympus.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-27 18:21:24.000000 types-ExifRead-3.0.0.5/exifread-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-27 18:23:46.000000 types-ExifRead-3.0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 18:23:47.634801 types-ExifRead-3.0.0.5/types_ExifRead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-27 18:23:47.000000 types-ExifRead-3.0.0.5/types_ExifRead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-27 18:23:47.000000 types-ExifRead-3.0.0.5/types_ExifRead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 18:23:47.000000 types-ExifRead-3.0.0.5/types_ExifRead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-27 18:23:47.000000 types-ExifRead-3.0.0.5/types_ExifRead.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:44.606984 types-ExifRead-3.0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-20 15:18:43.000000 types-ExifRead-3.0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:18:43.000000 types-ExifRead-3.0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:18:44.602984 types-ExifRead-3.0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:44.602984 types-ExifRead-3.0.0.6/exifread-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-20 15:18:43.000000 types-ExifRead-3.0.0.6/exifread-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/classes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/exif_log.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/heic.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/jpeg.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:44.602984 types-ExifRead-3.0.0.6/exifread-stubs/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/exif.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:44.602984 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/apple.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/canon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/casio.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/fujifilm.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/nikon.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/olympus.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-20 15:15:13.000000 types-ExifRead-3.0.0.6/exifread-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:18:44.606984 types-ExifRead-3.0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-07-20 15:18:43.000000 types-ExifRead-3.0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:18:44.602984 types-ExifRead-3.0.0.6/types_ExifRead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 15:18:44.000000 types-ExifRead-3.0.0.6/types_ExifRead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-20 15:18:44.000000 types-ExifRead-3.0.0.6/types_ExifRead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:18:44.000000 types-ExifRead-3.0.0.6/types_ExifRead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 15:18:44.000000 types-ExifRead-3.0.0.6/types_ExifRead.egg-info/top_level.txt
```

### Comparing `types-ExifRead-3.0.0.5/CHANGELOG.md` & `types-ExifRead-3.0.0.6/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 3.0.0.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 3.0.0.5 (2023-03-27)
 
 Add defaults for third-party stubs E-H (#9954)
 
 ## 3.0.0.4 (2023-02-21)
 
 Stubtest settings: change `ignore_missing_stub` default to `false` (#9779)
```

### Comparing `types-ExifRead-3.0.0.5/PKG-INFO` & `types-ExifRead-3.0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ExifRead
-Version: 3.0.0.5
+Version: 3.0.0.6
 Summary: Typing stubs for ExifRead
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ExifRead.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ExifRead`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ExifRead. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-ExifRead-3.0.0.5/exifread-stubs/_types.pyi` & `types-ExifRead-3.0.0.6/exifread-stubs/_types.pyi`

 * *Files identical despite different names*

### Comparing `types-ExifRead-3.0.0.5/exifread-stubs/classes.pyi` & `types-ExifRead-3.0.0.6/exifread-stubs/classes.pyi`

 * *Files identical despite different names*

### Comparing `types-ExifRead-3.0.0.5/exifread-stubs/exif_log.pyi` & `types-ExifRead-3.0.0.6/exifread-stubs/exif_log.pyi`

 * *Files identical despite different names*

### Comparing `types-ExifRead-3.0.0.5/exifread-stubs/heic.pyi` & `types-ExifRead-3.0.0.6/exifread-stubs/heic.pyi`

 * *Files identical despite different names*

### Comparing `types-ExifRead-3.0.0.5/exifread-stubs/tags/makernote/canon.pyi` & `types-ExifRead-3.0.0.6/exifread-stubs/tags/makernote/canon.pyi`

 * *Files identical despite different names*

### Comparing `types-ExifRead-3.0.0.5/exifread-stubs/utils.pyi` & `types-ExifRead-3.0.0.6/exifread-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-ExifRead-3.0.0.5/setup.py` & `types-ExifRead-3.0.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ExifRead`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ExifRead. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="3.0.0.5",
+      version="3.0.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ExifRead.md",
```

### Comparing `types-ExifRead-3.0.0.5/types_ExifRead.egg-info/PKG-INFO` & `types-ExifRead-3.0.0.6/types_ExifRead.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-ExifRead
-Version: 3.0.0.5
+Version: 3.0.0.6
 Summary: Typing stubs for ExifRead
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/ExifRead.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `ExifRead`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/ExifRead. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `6fd7e36e80e0448d9199d62d582c659c147be149`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-ExifRead-3.0.0.5/types_ExifRead.egg-info/SOURCES.txt` & `types-ExifRead-3.0.0.6/types_ExifRead.egg-info/SOURCES.txt`

 * *Files identical despite different names*

