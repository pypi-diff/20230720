# Comparing `tmp/types-PyMySQL-1.1.0.0.tar.gz` & `tmp/types-PyMySQL-1.1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-PyMySQL-1.1.0.0.tar", last modified: Wed Jun 28 12:35:47 2023, max compression
+gzip compressed data, was "types-PyMySQL-1.1.0.1.tar", last modified: Thu Jul 20 15:20:05 2023, max compression
```

## Comparing `types-PyMySQL-1.1.0.0.tar` & `types-PyMySQL-1.1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:47.619991 types-PyMySQL-1.1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-28 12:35:44.000000 types-PyMySQL-1.1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-28 12:35:44.000000 types-PyMySQL-1.1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-28 12:35:47.619991 types-PyMySQL-1.1.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:47.615991 types-PyMySQL-1.1.0.0/pymysql-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-28 12:35:44.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/charset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/connections.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:47.619991 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/CLIENT.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/COMMAND.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/CR.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/ER.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/FIELD_TYPE.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/FLAG.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/SERVER_STATUS.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/constants/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/converters.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/cursors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/err.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/times.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-28 12:35:28.000000 types-PyMySQL-1.1.0.0/pymysql-stubs/util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 12:35:47.619991 types-PyMySQL-1.1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-28 12:35:44.000000 types-PyMySQL-1.1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 12:35:47.619991 types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-28 12:35:47.000000 types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-28 12:35:47.000000 types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 12:35:47.000000 types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 12:35:47.000000 types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.531992 types-PyMySQL-1.1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-20 15:20:05.531992 types-PyMySQL-1.1.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.527992 types-PyMySQL-1.1.0.1/pymysql-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/charset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8061 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/connections.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.527992 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/CLIENT.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/COMMAND.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/CR.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/ER.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/FIELD_TYPE.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/FLAG.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/SERVER_STATUS.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/constants/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/converters.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/cursors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/err.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/times.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 15:15:13.000000 types-PyMySQL-1.1.0.1/pymysql-stubs/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:20:05.531992 types-PyMySQL-1.1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-20 15:20:04.000000 types-PyMySQL-1.1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:20:05.527992 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-20 15:20:05.000000 types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/top_level.txt
```

### Comparing `types-PyMySQL-1.1.0.0/CHANGELOG.md` & `types-PyMySQL-1.1.0.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 1.1.0.1 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
 ## 1.1.0.0 (2023-06-28)
 
 Bump PyMySQL to `1.1.*` (#10376)
 
 ## 1.0.19.7 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
```

### Comparing `types-PyMySQL-1.1.0.0/PKG-INFO` & `types-PyMySQL-1.1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0869b430d644b0580ca1d590b075a1db1d73677d` and was tested
-with mypy 1.4.1, pyright 1.1.315, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/__init__.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/connections.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/connections.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/constants/COMMAND.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/constants/COMMAND.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/constants/CR.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/constants/CR.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/constants/ER.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/constants/ER.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/converters.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/converters.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/cursors.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/cursors.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/pymysql-stubs/err.pyi` & `types-PyMySQL-1.1.0.1/pymysql-stubs/err.pyi`

 * *Files identical despite different names*

### Comparing `types-PyMySQL-1.1.0.0/setup.py` & `types-PyMySQL-1.1.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0869b430d644b0580ca1d590b075a1db1d73677d` and was tested
-with mypy 1.4.1, pyright 1.1.315, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.1.0.0",
+      version="1.1.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md",
```

### Comparing `types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/PKG-INFO` & `types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-PyMySQL
-Version: 1.1.0.0
+Version: 1.1.0.1
 Summary: Typing stubs for PyMySQL
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/PyMySQL.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -26,10 +26,10 @@
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `0869b430d644b0580ca1d590b075a1db1d73677d` and was tested
-with mypy 1.4.1, pyright 1.1.315, and
-pytype 2023.6.2.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-PyMySQL-1.1.0.0/types_PyMySQL.egg-info/SOURCES.txt` & `types-PyMySQL-1.1.0.1/types_PyMySQL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

