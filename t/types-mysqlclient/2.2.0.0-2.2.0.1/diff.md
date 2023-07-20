# Comparing `tmp/types-mysqlclient-2.2.0.0.tar.gz` & `tmp/types-mysqlclient-2.2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-mysqlclient-2.2.0.0.tar", last modified: Fri Jun 23 12:33:00 2023, max compression
+gzip compressed data, was "types-mysqlclient-2.2.0.1.tar", last modified: Thu Jul 20 15:20:32 2023, max compression
```

## Comparing `types-mysqlclient-2.2.0.0.tar` & `types-mysqlclient-2.2.0.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.121359 types-mysqlclient-2.2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/MySQLdb-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/_mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/connections.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/CLIENT.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/CR.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/ER.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/FIELD_TYPE.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/FLAG.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/cursors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/release.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-23 12:32:44.000000 types-mysqlclient-2.2.0.0/MySQLdb-stubs/times.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:33:00.121359 types-mysqlclient-2.2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-23 12:32:57.000000 types-mysqlclient-2.2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:33:00.117359 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 12:33:00.000000 types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:32.540322 types-mysqlclient-2.2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-20 15:20:31.000000 types-mysqlclient-2.2.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:31.000000 types-mysqlclient-2.2.0.1/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:32.536322 types-mysqlclient-2.2.0.1/MySQLdb-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 15:20:31.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/_mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/connections.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:32.536322 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/CLIENT.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/CR.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/ER.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/FIELD_TYPE.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/FLAG.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/cursors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/release.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-20 15:15:13.000000 types-mysqlclient-2.2.0.1/MySQLdb-stubs/times.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:20:32.536322 types-mysqlclient-2.2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:32.540322 types-mysqlclient-2.2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-20 15:20:31.000000 types-mysqlclient-2.2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:32.536322 types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-20 15:20:32.000000 types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 15:20:32.000000 types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:32.000000 types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:20:32.000000 types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/top_level.txt
```

### Comparing `types-mysqlclient-2.2.0.0/CHANGELOG.md` & `types-mysqlclient-2.2.0.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 2.2.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 2.2.0.0 (2023-06-23)
 
 Bump mysqlclient to 2.2 (#10353)
 
 Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
 
 ## 2.1.5.7 (2023-03-27)
```

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/__init__.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/_mysql.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/_mysql.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/connections.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/connections.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/CR.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/CR.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/constants/ER.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/constants/ER.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/converters.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/converters.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/cursors.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/cursors.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/MySQLdb-stubs/times.pyi` & `types-mysqlclient-2.2.0.1/MySQLdb-stubs/times.pyi`

 * *Files identical despite different names*

### Comparing `types-mysqlclient-2.2.0.0/PKG-INFO` & `types-mysqlclient-2.2.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mysqlclient
-Version: 2.2.0.0
+Version: 2.2.0.1
 Summary: Typing stubs for mysqlclient
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mysqlclient.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mysqlclient`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mysqlclient. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b10f482e36f67a9d7aae13c49a4d14cb17df97e6` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-mysqlclient-2.2.0.0/setup.py` & `types-mysqlclient-2.2.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mysqlclient`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mysqlclient. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b10f482e36f67a9d7aae13c49a4d14cb17df97e6` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="2.2.0.0",
+      version="2.2.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mysqlclient.md",
```

### Comparing `types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/PKG-INFO` & `types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-mysqlclient
-Version: 2.2.0.0
+Version: 2.2.0.1
 Summary: Typing stubs for mysqlclient
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/mysqlclient.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,10 +22,10 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `mysqlclient`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/mysqlclient. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b10f482e36f67a9d7aae13c49a4d14cb17df97e6` and was tested
-with mypy 1.3.0, pyright 1.1.314, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-mysqlclient-2.2.0.0/types_mysqlclient.egg-info/SOURCES.txt` & `types-mysqlclient-2.2.0.1/types_mysqlclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

