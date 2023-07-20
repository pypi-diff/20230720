# Comparing `tmp/OBP_devops-0.1.0.tar.gz` & `tmp/OBP_devops-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OBP_devops-0.1.0.tar", last modified: Wed May 31 12:35:06 2023, max compression
+gzip compressed data, was "OBP_devops-0.1.1.tar", last modified: Thu Jul 20 08:24:13 2023, max compression
```

## Comparing `OBP_devops-0.1.0.tar` & `OBP_devops-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-31 12:35:06.463791 OBP_devops-0.1.0/OBP_devops/
--rw-rw-rw-   0        0        0     7180 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/__init__.py
--rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.1.0/OBP_devops/cloudformation.py
--rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.1.0/OBP_devops/codebuild.py
--rw-rw-rw-   0        0        0     2632 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
--rw-rw-rw-   0        0        0     3016 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
--rw-rw-rw-   0        0        0     2480 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
--rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.1.0/OBP_devops/codepipeline.py
--rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.1.0/OBP_devops/ecr.py
--rw-rw-rw-   0        0        0     1906 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecr_private_tag_immutability_enabled.py
--rw-rw-rw-   0        0        0     1849 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_container_insights_enabled.py
--rw-rw-rw-   0        0        0     1861 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_containers_non_privileged.py
--rw-rw-rw-   0        0        0     1935 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/ecs_containers_read_only_access.py
--rw-rw-rw-   0        0        0     2058 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/ecs_fargate_latest_platform_version.py
--rw-rw-rw-   0        0        0     1886 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_memory_hard_limit.py
--rw-rw-rw-   0        0        0     1995 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_nonroot_user.py
--rw-rw-rw-   0        0        0     1892 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_pid_mode_check.py
--rw-rw-rw-   0        0        0     2091 2023-05-31 12:31:35.000000 OBP_devops-0.1.0/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
--rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.1.0/OBP_devops/eks.py
--rw-rw-rw-   0        0        0     3326 2023-01-30 07:27:29.000000 OBP_devops-0.1.0/OBP_devops/elastic_beanstalk.py
--rw-rw-rw-   0        0        0     6477 2023-05-31 12:13:47.000000 OBP_devops-0.1.0/OBP_devops/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/OBP_devops.egg-info/
--rw-rw-rw-   0        0        0      369 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-31 12:35:06.000000 OBP_devops-0.1.0/OBP_devops.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.1.0/README.md
--rw-rw-rw-   0        0        0      550 2023-05-31 12:31:36.000000 OBP_devops-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-31 12:35:06.479433 OBP_devops-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-20 08:24:13.863257 OBP_devops-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-07-20 08:24:13.850132 OBP_devops-0.1.1/OBP_devops/
+-rw-rw-rw-   0        0        0     7180 2023-07-20 08:22:47.000000 OBP_devops-0.1.1/OBP_devops/__init__.py
+-rw-rw-rw-   0        0        0     2600 2023-01-27 06:22:26.000000 OBP_devops-0.1.1/OBP_devops/cloudformation.py
+-rw-rw-rw-   0        0        0     9072 2023-01-27 06:22:26.000000 OBP_devops-0.1.1/OBP_devops/codebuild.py
+-rw-rw-rw-   0        0        0     2632 2023-05-31 12:31:36.000000 OBP_devops-0.1.1/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py
+-rw-rw-rw-   0        0        0     3016 2023-05-31 12:31:35.000000 OBP_devops-0.1.1/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py
+-rw-rw-rw-   0        0        0     2480 2023-05-31 12:31:35.000000 OBP_devops-0.1.1/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py
+-rw-rw-rw-   0        0        0     2365 2023-01-27 05:16:17.000000 OBP_devops-0.1.1/OBP_devops/codepipeline.py
+-rw-rw-rw-   0        0        0     4336 2023-01-27 06:22:27.000000 OBP_devops-0.1.1/OBP_devops/ecr.py
+-rw-rw-rw-   0        0        0     1906 2023-05-31 12:31:36.000000 OBP_devops-0.1.1/OBP_devops/ecr_private_tag_immutability_enabled.py
+-rw-rw-rw-   0        0        0     1849 2023-05-31 12:31:36.000000 OBP_devops-0.1.1/OBP_devops/ecs_container_insights_enabled.py
+-rw-rw-rw-   0        0        0     1926 2023-07-20 07:08:22.000000 OBP_devops-0.1.1/OBP_devops/ecs_containers_non_privileged.py
+-rw-rw-rw-   0        0        0     2000 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_containers_read_only_access.py
+-rw-rw-rw-   0        0        0     2058 2023-05-31 12:31:35.000000 OBP_devops-0.1.1/OBP_devops/ecs_fargate_latest_platform_version.py
+-rw-rw-rw-   0        0        0     1951 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_memory_hard_limit.py
+-rw-rw-rw-   0        0        0     2060 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_nonroot_user.py
+-rw-rw-rw-   0        0        0     1957 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_pid_mode_check.py
+-rw-rw-rw-   0        0        0     2156 2023-07-20 07:58:07.000000 OBP_devops-0.1.1/OBP_devops/ecs_task_definition_user_for_host_mode_check.py
+-rw-rw-rw-   0        0        0     4711 2023-01-27 06:22:27.000000 OBP_devops-0.1.1/OBP_devops/eks.py
+-rw-rw-rw-   0        0        0     3326 2023-01-30 07:27:29.000000 OBP_devops-0.1.1/OBP_devops/elastic_beanstalk.py
+-rw-rw-rw-   0        0        0     6477 2023-05-31 12:13:47.000000 OBP_devops-0.1.1/OBP_devops/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:24:13.860259 OBP_devops-0.1.1/OBP_devops.egg-info/
+-rw-rw-rw-   0        0        0      369 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-20 08:24:13.000000 OBP_devops-0.1.1/OBP_devops.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-07-20 08:24:13.862258 OBP_devops-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-17 06:00:32.000000 OBP_devops-0.1.1/README.md
+-rw-rw-rw-   0        0        0      550 2023-07-20 08:22:47.000000 OBP_devops-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-20 08:24:13.864257 OBP_devops-0.1.1/setup.cfg
```

### Comparing `OBP_devops-0.1.0/OBP_devops/__init__.py` & `OBP_devops-0.1.1/OBP_devops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from botocore.exceptions import ClientError
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 __author__ = 'Klera DevOps'
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 
 class aws_client:
     def __init__(self, **kwargs):
         if 'aws_access_key_id' in kwargs.keys() and 'aws_secret_access_key' in kwargs.keys():
             self.session = session.Session(
                 aws_access_key_id=kwargs['aws_access_key_id'],
```

### Comparing `OBP_devops-0.1.0/OBP_devops/cloudformation.py` & `OBP_devops-0.1.1/OBP_devops/cloudformation.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/codebuild.py` & `OBP_devops-0.1.1/OBP_devops/codebuild.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py` & `OBP_devops-0.1.1/OBP_devops/codedeploy_auto_rollback_monitor_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py` & `OBP_devops-0.1.1/OBP_devops/codedeploy_ec2_minimum_healthy_hosts_configured.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py` & `OBP_devops-0.1.1/OBP_devops/codedeploy_lambda_allatonce_traffic_shift_disabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/codepipeline.py` & `OBP_devops-0.1.1/OBP_devops/codepipeline.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/ecr.py` & `OBP_devops-0.1.1/OBP_devops/ecr.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/ecr_private_tag_immutability_enabled.py` & `OBP_devops-0.1.1/OBP_devops/ecr_private_tag_immutability_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_container_insights_enabled.py` & `OBP_devops-0.1.1/OBP_devops/ecs_container_insights_enabled.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_containers_non_privileged.py` & `OBP_devops-0.1.1/OBP_devops/ecs_containers_non_privileged.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     description = "Checks if the privileged parameter in the container definition of ECSTaskDefinitions is set to ‘true’. "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'High'
 
     # regions = self.session.get_available_regions('ecs')
 
     for region, definitions in task_definitions.items():
+        client = self.session.client('ecs', region_name=region)
         for task_definition in definitions:
             resp = client.describe_task_definition(taskDefinition=task_definition)
             container_definitions = resp['taskDefinition']['containerDefinitions']
             for definition in container_definitions:
 
                 try:
                     if definition['privileged'] == 'False':
```

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_containers_read_only_access.py` & `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_pid_mode_check.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,57 @@
+
 import logging
 
 from botocore.exceptions import ClientError
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_containers_read_only_access(self, task_definitions) -> dict:
+def ecs_task_definition_pid_mode_check(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
-    logger.info(" ---Inside OBP DevOps :: ecs_containers_read_only_access()")
+    logger.info(" ---Inside OBP DevOps :: ecs_task_definition_pid_mode_check()")
 
     result = True
     failReason = ''
     offenders = []
-    control_id = 'Id7.3'
-    compliance_type = "ecs_containers_read_only_access"
-    description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to " \
-                  "its root filesystems. ."
+    control_id = 'Id7.8'
+    compliance_type = "ecs_task_definition_pid_mode_check"
+    description = "Checks if ECSTaskDefinitions are configured to share a host’s process namespace with its Amazon " \
+                  "Elastic Container Service (Amazon ECS) containers."
     resource_type = "AWS ECS TaskDefinition"
-    risk_level = 'High'
+    risk_level = 'Medium'
 
     # regions = self.session.get_available_regions('ecs')
 
     for region, definitions in task_definitions.items():
+        client = self.session.client('ecs', region_name=region)
         for task_definition in definitions:
-            resp = client.describe_task_definition(taskDefinition=task_definition)
-            container_definitions = resp['taskDefinition']['containerDefinitions']
-            for definition in container_definitions:
-
-                try:
-                    if definition['readonlyRootFilesystem'] == 'False':
-                        raise KeyError
 
-                except KeyError:
+            try:
+
+                resp = client.describe_task_definition(taskDefinition=task_definition)
+                if resp['taskDefinition']['pidMode'] == 'host':
+                    raise KeyError
+
+            except KeyError:
                     result = False
-                    offenders.append(definition['name'])
-                    failReason = "The readonlyRootFilesystem parameter in the container definition of ECSTaskDefinitions is set to ‘false’."
+                    offenders.append(resp['taskDefinition']['taskDefinitionArn'])
+                    failReason = "ECSTaskDefinitions are not configured to share a host’s process namespace with its ECS containers as pidMode parameter is set to ‘host’."
                     continue
-
+            
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
         'Risk Level': risk_level,
         'ControlId': control_id
-    }
+    }
```

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_fargate_latest_platform_version.py` & `OBP_devops-0.1.1/OBP_devops/ecs_fargate_latest_platform_version.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_memory_hard_limit.py` & `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_memory_hard_limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     description = "Checks if ECS task definitions have a set memory limit for its container definitions. "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'Medium'
 
     # regions = self.session.get_available_regions('ecs')
 
     for region, definitions in task_definitions.items():
+        client = self.session.client('ecs', region_name=region)
         for task_definition in definitions:
             resp = client.describe_task_definition(taskDefinition=task_definition)
             container_definitions = resp['taskDefinition']['containerDefinitions']
             for definition in container_definitions:
 
                 try:
                     # print(definition)
```

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_nonroot_user.py` & `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_nonroot_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to its root filesystems. . "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'Medium'
 
     # regions = self.session.get_available_regions('ecs')
 
     for region, definitions in task_definitions.items():
+        client = self.session.client('ecs', region_name=region)
         for task_definition in definitions:
             resp = client.describe_task_definition(taskDefinition=task_definition)
             container_definitions = resp['taskDefinition']['containerDefinitions']
             for definition in container_definitions:
                 try:
                     if 'user' not in definition:
                         raise KeyError
```

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_pid_mode_check.py` & `OBP_devops-0.1.1/OBP_devops/ecs_task_definition_user_for_host_mode_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,53 @@
-
 import logging
 
 from botocore.exceptions import ClientError
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_task_definition_pid_mode_check(self, task_definitions) -> dict:
+def ecs_task_definition_user_for_host_mode_check(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
-    logger.info(" ---Inside OBP DevOps :: ecs_task_definition_pid_mode_check()")
+    logger.info(" ---Inside OBP DevOps :: ecs_task_definition_user_for_host_mode_check()")
 
     result = True
     failReason = ''
     offenders = []
-    control_id = 'Id7.8'
-    compliance_type = "ecs_task_definition_pid_mode_check"
-    description = "Checks if ECSTaskDefinitions are configured to share a host’s process namespace with its Amazon " \
-                  "Elastic Container Service (Amazon ECS) containers."
+    control_id = 'Id3.38'
+    compliance_type = "ecs_task_definition_user_for_host_mode_check"
+    description = "Checks if an Amazon ECS task definition with host networking mode has 'privileged' or 'user' container definitions. . "
     resource_type = "AWS ECS TaskDefinition"
     risk_level = 'Medium'
 
     # regions = self.session.get_available_regions('ecs')
 
     for region, definitions in task_definitions.items():
+        client = self.session.client('ecs', region_name=region)
         for task_definition in definitions:
 
             try:
 
                 resp = client.describe_task_definition(taskDefinition=task_definition)
-                if resp['taskDefinition']['pidMode'] == 'host':
-                    raise KeyError
+                if resp['taskDefinition']['networkMode'] == 'host':
+                    for containerdefintion in resp['taskDefinition']['containerDefinitions']:
+                        if containerdefintion['privileged'] == 'False' or '' and containerdefintion['user'] == 'root' or '':
+                            raise KeyError
+
 
             except KeyError:
                     result = False
                     offenders.append(resp['taskDefinition']['taskDefinitionArn'])
-                    failReason = "ECSTaskDefinitions are not configured to share a host’s process namespace with its ECS containers as pidMode parameter is set to ‘host’."
+                    failReason = "There are ECSTaskDefinitions with host network mode and container definitions of privileged=false or empty and user=root or empty.."
                     continue
             
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `OBP_devops-0.1.0/OBP_devops/ecs_task_definition_user_for_host_mode_check.py` & `OBP_devops-0.1.1/OBP_devops/ecs_containers_read_only_access.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,54 +4,54 @@
 
 from OBP_devops.utils import get_regions
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger()
 
 
-def ecs_task_definition_user_for_host_mode_check(self, task_definitions) -> dict:
+def ecs_containers_read_only_access(self, task_definitions) -> dict:
     """
     :param task_definitions:
     :param self:
     :return:
     """
-    logger.info(" ---Inside OBP DevOps :: ecs_task_definition_user_for_host_mode_check()")
+    logger.info(" ---Inside OBP DevOps :: ecs_containers_read_only_access()")
 
     result = True
     failReason = ''
     offenders = []
-    control_id = 'Id3.38'
-    compliance_type = "ecs_task_definition_user_for_host_mode_check"
-    description = "Checks if an Amazon ECS task definition with host networking mode has 'privileged' or 'user' container definitions. . "
+    control_id = 'Id7.3'
+    compliance_type = "ecs_containers_read_only_access"
+    description = "Checks if Amazon Elastic Container Service (Amazon ECS) Containers only have read-only access to " \
+                  "its root filesystems. ."
     resource_type = "AWS ECS TaskDefinition"
-    risk_level = 'Medium'
+    risk_level = 'High'
 
     # regions = self.session.get_available_regions('ecs')
 
     for region, definitions in task_definitions.items():
+        client = self.session.client('ecs', region_name=region)
         for task_definition in definitions:
+            resp = client.describe_task_definition(taskDefinition=task_definition)
+            container_definitions = resp['taskDefinition']['containerDefinitions']
+            for definition in container_definitions:
+
+                try:
+                    if definition['readonlyRootFilesystem'] == 'False':
+                        raise KeyError
 
-            try:
-
-                resp = client.describe_task_definition(taskDefinition=task_definition)
-                if resp['taskDefinition']['networkMode'] == 'host':
-                    for containerdefintion in resp['taskDefinition']['containerDefinitions']:
-                        if containerdefintion['privileged'] == 'False' or '' and containerdefintion['user'] == 'root' or '':
-                            raise KeyError
-
-
-            except KeyError:
+                except KeyError:
                     result = False
-                    offenders.append(resp['taskDefinition']['taskDefinitionArn'])
-                    failReason = "There are ECSTaskDefinitions with host network mode and container definitions of privileged=false or empty and user=root or empty.."
+                    offenders.append(definition['name'])
+                    failReason = "The readonlyRootFilesystem parameter in the container definition of ECSTaskDefinitions is set to ‘false’."
                     continue
-            
+
     return {
         'Result': result,
         'failReason': failReason,
         'resource_type': resource_type,
         'Offenders': offenders,
         'Compliance_type': compliance_type,
         'Description': description,
         'Risk Level': risk_level,
         'ControlId': control_id
-    }
+    }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `OBP_devops-0.1.0/OBP_devops/eks.py` & `OBP_devops-0.1.1/OBP_devops/eks.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/elastic_beanstalk.py` & `OBP_devops-0.1.1/OBP_devops/elastic_beanstalk.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops/utils.py` & `OBP_devops-0.1.1/OBP_devops/utils.py`

 * *Files identical despite different names*

### Comparing `OBP_devops-0.1.0/OBP_devops.egg-info/SOURCES.txt` & `OBP_devops-0.1.1/OBP_devops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

