# Comparing `tmp/spark_sdk-0.5.0rc0-py3-none-any.whl.zip` & `tmp/spark_sdk-0.5.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 35572 bytes, number of entries: 16
--rw-rw-r--  2.0 unx     1381 b- defN 23-Jul-17 10:04 spark_sdk/__init__.py
--rw-rw-r--  2.0 unx      772 b- defN 23-Jul-16 08:13 spark_sdk/conf.py
+Zip file size: 35636 bytes, number of entries: 16
+-rw-rw-r--  2.0 unx     1381 b- defN 23-Jul-19 07:01 spark_sdk/__init__.py
+-rw-rw-r--  2.0 unx      749 b- defN 23-Jul-19 02:02 spark_sdk/conf.py
 -rw-rw-r--  2.0 unx     4469 b- defN 22-Aug-12 12:38 spark_sdk/create_yaml_file.py
 -rw-rw-r--  2.0 unx     6309 b- defN 23-Mar-24 03:02 spark_sdk/datahub_api.py
 -rw-rw-r--  2.0 unx     9905 b- defN 22-Jun-06 02:01 spark_sdk/hive_metastore.py
 -rw-rw-r--  2.0 unx     3319 b- defN 23-Apr-26 04:20 spark_sdk/ingest_hive_datahub.py
 -rw-rw-r--  2.0 unx     2300 b- defN 23-Apr-24 07:08 spark_sdk/magics.py
 -rw-rw-r--  2.0 unx     1767 b- defN 23-Feb-13 06:42 spark_sdk/pandas_decrypt.py
--rw-rw-r--  2.0 unx    34923 b- defN 23-Jul-17 08:41 spark_sdk/pylineage.py
--rw-rw-r--  2.0 unx    51893 b- defN 23-Jul-17 10:05 spark_sdk/pyspark_add_on.py
+-rw-rw-r--  2.0 unx    35211 b- defN 23-Jul-18 09:06 spark_sdk/pylineage.py
+-rw-rw-r--  2.0 unx    51893 b- defN 23-Jul-19 10:39 spark_sdk/pyspark_add_on.py
 -rw-rw-r--  2.0 unx     4100 b- defN 23-Mar-12 15:53 spark_sdk/utils.py
--rw-rw-r--  2.0 unx       92 b- defN 22-Oct-10 08:46 spark_sdk-0.5.0rc0.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-rw-r--  2.0 unx     8526 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1335 b- defN 23-Jul-17 10:06 spark_sdk-0.5.0rc0.dist-info/RECORD
-16 files, 131193 bytes uncompressed, 33370 bytes compressed:  74.6%
+-rw-rw-r--  2.0 unx       92 b- defN 22-Oct-10 08:46 spark_sdk-0.5.0rc1.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-rw-r--  2.0 unx     8526 b- defN 23-Jul-19 10:40 spark_sdk-0.5.0rc1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-19 10:40 spark_sdk-0.5.0rc1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jul-19 10:40 spark_sdk-0.5.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1335 b- defN 23-Jul-19 10:40 spark_sdk-0.5.0rc1.dist-info/RECORD
+16 files, 131458 bytes uncompressed, 33434 bytes compressed:  74.6%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: spark_sdk/pyspark_add_on.py
 Comment: 
 
 Filename: spark_sdk/utils.py
 Comment: 
 
-Filename: spark_sdk-0.5.0rc0.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
+Filename: spark_sdk-0.5.0rc1.dist-info/.ipynb_checkpoints/requires-checkpoint.txt
 Comment: 
 
-Filename: spark_sdk-0.5.0rc0.dist-info/METADATA
+Filename: spark_sdk-0.5.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: spark_sdk-0.5.0rc0.dist-info/WHEEL
+Filename: spark_sdk-0.5.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: spark_sdk-0.5.0rc0.dist-info/top_level.txt
+Filename: spark_sdk-0.5.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: spark_sdk-0.5.0rc0.dist-info/RECORD
+Filename: spark_sdk-0.5.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spark_sdk/__init__.py

```diff
@@ -38,11 +38,11 @@
 SparkDataFrame.to_dwh = spark_dataframe_to_dwh
 SparkDataFrame.info = spark_dataframe_info
 SparkDataFrame.toPandas = PandasConversionMixin.toPandasLineage
 
 
 SparkDataFrame.show = show
 
-__version__ = '0.5.0rc0'
+__version__ = '0.5.0rc1'
 __all__ = ["PySpark", "PyArrow"]
```

## spark_sdk/conf.py

```diff
@@ -1,13 +1,13 @@
 HADOOP_HOST = "hdfs://hdfs-cluster.datalake.bigdata.local"
 HADOOP_PORT = 8020
 HIVE_IP_NODES1 = "master01-dc9c14u40.bigdata.local:9083"
 HIVE_IP_NODES2 = "master02-dc9c14u41.bigdata.local:9083"
 
-GMS_AUTH_TOKEN = "eyJhbGciOiJIUzI1NiJ9.eyJhY3RvclR5cGUiOiJVU0VSIiwiYWN0b3JJZCI6ImR1eXZuYyIsInR5cGUiOiJQRVJTT05BTCIsInZlcnNpb24iOiIyIiwianRpIjoiZTdhZWUxM2MtYzI1Yi00MjUzLWE1Y2MtZTkxNWZiMDNiYTBmIiwic3ViIjoiZHV5dm5jIiwiZXhwIjoxNjkwOTQzMDYxLCJpc3MiOiJkYXRhaHViLW1ldGFkYXRhLXNlcnZpY2UifQ.RG6K8bh-oZtEOZ6xXkY-4jxQtMY89F8THvfcL1qVpWk"
+GMS_AUTH_TOKEN = "eyJhbGciOiJIUzI1NiJ9.eyJhY3RvclR5cGUiOiJVU0VSIiwiYWN0b3JJZCI6ImR1eXZuYyIsInR5cGUiOiJQRVJTT05BTCIsInZlcnNpb24iOiIyIiwianRpIjoiMmMxMDM2MzQtNjI5My00OTM3LWFlYzctNTI0YmEyMzI3MGZlIiwic3ViIjoiZHV5dm5jIiwiaXNzIjoiZGF0YWh1Yi1tZXRhZGF0YS1zZXJ2aWNlIn0.zJISXPTw1HCI2lDIC0pfSACCg2GLfnRNVPfWBif8b88"
 GMS_URL_KEY = "http://ccatalog-gms.cads.live"
 # GMS_URL_KEY = "http://staging-ccatalog-gms.cads.live"
 
 import os
 from urllib.parse import urlparse
 domain = urlparse(GMS_URL_KEY).netloc
 os.environ['no_proxy'] = domain+","+"git.cads.live,vault.cads.live"
```

## spark_sdk/pylineage.py

```diff
@@ -7,15 +7,15 @@
 from datahub.emitter import mce_builder as builder
 from datahub.emitter.mcp import MetadataChangeProposalWrapper
 from datahub.metadata.schema_classes import DataFlowInfoClass, DataJobInfoClass, DataJobInputOutputClass,ChangeTypeClass,DatasetPropertiesClass
 from datahub.specific.dataset import DatasetPatchBuilder
 from datahub.emitter.mce_builder import make_dataset_urn,make_data_job_urn,make_data_flow_urn
 
 import logging
-debug = False
+debug = True
 
 if debug:
     logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.WARNING)
 else:
     logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.ERROR)
 
 def log(message, v):
@@ -562,64 +562,72 @@
 def scanVariable(variable_name, txt):
     import re
     pattern_var1 = r'{x}\s*=\s*["\']([^"\']+)["\']'.format(x = variable_name)
     matches_api1 = re.findall(pattern_var1, txt)
     if matches_api1:
         return matches_api1
     
-    pattern_api2 = r'url\s*=\s*["\'\f]([^"\']+)["\']'.format(x = variable_name)
+    pattern_api2 = r'{x}\s*=\s*["\'\f]([^"\']+)["\']'.format(x = variable_name)
     matches_api2 = re.findall(pattern_var1, txt)
     if matches_api2:
         return matches_api2
     
     pattern_assign = r'{x}\s*=\s*(\w+)'.format(x = variable_name)
     matches_assign = re.findall(pattern_assign, txt)
     for variable_name in matches_assign:
         return scanVariable(variable_name, txt)
     return None
 
+
 def parseUrl2Urn(url):
     from urllib.parse import urlparse
     return urlparse(url).netloc + urlparse(url).path.rstrip("/")
 
+
+def scanPattern(pattern_prefix, txt, _type, lineage):
+    pattern_simple = r'{x}["\']([^"\']+)["\']'.format(x=pattern_prefix)
+    matches_simple = re.findall(pattern_simple, txt)
+    if _type == 'api':
+        matches_simple = [parseUrl2Urn(x) for x in matches_simple]
+    _ = [lineage.addSource(f, _type = _type) for f in matches_simple if f]
+    log("matches_simple", matches_simple)
+
+    pattern_fstring = r'{x}f["\']([^"\']+)["\']'.format(x=pattern_prefix)
+    matches_fstring = re.findall(pattern_fstring, txt)
+    log("matches_fstring", matches_fstring)
+    for full_fstring in matches_fstring:
+        variables = re.findall(r'\{(.+?)\}', full_fstring)
+        for variable_name in variables:
+            matches_var = scanVariable(variable_name, txt)
+            log("matches_var", matches_var)
+            full_fstring = full_fstring.replace("{" + variable_name + "}", matches_var[0])
+        if _type == 'api':
+            full_fstring = parseUrl2Urn(full_fstring)
+        if full_fstring:
+            lineage.addSource(full_fstring, _type = _type)
+            log("full_fstring", full_fstring)
+    return lineage
+    
+
 def scanPythonFile(lineage):
     import re
     try:
         txt = open(get_job_location(), 'r').read()
+        # txt = open(get_job_location(), 'r').read()
+        x = ''
+        for line in txt.split("\n"):
+            if not line.strip().startswith("#"):
+                x += line + '\n'
+        txt = x
     except:
         txt = ''
 
-    # matches = 
-    
     if 'requests.post(' in txt or 'request("post"' in txt or 'requests.get(' in txt or 'request("get"' in txt:
-        pattern_api1 = r'url\s*=\s*["\'\f]([^"\']+)["\']'
-        matches_api1 = re.findall(pattern_api1, txt)
-        matches_api1 = [parseUrl2Urn(x) for x in matches_api1]
-        _ = [lineage.addSource(f, _type = 'api') for f in matches_api1 if f]
-        log("matches_api1", matches_api1)
-        
-        pattern_api2 = r'url\s*=\s*f["\']([^"\']+)["\']'
-        matches_api2 = re.findall(pattern_api2, txt)
-        log("matches_api2", matches_api2)
-        variables = [x for x in matches_api2 if x]
-        for full_url in matches_api2:
-            variables = re.findall(r'\{(.+?)\}', full_url)
-            for variable_name in variables:
-                matches_api3 = scanVariable(variable_name, txt)
-                full_url = full_url.replace("{" + variable_name + "}", matches_api3[0])
-            full_url = parseUrl2Urn(full_url)
-            if full_url:
-                lineage.addSource(full_url, _type = 'api')
-                log("matches_api3", full_url)
-        
-    pattern_pandas = r'pd\.read_csv\(["\']([^"\']+)["\']'
-    matches_pandas = re.findall(pattern_pandas, txt)
-    logging.warn("matches_pandas")
-    logging.warn(matches_pandas)
-    _ = [lineage.addSource(f, _type = 'file') for f in matches_pandas if f]
+        lineage = scanPattern(pattern_prefix = "url\s*=\s*", txt = txt, _type = 'api', lineage = lineage)
+    lineage = scanPattern(pattern_prefix = "pd\.read_csv\(", txt = txt, _type = 'file', lineage = lineage)
     return lineage
 
 
 def addLineageAfterToDwh(full_table_name):
     lineage = DatasetLineage()
     lineage.addSink(full_table_name)
     # _ = [lineage.addSource(f, _type = 'file') for f in scanPythonFile()]
@@ -635,14 +643,15 @@
             
         log("addLineageAfterToDwh pythonUrn", pythonUrn)
         log("addLineageAfterToDwh lineage sink", lineage.sink)
         log("addLineageAfterToDwh lineage source", lineage.source)
     return mcpws
 
 
+
 ####################################################
 import sys
 from collections import Counter
 from typing import List, Optional, Type, Union, no_type_check, overload, TYPE_CHECKING
 from warnings import catch_warnings, simplefilter, warn
 
 from pyspark.rdd import _load_from_socket
```

## Comparing `spark_sdk-0.5.0rc0.dist-info/METADATA` & `spark_sdk-0.5.0rc1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-sdk
-Version: 0.5.0rc0
+Version: 0.5.0rc1
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Platform: UNKNOWN
```

## Comparing `spark_sdk-0.5.0rc0.dist-info/RECORD` & `spark_sdk-0.5.0rc1.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-spark_sdk/__init__.py,sha256=crYKgbOxA3tft9L_Yom0Z_8yAPpLU1uQL1PYm5V_Hwk,1381
-spark_sdk/conf.py,sha256=jnglvfJx7JM1GwKQt-RswtnpXLukKhfaIYvgXyEsvBo,772
+spark_sdk/__init__.py,sha256=0ZGTHqxjiKH2W0tHqBqBI1Xi0-j9Y9A6GfiORR-wVXU,1381
+spark_sdk/conf.py,sha256=oM53EiK7W5pVJtneTaO477hvXs-p0oGUTKAFlaItBso,749
 spark_sdk/create_yaml_file.py,sha256=XOHhMiyzYqQ4-YEvhsMg8Lk6KbPzNox0BdnoswWn1F0,4469
 spark_sdk/datahub_api.py,sha256=fqn2j1TA8lbUHbJdBNeuvBq3nR7zWfzjH6Zp16z8NDQ,6309
 spark_sdk/hive_metastore.py,sha256=edPbjRIkyLo0OB1llkq9783cIbYGIuAXHEGXkCWFn70,9905
 spark_sdk/ingest_hive_datahub.py,sha256=6ap8pEuoU7-VHQFFZ_BTDfltpAViXKsCSkWzCwkYhfc,3319
 spark_sdk/magics.py,sha256=g4N6m9LKSZsbYd4iUdUqsl3H_PCNNIFauWPPblLQdNU,2300
 spark_sdk/pandas_decrypt.py,sha256=2PUMBKN0zbG19hkuB_gC_pXAaR78s2s20yjaUxE9B4Y,1767
-spark_sdk/pylineage.py,sha256=6pOe3WXzt2Wje3IMpDT5RW-b6OT2j2Sx7CQgWXQDAeM,34923
+spark_sdk/pylineage.py,sha256=vLvifW_JqZ1QEQiSKmBanqpV6exmsh8xJmtjHWafnQI,35211
 spark_sdk/pyspark_add_on.py,sha256=UshcNfSsicsVL49e5Td_vQnCL0i3ogK5RRXJ2eL4wpA,51893
 spark_sdk/utils.py,sha256=PmfEZXaqTW9rEcJ8wxrtMRqm3QmPFyL80I9tQ4x7yIU,4100
-spark_sdk-0.5.0rc0.dist-info/.ipynb_checkpoints/requires-checkpoint.txt,sha256=ZGBYK1Crp59m1x-Y3tALQiIew3A2hUYcSce2VIX2Y90,92
-spark_sdk-0.5.0rc0.dist-info/METADATA,sha256=-f8D7Hfnb-4J1cTHayENadmqIL5bLr_cGZuiIsrwcdA,8526
-spark_sdk-0.5.0rc0.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-spark_sdk-0.5.0rc0.dist-info/top_level.txt,sha256=hweYK71GSSYJx1YB2cNkxNw2KWVincoyKY8AqJc00Wg,10
-spark_sdk-0.5.0rc0.dist-info/RECORD,,
+spark_sdk-0.5.0rc1.dist-info/.ipynb_checkpoints/requires-checkpoint.txt,sha256=ZGBYK1Crp59m1x-Y3tALQiIew3A2hUYcSce2VIX2Y90,92
+spark_sdk-0.5.0rc1.dist-info/METADATA,sha256=zdhGZsksYgUWecCPoiI3kZMCkLoVDPFhE5RiHoZAV9s,8526
+spark_sdk-0.5.0rc1.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+spark_sdk-0.5.0rc1.dist-info/top_level.txt,sha256=hweYK71GSSYJx1YB2cNkxNw2KWVincoyKY8AqJc00Wg,10
+spark_sdk-0.5.0rc1.dist-info/RECORD,,
```

