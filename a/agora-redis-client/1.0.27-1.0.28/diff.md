# Comparing `tmp/agora_redis_client-1.0.27-py2.py3-none-any.whl.zip` & `tmp/agora_redis_client-1.0.28-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2641 bytes, number of entries: 7
+Zip file size: 2643 bytes, number of entries: 7
 -rw-r--r--  2.0 fat       31 b- defN 23-Jun-14 11:28 agora_redis_client/__init__.py
 -rw-r--r--  2.0 fat     1325 b- defN 23-Jun-14 11:28 agora_redis_client/redis_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-11 22:19 agora_redis_client/version.py
--rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.0.27.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.0.27.dist-info/WHEEL
--rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.0.27.dist-info/METADATA
--rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.0.27.dist-info/RECORD
-7 files, 3035 bytes uncompressed, 1561 bytes compressed:  48.6%
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-20 18:50 agora_redis_client/version.py
+-rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.0.28.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.0.28.dist-info/WHEEL
+-rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.0.28.dist-info/METADATA
+-rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.0.28.dist-info/RECORD
+7 files, 3035 bytes uncompressed, 1563 bytes compressed:  48.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: agora_redis_client/redis_client.py
 Comment: 
 
 Filename: agora_redis_client/version.py
 Comment: 
 
-Filename: agora_redis_client-1.0.27.dist-info/LICENSE
+Filename: agora_redis_client-1.0.28.dist-info/LICENSE
 Comment: 
 
-Filename: agora_redis_client-1.0.27.dist-info/WHEEL
+Filename: agora_redis_client-1.0.28.dist-info/WHEEL
 Comment: 
 
-Filename: agora_redis_client-1.0.27.dist-info/METADATA
+Filename: agora_redis_client-1.0.28.dist-info/METADATA
 Comment: 
 
-Filename: agora_redis_client-1.0.27.dist-info/RECORD
+Filename: agora_redis_client-1.0.28.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_redis_client/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.27'
+__version__ = '1.0.28'
```

## Comparing `agora_redis_client-1.0.27.dist-info/METADATA` & `agora_redis_client-1.0.28.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: agora_redis_client
-Version: 1.0.27
+Version: 1.0.28
 Summary: Redis Client for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.0.27
-Requires-Dist: agora_config == 1.0.27
+Requires-Dist: agora_logging == 1.0.28
+Requires-Dist: agora_config == 1.0.28
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_redisclient
 
 This package is the Redis Client for the Agora Edge Apps SDK (Python) developed by SLB.
```

