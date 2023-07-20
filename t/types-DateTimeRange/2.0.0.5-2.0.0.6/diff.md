# Comparing `tmp/types-DateTimeRange-2.0.0.5.tar.gz` & `tmp/types-DateTimeRange-2.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-DateTimeRange-2.0.0.5.tar", last modified: Wed Mar 29 12:35:03 2023, max compression
+gzip compressed data, was "types-DateTimeRange-2.0.0.6.tar", last modified: Thu Jul 20 15:21:39 2023, max compression
```

## Comparing `types-DateTimeRange-2.0.0.5.tar` & `types-DateTimeRange-2.0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:35:03.187036 types-DateTimeRange-2.0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-03-29 12:35:02.000000 types-DateTimeRange-2.0.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-29 12:35:02.000000 types-DateTimeRange-2.0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-29 12:35:03.187036 types-DateTimeRange-2.0.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:35:03.187036 types-DateTimeRange-2.0.0.5/datetimerange-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-29 12:35:02.000000 types-DateTimeRange-2.0.0.5/datetimerange-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-29 12:34:30.000000 types-DateTimeRange-2.0.0.5/datetimerange-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-29 12:34:30.000000 types-DateTimeRange-2.0.0.5/datetimerange-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 12:35:03.187036 types-DateTimeRange-2.0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-29 12:35:02.000000 types-DateTimeRange-2.0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 12:35:03.187036 types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-03-29 12:35:03.000000 types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-29 12:35:03.000000 types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 12:35:03.000000 types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-29 12:35:03.000000 types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-29 12:35:03.000000 types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:39.277112 types-DateTimeRange-2.0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-20 15:21:38.000000 types-DateTimeRange-2.0.0.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:38.000000 types-DateTimeRange-2.0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 15:21:39.277112 types-DateTimeRange-2.0.0.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:39.277112 types-DateTimeRange-2.0.0.6/datetimerange-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 15:21:38.000000 types-DateTimeRange-2.0.0.6/datetimerange-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-20 15:15:13.000000 types-DateTimeRange-2.0.0.6/datetimerange-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 15:15:13.000000 types-DateTimeRange-2.0.0.6/datetimerange-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:39.277112 types-DateTimeRange-2.0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-20 15:21:38.000000 types-DateTimeRange-2.0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:39.277112 types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-07-20 15:21:39.000000 types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 15:21:39.000000 types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:39.000000 types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 15:21:39.000000 types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:21:39.000000 types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/top_level.txt
```

### Comparing `types-DateTimeRange-2.0.0.5/CHANGELOG.md` & `types-DateTimeRange-2.0.0.6/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.0.0.6 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2.0.0.5 (2023-03-29)
 
 Remove unnecessary ellipsis expressions (#9976)
 
 Ignore flake8 F821 warnings in stub files
 
 ## 2.0.0.4 (2023-03-27)
```

### Comparing `types-DateTimeRange-2.0.0.5/PKG-INFO` & `types-DateTimeRange-2.0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-DateTimeRange
-Version: 2.0.0.5
+Version: 2.0.0.6
 Summary: Typing stubs for DateTimeRange
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/DateTimeRange.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,10 @@
 
 *Note:* The `DateTimeRange` package includes type annotations or type stubs
 since version 2.1.0. Please uninstall the `types-DateTimeRange`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ed915c5cde48329e3d1e597e60c4baee27b7854a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-DateTimeRange-2.0.0.5/datetimerange-stubs/__init__.pyi` & `types-DateTimeRange-2.0.0.6/datetimerange-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-DateTimeRange-2.0.0.5/setup.py` & `types-DateTimeRange-2.0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,19 +17,21 @@
 
 *Note:* The `DateTimeRange` package includes type annotations or type stubs
 since version 2.1.0. Please uninstall the `types-DateTimeRange`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ed915c5cde48329e3d1e597e60c4baee27b7854a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.5",
+      version="2.0.0.6",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/DateTimeRange.md",
```

### Comparing `types-DateTimeRange-2.0.0.5/types_DateTimeRange.egg-info/PKG-INFO` & `types-DateTimeRange-2.0.0.6/types_DateTimeRange.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-DateTimeRange
-Version: 2.0.0.5
+Version: 2.0.0.6
 Summary: Typing stubs for DateTimeRange
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/DateTimeRange.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -27,8 +27,10 @@
 
 *Note:* The `DateTimeRange` package includes type annotations or type stubs
 since version 2.1.0. Please uninstall the `types-DateTimeRange`
 package if you use this or a newer version.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ed915c5cde48329e3d1e597e60c4baee27b7854a`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

