# Comparing `tmp/query_everywhere-0.1.8.tar.gz` & `tmp/query_everywhere-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "query_everywhere-0.1.8.tar", max compression
+gzip compressed data, was "query_everywhere-0.1.9.tar", max compression
```

## Comparing `query_everywhere-0.1.8.tar` & `query_everywhere-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1272 2023-07-20 01:38:28.471109 query_everywhere-0.1.8/README.md
--rw-r--r--   0        0        0      376 2023-07-20 03:56:10.030961 query_everywhere-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5350 2023-07-20 03:55:46.419038 query_everywhere-0.1.8/query_everywhere/__init__.py
--rw-r--r--   0        0        0     1644 1970-01-01 00:00:00.000000 query_everywhere-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1293 2023-07-20 08:15:55.897194 query_everywhere-0.1.9/README.md
+-rw-r--r--   0        0        0      785 2023-07-20 08:16:27.672884 query_everywhere-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-07-20 08:00:57.237970 query_everywhere-0.1.9/query_everywhere/__init__.py
+-rw-r--r--   0        0        0     6205 2023-07-20 08:13:45.382733 query_everywhere-0.1.9/query_everywhere/queryer.py
+-rw-r--r--   0        0        0     1665 1970-01-01 00:00:00.000000 query_everywhere-0.1.9/PKG-INFO
```

### Comparing `query_everywhere-0.1.8/README.md` & `query_everywhere-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -53,7 +53,8 @@
 | gt | greater than |
 | lte | less than or equal to |
 | gte | greater than or equal to |
 | startswith | starts with the given value |
 | endswith | ends with the given value |
 | contains | contains the given value |
 | icontains | contains the given value in the case-insensitive way |
+| isnull | is null |
```

### Comparing `query_everywhere-0.1.8/PKG-INFO` & `query_everywhere-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: query-everywhere
-Version: 0.1.8
+Version: 0.1.9
 Summary: Query every resource in RDBMS for REST
 Author: -LAN-
 Author-email: laipz8200@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: sqlalchemy (>=2.0.19,<3.0.0)
@@ -65,8 +65,9 @@
 | gt | greater than |
 | lte | less than or equal to |
 | gte | greater than or equal to |
 | startswith | starts with the given value |
 | endswith | ends with the given value |
 | contains | contains the given value |
 | icontains | contains the given value in the case-insensitive way |
+| isnull | is null |
```

