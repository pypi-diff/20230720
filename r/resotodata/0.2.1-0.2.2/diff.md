# Comparing `tmp/resotodata-0.2.1.tar.gz` & `tmp/resotodata-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotodata-0.2.1.tar", last modified: Thu Jul 20 12:23:14 2023, max compression
+gzip compressed data, was "resotodata-0.2.2.tar", last modified: Thu Jul 20 16:17:32 2023, max compression
```

## Comparing `resotodata-0.2.1.tar` & `resotodata-0.2.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:23:14.753901 resotodata-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 12:22:36.000000 resotodata-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 12:23:14.753901 resotodata-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-20 12:22:36.000000 resotodata-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:23:14.717901 resotodata-0.2.1/resotodata/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13346 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/co2.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:23:14.753901 resotodata-0.2.1/resotodata/data/
--rw-r--r--   0 runner    (1001) docker     (123)    16904 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/data/ccfdataset.json
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/data/colors.json
--rw-r--r--   0 runner    (1001) docker     (123) 18763286 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/data/instances.json
--rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/data/regions.json
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-20 12:22:36.000000 resotodata-0.2.1/resotodata/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:23:14.721901 resotodata-0.2.1/resotodata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 12:23:14.000000 resotodata-0.2.1/resotodata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 12:23:14.753901 resotodata-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-20 12:22:36.000000 resotodata-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 12:23:14.753901 resotodata-0.2.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 12:22:36.000000 resotodata-0.2.1/test/test_args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:32.339439 resotodata-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 16:17:03.000000 resotodata-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 16:17:32.339439 resotodata-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-20 16:17:03.000000 resotodata-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:32.319439 resotodata-0.2.2/resotodata/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14329 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/co2.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:32.339439 resotodata-0.2.2/resotodata/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    17029 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/data/ccfdataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/data/colors.json
+-rw-r--r--   0 runner    (1001) docker     (123) 18763286 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/data/instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13805 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/data/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-20 16:17:03.000000 resotodata-0.2.2/resotodata/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:32.319439 resotodata-0.2.2/resotodata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 16:17:32.000000 resotodata-0.2.2/resotodata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 16:17:32.339439 resotodata-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-20 16:17:03.000000 resotodata-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:17:32.339439 resotodata-0.2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-20 16:17:03.000000 resotodata-0.2.2/test/test_args.py
```

### Comparing `resotodata-0.2.1/PKG-INFO` & `resotodata-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Miscellaneous Resoto data.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resotodata-0.2.1/README.md` & `resotodata-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `resotodata-0.2.1/resotodata/__main__.py` & `resotodata-0.2.2/resotodata/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -323,15 +323,34 @@
             f.write(export_ts)
 
         print("Exporting CCF dataset constants")
         result = subprocess.run(
             ["./node_modules/.bin/ts-node", "export.ts"], cwd=tmpdir, check=True, capture_output=True, text=True
         )
 
-    return json.loads(result.stdout)
+    ccfdataset = json.loads(result.stdout)
+
+    # Add missing AMD EPYC 3rd Gen data to AWS
+    aws_cloud_constants = ccfdataset.get("aws", {}).get("AWS_CLOUD_CONSTANTS", {})
+    azure_cloud_constants = ccfdataset.get("azure", {}).get("AZURE_CLOUD_CONSTANTS", {})
+    if (
+        not "AMD EPYC 3rd Gen" in aws_cloud_constants["MIN_WATTS_BY_COMPUTE_PROCESSOR"]
+        and "AMD EPYC 3rd Gen" in azure_cloud_constants["MIN_WATTS_BY_COMPUTE_PROCESSOR"]
+    ):
+        aws_cloud_constants["MIN_WATTS_BY_COMPUTE_PROCESSOR"]["AMD EPYC 3rd Gen"] = azure_cloud_constants[
+            "MIN_WATTS_BY_COMPUTE_PROCESSOR"
+        ]["AMD EPYC 3rd Gen"]
+        aws_cloud_constants["MAX_WATTS_BY_COMPUTE_PROCESSOR"]["AMD EPYC 3rd Gen"] = azure_cloud_constants[
+            "MAX_WATTS_BY_COMPUTE_PROCESSOR"
+        ]["AMD EPYC 3rd Gen"]
+        aws_cloud_constants["MEMORY_BY_COMPUTE_PROCESSOR"]["AMD EPYC 3rd Gen"] = azure_cloud_constants[
+            "MEMORY_BY_COMPUTE_PROCESSOR"
+        ]["AMD EPYC 3rd Gen"]
+
+    return ccfdataset
 
 
 def get_aws_instances() -> dict:
     print("Checking if git is installed")
     for tool in ("git",):
         if not shutil.which(tool):
             raise RuntimeError(f"{tool} not found in path")
```

### Comparing `resotodata-0.2.1/resotodata/data/ccfdataset.json` & `resotodata-0.2.2/resotodata/data/ccfdataset.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997576208513709%*

 * *Differences: {"'aws'": "{'AWS_CLOUD_CONSTANTS': {'MEMORY_BY_COMPUTE_PROCESSOR': {'AMD EPYC 3rd Gen': 128}, "*

 * *          "'MIN_WATTS_BY_COMPUTE_PROCESSOR': {'AMD EPYC 3rd Gen': 0.45}, "*

 * *          "'MAX_WATTS_BY_COMPUTE_PROCESSOR': {'AMD EPYC 3rd Gen': 2.02}}}"}*

```diff
@@ -7,14 +7,15 @@
             "KILOWATT_HOURS_BY_SERVICE_AND_USAGE_UNIT": {
                 "total": {}
             },
             "MAX_WATTS_AVG": 3.5,
             "MAX_WATTS_BY_COMPUTE_PROCESSOR": {
                 "AMD EPYC 1st Gen": 2.55,
                 "AMD EPYC 2nd Gen": 1.69,
+                "AMD EPYC 3rd Gen": 2.02,
                 "AMD Radeon Pro V520": 229,
                 "AWS Graviton2": 1.69,
                 "Broadwell": 3.69,
                 "Cascade Lake": 3.97,
                 "Coffee Lake": 5.42,
                 "Haswell": 4.74,
                 "Ivy Bridge": 8.25,
@@ -30,28 +31,30 @@
                 "Sandy Bridge": 8.58,
                 "Skylake": 4.26
             },
             "MEMORY_AVG": 80.69,
             "MEMORY_BY_COMPUTE_PROCESSOR": {
                 "AMD EPYC 1st Gen": 89.6,
                 "AMD EPYC 2nd Gen": 129.78,
+                "AMD EPYC 3rd Gen": 128,
                 "AWS Graviton2": 129.78,
                 "Broadwell": 69.65,
                 "Cascade Lake": 98.12,
                 "Coffee Lake": 19.56,
                 "Haswell": 27.71,
                 "Ivy Bridge": 9.67,
                 "Sandy Bridge": 16.7,
                 "Skylake": 81.32
             },
             "MEMORY_COEFFICIENT": 0.000392,
             "MIN_WATTS_AVG": 0.74,
             "MIN_WATTS_BY_COMPUTE_PROCESSOR": {
                 "AMD EPYC 1st Gen": 0.82,
                 "AMD EPYC 2nd Gen": 0.47,
+                "AMD EPYC 3rd Gen": 0.45,
                 "AMD Radeon Pro V520": 26,
                 "AWS Graviton2": 0.47,
                 "Broadwell": 0.71,
                 "Cascade Lake": 0.64,
                 "Coffee Lake": 1.14,
                 "Haswell": 1,
                 "Ivy Bridge": 3.04,
```

### Comparing `resotodata-0.2.1/resotodata/data/colors.json` & `resotodata-0.2.2/resotodata/data/colors.json`

 * *Files identical despite different names*

### Comparing `resotodata-0.2.1/resotodata/data/instances.json` & `resotodata-0.2.2/resotodata/data/instances.json`

 * *Files identical despite different names*

### Comparing `resotodata-0.2.1/resotodata/data/regions.json` & `resotodata-0.2.2/resotodata/data/regions.json`

 * *Files identical despite different names*

### Comparing `resotodata-0.2.1/resotodata/utils.py` & `resotodata-0.2.2/resotodata/utils.py`

 * *Files identical despite different names*

### Comparing `resotodata-0.2.1/resotodata.egg-info/PKG-INFO` & `resotodata-0.2.2/resotodata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotodata
-Version: 0.2.1
+Version: 0.2.2
 Summary: Miscellaneous Resoto data.
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `resotodata-0.2.1/resotodata.egg-info/SOURCES.txt` & `resotodata-0.2.2/resotodata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotodata-0.2.1/setup.py` & `resotodata-0.2.2/setup.py`

 * *Files identical despite different names*

