# Comparing `tmp/roboflow-1.1.1.tar.gz` & `tmp/roboflow-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roboflow-1.1.1.tar", last modified: Tue Jul 11 21:33:44 2023, max compression
+gzip compressed data, was "roboflow-1.1.2.tar", last modified: Thu Jul 20 16:08:02 2023, max compression
```

## Comparing `roboflow-1.1.1.tar` & `roboflow-1.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-11 21:33:17.000000 roboflow-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-11 21:33:44.297987 roboflow-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-11 21:33:17.000000 roboflow-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-11 21:33:17.000000 roboflow-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/archive/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    27929 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/core/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/models/semantic_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/roboflow/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/active_learning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/clip_compare_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/two_stage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-11 21:33:17.000000 roboflow-1.1.1/roboflow/util/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.293986 roboflow-1.1.1/roboflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 21:33:44.000000 roboflow-1.1.1/roboflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 21:33:44.297987 roboflow-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-11 21:33:17.000000 roboflow-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/test_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/test_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/models/test_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/test_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 21:33:44.297987 roboflow-1.1.1/tests/util/dummy_module/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/dummy_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/test_image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-11 21:33:17.000000 roboflow-1.1.1/tests/util/test_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.550425 roboflow-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-07-20 16:07:26.000000 roboflow-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-20 16:08:02.550425 roboflow-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6312 2023-07-20 16:07:26.000000 roboflow-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 16:07:26.000000 roboflow-1.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.542425 roboflow-1.1.2/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.542425 roboflow-1.1.2/roboflow/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/archive/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.546424 roboflow-1.1.2/roboflow/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25310 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/core/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27921 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/core/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19331 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/core/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.546424 roboflow-1.1.2/roboflow/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/models/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/models/instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20832 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/models/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/models/semantic_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.546424 roboflow-1.1.2/roboflow/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/active_learning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/clip_compare_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/two_stage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-07-20 16:07:26.000000 roboflow-1.1.2/roboflow/util/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.542425 roboflow-1.1.2/roboflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8194 2023-07-20 16:08:02.000000 roboflow-1.1.2/roboflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-20 16:08:02.000000 roboflow-1.1.2/roboflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:08:02.000000 roboflow-1.1.2/roboflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-20 16:08:02.000000 roboflow-1.1.2/roboflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 16:08:02.000000 roboflow-1.1.2/roboflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:08:02.550425 roboflow-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-20 16:07:26.000000 roboflow-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.546424 roboflow-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.550425 roboflow-1.1.2/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/models/test_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/models/test_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/models/test_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/test_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.550425 roboflow-1.1.2/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:08:02.550425 roboflow-1.1.2/tests/util/dummy_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/util/dummy_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/util/test_image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-20 16:07:26.000000 roboflow-1.1.2/tests/util/test_versions.py
```

### Comparing `roboflow-1.1.1/LICENSE` & `roboflow-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/PKG-INFO` & `roboflow-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.1.1
+Version: 1.1.2
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.1.1 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.1.2 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.1.1/README.md` & `roboflow-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/__init__.py` & `roboflow-1.1.2/roboflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import requests
 
 from roboflow.config import API_URL, APP_URL, DEMO_KEYS, load_roboflow_api_key
 from roboflow.core.project import Project
 from roboflow.core.workspace import Workspace
 from roboflow.util.general import write_line
 
-__version__ = "1.1.1"
+__version__ = "1.1.2"
 
 
 def check_key(api_key, model, notebook, num_retries=0):
     if type(api_key) is not str:
         raise RuntimeError(
             "API Key is of Incorrect Type \n Expected Type: "
             + str(type(""))
```

### Comparing `roboflow-1.1.1/roboflow/archive/plot.py` & `roboflow-1.1.2/roboflow/archive/plot.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/config.py` & `roboflow-1.1.2/roboflow/config.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/core/project.py` & `roboflow-1.1.2/roboflow/core/project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/core/version.py` & `roboflow-1.1.2/roboflow/core/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,19 +177,19 @@
         self.__wait_if_generating()
 
         if model_format == "yolov8":
             # if ultralytics is installed, we will assume users will want to use yolov8 and we check for the supported version
             try:
                 import_module("ultralytics")
                 print_warn_for_wrong_dependencies_versions(
-                    [("ultralytics", "<=", "8.0.20")]
+                    [("ultralytics", "==", "8.0.134")]
                 )
             except ImportError as e:
                 print(
-                    "[WARNING] we noticed you are downloading a `yolov8` datasets but you don't have `ultralytics` installed. Roboflow `.deploy` supports only models trained with `ultralytics<=8.0.20`, to intall it `pip install ultralytics<=8.0.20`."
+                    "[WARNING] we noticed you are downloading a `yolov8` datasets but you don't have `ultralytics` installed. Roboflow `.deploy` supports only models trained with `ultralytics==8.0.134`, to intall it `pip install ultralytics==8.0.134`."
                 )
                 # silently fail
                 pass
 
         model_format = self.__get_format_identifier(model_format)
 
         if model_format not in self.exports:
@@ -430,15 +430,15 @@
             previous_epochs = copy.deepcopy(epochs)
 
             time.sleep(5)
 
         # return the model object
         return self.model
 
-    # @warn_for_wrong_dependencies_versions([("ultralytics", "<=", "8.0.20")])
+    # @warn_for_wrong_dependencies_versions([("ultralytics", "==", "8.0.134")])
     def deploy(self, model_type: str, model_path: str) -> None:
         """Uploads provided weights file to Roboflow
 
         Args:
             model_path (str): File path to model weights to be uploaded
         """
 
@@ -460,15 +460,15 @@
 
             except ImportError as e:
                 raise (
                     "The ultralytics python package is required to deploy yolov8 models. Please install it with `pip install ultralytics`"
                 )
 
             print_warn_for_wrong_dependencies_versions(
-                [("ultralytics", "<=", "8.0.20")]
+                [("ultralytics", "==", "8.0.134")]
             )
 
         elif "yolov5" in model_type or "yolov7" in model_type:
             try:
                 import torch
             except ImportError as e:
                 raise (
@@ -589,22 +589,22 @@
             data=open(os.path.join(model_path, "roboflow_deploy.zip"), "rb"),
         )
         try:
             res.raise_for_status()
 
             if self.public:
                 print(
-                    f"View the status of your deployment at: {APP_URL}/{self.workspace}/{self.project}/deploy/{self.version}"
+                    f"View the status of your deployment at: {APP_URL}/{self.workspace}/{self.project}/{self.version}"
                 )
                 print(
                     f"Share your model with the world at: {UNIVERSE_URL}/{self.workspace}/{self.project}/model/{self.version}"
                 )
             else:
                 print(
-                    f"View the status of your deployment at: {APP_URL}/{self.workspace}/{self.project}/deploy/{self.version}"
+                    f"View the status of your deployment at: {APP_URL}/{self.workspace}/{self.project}/{self.version}"
                 )
 
         except Exception as e:
             print(f"An error occured when uploading the model: {e}")
 
     def __download_zip(self, link, location, format):
         """
@@ -726,15 +726,15 @@
                 content["test"] = location + content["test"].lstrip(".")
             if format in ["yolov5pytorch", "yolov7pytorch", "yolov8"]:
                 content["train"] = location + content["train"].lstrip("..")
                 content["val"] = location + content["val"].lstrip("..")
             try:
                 # get_wrong_dependencies_versions raises exception if ultralytics is not installed at all
                 if format == "yolov8" and not get_wrong_dependencies_versions(
-                    dependencies_versions=[("ultralytics", ">=", "8.0.30")]
+                    dependencies_versions=[("ultralytics", "==", "8.0.134")]
                 ):
                     content["train"] = "train/images"
                     content["val"] = "valid/images"
                     content["test"] = "test/images"
             except ModuleNotFoundError:
                 pass
             return content
```

### Comparing `roboflow-1.1.1/roboflow/core/workspace.py` & `roboflow-1.1.2/roboflow/core/workspace.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/models/classification.py` & `roboflow-1.1.2/roboflow/models/classification.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/models/inference.py` & `roboflow-1.1.2/roboflow/models/inference.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/models/instance_segmentation.py` & `roboflow-1.1.2/roboflow/models/instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/models/object_detection.py` & `roboflow-1.1.2/roboflow/models/object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/models/semantic_segmentation.py` & `roboflow-1.1.2/roboflow/models/semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/util/active_learning_utils.py` & `roboflow-1.1.2/roboflow/util/active_learning_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/util/clip_compare_utils.py` & `roboflow-1.1.2/roboflow/util/clip_compare_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/util/image_utils.py` & `roboflow-1.1.2/roboflow/util/image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/util/prediction.py` & `roboflow-1.1.2/roboflow/util/prediction.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/util/two_stage_utils.py` & `roboflow-1.1.2/roboflow/util/two_stage_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow/util/versions.py` & `roboflow-1.1.2/roboflow/util/versions.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/roboflow.egg-info/PKG-INFO` & `roboflow-1.1.2/roboflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roboflow
-Version: 1.1.1
+Version: 1.1.2
 Summary: python client for the Roboflow application
 Home-page: https://github.com/roboflow-ai/roboflow-python
 Author: Roboflow
 Author-email: jacob@roboflow.com
 License: UNKNOWN
 Description: # Roboflow Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: roboflow Version: 1.1.1 Summary: python client for
+Metadata-Version: 2.1 Name: roboflow Version: 1.1.2 Summary: python client for
 the Roboflow application Home-page: https://github.com/roboflow-ai/roboflow-
 python Author: Roboflow Author-email: jacob@roboflow.com License: UNKNOWN
 Description: # Roboflow Python --- ![roboflow logo](https://media.roboflow.com/
 homepage/cv_pipeline_compact.png?updatedAt=1679939317160)
 [https://media.roboflow.com/notebooks/template/icons/purple/youtube.png?ik-sdk-
           version=javascript-1.4.3&updatedAt=1672949634652] [https://
 raw.githubusercontent.com/ultralytics/assets/main/social/logo-transparent.png]
```

### Comparing `roboflow-1.1.1/roboflow.egg-info/SOURCES.txt` & `roboflow-1.1.2/roboflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/setup.py` & `roboflow-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/models/test_instance_segmentation.py` & `roboflow-1.1.2/tests/models/test_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/models/test_object_detection.py` & `roboflow-1.1.2/tests/models/test_object_detection.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/models/test_semantic_segmentation.py` & `roboflow-1.1.2/tests/models/test_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/test_project.py` & `roboflow-1.1.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/test_queries.py` & `roboflow-1.1.2/tests/test_queries.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/test_version.py` & `roboflow-1.1.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/util/test_image_utils.py` & `roboflow-1.1.2/tests/util/test_image_utils.py`

 * *Files identical despite different names*

### Comparing `roboflow-1.1.1/tests/util/test_versions.py` & `roboflow-1.1.2/tests/util/test_versions.py`

 * *Files identical despite different names*

