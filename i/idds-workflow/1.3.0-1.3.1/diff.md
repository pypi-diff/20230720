# Comparing `tmp/idds-workflow-1.3.0.tar.gz` & `tmp/idds-workflow-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-workflow-1.3.0.tar", last modified: Wed Jul 12 16:01:39 2023, max compression
+gzip compressed data, was "idds-workflow-1.3.1.tar", last modified: Thu Jul 20 07:28:48 2023, max compression
```

## Comparing `idds-workflow-1.3.0.tar` & `idds-workflow-1.3.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.045985 idds-workflow-1.3.0/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.045985 idds-workflow-1.3.0/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/lib/idds/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:34.000000 idds-workflow-1.3.0/lib/idds/workflow/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    80453 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/work.py
--rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/lib/idds/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/datawork.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/processingwork.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    81884 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/work.py
--rw-r--r--   0 runner    (1001) docker     (123)   103065 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/lib/idds/workflowv2/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/lib/idds_workflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-12 16:01:39.000000 idds-workflow-1.3.0/lib/idds_workflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-12 16:01:25.000000 idds-workflow-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.045985 idds-workflow-1.3.0/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 16:01:39.049986 idds-workflow-1.3.0/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 16:01:34.000000 idds-workflow-1.3.0/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.546097 idds-workflow-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 07:28:48.546097 idds-workflow-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.542097 idds-workflow-1.3.1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.542097 idds-workflow-1.3.1/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.542097 idds-workflow-1.3.1/lib/idds/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 07:28:43.000000 idds-workflow-1.3.1/lib/idds/workflow/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80453 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90930 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.546097 idds-workflow-1.3.1/lib/idds/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/datawork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/processingwork.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81884 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/work.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103065 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/lib/idds/workflowv2/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.546097 idds-workflow-1.3.1/lib/idds_workflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-07-20 07:28:48.000000 idds-workflow-1.3.1/lib/idds_workflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 07:28:48.000000 idds-workflow-1.3.1/lib/idds_workflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:28:48.000000 idds-workflow-1.3.1/lib/idds_workflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 07:28:48.000000 idds-workflow-1.3.1/lib/idds_workflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 07:28:48.000000 idds-workflow-1.3.1/lib/idds_workflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 07:28:48.546097 idds-workflow-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-20 07:28:36.000000 idds-workflow-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.542097 idds-workflow-1.3.1/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:28:48.546097 idds-workflow-1.3.1/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 07:28:43.000000 idds-workflow-1.3.1/tools/env/environment.yml
```

### Comparing `idds-workflow-1.3.0/LICENSE.rst` & `idds-workflow-1.3.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/PKG-INFO` & `idds-workflow-1.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 1.3.0
+Version: 1.3.1
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-workflow-1.3.0/lib/idds/workflow/base.py` & `idds-workflow-1.3.1/lib/idds/workflow/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflow/datawork.py` & `idds-workflow-1.3.1/lib/idds/workflow/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflow/processingwork.py` & `idds-workflow-1.3.1/lib/idds/workflow/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflow/utils.py` & `idds-workflow-1.3.1/lib/idds/workflow/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflow/work.py` & `idds-workflow-1.3.1/lib/idds/workflow/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflow/workflow.py` & `idds-workflow-1.3.1/lib/idds/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/base.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/base.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/datawork.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/datawork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/processingwork.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/processingwork.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/tree.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/tree.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/utils.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/utils.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/work.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/work.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds/workflowv2/workflow.py` & `idds-workflow-1.3.1/lib/idds/workflowv2/workflow.py`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/lib/idds_workflow.egg-info/PKG-INFO` & `idds-workflow-1.3.1/lib/idds_workflow.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-workflow
-Version: 1.3.0
+Version: 1.3.1
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-workflow-1.3.0/lib/idds_workflow.egg-info/SOURCES.txt` & `idds-workflow-1.3.1/lib/idds_workflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-workflow-1.3.0/setup.py` & `idds-workflow-1.3.1/setup.py`

 * *Files identical despite different names*

