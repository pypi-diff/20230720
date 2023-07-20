# Comparing `tmp/abnosql-0.0.4.tar.gz` & `tmp/abnosql-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abnosql-0.0.4.tar", last modified: Thu Jul 20 12:00:28 2023, max compression
+gzip compressed data, was "abnosql-0.0.5.tar", last modified: Thu Jul 20 17:24:57 2023, max compression
```

## Comparing `abnosql-0.0.4.tar` & `abnosql-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 12:00:12.000000 abnosql-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-07-20 12:00:28.544541 abnosql-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14946 2023-07-20 12:00:12.000000 abnosql-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/kms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/mock_azure_kms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/mock_cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/mocks/mock_dynamodbx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/plugins/kms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/kms/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/kms/azure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql/plugins/table/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/cosmos.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     7772 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/plugins/table/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    13533 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/table.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 12:00:12.000000 abnosql-0.0.4/abnosql/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:00:28.544541 abnosql-0.0.4/abnosql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16074 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 12:00:28.000000 abnosql-0.0.4/abnosql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 12:00:28.544541 abnosql-0.0.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-20 12:00:12.000000 abnosql-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-20 17:24:39.000000 abnosql-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-20 17:24:57.727913 abnosql-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-07-20 17:24:39.000000 abnosql-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4095 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/kms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/mock_azure_kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/mock_cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/mocks/mock_dynamodbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/plugins/kms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/kms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/kms/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/kms/azure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql/plugins/table/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/cosmos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/plugins/table/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 17:24:39.000000 abnosql-0.0.5/abnosql/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:24:57.727913 abnosql-0.0.5/abnosql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16918 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 17:24:57.000000 abnosql-0.0.5/abnosql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-20 17:24:57.727913 abnosql-0.0.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2818 2023-07-20 17:24:39.000000 abnosql-0.0.5/setup.py
```

### Comparing `abnosql-0.0.4/LICENSE` & `abnosql-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/PKG-INFO` & `abnosql-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.4
+Version: 0.0.5
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
@@ -49,14 +49,15 @@
 
 - [NoSQL Abstraction Library](#nosql-abstraction-library)
   - [Installation](#installation)
 - [Usage](#usage)
   - [API Docs](#api-docs)
   - [Querying](#querying)
   - [Indexes](#indexes)
+  - [Updates](#updates)
   - [Partition Keys](#partition-keys)
   - [Client Side Encryption](#client-side-encryption)
   - [Pagination](#pagination)
   - [Audit](#audit)
 - [Configuration](#configuration)
   - [AWS DynamoDB](#aws-dynamodb)
   - [Azure Cosmos NoSQL](#azure-cosmos-nosql)
@@ -88,14 +89,15 @@
 # Usage
 
 ```
 from abnosql import table
 import os
 
 os.environ['ABNOSQL_DB'] = 'dynamodb'
+os.environ['ABNOSQL_KEY_ATTRS'] = 'hk,rk'
 
 item = {
     'hk': '1',
     'rk': 'a',
     'num': 5,
     'obj': {
         'foo': 'bar',
@@ -104,15 +106,25 @@
     },
     'list': [1, 2, 3],
     'str': 'str'
 }
 
 tb = table('mytable')
 
+# create/replace
 tb.put_item(item)
+
+# update - using ABNOSQL_KEY_ATTRS
+updated_item = tb.put_item(
+    {'hk': '1', 'rk': 'a', 'str': 'STR'},
+    update=True
+)
+assert updated_item['str'] == 'STR'
+
+# bulk
 tb.put_items([item])
 
 # note partition/hash key should be first kwarg
 assert tb.get_item(hk='1', rk='a') == item
 
 assert tb.query({'hk': '1'})['items'] == [item]
 
@@ -143,14 +155,26 @@
 Care should be taken with `query_sql()` to not to use SQL features that are specific to any specific provider (breaking the abstraction capability of using abnosql in the first place)
 
 ## Indexes
 
 Beyond partition and range keys defined on the table, indexes are not currently supported - and these will likey differ between providers anyway (eg DynamoDB supports [Secondary Indexes](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/SecondaryIndexes.html), whereas [Cosmos](https://learn.microsoft.com/en-us/azure/cosmos-db/index-overview) has Range, Spatial and Composite.
 
 
+## Updates
+
+`put_item()` and `put_items()` support `update` boolean attribute, which if supplied will do an `update_item()` on DynamoDB, and a `patch_item()` on Cosmos.  For this to work however, you must specify the key attribute names, either via `ABNOSQL_KEY_ATTRS` env var as a comma separated list (eg perhaps multiple tables all share common partition/range key scheme), or as the `key_attrs` config item  when instantiating the table, eg:
+
+```
+tb = table('mytable', {'key_attrs': ['hk', 'rk']})
+```
+
+If you don't need to do any updates and only need to do create/replace, then these key attribute names do not need to be supplied
+
+All items being updated must actually exist first, or else exception raised
+
 ## Partition Keys
 
 A few methods such as `get_item()`, `delete_item()` and `query()` need to know partition/hash keys as defined on the table.  To avoid having to configure this or lookup from the provider, the convention used is that the first kwarg or dictionary item is the partition key, and if supplied the 2nd is the range/sort key.
 
 ## Client Side Encryption
 
 If configured in table config with `kms` attribute, abnosql will perform client side encryption using AWS KMS or Azure KeyVault
@@ -174,15 +198,15 @@
         'attrs': ['obj', 'str']
     }
 }
 ```
 
 Where:
 - `key_ids`: list of AWS KMS Key ARNs or Azure KeyVault identifier (URL to RSA CMK).  This is picked up via `ABNOSQL_KMS_KEYS` env var as a comma separated list (*NOTE: env var recommended to avoid provider specific code*)
-- `key_attrs`: list of key attributes in the item from which the AAD/encryption context is set
+- `key_attrs`: list of key attributes in the item from which the AAD/encryption context is set.  Taken from `ABNOSQL_KEY_ATTRS` env var or table `key_attrs` if defined there
 - `attrs`: list of attributes keys to encrypt
 - `key_bytes`: optional for azure, use your own AESGCM key if specified, otherwise generate one
 
 If `kms` config attribute is present, abnosql will look for the `ABNOSQL_KMS` provider to load the appropriate provider KMS module (eg "aws" or "azure"), and if not present use default depending on the database (eg cosmos will use azure, dynamodb will use aws)
 
 In example above, the key_attrs `['hk', 'rk']` are used to define the encryption context / AAD used, and attrs `['obj', 'str']` what attributes to encrypt/decrypt
 
@@ -208,24 +232,24 @@
 
 `query` and `query_sql` accept `limit` and `next` optional kwargs and return `next` in response. Use these to paginate.
 
 This works for AWS DyanmoDB, however Azure Cosmos has a limitation with continuation token for cross partitions queries (see [Python SDK documentation](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos)).  For Cosmos, abnosql appends OFFSET and LIMIT in the SQL statement if not already present, and returns `next`.  `limit` is defaulted to 100.  See the tests for examples
 
 ## Audit
 
-`put_item()` and `put_items()` take an optional `user` kwarg.  If supplied, absnosql will add the following to the item:
+`put_item()` and `put_items()` take an optional `audit_user` kwarg.  If supplied, absnosql will add the following to the item:
 
-- `createdBy` - value of `user`, added if does not exist in item supplied to put_item()
+- `createdBy` - value of `audit_user`, added if does not exist in item supplied to put_item()
 - `createdDate` - UTC ISO timestamp string, added if does not exist
-- `modifiedBy` - value of `user` always added
+- `modifiedBy` - value of `audit_user` always added
 - `modifiedDate` - UTC ISO timestamp string, always added
 
-Because abnosql doesnt first check if the item already exists, and doesn't support update expressions, there can be a risk with the created* values being re-added if the existing item is not read first and then supplied to put_item(). Its up to application logic to do this - using this feature or not :-)
+NOTE: created* will only be added if `update` is not True in a `put_item()` operation
 
-If you prefer snake_case over CamelCase, you can set env var `ABNOSQ_AUDIT_CAMELCASE` = `FALSE`
+If you prefer snake_case over CamelCase, you can set env var `ABNOSQL_AUDIT_CAMELCASE` = `FALSE`
 
 # Configuration
 
 It is recommended to use environment variables where possible to avoid provider specific application code
 
 if `ABNOSQL_DB` env var is not set, abnosql will attempt to apply defaults based on available environment variables:
```

### Comparing `abnosql-0.0.4/README.md` & `abnosql-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 - [NoSQL Abstraction Library](#nosql-abstraction-library)
   - [Installation](#installation)
 - [Usage](#usage)
   - [API Docs](#api-docs)
   - [Querying](#querying)
   - [Indexes](#indexes)
+  - [Updates](#updates)
   - [Partition Keys](#partition-keys)
   - [Client Side Encryption](#client-side-encryption)
   - [Pagination](#pagination)
   - [Audit](#audit)
 - [Configuration](#configuration)
   - [AWS DynamoDB](#aws-dynamodb)
   - [Azure Cosmos NoSQL](#azure-cosmos-nosql)
@@ -52,14 +53,15 @@
 # Usage
 
 ```
 from abnosql import table
 import os
 
 os.environ['ABNOSQL_DB'] = 'dynamodb'
+os.environ['ABNOSQL_KEY_ATTRS'] = 'hk,rk'
 
 item = {
     'hk': '1',
     'rk': 'a',
     'num': 5,
     'obj': {
         'foo': 'bar',
@@ -68,15 +70,25 @@
     },
     'list': [1, 2, 3],
     'str': 'str'
 }
 
 tb = table('mytable')
 
+# create/replace
 tb.put_item(item)
+
+# update - using ABNOSQL_KEY_ATTRS
+updated_item = tb.put_item(
+    {'hk': '1', 'rk': 'a', 'str': 'STR'},
+    update=True
+)
+assert updated_item['str'] == 'STR'
+
+# bulk
 tb.put_items([item])
 
 # note partition/hash key should be first kwarg
 assert tb.get_item(hk='1', rk='a') == item
 
 assert tb.query({'hk': '1'})['items'] == [item]
 
@@ -107,14 +119,26 @@
 Care should be taken with `query_sql()` to not to use SQL features that are specific to any specific provider (breaking the abstraction capability of using abnosql in the first place)
 
 ## Indexes
 
 Beyond partition and range keys defined on the table, indexes are not currently supported - and these will likey differ between providers anyway (eg DynamoDB supports [Secondary Indexes](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/SecondaryIndexes.html), whereas [Cosmos](https://learn.microsoft.com/en-us/azure/cosmos-db/index-overview) has Range, Spatial and Composite.
 
 
+## Updates
+
+`put_item()` and `put_items()` support `update` boolean attribute, which if supplied will do an `update_item()` on DynamoDB, and a `patch_item()` on Cosmos.  For this to work however, you must specify the key attribute names, either via `ABNOSQL_KEY_ATTRS` env var as a comma separated list (eg perhaps multiple tables all share common partition/range key scheme), or as the `key_attrs` config item  when instantiating the table, eg:
+
+```
+tb = table('mytable', {'key_attrs': ['hk', 'rk']})
+```
+
+If you don't need to do any updates and only need to do create/replace, then these key attribute names do not need to be supplied
+
+All items being updated must actually exist first, or else exception raised
+
 ## Partition Keys
 
 A few methods such as `get_item()`, `delete_item()` and `query()` need to know partition/hash keys as defined on the table.  To avoid having to configure this or lookup from the provider, the convention used is that the first kwarg or dictionary item is the partition key, and if supplied the 2nd is the range/sort key.
 
 ## Client Side Encryption
 
 If configured in table config with `kms` attribute, abnosql will perform client side encryption using AWS KMS or Azure KeyVault
@@ -138,15 +162,15 @@
         'attrs': ['obj', 'str']
     }
 }
 ```
 
 Where:
 - `key_ids`: list of AWS KMS Key ARNs or Azure KeyVault identifier (URL to RSA CMK).  This is picked up via `ABNOSQL_KMS_KEYS` env var as a comma separated list (*NOTE: env var recommended to avoid provider specific code*)
-- `key_attrs`: list of key attributes in the item from which the AAD/encryption context is set
+- `key_attrs`: list of key attributes in the item from which the AAD/encryption context is set.  Taken from `ABNOSQL_KEY_ATTRS` env var or table `key_attrs` if defined there
 - `attrs`: list of attributes keys to encrypt
 - `key_bytes`: optional for azure, use your own AESGCM key if specified, otherwise generate one
 
 If `kms` config attribute is present, abnosql will look for the `ABNOSQL_KMS` provider to load the appropriate provider KMS module (eg "aws" or "azure"), and if not present use default depending on the database (eg cosmos will use azure, dynamodb will use aws)
 
 In example above, the key_attrs `['hk', 'rk']` are used to define the encryption context / AAD used, and attrs `['obj', 'str']` what attributes to encrypt/decrypt
 
@@ -172,24 +196,24 @@
 
 `query` and `query_sql` accept `limit` and `next` optional kwargs and return `next` in response. Use these to paginate.
 
 This works for AWS DyanmoDB, however Azure Cosmos has a limitation with continuation token for cross partitions queries (see [Python SDK documentation](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos)).  For Cosmos, abnosql appends OFFSET and LIMIT in the SQL statement if not already present, and returns `next`.  `limit` is defaulted to 100.  See the tests for examples
 
 ## Audit
 
-`put_item()` and `put_items()` take an optional `user` kwarg.  If supplied, absnosql will add the following to the item:
+`put_item()` and `put_items()` take an optional `audit_user` kwarg.  If supplied, absnosql will add the following to the item:
 
-- `createdBy` - value of `user`, added if does not exist in item supplied to put_item()
+- `createdBy` - value of `audit_user`, added if does not exist in item supplied to put_item()
 - `createdDate` - UTC ISO timestamp string, added if does not exist
-- `modifiedBy` - value of `user` always added
+- `modifiedBy` - value of `audit_user` always added
 - `modifiedDate` - UTC ISO timestamp string, always added
 
-Because abnosql doesnt first check if the item already exists, and doesn't support update expressions, there can be a risk with the created* values being re-added if the existing item is not read first and then supplied to put_item(). Its up to application logic to do this - using this feature or not :-)
+NOTE: created* will only be added if `update` is not True in a `put_item()` operation
 
-If you prefer snake_case over CamelCase, you can set env var `ABNOSQ_AUDIT_CAMELCASE` = `FALSE`
+If you prefer snake_case over CamelCase, you can set env var `ABNOSQL_AUDIT_CAMELCASE` = `FALSE`
 
 # Configuration
 
 It is recommended to use environment variables where possible to avoid provider specific application code
 
 if `ABNOSQL_DB` env var is not set, abnosql will attempt to apply defaults based on available environment variables:
```

### Comparing `abnosql-0.0.4/abnosql/cli.py` & `abnosql-0.0.5/abnosql/cli.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/kms.py` & `abnosql-0.0.5/abnosql/kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/mocks/mock_azure_kms.py` & `abnosql-0.0.5/abnosql/mocks/mock_azure_kms.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/mocks/mock_cosmos.py` & `abnosql-0.0.5/abnosql/mocks/mock_cosmos.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 
 from abnosql.plugins.table.memory import get_table_count
 from abnosql import table
 
 
 KEY_ATTRS: t.Dict[str, t.List[str]] = {}
 CRYPTO_ATTRS: t.Dict[str, t.List[str]] = {}
+COSMOS_POST_PATCH_VALS = {
+    '_rid': '2pFqAMMTYY8BAAAAAAAAAA==',
+    '_self': 'dbs/2pFqAA==/colls/2pFqAMMTYY8=/docs/2pFqAMMTYY8BAAAAAAAAAA==/'
+}
 
 
 def set_keyattrs(key_attrs: t.Dict[str, t.List[str]]):
     global KEY_ATTRS
     KEY_ATTRS = key_attrs
 
 
@@ -100,14 +104,24 @@
             if request.method == 'GET':
                 item = tb.get_item(**key)
                 if item is not None:
                     return _response(200, item)
             elif request.method == 'DELETE':
                 tb.delete_item(**key)
                 return _response(204, None)
+            elif request.method == 'PATCH':
+                data = json.loads(request.body)
+                item = {
+                    _['path'][1:]: _['value']
+                    for _ in data['operations']
+                }
+                item.update(key)
+                item = tb.put_item(item, update=True)
+                item.update(COSMOS_POST_PATCH_VALS)
+                return _response(200, item)
 
         # /dbs/{database}/colls/{table}/docs
         elif len(parts) == 5 and parts[-1] == 'docs':
             if request.method == 'POST':
                 is_query = headers.get('x-ms-documentdb-isquery') == 'true'
                 item = json.loads(request.body)
                 if is_query is True:
@@ -123,28 +137,29 @@
                             get_table_count(table_name)
                         )
                     }
                     return _response(
                         200, {'Documents': items}, headers
                     )
                 else:
-                    tb.put_item(item)
-                return _response(201, None)
+                    item = tb.put_item(item)
+                    item.update(COSMOS_POST_PATCH_VALS)
+                    return _response(201, item)
 
         # upsert_item() reads the collection
         # /dbs/{database}/colls/{table}
         elif len(parts) == 4 and parts[-2] == 'colls':
             if request.method == 'GET':
                 return _response(200, {})
 
         return _response(404)
 
     @functools.wraps(f)
     def decorated(*args, **kwargs):
-        for method in ['GET', 'POST', 'DELETE', 'PUT']:
+        for method in ['GET', 'POST', 'DELETE', 'PUT', 'PATCH']:
             responses.add_callback(
                 getattr(responses, method),
                 re.compile(r'^https://.*.documents.azure.(com|cn).*'),
                 _callback
             )
         return f(*args, **kwargs)
     return decorated
```

### Comparing `abnosql-0.0.4/abnosql/mocks/mock_dynamodbx.py` & `abnosql-0.0.5/abnosql/mocks/mock_dynamodbx.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/plugin.py` & `abnosql-0.0.5/abnosql/plugin.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/plugins/kms/aws.py` & `abnosql-0.0.5/abnosql/plugins/kms/aws.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/plugins/kms/azure.py` & `abnosql-0.0.5/abnosql/plugins/kms/azure.py`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql/plugins/table/cosmos.py` & `abnosql-0.0.5/abnosql/plugins/table/cosmos.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import typing as t
 
 import pluggy  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
 from abnosql.table import add_audit
+from abnosql.table import get_key_attrs
 from abnosql.table import get_sql_params
 from abnosql.table import kms_decrypt_item
 from abnosql.table import kms_encrypt_item
 from abnosql.table import kms_process_query_items
 from abnosql.table import parse_connstr
 from abnosql.table import TableBase
+from abnosql.table import validate_key_attrs
 from abnosql.table import validate_query_attrs
 
 hookimpl = pluggy.HookimplMarker('abnosql.table')
 
 try:
     from azure.cosmos import CosmosClient  # type: ignore
     from azure.cosmos.exceptions import CosmosHttpResponseError  # type: ignore
@@ -72,14 +74,15 @@
 
     def __init__(
         self, pm: PM, name: str, config: t.Optional[dict] = None
     ) -> None:
         self.pm = pm
         self.name = name
         self.set_config(config)
+        self.key_attrs = get_key_attrs(self.config)
         self.database_client = None
 
     @cosmos_ex_handler()
     def set_config(self, config: t.Optional[dict]):
         if config is None:
             config = {}
         _config = self.pm.hook.set_config(table=self.name)
@@ -133,34 +136,53 @@
         item = kms_decrypt_item(self.config, item)
         return item
 
     @cosmos_ex_handler()
     def put_item(
         self,
         item: t.Dict,
-        user: t.Optional[str] = None
-    ):
-        if user:
-            item = add_audit(item, user)
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
+    ) -> t.Dict:
+        if audit_user:
+            item = add_audit(item, update or False, audit_user)
         _item = self.pm.hook.put_item_pre(table=self.name, item=item)
         if _item:
             item = _item[0]
         item = kms_encrypt_item(self.config, item)
-        self._container(self.name).upsert_item(item)
+        # do update
+        if update is True:
+            validate_key_attrs(self.key_attrs, item)
+            key = {k: item.pop(k) for k in self.key_attrs}
+            kwargs = {
+                'item': key[self.key_attrs[-1]],
+                'partition_key': key[self.key_attrs[0]],
+                'patch_operations': [
+                    {'op': 'add', 'path': f'/{k}', 'value': v}
+                    for k, v in item.items()
+                ]
+            }
+            item = self._container(self.name).patch_item(**kwargs)
+        # do create/replace
+        else:
+            item = self._container(self.name).upsert_item(item)
+        item = strip_cosmos_attrs(item)
         self.pm.hook.put_item_post(table=self.name, item=item)
+        return item
 
     @cosmos_ex_handler()
     def put_items(
         self,
         items: t.Iterable[t.Dict],
-        user: t.Optional[str] = None
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
     ):
         # TODO(batch)
         for item in items:
-            self.put_item(item, user)
+            self.put_item(item, update=update, audit_user=audit_user)
         self.pm.hook.put_items_post(table=self.name, items=items)
 
     @cosmos_ex_handler()
     def delete_item(self, **kwargs):
         self._container(self.name).delete_item(
             **get_key_kwargs(**kwargs)
         )
```

### Comparing `abnosql-0.0.4/abnosql/plugins/table/dynamodb.py` & `abnosql-0.0.5/abnosql/plugins/table/dynamodb.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 import typing as t
 
 import pluggy  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
 from abnosql.table import add_audit
+from abnosql.table import get_key_attrs
 from abnosql.table import get_sql_params
 from abnosql.table import kms_decrypt_item
 from abnosql.table import kms_encrypt_item
 from abnosql.table import kms_process_query_items
 from abnosql.table import TableBase
+from abnosql.table import validate_key_attrs
 from abnosql.table import validate_query_attrs
 
 hookimpl = pluggy.HookimplMarker('abnosql.table')
 
 AWS_DEFAULT_REGION = os.environ.get('AWS_DEFAULT_REGION', 'us-east-1')
 
 try:
@@ -146,14 +148,15 @@
         self.name = name
         self.set_config(config)
         self.session = self.config.get(
             'session', boto3.session.Session(
                 region_name=AWS_DEFAULT_REGION
             )
         )
+        self.key_attrs = get_key_attrs(self.config)
         self.table = self.session.resource('dynamodb').Table(name)
 
     @dynamodb_ex_handler()
     def set_config(self, config: t.Optional[dict]):
         if config is None:
             config = {}
         _config = self.pm.hook.set_config(table=self.name)
@@ -174,34 +177,63 @@
         item = kms_decrypt_item(self.config, item)
         return item
 
     @dynamodb_ex_handler()
     def put_item(
         self, item:
         t.Dict,
-        user: t.Optional[str] = None
-    ):
-        if user:
-            item = add_audit(item, user)
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
+    ) -> t.Dict:
+        if audit_user:
+            item = add_audit(item, update or False, audit_user)
         _item = self.pm.hook.put_item_pre(table=self.name, item=item)
         if _item:
             item = _item[0]
         item = kms_encrypt_item(self.config, item)
-        self.table.put_item(Item=item)
+
+        # do update
+        if update is True:
+            validate_key_attrs(self.key_attrs, item)
+            kwargs = {
+                'Key': {k: item.pop(k) for k in self.key_attrs},
+                'ReturnValues': 'ALL_NEW'
+            }
+            exp = []
+            vals = {}
+            aliases = {}
+            for k, v in sorted(item.items()):
+                if isinstance(v, str) and v == '':
+                    v = None
+                aliases['#%s' % k] = k
+                exp.append('#%s = :%s' % (k, k))
+                vals[':%s' % k] = v
+            kwargs['UpdateExpression'] = 'set %s' % ', '.join(exp)
+            kwargs['ExpressionAttributeNames'] = aliases
+            kwargs['ExpressionAttributeValues'] = vals
+            response = self.table.update_item(**kwargs)
+            item.update(response.get('Attributes'))
+
+        # do create/replace
+        else:
+            self.table.put_item(Item=item)
+
         self.pm.hook.put_item_post(table=self.name, item=item)
+        return item
 
     @dynamodb_ex_handler()
     def put_items(
         self,
         items: t.Iterable[t.Dict],
-        user: t.Optional[str] = None
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
     ):
         # TODO(batch)
         for item in items:
-            self.put_item(item, user)
+            self.put_item(item, update=update, audit_user=audit_user)
         self.pm.hook.put_items_post(table=self.name, items=items)
 
     @dynamodb_ex_handler()
     def delete_item(self, **kwargs):
         key = get_key(**kwargs)
         self.table.delete_item(Key=key)
         self.pm.hook.delete_item_post(table=self.name, key=key)
```

### Comparing `abnosql-0.0.4/abnosql/plugins/table/memory.py` & `abnosql-0.0.5/abnosql/plugins/table/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sqlglot.executor import execute  # type: ignore
 from sqlglot import exp  # type: ignore
 from sqlglot import parse_one  # type: ignore
 
 import abnosql.exceptions as ex
 from abnosql.plugin import PM
 from abnosql.table import add_audit
+from abnosql.table import get_key_attrs
 from abnosql.table import get_sql_params
 from abnosql.table import kms_decrypt_item
 from abnosql.table import kms_encrypt_item
 from abnosql.table import kms_process_query_items
 from abnosql.table import quote_str
 from abnosql.table import TableBase
 from abnosql.table import validate_query_attrs
@@ -144,15 +145,15 @@
 
     def __init__(
         self, pm: PM, name: str, config: t.Optional[dict] = None
     ) -> None:
         self.pm = pm
         self.name = name
         self.set_config(config)
-        self.key_attrs = self.config.get('key_attrs', ['id'])
+        self.key_attrs = get_key_attrs(self.config)
         self.items = self.config.get('items', {})
 
     @memory_ex_handler()
     def set_config(self, config: t.Optional[dict]):
         if config is None:
             config = {}
         _config = self.pm.hook.set_config(table=self.name)
@@ -175,37 +176,47 @@
         item = kms_decrypt_item(self.config, item)
         return item
 
     @memory_ex_handler()
     def put_item(
         self,
         item: t.Dict,
-        user: t.Optional[str] = None
-    ):
-        if user:
-            item = add_audit(item, user)
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
+    ) -> t.Dict:
+        if audit_user:
+            item = add_audit(item, update or False, audit_user)
         key = ':'.join([item[_] for _ in self.key_attrs])
         item = kms_encrypt_item(self.config, item)
         if self.items:
-            self.items[key] = item
+            if update is True:
+                self.items[key].update(item)
+            else:
+                self.items[key] = item
         else:
             global TABLES
             if self.name not in TABLES:
                 TABLES[self.name] = {}
-            TABLES[self.name][key] = item
+            if update is True:
+                TABLES[self.name][key].update(item)
+            else:
+                TABLES[self.name][key] = item
+        item = TABLES[self.name][key].copy()
         self.pm.hook.put_item_post(table=self.name, item=item)
+        return item
 
     @memory_ex_handler()
     def put_items(
         self,
         items: t.Iterable[t.Dict],
-        user: t.Optional[str] = None
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
     ):
         for item in items:
-            self.put_item(item, user)
+            self.put_item(item, update=update, audit_user=audit_user)
         self.pm.hook.put_items_post(table=self.name, items=items)
 
     @memory_ex_handler()
     def delete_item(self, **kwargs):
         key = get_key(**kwargs)
         if self.items:
             self.items.pop(key, None)
```

### Comparing `abnosql-0.0.4/abnosql/table.py` & `abnosql-0.0.5/abnosql/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -130,38 +130,46 @@
         """
         pass
 
     @abstractmethod
     def put_item(
         self,
         item: t.Dict,
-        user: t.Optional[str] = None
-    ):
+        update: t.Optional[bool] = False,
+        audit_user: t.Optional[str] = None
+    ) -> t.Dict:
         """Puts table/collection item
 
         Args:
 
             item: dictionary
-            user: optional user / system ID string to add audit atts
+            update: perform update/patch - item must already exist
+            audit_user: optional user / system ID string to add audit attrs
+
+        Returns:
+
+            item: dictionary of created/updated item
 
         """
         pass
 
     @abstractmethod
     def put_items(
         self,
         items: t.Iterable[t.Dict],
+        update: t.Optional[bool] = False,
         audit_user: t.Optional[str] = None
     ):
         """Puts multiple table/collection items
 
         Args:
 
             items: list of item dictionaries
-            user: user / system ID string to add audit attrs
+            update: perform update/patch - items must already exist
+            audit_user: user / system ID string to add audit attrs
 
         """
         pass
 
     @abstractmethod
     def delete_item(self, **kwargs):
         """Deletes table/collection item
@@ -306,14 +314,62 @@
     """
     # sqlglot can do this (and sqlparse), but lets keep it simple
     tokens = [_.strip() for _ in statement.split(' ') if _.strip() != '']
     if len(tokens) == 0 or tokens[0].upper() != 'SELECT':
         raise ex.ValidationException('statement must start with SELECT')
 
 
+def get_key_attrs(config: t.Optional[t.Dict] = None) -> list:
+    """Get key attributes from ABNOSQL_KEY_ATTRS env var or config
+
+    Args:
+
+        config: config dict
+
+    Returns:
+
+        key_attrs: list of key attribute names
+
+    """
+    key_attrs = [
+        _ for _ in os.environ.get('ABNOSQL_KEY_ATTRS', '').split(',')
+        if _.strip() != ''
+    ]
+    _key_attrs = config.get('key_attrs') if isinstance(config, dict) else None
+    if isinstance(_key_attrs, list):
+        key_attrs = _key_attrs
+    if len(key_attrs) > 2:
+        raise ValueError('must not be more than 2 key_attrs defined')
+    return key_attrs
+
+
+def validate_key_attrs(key_attrs: t.Iterable[str], item: t.Dict):
+    """Validate key attributes in either ABNOSQL_KEY_ATTRS env var or config
+
+    Args:
+
+        key_attrs: list of key attribute names
+        config: config dict
+
+    """
+    if not isinstance(key_attrs, list) or len(key_attrs) == 0:
+        raise ex.ValidationException('key_attrs not defined')
+    missing = [
+        k for k in key_attrs if item.get(k) is None
+    ]
+    if len(missing):
+        raise ex.ValidationException(
+            f'key_attrs missing from item: {missing}'
+        )
+    if len(item) - len(key_attrs) <= 0:
+        raise ex.ValidationException(
+            'item contains no additional keys beyond key_attrs'
+        )
+
+
 def kms_encrypt_item(config: t.Dict, item: t.Dict) -> t.Dict:
     """Encrypt item values as defined in config
 
     Each attribute value is encrypted with data key generated each time for both providers:
 
     - aws_kms uses aws-encryption-sdk
     - azure_kms uses Azure Keyvault RSA CMK to envelope encrypt data key
@@ -416,31 +472,32 @@
     for item in items:
         for attr in kcfg['attrs']:
             item.pop(attr, None)
         _items.append(item)
     return _items
 
 
-def add_audit(item: t.Dict, user: str) -> t.Dict:
-    """Add created_by + created_date and/or modified_by + modified_date to item
+def add_audit(item: t.Dict, update: bool, user: str) -> t.Dict:
+    """Add createdBy + createdDate and/or modifiedBy + modifiedDate to item
 
     Args:
 
         item: item dict
+        update: bool, true if operation is update otherwise false
         user: user/system ID string
 
     Returns:
         item
 
     """
     camel_case = os.environ.get('ABNOSQL_AUDIT_CAMELCASE', 'TRUE') == 'TRUE'
     by_attr = 'By' if camel_case else '_by'
     date_attr = 'Date' if camel_case else '_date'
     dt_iso = datetime.now(timezone.utc).strftime('%Y-%m-%dT%H:%M:%SZ')
-    if f'created{by_attr}' not in item:
+    if update is not True and f'created{by_attr}' not in item:
         item.update({
             f'created{by_attr}': user,
             f'created{date_attr}': dt_iso
         })
     item.update({
         f'modified{by_attr}': user,
         f'modified{date_attr}': dt_iso
@@ -506,14 +563,17 @@
         }
         provider = kcfg.get('provider')
         if database is not None and provider is None:
             provider = defaults.get(database)
         _kms_module = kms(kcfg, provider)
         config['kms']['pm'] = _kms_module
 
+        if 'key_attrs' not in kcfg:
+            config['kms']['key_attrs'] = get_key_attrs(config)
+
         if 'session' in config and 'session' not in kcfg:
             # aws_encryption_sdk uses botocore session
             config['kms']['session'] = config['session']._session
 
         # check required attrs
         missing = [
             _ for _ in ['attrs', 'key_attrs']
```

### Comparing `abnosql-0.0.4/abnosql.egg-info/PKG-INFO` & `abnosql-0.0.5/abnosql.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abnosql
-Version: 0.0.4
+Version: 0.0.5
 Summary: NoSQL Abstraction Library
 Home-page: https://github.com/rog555/abnosql
 Download-URL: http://pypi.python.org/pypi/abnosql
 Author: Roger Foskett
 Author-email: r_foskett@hotmail.com
 Maintainer: Roger Foskett
 Maintainer-email: r_foskett@hotmail.com
@@ -49,14 +49,15 @@
 
 - [NoSQL Abstraction Library](#nosql-abstraction-library)
   - [Installation](#installation)
 - [Usage](#usage)
   - [API Docs](#api-docs)
   - [Querying](#querying)
   - [Indexes](#indexes)
+  - [Updates](#updates)
   - [Partition Keys](#partition-keys)
   - [Client Side Encryption](#client-side-encryption)
   - [Pagination](#pagination)
   - [Audit](#audit)
 - [Configuration](#configuration)
   - [AWS DynamoDB](#aws-dynamodb)
   - [Azure Cosmos NoSQL](#azure-cosmos-nosql)
@@ -88,14 +89,15 @@
 # Usage
 
 ```
 from abnosql import table
 import os
 
 os.environ['ABNOSQL_DB'] = 'dynamodb'
+os.environ['ABNOSQL_KEY_ATTRS'] = 'hk,rk'
 
 item = {
     'hk': '1',
     'rk': 'a',
     'num': 5,
     'obj': {
         'foo': 'bar',
@@ -104,15 +106,25 @@
     },
     'list': [1, 2, 3],
     'str': 'str'
 }
 
 tb = table('mytable')
 
+# create/replace
 tb.put_item(item)
+
+# update - using ABNOSQL_KEY_ATTRS
+updated_item = tb.put_item(
+    {'hk': '1', 'rk': 'a', 'str': 'STR'},
+    update=True
+)
+assert updated_item['str'] == 'STR'
+
+# bulk
 tb.put_items([item])
 
 # note partition/hash key should be first kwarg
 assert tb.get_item(hk='1', rk='a') == item
 
 assert tb.query({'hk': '1'})['items'] == [item]
 
@@ -143,14 +155,26 @@
 Care should be taken with `query_sql()` to not to use SQL features that are specific to any specific provider (breaking the abstraction capability of using abnosql in the first place)
 
 ## Indexes
 
 Beyond partition and range keys defined on the table, indexes are not currently supported - and these will likey differ between providers anyway (eg DynamoDB supports [Secondary Indexes](https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/SecondaryIndexes.html), whereas [Cosmos](https://learn.microsoft.com/en-us/azure/cosmos-db/index-overview) has Range, Spatial and Composite.
 
 
+## Updates
+
+`put_item()` and `put_items()` support `update` boolean attribute, which if supplied will do an `update_item()` on DynamoDB, and a `patch_item()` on Cosmos.  For this to work however, you must specify the key attribute names, either via `ABNOSQL_KEY_ATTRS` env var as a comma separated list (eg perhaps multiple tables all share common partition/range key scheme), or as the `key_attrs` config item  when instantiating the table, eg:
+
+```
+tb = table('mytable', {'key_attrs': ['hk', 'rk']})
+```
+
+If you don't need to do any updates and only need to do create/replace, then these key attribute names do not need to be supplied
+
+All items being updated must actually exist first, or else exception raised
+
 ## Partition Keys
 
 A few methods such as `get_item()`, `delete_item()` and `query()` need to know partition/hash keys as defined on the table.  To avoid having to configure this or lookup from the provider, the convention used is that the first kwarg or dictionary item is the partition key, and if supplied the 2nd is the range/sort key.
 
 ## Client Side Encryption
 
 If configured in table config with `kms` attribute, abnosql will perform client side encryption using AWS KMS or Azure KeyVault
@@ -174,15 +198,15 @@
         'attrs': ['obj', 'str']
     }
 }
 ```
 
 Where:
 - `key_ids`: list of AWS KMS Key ARNs or Azure KeyVault identifier (URL to RSA CMK).  This is picked up via `ABNOSQL_KMS_KEYS` env var as a comma separated list (*NOTE: env var recommended to avoid provider specific code*)
-- `key_attrs`: list of key attributes in the item from which the AAD/encryption context is set
+- `key_attrs`: list of key attributes in the item from which the AAD/encryption context is set.  Taken from `ABNOSQL_KEY_ATTRS` env var or table `key_attrs` if defined there
 - `attrs`: list of attributes keys to encrypt
 - `key_bytes`: optional for azure, use your own AESGCM key if specified, otherwise generate one
 
 If `kms` config attribute is present, abnosql will look for the `ABNOSQL_KMS` provider to load the appropriate provider KMS module (eg "aws" or "azure"), and if not present use default depending on the database (eg cosmos will use azure, dynamodb will use aws)
 
 In example above, the key_attrs `['hk', 'rk']` are used to define the encryption context / AAD used, and attrs `['obj', 'str']` what attributes to encrypt/decrypt
 
@@ -208,24 +232,24 @@
 
 `query` and `query_sql` accept `limit` and `next` optional kwargs and return `next` in response. Use these to paginate.
 
 This works for AWS DyanmoDB, however Azure Cosmos has a limitation with continuation token for cross partitions queries (see [Python SDK documentation](https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos)).  For Cosmos, abnosql appends OFFSET and LIMIT in the SQL statement if not already present, and returns `next`.  `limit` is defaulted to 100.  See the tests for examples
 
 ## Audit
 
-`put_item()` and `put_items()` take an optional `user` kwarg.  If supplied, absnosql will add the following to the item:
+`put_item()` and `put_items()` take an optional `audit_user` kwarg.  If supplied, absnosql will add the following to the item:
 
-- `createdBy` - value of `user`, added if does not exist in item supplied to put_item()
+- `createdBy` - value of `audit_user`, added if does not exist in item supplied to put_item()
 - `createdDate` - UTC ISO timestamp string, added if does not exist
-- `modifiedBy` - value of `user` always added
+- `modifiedBy` - value of `audit_user` always added
 - `modifiedDate` - UTC ISO timestamp string, always added
 
-Because abnosql doesnt first check if the item already exists, and doesn't support update expressions, there can be a risk with the created* values being re-added if the existing item is not read first and then supplied to put_item(). Its up to application logic to do this - using this feature or not :-)
+NOTE: created* will only be added if `update` is not True in a `put_item()` operation
 
-If you prefer snake_case over CamelCase, you can set env var `ABNOSQ_AUDIT_CAMELCASE` = `FALSE`
+If you prefer snake_case over CamelCase, you can set env var `ABNOSQL_AUDIT_CAMELCASE` = `FALSE`
 
 # Configuration
 
 It is recommended to use environment variables where possible to avoid provider specific application code
 
 if `ABNOSQL_DB` env var is not set, abnosql will attempt to apply defaults based on available environment variables:
```

### Comparing `abnosql-0.0.4/abnosql.egg-info/SOURCES.txt` & `abnosql-0.0.5/abnosql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/abnosql.egg-info/requires.txt` & `abnosql-0.0.5/abnosql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `abnosql-0.0.4/setup.py` & `abnosql-0.0.5/setup.py`

 * *Files identical despite different names*

