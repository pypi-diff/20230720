# Comparing `tmp/abnosql-0.0.3.tar.gz` & `tmp/abnosql-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.3.tar", last modified: Tue Jul 18 02:48:48 2023, max compression
+gzip compressed data, was "abnosql-0.0.4.tar", last modified: Thu Jul 20 12:00:28 2023, max compression
```

## Comparing `abnosql-0.0.3.tar` & `abnosql-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 02:48:34.000000 abnosql-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-18 02:48:48.687415 abnosql-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14393 2023-07-18 02:48:34.000000 abnosql-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/kms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/mock_azure_kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/plugins/kms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/kms/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/kms/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-18 02:48:34.000000 abnosql-0.0.3/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:48:48.687415 abnosql-0.0.3/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15521 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 02:48:48.000000 abnosql-0.0.3/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 02:48:48.691414 abnosql-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-18 02:48:34.000000 abnosql-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 12:00:12.000000 abnosql-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-07-20 12:00:28.544541 abnosql-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14946 2023-07-20 12:00:12.000000 abnosql-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/kms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/mock_azure_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/plugins/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/kms/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/kms/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 12:00:28.544541 abnosql-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-20 12:00:12.000000 abnosql-0.0.4/setup.py
```

### Comparing `abnosql-0.0.3/LICENSE` & `abnosql-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/PKG-INFO` & `abnosql-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.3
+Version: 0.0.4
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
@@ -117,15 +117,15 @@
 assert tb.query({'hk': '1'})['items'] == [item]
 
 # scan
 assert tb.query()['items'] == [item]
 
 # be careful not to use cloud specific statements!
 assert tb.query_sql(
-    'SELECT * FROM mytable WHERE hk = @hk AND num > @num',
+    'SELECT * FROM mytable WHERE mytable.hk = @hk AND mytable.num > @num',
     {'@hk': '1', '@num': 4}
 )['items'] == [item]
 
 tb.delete_item({'hk': '1', 'rk': 'a'})
 ```
 
 ## API Docs
@@ -210,25 +210,33 @@
 
 This works for AWS DyanmoDB, however Azure Cosmos has a limitation with continuation token for cross partitions queries (see [Python SDK documentation](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos)).  For Cosmos, abnosql appends OFFSET and LIMIT in the SQL statement if not already present, and returns `next`.  `limit` is defaulted to 100.  See the tests for examples
 
 ## Audit
 
 `put_item()` and `put_items()` take an optional `user` kwarg.  If supplied, absnosql will add the following to the item:
 
-- `created_by` - value of `user`, added if does not exist in item supplied to put_item()
-- `created_date` - UTC ISO timestamp string, added if does not exist
-- `modified_by` - value of `user` always added
-- `modified_date` - UTC ISO timestamp string, always added
+- `createdBy` - value of `user`, added if does not exist in item supplied to put_item()
+- `createdDate` - UTC ISO timestamp string, added if does not exist
+- `modifiedBy` - value of `user` always added
+- `modifiedDate` - UTC ISO timestamp string, always added
 
 Because abnosql doesnt first check if the item already exists, and doesn't support update expressions, there can be a risk with the created* values being re-added if the existing item is not read first and then supplied to put_item(). Its up to application logic to do this - using this feature or not :-)
 
+If you prefer snake_case over CamelCase, you can set env var `ABNOSQ_AUDIT_CAMELCASE` = `FALSE`
+
 # Configuration
 
 It is recommended to use environment variables where possible to avoid provider specific application code
 
+if `ABNOSQL_DB` env var is not set, abnosql will attempt to apply defaults based on available environment variables:
+
+- `AWS_DEFAULT_REGION` - sets database to `dynamodb` (see [aws docs](https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html))
+- `FUNCTIONS_WORKER_RUNTIME` - sets database to `cosmos` (see [azure docs](https://learn.microsoft.com/en-us/azure/azure-functions/functions-app-settings#functions_worker_runtime))
+
+
 ## AWS DynamoDB
 
 Set the following environment variable and use the usual AWS environment variables that boto3 uses
 
 - `ABNOSQL_DB` = "dynamodb"
 
 Or set the boto3 session in the config
```

### Comparing `abnosql-0.0.3/README.md` & `abnosql-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 assert tb.query({'hk': '1'})['items'] == [item]
 
 # scan
 assert tb.query()['items'] == [item]
 
 # be careful not to use cloud specific statements!
 assert tb.query_sql(
-    'SELECT * FROM mytable WHERE hk = @hk AND num > @num',
+    'SELECT * FROM mytable WHERE mytable.hk = @hk AND mytable.num > @num',
     {'@hk': '1', '@num': 4}
 )['items'] == [item]
 
 tb.delete_item({'hk': '1', 'rk': 'a'})
 ```
 
 ## API Docs
@@ -174,25 +174,33 @@
 
 This works for AWS DyanmoDB, however Azure Cosmos has a limitation with continuation token for cross partitions queries (see [Python SDK documentation](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos)).  For Cosmos, abnosql appends OFFSET and LIMIT in the SQL statement if not already present, and returns `next`.  `limit` is defaulted to 100.  See the tests for examples
 
 ## Audit
 
 `put_item()` and `put_items()` take an optional `user` kwarg.  If supplied, absnosql will add the following to the item:
 
-- `created_by` - value of `user`, added if does not exist in item supplied to put_item()
-- `created_date` - UTC ISO timestamp string, added if does not exist
-- `modified_by` - value of `user` always added
-- `modified_date` - UTC ISO timestamp string, always added
+- `createdBy` - value of `user`, added if does not exist in item supplied to put_item()
+- `createdDate` - UTC ISO timestamp string, added if does not exist
+- `modifiedBy` - value of `user` always added
+- `modifiedDate` - UTC ISO timestamp string, always added
 
 Because abnosql doesnt first check if the item already exists, and doesn't support update expressions, there can be a risk with the created* values being re-added if the existing item is not read first and then supplied to put_item(). Its up to application logic to do this - using this feature or not :-)
 
+If you prefer snake_case over CamelCase, you can set env var `ABNOSQ_AUDIT_CAMELCASE` = `FALSE`
+
 # Configuration
 
 It is recommended to use environment variables where possible to avoid provider specific application code
 
+if `ABNOSQL_DB` env var is not set, abnosql will attempt to apply defaults based on available environment variables:
+
+- `AWS_DEFAULT_REGION` - sets database to `dynamodb` (see [aws docs](https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html))
+- `FUNCTIONS_WORKER_RUNTIME` - sets database to `cosmos` (see [azure docs](https://learn.microsoft.com/en-us/azure/azure-functions/functions-app-settings#functions_worker_runtime))
+
+
 ## AWS DynamoDB
 
 Set the following environment variable and use the usual AWS environment variables that boto3 uses
 
 - `ABNOSQL_DB` = "dynamodb"
 
 Or set the boto3 session in the config
```

### Comparing `abnosql-0.0.3/abnosql/cli.py` & `abnosql-0.0.4/abnosql/cli.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/kms.py` & `abnosql-0.0.4/abnosql/kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/mocks/mock_azure_kms.py` & `abnosql-0.0.4/abnosql/mocks/mock_azure_kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.4/abnosql/mocks/mock_cosmos.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.4/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/plugin.py` & `abnosql-0.0.4/abnosql/plugin.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/plugins/kms/aws.py` & `abnosql-0.0.4/abnosql/plugins/kms/aws.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/plugins/kms/azure.py` & `abnosql-0.0.4/abnosql/plugins/kms/azure.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.4/abnosql/plugins/table/cosmos.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.4/abnosql/plugins/table/dynamodb.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/plugins/table/memory.py` & `abnosql-0.0.4/abnosql/plugins/table/memory.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql/table.py` & `abnosql-0.0.4/abnosql/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -428,23 +428,26 @@
         item: item dict
         user: user/system ID string
 
     Returns:
         item
 
     """
+    camel_case = os.environ.get('ABNOSQL_AUDIT_CAMELCASE', 'TRUE') == 'TRUE'
+    by_attr = 'By' if camel_case else '_by'
+    date_attr = 'Date' if camel_case else '_date'
     dt_iso = datetime.now(timezone.utc).strftime('%Y-%m-%dT%H:%M:%SZ')
-    if 'created_by' not in item:
+    if f'created{by_attr}' not in item:
         item.update({
-            'created_by': user,
-            'created_date': dt_iso
+            f'created{by_attr}': user,
+            f'created{date_attr}': dt_iso
         })
     item.update({
-        'modified_by': user,
-        'modified_date': dt_iso
+        f'modified{by_attr}': user,
+        f'modified{date_attr}': dt_iso
     })
     return item
 
 
 def parse_connstr():
     connstr = os.environ.get('ABNOSQL_DB')
     if connstr:
@@ -467,15 +470,29 @@
 
     Returns:
         TableBase object
 
     """
     if database is None:
         p = parse_connstr()
-        database = p.scheme or p.path
+        database = p.scheme or p.path if p else None
+
+    # infer database from available env vars
+    # aws: https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html  # noqa
+    # azure: https://learn.microsoft.com/en-us/azure/azure-functions/functions-app-settings#azure_functions_environment  # noqa
+    if database is None:
+        defaults = {
+            'AWS_DEFAULT_REGION': 'dynamodb',
+            'FUNCTIONS_WORKER_RUNTIME': 'cosmos'
+        }
+        for envvar, _database in defaults.items():
+            if os.environ.get(envvar) is not None:
+                database = _database
+                break
+
     pm = plugin.get_pm('table')
     module = pm.get_plugin(database)
     if module is None:
         raise ex.PluginException(f'table.{database} plugin not found')
     if not isinstance(config, dict):
         config = {}
     _module = module.Table(pm, name, config)
```

### Comparing `abnosql-0.0.3/abnosql.egg-info/PKG-INFO` & `abnosql-0.0.4/abnosql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.3
+Version: 0.0.4
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
@@ -117,15 +117,15 @@
 assert tb.query({'hk': '1'})['items'] == [item]
 
 # scan
 assert tb.query()['items'] == [item]
 
 # be careful not to use cloud specific statements!
 assert tb.query_sql(
-    'SELECT * FROM mytable WHERE hk = @hk AND num > @num',
+    'SELECT * FROM mytable WHERE mytable.hk = @hk AND mytable.num > @num',
     {'@hk': '1', '@num': 4}
 )['items'] == [item]
 
 tb.delete_item({'hk': '1', 'rk': 'a'})
 ```
 
 ## API Docs
@@ -210,25 +210,33 @@
 
 This works for AWS DyanmoDB, however Azure Cosmos has a limitation with continuation token for cross partitions queries (see [Python SDK documentation](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos)).  For Cosmos, abnosql appends OFFSET and LIMIT in the SQL statement if not already present, and returns `next`.  `limit` is defaulted to 100.  See the tests for examples
 
 ## Audit
 
 `put_item()` and `put_items()` take an optional `user` kwarg.  If supplied, absnosql will add the following to the item:
 
-- `created_by` - value of `user`, added if does not exist in item supplied to put_item()
-- `created_date` - UTC ISO timestamp string, added if does not exist
-- `modified_by` - value of `user` always added
-- `modified_date` - UTC ISO timestamp string, always added
+- `createdBy` - value of `user`, added if does not exist in item supplied to put_item()
+- `createdDate` - UTC ISO timestamp string, added if does not exist
+- `modifiedBy` - value of `user` always added
+- `modifiedDate` - UTC ISO timestamp string, always added
 
 Because abnosql doesnt first check if the item already exists, and doesn't support update expressions, there can be a risk with the created* values being re-added if the existing item is not read first and then supplied to put_item(). Its up to application logic to do this - using this feature or not :-)
 
+If you prefer snake_case over CamelCase, you can set env var `ABNOSQ_AUDIT_CAMELCASE` = `FALSE`
+
 # Configuration
 
 It is recommended to use environment variables where possible to avoid provider specific application code
 
+if `ABNOSQL_DB` env var is not set, abnosql will attempt to apply defaults based on available environment variables:
+
+- `AWS_DEFAULT_REGION` - sets database to `dynamodb` (see [aws docs](https://docs.aws.amazon.com/lambda/latest/dg/configuration-envvars.html))
+- `FUNCTIONS_WORKER_RUNTIME` - sets database to `cosmos` (see [azure docs](https://learn.microsoft.com/en-us/azure/azure-functions/functions-app-settings#functions_worker_runtime))
+
+
 ## AWS DynamoDB
 
 Set the following environment variable and use the usual AWS environment variables that boto3 uses
 
 - `ABNOSQL_DB` = "dynamodb"
 
 Or set the boto3 session in the config
```

### Comparing `abnosql-0.0.3/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.4/abnosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/abnosql.egg-info/requires.txt` & `abnosql-0.0.4/abnosql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.3/setup.py` & `abnosql-0.0.4/setup.py`

 * *Files identical despite different names*

