# Comparing `tmp/prefect-gcp-0.4.4.tar.gz` & `tmp/prefect-gcp-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-g0j5y6zy/prefect-gcp-0.4.4.tar", last modified: Mon Jun 26 16:15:16 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-gcp/prefect-gcp/dist/.tmp-hz916qvi/prefect-gcp-0.4.5.tar", last modified: Thu Jul 20 14:29:24 2023, max compression
```

## Comparing `prefect-gcp-0.4.4.tar` & `prefect-gcp-0.4.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    31619 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/prefect_gcp/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/prefect_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 16:15:16.000000 prefect-gcp-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_aiplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_cloud_run.py
--rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_cloud_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-26 16:13:33.000000 prefect-gcp-0.4.4/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16865 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34227 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45741 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8913 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13455 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31485 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/prefect_gcp/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/prefect_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:24.000000 prefect-gcp-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7102 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_aiplatform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29089 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_cloud_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20315 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_cloud_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-20 14:28:09.000000 prefect-gcp-0.4.5/versioneer.py
```

### Comparing `prefect-gcp-0.4.4/LICENSE` & `prefect-gcp-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/PKG-INFO` & `prefect-gcp-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.4
+Version: 0.4.5
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.4 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.5 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.4/README.md` & `prefect-gcp-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/__init__.py` & `prefect-gcp-0.4.5/prefect_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/aiplatform.py` & `prefect-gcp-0.4.5/prefect_gcp/aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/bigquery.py` & `prefect-gcp-0.4.5/prefect_gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/cloud_run.py` & `prefect-gcp-0.4.5/prefect_gcp/cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/cloud_storage.py` & `prefect-gcp-0.4.5/prefect_gcp/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/credentials.py` & `prefect-gcp-0.4.5/prefect_gcp/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/deployments/steps.py` & `prefect-gcp-0.4.5/prefect_gcp/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/secret_manager.py` & `prefect-gcp-0.4.5/prefect_gcp/secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp/worker.py` & `prefect-gcp-0.4.5/prefect_gcp/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """ <!-- # noqa -->
-<span class="badge-api beta"/>
 
 Module containing the Cloud Run worker used for executing flow runs as Cloud Run jobs.
 
-Note this module is in **beta**. The interfaces within may change without notice.
-
 Get started by creating a Cloud Run work pool:
 
 ```bash
 prefect work-pool create 'my-cloud-run-pool' --type cloud-run
 ```
 
 Then start a Cloud Run worker with the following command:
@@ -519,15 +516,14 @@
     job_configuration_variables = CloudRunWorkerVariables
     _description = (
         "Execute flow runs within containers on Google Cloud Run. Requires "
         "a Google Cloud Platform account."
     )
     _display_name = "Google Cloud Run"
     _documentation_url = "https://prefecthq.github.io/prefect-gcp/worker/"
-    _is_beta = True
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/4SpnOBvMYkHp6z939MDKP6/549a91bc1ce9afd4fb12c68db7b68106/social-icon-google-cloud-1200-630.png?h=250"  # noqa
 
     def _create_job_error(self, exc, configuration):
         """Provides a nicer error for 404s when trying to create a Cloud Run Job."""
         # TODO consider lookup table instead of the if/else,
         # also check for documented errors
         if exc.status_code == 404:
```

### Comparing `prefect-gcp-0.4.4/prefect_gcp.egg-info/PKG-INFO` & `prefect-gcp-0.4.5/prefect_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-gcp
-Version: 0.4.4
+Version: 0.4.5
 Summary: Prefect tasks and subflows for interacting with Google Cloud Platform.
 Home-page: https://github.com/PrefectHQ/prefect-gcp
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.4 Summary: Prefect tasks
+Metadata-Version: 2.1 Name: prefect-gcp Version: 0.4.5 Summary: Prefect tasks
 and subflows for interacting with Google Cloud Platform. Home-page: https://
 github.com/PrefectHQ/prefect-gcp Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-gcp-0.4.4/prefect_gcp.egg-info/SOURCES.txt` & `prefect-gcp-0.4.5/prefect_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/prefect_gcp.egg-info/requires.txt` & `prefect-gcp-0.4.5/prefect_gcp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/setup.cfg` & `prefect-gcp-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/setup.py` & `prefect-gcp-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_aiplatform.py` & `prefect-gcp-0.4.5/tests/test_aiplatform.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_bigquery.py` & `prefect-gcp-0.4.5/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_block_standards.py` & `prefect-gcp-0.4.5/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_cloud_run.py` & `prefect-gcp-0.4.5/tests/test_cloud_run.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_cloud_storage.py` & `prefect-gcp-0.4.5/tests/test_cloud_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_credentials.py` & `prefect-gcp-0.4.5/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_secret_manager.py` & `prefect-gcp-0.4.5/tests/test_secret_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/tests/test_worker.py` & `prefect-gcp-0.4.5/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-gcp-0.4.4/versioneer.py` & `prefect-gcp-0.4.5/versioneer.py`

 * *Files identical despite different names*

