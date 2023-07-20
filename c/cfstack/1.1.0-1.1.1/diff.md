# Comparing `tmp/cfstack-1.1.0.tar.gz` & `tmp/cfstack-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfstack-1.1.0.tar", last modified: Thu Jul 20 19:00:42 2023, max compression
+gzip compressed data, was "cfstack-1.1.1.tar", last modified: Thu Jul 20 19:44:29 2023, max compression
```

## Comparing `cfstack-1.1.0.tar` & `cfstack-1.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.786232 cfstack-1.1.0/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)    35149 2023-07-18 17:43:42.000000 cfstack-1.1.0/LICENSE
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 19:00:42.786232 cfstack-1.1.0/PKG-INFO
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       38 2023-07-20 19:00:42.786232 cfstack-1.1.0/setup.cfg
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      581 2023-07-20 18:59:40.000000 cfstack-1.1.0/setup.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.778232 cfstack-1.1.0/src/
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.782232 cfstack-1.1.0/src/cfstack/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       37 2023-07-19 16:32:24.000000 cfstack-1.1.0/src/cfstack/__init__.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.782232 cfstack-1.1.0/src/cfstack/changeset/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      141 2023-07-19 16:52:23.000000 cfstack-1.1.0/src/cfstack/changeset/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      752 2023-07-20 18:34:22.000000 cfstack-1.1.0/src/cfstack/changeset/check_changeset_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1170 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/changeset/create_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      364 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/changeset/delete_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      371 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/changeset/execute_changeset.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      332 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/changeset/generate_changesetname.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     5115 2023-07-19 15:13:21.000000 cfstack-1.1.0/src/cfstack/execute.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.782232 cfstack-1.1.0/src/cfstack/s3utility/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       93 2023-07-19 16:52:54.000000 cfstack-1.1.0/src/cfstack/s3utility/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      126 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/s3utility/create_client.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      572 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/s3utility/delete_file_s3.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      523 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/s3utility/read_file_s3.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      720 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/s3utility/upload_file_s3.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.786232 cfstack-1.1.0/src/cfstack/stack/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      120 2023-07-19 16:53:56.000000 cfstack-1.1.0/src/cfstack/stack/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1067 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/stack/check_stack_delete_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      470 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/stack/check_stack_exists.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1049 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/stack/check_stack_update_status.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      392 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/stack/delete_stack.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.786232 cfstack-1.1.0/src/cfstack/utility/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      194 2023-07-19 16:54:47.000000 cfstack-1.1.0/src/cfstack/utility/__init__.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      955 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/utility/calculate_shamap.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1392 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/utility/compare_shamap.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      136 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/utility/create_client.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      949 2023-07-19 17:43:05.000000 cfstack-1.1.0/src/cfstack/utility/execute_delete.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1857 2023-07-19 17:43:48.000000 cfstack-1.1.0/src/cfstack/utility/execute_deploy.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1980 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/utility/first_time_upload.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      297 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/utility/parameter_preprocessing.py
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      917 2023-07-18 17:43:42.000000 cfstack-1.1.0/src/cfstack/utility/upload_template_s3.py
-drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:00:42.782232 cfstack-1.1.0/src/cfstack.egg-info/
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 19:00:42.000000 cfstack-1.1.0/src/cfstack.egg-info/PKG-INFO
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1236 2023-07-20 19:00:42.000000 cfstack-1.1.0/src/cfstack.egg-info/SOURCES.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        1 2023-07-20 19:00:42.000000 cfstack-1.1.0/src/cfstack.egg-info/dependency_links.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        6 2023-07-20 19:00:42.000000 cfstack-1.1.0/src/cfstack.egg-info/requires.txt
--rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        8 2023-07-20 19:00:42.000000 cfstack-1.1.0/src/cfstack.egg-info/top_level.txt
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.908753 cfstack-1.1.1/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)    35149 2023-07-18 17:43:42.000000 cfstack-1.1.1/LICENSE
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 19:44:29.908753 cfstack-1.1.1/PKG-INFO
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       38 2023-07-20 19:44:29.908753 cfstack-1.1.1/setup.cfg
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      581 2023-07-20 19:44:27.000000 cfstack-1.1.1/setup.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.904753 cfstack-1.1.1/src/
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.904753 cfstack-1.1.1/src/cfstack/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       37 2023-07-19 16:32:24.000000 cfstack-1.1.1/src/cfstack/__init__.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.904753 cfstack-1.1.1/src/cfstack/changeset/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      141 2023-07-19 16:52:23.000000 cfstack-1.1.1/src/cfstack/changeset/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      687 2023-07-20 19:42:36.000000 cfstack-1.1.1/src/cfstack/changeset/check_changeset_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1170 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/changeset/create_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      364 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/changeset/delete_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      371 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/changeset/execute_changeset.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      332 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/changeset/generate_changesetname.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     5115 2023-07-19 15:13:21.000000 cfstack-1.1.1/src/cfstack/execute.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.904753 cfstack-1.1.1/src/cfstack/s3utility/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)       93 2023-07-19 16:52:54.000000 cfstack-1.1.1/src/cfstack/s3utility/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      126 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/s3utility/create_client.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      572 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/s3utility/delete_file_s3.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      523 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/s3utility/read_file_s3.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      720 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/s3utility/upload_file_s3.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.904753 cfstack-1.1.1/src/cfstack/stack/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      120 2023-07-19 16:53:56.000000 cfstack-1.1.1/src/cfstack/stack/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1067 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/stack/check_stack_delete_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      470 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/stack/check_stack_exists.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1049 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/stack/check_stack_update_status.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      392 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/stack/delete_stack.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.908753 cfstack-1.1.1/src/cfstack/utility/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      194 2023-07-19 16:54:47.000000 cfstack-1.1.1/src/cfstack/utility/__init__.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      955 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/utility/calculate_shamap.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1392 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/utility/compare_shamap.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      136 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/utility/create_client.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      949 2023-07-19 17:43:05.000000 cfstack-1.1.1/src/cfstack/utility/execute_delete.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1839 2023-07-20 19:43:33.000000 cfstack-1.1.1/src/cfstack/utility/execute_deploy.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1980 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/utility/first_time_upload.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      297 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/utility/parameter_preprocessing.py
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      917 2023-07-18 17:43:42.000000 cfstack-1.1.1/src/cfstack/utility/upload_template_s3.py
+drwxrwxr-x   0 yashprime  (1000) yashprime  (1000)        0 2023-07-20 19:44:29.904753 cfstack-1.1.1/src/cfstack.egg-info/
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)      406 2023-07-20 19:44:29.000000 cfstack-1.1.1/src/cfstack.egg-info/PKG-INFO
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)     1236 2023-07-20 19:44:29.000000 cfstack-1.1.1/src/cfstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        1 2023-07-20 19:44:29.000000 cfstack-1.1.1/src/cfstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        6 2023-07-20 19:44:29.000000 cfstack-1.1.1/src/cfstack.egg-info/requires.txt
+-rw-rw-r--   0 yashprime  (1000) yashprime  (1000)        8 2023-07-20 19:44:29.000000 cfstack-1.1.1/src/cfstack.egg-info/top_level.txt
```

### Comparing `cfstack-1.1.0/LICENSE` & `cfstack-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/setup.py` & `cfstack-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("src/README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='cfstack',
-    version='1.1.0',
+    version='1.1.1',
     description='A utility to manage CloudFormation stacks',
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=[
             "boto3"
     ],
     python_requires='>=3',
```

### Comparing `cfstack-1.1.0/src/cfstack/changeset/create_changeset.py` & `cfstack-1.1.1/src/cfstack/changeset/create_changeset.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/execute.py` & `cfstack-1.1.1/src/cfstack/execute.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/s3utility/delete_file_s3.py` & `cfstack-1.1.1/src/cfstack/s3utility/delete_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/s3utility/read_file_s3.py` & `cfstack-1.1.1/src/cfstack/s3utility/read_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/s3utility/upload_file_s3.py` & `cfstack-1.1.1/src/cfstack/s3utility/upload_file_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/stack/check_stack_delete_status.py` & `cfstack-1.1.1/src/cfstack/stack/check_stack_delete_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/stack/check_stack_update_status.py` & `cfstack-1.1.1/src/cfstack/stack/check_stack_update_status.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/utility/calculate_shamap.py` & `cfstack-1.1.1/src/cfstack/utility/calculate_shamap.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/utility/compare_shamap.py` & `cfstack-1.1.1/src/cfstack/utility/compare_shamap.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/utility/execute_delete.py` & `cfstack-1.1.1/src/cfstack/utility/execute_delete.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/utility/execute_deploy.py` & `cfstack-1.1.1/src/cfstack/utility/execute_deploy.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,12 +32,11 @@
     response_exec = execute_changeset(client,response)
     if response_exec != "Executed":
         delete_changeset(client,response)
         return executed
     
    
     status = check_stack_update_status(client,stack)
-    print(status)
     if status == "Updated":
         delete_changeset(client,response)
         executed = "Deployed"                    
     return executed
```

### Comparing `cfstack-1.1.0/src/cfstack/utility/first_time_upload.py` & `cfstack-1.1.1/src/cfstack/utility/first_time_upload.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack/utility/upload_template_s3.py` & `cfstack-1.1.1/src/cfstack/utility/upload_template_s3.py`

 * *Files identical despite different names*

### Comparing `cfstack-1.1.0/src/cfstack.egg-info/SOURCES.txt` & `cfstack-1.1.1/src/cfstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

