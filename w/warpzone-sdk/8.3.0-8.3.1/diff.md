# Comparing `tmp/warpzone_sdk-8.3.0.tar.gz` & `tmp/warpzone_sdk-8.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "warpzone_sdk-8.3.0.tar", max compression
+gzip compressed data, was "warpzone_sdk-8.3.1.tar", max compression
```

## Comparing `warpzone_sdk-8.3.0.tar` & `warpzone_sdk-8.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1071 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/pyproject.toml
--rw-r--r--   0        0        0     1293 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/__init__.py
--rw-r--r--   0        0        0       21 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/blobstorage/__init__.py
--rw-r--r--   0        0        0     2844 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/blobstorage/client.py
--rw-r--r--   0        0        0       24 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/enums/__init__.py
--rw-r--r--   0        0        0      213 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/enums/topicenum.py
--rw-r--r--   0        0        0       27 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/__init__.py
--rw-r--r--   0        0        0     2108 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/functionize.py
--rw-r--r--   0        0        0     3840 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/integrations.py
--rw-r--r--   0        0        0     2223 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/monitor.py
--rw-r--r--   0        0        0     2105 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/process.py
--rw-r--r--   0        0        0       46 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/processors/__init__.py
--rw-r--r--   0        0        0      781 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/processors/dependencies.py
--rw-r--r--   0        0        0     2067 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/processors/outputs.py
--rw-r--r--   0        0        0     1727 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/processors/triggers.py
--rw-r--r--   0        0        0     2268 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/signature.py
--rw-r--r--   0        0        0      547 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/function/types.py
--rw-r--r--   0        0        0     2108 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/healthchecks/__init__.py
--rw-r--r--   0        0        0     1112 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/healthchecks/model.py
--rw-r--r--   0        0        0       87 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/monitor/__init__.py
--rw-r--r--   0        0        0     1650 2023-07-14 06:03:28.491162 warpzone_sdk-8.3.0/warpzone/monitor/logs.py
--rw-r--r--   0        0        0     4781 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/monitor/traces.py
--rw-r--r--   0        0        0       21 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/servicebus/data/__init__.py
--rw-r--r--   0        0        0     5636 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/servicebus/data/client.py
--rw-r--r--   0        0        0       21 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/servicebus/events/__init__.py
--rw-r--r--   0        0        0     4250 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/servicebus/events/client.py
--rw-r--r--   0        0        0       21 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/db/__init__.py
--rw-r--r--   0        0        0     1317 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/db/base_client.py
--rw-r--r--   0        0        0     1422 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/db/client.py
--rw-r--r--   0        0        0     1148 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/db/client_async.py
--rw-r--r--   0        0        0       47 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/tables/__init__.py
--rw-r--r--   0        0        0     2916 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/tables/client.py
--rw-r--r--   0        0        0     2516 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/tables/client_async.py
--rw-r--r--   0        0        0      521 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/tables/helpers.py
--rw-r--r--   0        0        0     2470 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/tablestorage/tables/operations.py
--rw-r--r--   0        0        0      248 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/testing/__init__.py
--rw-r--r--   0        0        0     3661 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/testing/assertions.py
--rw-r--r--   0        0        0     3661 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/testing/data.py
--rw-r--r--   0        0        0       27 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/transform/__init__.py
--rw-r--r--   0        0        0     1641 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/transform/data.py
--rw-r--r--   0        0        0     1968 2023-07-14 06:03:28.495163 warpzone_sdk-8.3.0/warpzone/transform/schema.py
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1293 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/__init__.py
+-rw-r--r--   0        0        0       21 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/blobstorage/__init__.py
+-rw-r--r--   0        0        0     2844 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/blobstorage/client.py
+-rw-r--r--   0        0        0       24 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/enums/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/enums/topicenum.py
+-rw-r--r--   0        0        0       27 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/__init__.py
+-rw-r--r--   0        0        0     2108 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/functionize.py
+-rw-r--r--   0        0        0     3840 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/integrations.py
+-rw-r--r--   0        0        0     2223 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/monitor.py
+-rw-r--r--   0        0        0     2105 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/process.py
+-rw-r--r--   0        0        0       46 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/processors/__init__.py
+-rw-r--r--   0        0        0      781 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/processors/dependencies.py
+-rw-r--r--   0        0        0     2067 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/processors/outputs.py
+-rw-r--r--   0        0        0     1727 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/processors/triggers.py
+-rw-r--r--   0        0        0     2268 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/signature.py
+-rw-r--r--   0        0        0      547 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/function/types.py
+-rw-r--r--   0        0        0     2108 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/healthchecks/__init__.py
+-rw-r--r--   0        0        0     1112 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/healthchecks/model.py
+-rw-r--r--   0        0        0       87 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/monitor/__init__.py
+-rw-r--r--   0        0        0     1650 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/monitor/logs.py
+-rw-r--r--   0        0        0     4781 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/monitor/traces.py
+-rw-r--r--   0        0        0       21 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/servicebus/data/__init__.py
+-rw-r--r--   0        0        0     5636 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/servicebus/data/client.py
+-rw-r--r--   0        0        0       21 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/servicebus/events/__init__.py
+-rw-r--r--   0        0        0     4250 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/servicebus/events/client.py
+-rw-r--r--   0        0        0       21 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/db/__init__.py
+-rw-r--r--   0        0        0     1315 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/db/base_client.py
+-rw-r--r--   0        0        0     1422 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/db/client.py
+-rw-r--r--   0        0        0     1148 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/db/client_async.py
+-rw-r--r--   0        0        0       47 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/tables/__init__.py
+-rw-r--r--   0        0        0     2916 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/tables/client.py
+-rw-r--r--   0        0        0     2516 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/tables/client_async.py
+-rw-r--r--   0        0        0      521 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/tables/helpers.py
+-rw-r--r--   0        0        0     2470 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/tablestorage/tables/operations.py
+-rw-r--r--   0        0        0      248 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/testing/__init__.py
+-rw-r--r--   0        0        0     3661 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/testing/assertions.py
+-rw-r--r--   0        0        0     3661 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/testing/data.py
+-rw-r--r--   0        0        0       27 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/transform/__init__.py
+-rw-r--r--   0        0        0     1641 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/transform/data.py
+-rw-r--r--   0        0        0     1968 2023-07-20 10:30:52.769883 warpzone_sdk-8.3.1/warpzone/transform/schema.py
+-rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 warpzone_sdk-8.3.1/PKG-INFO
```

### Comparing `warpzone_sdk-8.3.0/pyproject.toml` & `warpzone_sdk-8.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "warpzone-sdk"
-version = "8.3.0"
+version = "8.3.1"
 description = "The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage"
 authors = ["Mikkel Ladekarl Folmersen Nygaard <mny@energinet.dk>", "Ulrik Christensen <uch@energinet.dk>"]
 packages = [
     { include = "warpzone" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `warpzone_sdk-8.3.0/warpzone/__init__.py` & `warpzone_sdk-8.3.1/warpzone/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/blobstorage/client.py` & `warpzone_sdk-8.3.1/warpzone/blobstorage/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/functionize.py` & `warpzone_sdk-8.3.1/warpzone/function/functionize.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/integrations.py` & `warpzone_sdk-8.3.1/warpzone/function/integrations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/monitor.py` & `warpzone_sdk-8.3.1/warpzone/function/monitor.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/process.py` & `warpzone_sdk-8.3.1/warpzone/function/process.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/processors/dependencies.py` & `warpzone_sdk-8.3.1/warpzone/function/processors/dependencies.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/processors/outputs.py` & `warpzone_sdk-8.3.1/warpzone/function/processors/outputs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/processors/triggers.py` & `warpzone_sdk-8.3.1/warpzone/function/processors/triggers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/signature.py` & `warpzone_sdk-8.3.1/warpzone/function/signature.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/function/types.py` & `warpzone_sdk-8.3.1/warpzone/function/types.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/healthchecks/__init__.py` & `warpzone_sdk-8.3.1/warpzone/healthchecks/__init__.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/healthchecks/model.py` & `warpzone_sdk-8.3.1/warpzone/healthchecks/model.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/monitor/logs.py` & `warpzone_sdk-8.3.1/warpzone/monitor/logs.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/monitor/traces.py` & `warpzone_sdk-8.3.1/warpzone/monitor/traces.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/servicebus/data/client.py` & `warpzone_sdk-8.3.1/warpzone/servicebus/data/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/servicebus/events/client.py` & `warpzone_sdk-8.3.1/warpzone/servicebus/events/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/db/base_client.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/db/base_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 
 def generate_query_string(time_interval: pd.Interval) -> str:
     if time_interval:
         start_time_str = time_interval.left.strftime(TABLE_STORAGE_TIME_FORMAT)
         end_time_str = time_interval.right.strftime(TABLE_STORAGE_TIME_FORMAT)
         return (
-            f"((PartitionKey ge '{start_time_str}')"
-            f" and (PartitionKey le '{end_time_str}'))"
+            f"(PartitionKey ge '{start_time_str}')"
+            f" and (PartitionKey le '{end_time_str}')"
         )
     else:
         return ""
 
 
 def generate_dataframe_from_records(
     records: list[dict], blob_client: WarpzoneBlobClient
```

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/db/client.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/db/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/db/client_async.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/db/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/tables/client.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/tables/client.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/tables/client_async.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/tables/client_async.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/tables/helpers.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/tables/helpers.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/tablestorage/tables/operations.py` & `warpzone_sdk-8.3.1/warpzone/tablestorage/tables/operations.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/testing/assertions.py` & `warpzone_sdk-8.3.1/warpzone/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/testing/data.py` & `warpzone_sdk-8.3.1/warpzone/testing/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/transform/data.py` & `warpzone_sdk-8.3.1/warpzone/transform/data.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/warpzone/transform/schema.py` & `warpzone_sdk-8.3.1/warpzone/transform/schema.py`

 * *Files identical despite different names*

### Comparing `warpzone_sdk-8.3.0/PKG-INFO` & `warpzone_sdk-8.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: warpzone-sdk
-Version: 8.3.0
+Version: 8.3.1
 Summary: The main objective of this package is to centralize logic used to interact with Azure Functions, Azure Service Bus and Azure Table Storage
 Author: Mikkel Ladekarl Folmersen Nygaard
 Author-email: mny@energinet.dk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

