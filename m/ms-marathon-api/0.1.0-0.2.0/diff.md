# Comparing `tmp/ms_marathon_api-0.1.0.tar.gz` & `tmp/ms_marathon_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_marathon_api-0.1.0.tar", max compression
+gzip compressed data, was "ms_marathon_api-0.2.0.tar", max compression
```

## Comparing `ms_marathon_api-0.1.0.tar` & `ms_marathon_api-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    35149 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/LICENSE
--rw-r--r--   0        0        0      614 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/__tests__/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__tests__/__init__.py
--rw-r--r--   0        0        0     4368 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__tests__/test_timereporting.py
--rw-r--r--   0        0        0     1579 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/timereporting.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__tests__/__init__.py
--rw-r--r--   0        0        0     2692 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py
--rw-r--r--   0        0        0     1167 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/mysql.py
--rw-r--r--   0        0        0     2300 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/dto/TimeReportingDTO.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/dto/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/queries/__init__.py
--rw-r--r--   0        0        0      228 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/ms_marathon_api/marathon/queries/marathon.py
--rw-r--r--   0        0        0      959 2023-07-19 09:40:14.332314 ms_marathon_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 ms_marathon_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0      614 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/__tests__/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/api/__tests__/__init__.py
+-rw-r--r--   0        0        0     4368 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/api/__tests__/test_timereporting.py
+-rw-r--r--   0        0        0     1808 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/api/timereporting.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/connection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/connection/__tests__/__init__.py
+-rw-r--r--   0        0        0     2692 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py
+-rw-r--r--   0        0        0     1167 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/connection/mysql.py
+-rw-r--r--   0        0        0     2300 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/dto/TimeReportingDTO.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/dto/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/queries/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/ms_marathon_api/marathon/queries/marathon.py
+-rw-r--r--   0        0        0      959 2023-07-20 10:00:38.163564 ms_marathon_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 ms_marathon_api-0.2.0/PKG-INFO
```

### Comparing `ms_marathon_api-0.1.0/LICENSE` & `ms_marathon_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.1.0/README.md` & `ms_marathon_api-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/__tests__/test_timereporting.py` & `ms_marathon_api-0.2.0/ms_marathon_api/marathon/api/__tests__/test_timereporting.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.1.0/ms_marathon_api/marathon/api/timereporting.py` & `ms_marathon_api-0.2.0/ms_marathon_api/marathon/api/timereporting.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,18 +36,22 @@
         )
 
         self.mysql_connection.close()
 
         return timereportings
 
     def export_to_bigquery(self, dataset_id, project_name, table_name, data):
+        BIGQUERY_DELETE_QUERY = f"DELETE FROM `{project_name}.{dataset_id}.{table_name}` WHERE TRUE"  # noqa: E501
         bigquery_manager = BigQueryManager(
             project_id=project_name, dataset_id=dataset_id
         )
 
         bigquery_manager.create_table_if_not_exists(
             table_id=table_name, schema=BIGQUERY_TABLE_SCHEMA
         )
 
+        # Deleting all data before insert it again
+        bigquery_manager.execute_query(BIGQUERY_DELETE_QUERY)
+
         bigquery_manager.load_massive_data(
             rows_to_insert=data, table_name=table_name
         )
```

### Comparing `ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py` & `ms_marathon_api-0.2.0/ms_marathon_api/marathon/connection/__tests__/test_mysql_connection.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.1.0/ms_marathon_api/marathon/connection/mysql.py` & `ms_marathon_api-0.2.0/ms_marathon_api/marathon/connection/mysql.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.1.0/ms_marathon_api/marathon/dto/TimeReportingDTO.py` & `ms_marathon_api-0.2.0/ms_marathon_api/marathon/dto/TimeReportingDTO.py`

 * *Files identical despite different names*

### Comparing `ms_marathon_api-0.1.0/pyproject.toml` & `ms_marathon_api-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-marathon-api"
-version = "0.1.0"
+version = "0.2.0"
 description = "API to connect with Marathon system and migrate data to Bigquery"
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_marathon_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_marathon_api-0.1.0/PKG-INFO` & `ms_marathon_api-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-marathon-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: API to connect with Marathon system and migrate data to Bigquery
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

