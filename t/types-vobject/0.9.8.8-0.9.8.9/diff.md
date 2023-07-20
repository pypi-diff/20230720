# Comparing `tmp/types-vobject-0.9.8.8.tar.gz` & `tmp/types-vobject-0.9.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-vobject-0.9.8.8.tar", last modified: Wed Jan 25 01:18:32 2023, max compression
+gzip compressed data, was "types-vobject-0.9.8.9.tar", last modified: Tue Feb  7 01:21:41 2023, max compression
```

## Comparing `types-vobject-0.9.8.8.tar` & `types-vobject-0.9.8.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:18:32.342470 types-vobject-0.9.8.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-01-25 01:18:31.000000 types-vobject-0.9.8.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-01-25 01:18:31.000000 types-vobject-0.9.8.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-25 01:18:32.342470 types-vobject-0.9.8.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 01:18:32.342470 types-vobject-0.9.8.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-01-25 01:18:31.000000 types-vobject-0.9.8.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:18:32.342470 types-vobject-0.9.8.8/types_vobject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-01-25 01:18:32.000000 types-vobject-0.9.8.8/types_vobject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-25 01:18:32.000000 types-vobject-0.9.8.8/types_vobject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 01:18:32.000000 types-vobject-0.9.8.8/types_vobject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-25 01:18:32.000000 types-vobject-0.9.8.8/types_vobject.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 01:18:32.342470 types-vobject-0.9.8.8/vobject-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-25 01:18:31.000000 types-vobject-0.9.8.8/vobject-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/behavior.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/change_tz.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/hcalendar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/icalendar.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/ics_diff.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/vcard.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-25 01:18:09.000000 types-vobject-0.9.8.8/vobject-stubs/win32tz.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:41.148553 types-vobject-0.9.8.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-02-07 01:21:40.000000 types-vobject-0.9.8.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-07 01:21:40.000000 types-vobject-0.9.8.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-07 01:21:41.148553 types-vobject-0.9.8.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 01:21:41.148553 types-vobject-0.9.8.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-02-07 01:21:40.000000 types-vobject-0.9.8.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:41.148553 types-vobject-0.9.8.9/types_vobject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-07 01:21:41.000000 types-vobject-0.9.8.9/types_vobject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-02-07 01:21:41.000000 types-vobject-0.9.8.9/types_vobject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 01:21:41.000000 types-vobject-0.9.8.9/types_vobject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-07 01:21:41.000000 types-vobject-0.9.8.9/types_vobject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 01:21:41.148553 types-vobject-0.9.8.9/vobject-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-07 01:21:40.000000 types-vobject-0.9.8.9/vobject-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/behavior.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/change_tz.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/hcalendar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/icalendar.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/ics_diff.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/vcard.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-02-07 01:20:33.000000 types-vobject-0.9.8.9/vobject-stubs/win32tz.pyi
```

### Comparing `types-vobject-0.9.8.8/CHANGELOG.md` & `types-vobject-0.9.8.9/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.9.8.9 (2023-02-07)
+
+Bump mypy to 1.0 (#9684)
+
 ## 0.9.8.8 (2023-01-25)
 
 Fix some stubtest complaints before they happen (#9585)
 
 Add missing objects to various stubs
 
 ## 0.9.8.7 (2023-01-18)
```

### Comparing `types-vobject-0.9.8.8/PKG-INFO` & `types-vobject-0.9.8.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-vobject
-Version: 0.9.8.8
+Version: 0.9.8.9
 Summary: Typing stubs for vobject
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/vobject.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `vobject`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/vobject. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9b4fa0a325f2806bde895d2cd374d42cd06e67e`.
+This package was generated from typeshed commit `c4c4bee8aa368b8c05d06559904531596e8a7be6`.
```

### Comparing `types-vobject-0.9.8.8/setup.py` & `types-vobject-0.9.8.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `vobject`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/vobject. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9b4fa0a325f2806bde895d2cd374d42cd06e67e`.
+This package was generated from typeshed commit `c4c4bee8aa368b8c05d06559904531596e8a7be6`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.9.8.8",
+      version="0.9.8.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/vobject.md",
```

### Comparing `types-vobject-0.9.8.8/types_vobject.egg-info/PKG-INFO` & `types-vobject-0.9.8.9/types_vobject.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-vobject
-Version: 0.9.8.8
+Version: 0.9.8.9
 Summary: Typing stubs for vobject
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/vobject.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `vobject`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/vobject. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `a9b4fa0a325f2806bde895d2cd374d42cd06e67e`.
+This package was generated from typeshed commit `c4c4bee8aa368b8c05d06559904531596e8a7be6`.
```

### Comparing `types-vobject-0.9.8.8/vobject-stubs/base.pyi` & `types-vobject-0.9.8.9/vobject-stubs/base.pyi`

 * *Files identical despite different names*

### Comparing `types-vobject-0.9.8.8/vobject-stubs/behavior.pyi` & `types-vobject-0.9.8.9/vobject-stubs/behavior.pyi`

 * *Files identical despite different names*

### Comparing `types-vobject-0.9.8.8/vobject-stubs/icalendar.pyi` & `types-vobject-0.9.8.9/vobject-stubs/icalendar.pyi`

 * *Files identical despite different names*

### Comparing `types-vobject-0.9.8.8/vobject-stubs/vcard.pyi` & `types-vobject-0.9.8.9/vobject-stubs/vcard.pyi`

 * *Files identical despite different names*

### Comparing `types-vobject-0.9.8.8/vobject-stubs/win32tz.pyi` & `types-vobject-0.9.8.9/vobject-stubs/win32tz.pyi`

 * *Files identical despite different names*

