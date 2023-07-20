# Comparing `tmp/threemystic_cloud_data_client-0.1.14.tar.gz` & `tmp/threemystic_cloud_data_client-0.1.15.tar.gz`

## Comparing `threemystic_cloud_data_client-0.1.14.tar` & `threemystic_cloud_data_client-0.1.15.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/__version__.py
--rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_data_client.py
--rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cli/__init__.py
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cli/actions/base_class/base.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cli/actions/config/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
--rw-r--r--   0        0        0     5750 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
--rw-r--r--   0        0        0    23358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
--rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
--rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
--rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
--rw-r--r--   0        0        0    10170 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
--rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
--rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
--rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/base_class/base.py
--rw-r--r--   0        0        0    11686 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
--rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/__init__.py
--rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
--rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/README.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/hatch.toml
--rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/pyproject.toml
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/__version__.py
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_data_client.py
+-rw-r--r--   0        0        0     4150 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cli/__init__.py
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cli/actions/base_class/base.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cli/actions/config/__init__.py
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/__init__.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/base_class/base.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/client/__init__.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py
+-rw-r--r--   0        0        0     5730 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/config/base_class/base.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/base_class/base.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/__init__.py
+-rw-r--r--   0        0        0    23358 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py
+-rw-r--r--   0        0        0    11920 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py
+-rw-r--r--   0        0        0    10170 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py
+-rw-r--r--   0        0        0     5770 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py
+-rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py
+-rw-r--r--   0        0        0    11874 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/config/base_class/base.py
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/base_class/base.py
+-rw-r--r--   0        0        0    11700 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py
+-rw-r--r--   0        0        0    21820 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/__init__.py
+-rw-r--r--   0        0        0     4709 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py
+-rw-r--r--   0        0        0    14025 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/config/base_class/base.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/hatch.toml
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 threemystic_cloud_data_client-0.1.15/PKG-INFO
```

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_data_client.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_data_client.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cli/__init__.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cli/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cli/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cli/actions/config/__init__.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cli/actions/config/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/__init__.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/client/actions/vmimage.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,31 @@
   def __init__(self, *args, **kwargs):
     super().__init__(
       data_action="ami", 
       logger_name= "cloud_data_client_aws_client_action",
       uniqueid_lambda = lambda: True,
       *args, **kwargs)
     
+    
+    self.data_id_name = "ImageId"
+    
+    self.arn_lambda = (lambda item: self.get_cloud_client().get_resource_general_arn(
+      resource_type= "ec2",
+      resource_type_sub= "image", **item # {region, account_id, resource_id}
+    ))
+    
     self.auto_region_resourcebytype= ["Amazon Elastic Compute Cloud - Compute"]
     self.resource_group_filter = [
       {
         'Name': 'resource-type',
         'Values': [
           'AWS::EC2::Image',
         ]
       }
     ]
-    self.arn_lambda = (lambda item: self.get_cloud_client().get_resource_general_arn(
-      resource_type= "ec2",
-      resource_type_sub= "image", **item # {region, account_id, resource_id}
-    ))
-    self.data_id_name = "ImageId"
   
   
   
   async def _process_account_data_region(self, account, region, resource_groups, loop, *args, **kwargs):
     ec2_client = self.get_cloud_client().get_boto_client(
       client= "ec2",
       account= account,
@@ -41,8 +44,8 @@
       boto_key="Images"
     )
 
     return {
       "region": region,
       "resource_groups": resource_groups,
       "data": awsdata
-    }
+    }
```

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/client/actions/base_class/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,48 +10,48 @@
   def auto_region_resourcebytype(self, *args, **kwargs):
     if hasattr(self, "_auto_region_resourcebytype"):
       return self._auto_region_resourcebytype
     
     return []
   
   @auto_region_resourcebytype.setter
-  def _set_auto_region_resourcebytype(self, value, *args, **kwargs):
+  def auto_region_resourcebytype(self, value, *args, **kwargs):
     self._auto_region_resourcebytype = value
 
   @property  
   def resource_group_filter(self, *args, **kwargs):
     if hasattr(self, "_resource_group_filter"):
       return self._resource_group_filter
     
     return []
   
   @resource_group_filter.setter
-  def _set_resource_group_filter(self, value, *args, **kwargs):
+  def resource_group_filter(self, value, *args, **kwargs):
     self._resource_group_filter = value
   
   @property
   def arn_lambda(self, *args, **kwargs):
     if hasattr(self, "_arn_lambda"):
       return self._arn_lambda
     
     return lambda item: None
   
   @arn_lambda.setter
-  def _set_arn_lambda(self, value, *args, **kwargs):
+  def arn_lambda(self, value, *args, **kwargs):
     self._arn_lambda = value
   
   @property
   def data_id_name(self):
     if hasattr(self, "_data_id_name"):
       return self._data_id_name
     
     return None
   
   @data_id_name.setter
-  def _set_data_id_name(self, value):
+  def data_id_name(self, value):
     self._data_id_name = value
 
   def get_accounts(self, *args, **kwargs):
 
     if len(self.get_runparam_key(data_key= "data_accounts", default_value= [])) < 1:
       return [ 
         account for account in self.get_cloud_client().get_accounts()
```

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/aws/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/__init__.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/budget.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/certificates.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/cloudstorage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/database.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/datawarehouse.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/dns.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/memorydb.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/secrets.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/storage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vm.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmimage.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/vmss.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/client/actions/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/azure/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/base_class/base.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/base_class/base.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/base_class/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,21 +39,21 @@
       "--budget": {
         "default": None, 
         "const": "budget",
         "dest": "data_action",
         "help": "Data Action: This pulls a general budget to provide you insights in your accounts/subscriptions",
         "action": 'store_const'
       },
-      "--secrets": {
-        "default": None, 
-        "const": "secrets",
-        "dest": "data_action",
-        "help": "Data Action: Pulls Key Vaults Secrets and Keys / Paramater Store",
-        "action": 'store_const'
-      },
+      # "--secrets": {
+      #   "default": None, 
+      #   "const": "secrets",
+      #   "dest": "data_action",
+      #   "help": "Data Action: Pulls Key Vaults Secrets and Keys / Paramater Store",
+      #   "action": 'store_const'
+      # },
       "--storage": {
         "default": None, 
         "const": "storage",
         "dest": "data_action",
         "help": "Data Action: This pulls either VM Disks or EC2 Storage depending on the provider",
         "action": 'store_const'
       },
```

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/base_class/base_data.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/__init__.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/__init__.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/config/step_1.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py` & `threemystic_cloud_data_client-0.1.15/threemystic_cloud_data_client/cloud_providers/general/config/step_2.py`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/.gitignore` & `threemystic_cloud_data_client-0.1.15/.gitignore`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/LICENSE` & `threemystic_cloud_data_client-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/README.md` & `threemystic_cloud_data_client-0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/hatch.toml` & `threemystic_cloud_data_client-0.1.15/hatch.toml`

 * *Files identical despite different names*

### Comparing `threemystic_cloud_data_client-0.1.14/pyproject.toml` & `threemystic_cloud_data_client-0.1.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "colorama; platform_system == 'Windows'",
   "threemystic-common >= 0.1.15",
-  "threemystic-cloud-client >= 0.1.34",
+  "threemystic-cloud-client >= 0.1.35",
   "typing-extensions >= 4.4.0",
   "asyncio >= 3.4.3",
   "tqdm >= 4.65.0",
   "azure-mgmt-cosmosdb >= 9",
   "azure-mgmt-costmanagement >= 4",
   "azure-mgmt-dns >= 8",
   "azure-mgmt-keyvault >= 10",
```

### Comparing `threemystic_cloud_data_client-0.1.14/PKG-INFO` & `threemystic_cloud_data_client-0.1.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threemystic-cloud-data-client
-Version: 0.1.14
+Version: 0.1.15
 Summary: A tool for collecting data from various cloud providers
 Project-URL: Homepage, https://github.com/3MysticApes/3mystic_cloud_data_client
 Project-URL: Bug Tracker, https://github.com/3MysticApes/3mystic_cloud_data_client/issues
 Author: Ron Truex
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
@@ -34,15 +34,15 @@
 Requires-Dist: azure-mgmt-redis>=14
 Requires-Dist: azure-mgmt-resourcegraph>=8
 Requires-Dist: azure-mgmt-sql>=3
 Requires-Dist: azure-mgmt-sqlvirtualmachine>=0.6
 Requires-Dist: azure-mgmt-subscription>=3
 Requires-Dist: azure-mgmt-synapse>=2
 Requires-Dist: colorama; platform_system == 'Windows'
-Requires-Dist: threemystic-cloud-client>=0.1.34
+Requires-Dist: threemystic-cloud-client>=0.1.35
 Requires-Dist: threemystic-common>=0.1.15
 Requires-Dist: tqdm>=4.65.0
 Requires-Dist: typing-extensions>=4.4.0
 Description-Content-Type: text/markdown
 
 # 3mystic_cloud_data_client
 A set of scripts to help uniformly pull data from the cloud providers for various resources.
```

