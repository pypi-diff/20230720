# Comparing `tmp/prefect-aws-0.3.5.tar.gz` & `tmp/prefect-aws-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-dykgbcpt/prefect-aws-0.3.5.tar", last modified: Fri Jul 14 19:13:13 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-aws/prefect-aws/dist/.tmp-cr11euy2/prefect-aws-0.3.6.tar", last modified: Thu Jul 20 14:29:19 2023, max compression
```

## Comparing `prefect-aws-0.3.5.tar` & `prefect-aws-0.3.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/secrets_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56988 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/prefect_aws/workers/ecs_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/prefect_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 19:13:13.000000 prefect-aws-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_client_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_client_waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27593 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/tests/test_secrets_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-07-14 19:12:11.000000 prefect-aws-0.3.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8199 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57782 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35070 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17380 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/secrets_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56968 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/prefect_aws/workers/ecs_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/prefect_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:19.000000 prefect-aws-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_client_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_client_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27593 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/tests/test_secrets_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80043 2023-07-20 14:28:12.000000 prefect-aws-0.3.6/versioneer.py
```

### Comparing `prefect-aws-0.3.5/LICENSE` & `prefect-aws-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/PKG-INFO` & `prefect-aws-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.5
+Version: 0.3.6
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.5 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.6 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.5/README.md` & `prefect-aws-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/__init__.py` & `prefect-aws-0.3.6/prefect_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/batch.py` & `prefect-aws-0.3.6/prefect_aws/batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/client_parameters.py` & `prefect-aws-0.3.6/prefect_aws/client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/client_waiter.py` & `prefect-aws-0.3.6/prefect_aws/client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/credentials.py` & `prefect-aws-0.3.6/prefect_aws/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/deployments/steps.py` & `prefect-aws-0.3.6/prefect_aws/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/ecs.py` & `prefect-aws-0.3.6/prefect_aws/ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/s3.py` & `prefect-aws-0.3.6/prefect_aws/s3.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/secrets_manager.py` & `prefect-aws-0.3.6/prefect_aws/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/prefect_aws/workers/ecs_worker.py` & `prefect-aws-0.3.6/prefect_aws/workers/ecs_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -508,15 +508,14 @@
     job_configuration_variables = ECSVariables
     _description = (
         "Execute flow runs within containers on AWS ECS. Works with EC2 "
         "and Fargate clusters. Requires an AWS account."
     )
     _display_name = "AWS Elastic Container Service"
     _documentation_url = "https://prefecthq.github.io/prefect-aws/ecs_worker/"
-    _is_beta = True
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/1jbV4lceHOjGgunX15lUwT/db88e184d727f721575aeb054a37e277/aws.png?h=250"  # noqa
 
     async def run(
         self,
         flow_run: "FlowRun",
         configuration: ECSJobConfiguration,
         task_status: Optional[anyio.abc.TaskStatus] = None,
```

### Comparing `prefect-aws-0.3.5/prefect_aws.egg-info/PKG-INFO` & `prefect-aws-0.3.6/prefect_aws.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-aws
-Version: 0.3.5
+Version: 0.3.6
 Summary: Prefect collection of tasks and subflows to integrate with AWS
 Home-page: https://github.com/PrefectHQ/prefect-aws
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.5 Summary: Prefect
+Metadata-Version: 2.1 Name: prefect-aws Version: 0.3.6 Summary: Prefect
 collection of tasks and subflows to integrate with AWS Home-page: https://
 github.com/PrefectHQ/prefect-aws Author: Prefect Technologies, Inc. Author-
 email: help@prefect.io License: Apache License 2.0 Keywords: prefect
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: System Administrators Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
```

### Comparing `prefect-aws-0.3.5/prefect_aws.egg-info/SOURCES.txt` & `prefect-aws-0.3.6/prefect_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/setup.cfg` & `prefect-aws-0.3.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/setup.py` & `prefect-aws-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_batch.py` & `prefect-aws-0.3.6/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_block_standards.py` & `prefect-aws-0.3.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_client_parameters.py` & `prefect-aws-0.3.6/tests/test_client_parameters.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_client_waiter.py` & `prefect-aws-0.3.6/tests/test_client_waiter.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_credentials.py` & `prefect-aws-0.3.6/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_ecs.py` & `prefect-aws-0.3.6/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_s3.py` & `prefect-aws-0.3.6/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/tests/test_secrets_manager.py` & `prefect-aws-0.3.6/tests/test_secrets_manager.py`

 * *Files identical despite different names*

### Comparing `prefect-aws-0.3.5/versioneer.py` & `prefect-aws-0.3.6/versioneer.py`

 * *Files identical despite different names*

