# Comparing `tmp/cfstack-1.1.2.tar.gz` & `tmp/cfstack-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfstack-1.1.2.tar", last modified: Thu Jul 20 19:53:52 2023, max compression
+gzip compressed data, was "cfstack-1.1.3.tar", last modified: Thu Jul 20 20:02:49 2023, max compression
```

## Comparing `cfstack-1.1.2.tar` & `cfstack-1.1.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.750161 cfstack-1.1.2/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)    35149 2023-07-18 17:43:42.000000 cfstack-1.1.2/LICENSE
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 19:53:52.750161 cfstack-1.1.2/PKG-INFO
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       38 2023-07-20 19:53:52.750161 cfstack-1.1.2/setup.cfg
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      581 2023-07-20 19:53:50.000000 cfstack-1.1.2/setup.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.742161 cfstack-1.1.2/src/
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.742161 cfstack-1.1.2/src/cfstack/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       37 2023-07-19 16:32:24.000000 cfstack-1.1.2/src/cfstack/__init__.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.746161 cfstack-1.1.2/src/cfstack/changeset/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      141 2023-07-19 16:52:23.000000 cfstack-1.1.2/src/cfstack/changeset/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      687 2023-07-20 19:42:36.000000 cfstack-1.1.2/src/cfstack/changeset/check_changeset_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1170 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/changeset/create_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      364 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/changeset/delete_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      371 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/changeset/execute_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      332 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/changeset/generate_changesetname.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     5216 2023-07-20 19:52:29.000000 cfstack-1.1.2/src/cfstack/execute.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.746161 cfstack-1.1.2/src/cfstack/s3utility/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       93 2023-07-19 16:52:54.000000 cfstack-1.1.2/src/cfstack/s3utility/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      126 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/s3utility/create_client.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      572 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/s3utility/delete_file_s3.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      523 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/s3utility/read_file_s3.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      720 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/s3utility/upload_file_s3.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.746161 cfstack-1.1.2/src/cfstack/stack/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      120 2023-07-19 16:53:56.000000 cfstack-1.1.2/src/cfstack/stack/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1067 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/stack/check_stack_delete_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      470 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/stack/check_stack_exists.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1049 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/stack/check_stack_update_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      392 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/stack/delete_stack.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.746161 cfstack-1.1.2/src/cfstack/utility/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      194 2023-07-19 16:54:47.000000 cfstack-1.1.2/src/cfstack/utility/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      955 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/utility/calculate_shamap.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1392 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/utility/compare_shamap.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      136 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/utility/create_client.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      949 2023-07-19 17:43:05.000000 cfstack-1.1.2/src/cfstack/utility/execute_delete.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1839 2023-07-20 19:43:33.000000 cfstack-1.1.2/src/cfstack/utility/execute_deploy.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1980 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/utility/first_time_upload.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      297 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/utility/parameter_preprocessing.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      917 2023-07-18 17:43:42.000000 cfstack-1.1.2/src/cfstack/utility/upload_template_s3.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:53:52.746161 cfstack-1.1.2/src/cfstack.egg-info/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 19:53:52.000000 cfstack-1.1.2/src/cfstack.egg-info/PKG-INFO
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1236 2023-07-20 19:53:52.000000 cfstack-1.1.2/src/cfstack.egg-info/SOURCES.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        1 2023-07-20 19:53:52.000000 cfstack-1.1.2/src/cfstack.egg-info/dependency_links.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        6 2023-07-20 19:53:52.000000 cfstack-1.1.2/src/cfstack.egg-info/requires.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        8 2023-07-20 19:53:52.000000 cfstack-1.1.2/src/cfstack.egg-info/top_level.txt
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.535181 cfstack-1.1.3/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)    35149 2023-07-18 17:43:42.000000 cfstack-1.1.3/LICENSE
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 20:02:49.535181 cfstack-1.1.3/PKG-INFO
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       38 2023-07-20 20:02:49.535181 cfstack-1.1.3/setup.cfg
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      581 2023-07-20 20:02:48.000000 cfstack-1.1.3/setup.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.531180 cfstack-1.1.3/src/
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.531180 cfstack-1.1.3/src/cfstack/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       37 2023-07-19 16:32:24.000000 cfstack-1.1.3/src/cfstack/__init__.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.531180 cfstack-1.1.3/src/cfstack/changeset/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      141 2023-07-19 16:52:23.000000 cfstack-1.1.3/src/cfstack/changeset/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      687 2023-07-20 19:42:36.000000 cfstack-1.1.3/src/cfstack/changeset/check_changeset_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1170 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/changeset/create_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      364 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/changeset/delete_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      371 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/changeset/execute_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      332 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/changeset/generate_changesetname.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     5351 2023-07-20 20:02:15.000000 cfstack-1.1.3/src/cfstack/execute.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.535181 cfstack-1.1.3/src/cfstack/s3utility/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       93 2023-07-19 16:52:54.000000 cfstack-1.1.3/src/cfstack/s3utility/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      126 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/s3utility/create_client.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      572 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/s3utility/delete_file_s3.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      523 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/s3utility/read_file_s3.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      720 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/s3utility/upload_file_s3.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.535181 cfstack-1.1.3/src/cfstack/stack/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      120 2023-07-19 16:53:56.000000 cfstack-1.1.3/src/cfstack/stack/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1067 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/stack/check_stack_delete_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      470 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/stack/check_stack_exists.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1049 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/stack/check_stack_update_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      392 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/stack/delete_stack.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.535181 cfstack-1.1.3/src/cfstack/utility/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      194 2023-07-19 16:54:47.000000 cfstack-1.1.3/src/cfstack/utility/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      955 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/utility/calculate_shamap.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1392 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/utility/compare_shamap.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      136 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/utility/create_client.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      949 2023-07-19 17:43:05.000000 cfstack-1.1.3/src/cfstack/utility/execute_delete.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1839 2023-07-20 19:43:33.000000 cfstack-1.1.3/src/cfstack/utility/execute_deploy.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1980 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/utility/first_time_upload.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      297 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/utility/parameter_preprocessing.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      917 2023-07-18 17:43:42.000000 cfstack-1.1.3/src/cfstack/utility/upload_template_s3.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 20:02:49.531180 cfstack-1.1.3/src/cfstack.egg-info/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 20:02:49.000000 cfstack-1.1.3/src/cfstack.egg-info/PKG-INFO
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1236 2023-07-20 20:02:49.000000 cfstack-1.1.3/src/cfstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        1 2023-07-20 20:02:49.000000 cfstack-1.1.3/src/cfstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        6 2023-07-20 20:02:49.000000 cfstack-1.1.3/src/cfstack.egg-info/requires.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        8 2023-07-20 20:02:49.000000 cfstack-1.1.3/src/cfstack.egg-info/top_level.txt
```

### Comparing `cfstack-1.1.2/LICENSE` & `cfstack-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/setup.py` & `cfstack-1.1.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("src/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cfstack',
-    version='1.1.2',
+    version='1.1.3',
     description='A utility to manage CloudFormation stacks',
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
             "boto3"
     ],
     python_requires='>=3',
```

### Comparing `cfstack-1.1.2/src/cfstack/changeset/check_changeset_status.py` & `cfstack-1.1.3/src/cfstack/changeset/check_changeset_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/changeset/create_changeset.py` & `cfstack-1.1.3/src/cfstack/changeset/create_changeset.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/execute.py` & `cfstack-1.1.3/src/cfstack/execute.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,24 +45,27 @@
                 "Key":stack_path.split("/")[-1]
             }
             upload_file_s3(s3client,stack_file_details,True)
  
        
     
     # Step 4
+    
     different_stacks,todelete_stacks=compare_shamap(prod_s3,prod_calc)
+    no_change_instacks = True
     should_s3prod_be_updated = False
     for region in different_stacks["Stacks"]:
         for stack in different_stacks["Stacks"][region]:
             if different_stacks["Stacks"][region][stack]["SkipUpdate"]:
                 if not (stack in prod_s3["Stacks"][region]):
                     del prod_calc["Stacks"][region][stack]
                 else:
                     prod_calc["Stacks"][region][stack]=prod_s3["Stacks"][region][stack]
                 continue
+            no_change_instacks = False
             stack_path = different_stacks["Stacks"][region][stack]["TemplatePath"]
             stack_parameters = different_stacks["Stacks"][region][stack]["Parameters"]
             stack_details={"Region":region,"StackName":stack,"TemplateURL":f"https://{bucket_name}.s3.{bucket_region}.amazonaws.com/{stack_path.split('/')[-1]}","Parameters":parameter_preprocessing(stack_parameters)}
             status=execute_deploy(stack_details)
             if status == "Deployed":
                 stack_file_details = {
                     "FilePath":different_stacks["Stacks"][region][stack]["TemplatePath"],   
@@ -79,14 +82,15 @@
 
     # Step 5
     for region in todelete_stacks["Stacks"]:
         for stack in todelete_stacks["Stacks"][region]:
             stack_path = todelete_stacks["Stacks"][region][stack]["TemplatePath"]
             stack_parameters = todelete_stacks["Stacks"][region][stack]["Parameters"]
             stack_details={"Region":region,"StackName":stack,"TemplateURL":f"https://{bucket_name}.s3.{bucket_region}.amazonaws.com/{stack_path.split('/')[-1]}","Parameters":parameter_preprocessing(stack_parameters)}
+            no_change_instacks = False
             status=execute_delete(stack_details)
             if status == "Deleted":
                 stack_file_prod_details = {
                     "FilePath":todelete_stacks["Stacks"][region][stack]["TemplatePath"],   
                     "BucketName":bucket_name,
                     "Key":"templates-prod/"+stack_path.split('/')[-1]
                 }
@@ -110,11 +114,12 @@
             json.dump(prod_calc, outfile)
         prod_file_details={
             "BucketName":bucket_name,
             "FilePath":"prod_calc.json",
             "Key":"prod.json"   
         }
         upload_file_s3(s3client,prod_file_details,True)
-    else:
+    
+    if no_change_instacks:
         print("No changes in any stack")
     
     return status_code
```

### Comparing `cfstack-1.1.2/src/cfstack/s3utility/delete_file_s3.py` & `cfstack-1.1.3/src/cfstack/s3utility/delete_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/s3utility/read_file_s3.py` & `cfstack-1.1.3/src/cfstack/s3utility/read_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/s3utility/upload_file_s3.py` & `cfstack-1.1.3/src/cfstack/s3utility/upload_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/stack/check_stack_delete_status.py` & `cfstack-1.1.3/src/cfstack/stack/check_stack_delete_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/stack/check_stack_update_status.py` & `cfstack-1.1.3/src/cfstack/stack/check_stack_update_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/utility/calculate_shamap.py` & `cfstack-1.1.3/src/cfstack/utility/calculate_shamap.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/utility/compare_shamap.py` & `cfstack-1.1.3/src/cfstack/utility/compare_shamap.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/utility/execute_delete.py` & `cfstack-1.1.3/src/cfstack/utility/execute_delete.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/utility/execute_deploy.py` & `cfstack-1.1.3/src/cfstack/utility/execute_deploy.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/utility/first_time_upload.py` & `cfstack-1.1.3/src/cfstack/utility/first_time_upload.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack/utility/upload_template_s3.py` & `cfstack-1.1.3/src/cfstack/utility/upload_template_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.2/src/cfstack.egg-info/SOURCES.txt` & `cfstack-1.1.3/src/cfstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

