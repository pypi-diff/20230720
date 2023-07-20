# Comparing `tmp/manot-0.8.3.tar.gz` & `tmp/manot-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manot-0.8.3.tar", last modified: Wed May 31 11:11:15 2023, max compression
+gzip compressed data, was "manot-0.8.4.tar", last modified: Thu Jul 20 08:31:07 2023, max compression
```

## Comparing `manot-0.8.3.tar` & `manot-0.8.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/
--rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.3/LICENSE
--rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-05-31 11:11:14.999904 manot-0.8.3/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)     6135 2023-05-31 09:09:00.000000 manot-0.8.3/README.md
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/manot.egg-info/
--rw-rw-r--   0 armen     (1000) armen     (1000)     7099 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/PKG-INFO
--rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/SOURCES.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/dependency_links.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/requires.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-05-31 11:11:14.000000 manot-0.8.3/manot.egg-info/top_level.txt
--rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-05-31 11:11:07.000000 manot-0.8.3/pyproject.toml
--rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-05-31 11:11:14.999904 manot-0.8.3/setup.cfg
--rw-rw-r--   0 armen     (1000) armen     (1000)      816 2023-05-31 11:11:07.000000 manot-0.8.3/setup.py
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/src/
-drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-05-31 11:11:14.999904 manot-0.8.3/src/manot/
--rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.3/src/manot/__init__.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.3/src/manot/logger.py
--rw-rw-r--   0 armen     (1000) armen     (1000)    12035 2023-05-31 10:48:45.000000 manot-0.8.3/src/manot/manot.py
--rw-rw-r--   0 armen     (1000) armen     (1000)     4890 2023-05-31 09:09:00.000000 manot-0.8.3/src/manot/upload_manager.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1061 2023-02-14 12:07:02.000000 manot-0.8.4/LICENSE
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7264 2023-07-20 08:31:07.203016 manot-0.8.4/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)     6300 2023-07-18 11:34:28.000000 manot-0.8.4/README.md
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/manot.egg-info/
+-rw-rw-r--   0 armen     (1000) armen     (1000)     7264 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/PKG-INFO
+-rw-rw-r--   0 armen     (1000) armen     (1000)      274 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/SOURCES.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        1 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/dependency_links.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)       59 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/requires.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)        6 2023-07-20 08:31:07.000000 manot-0.8.4/manot.egg-info/top_level.txt
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1074 2023-07-18 11:34:28.000000 manot-0.8.4/pyproject.toml
+-rw-rw-r--   0 armen     (1000) armen     (1000)       38 2023-07-20 08:31:07.203016 manot-0.8.4/setup.cfg
+-rw-rw-r--   0 armen     (1000) armen     (1000)      819 2023-07-18 11:34:28.000000 manot-0.8.4/setup.py
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/src/
+drwxrwxr-x   0 armen     (1000) armen     (1000)        0 2023-07-20 08:31:07.203016 manot-0.8.4/src/manot/
+-rw-rw-r--   0 armen     (1000) armen     (1000)       78 2023-02-14 12:07:02.000000 manot-0.8.4/src/manot/__init__.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     1358 2023-02-14 12:07:02.000000 manot-0.8.4/src/manot/logger.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)    12155 2023-07-20 08:29:25.000000 manot-0.8.4/src/manot/manot.py
+-rw-rw-r--   0 armen     (1000) armen     (1000)     4895 2023-07-20 08:29:21.000000 manot-0.8.4/src/manot/upload_manager.py
```

### Comparing `manot-0.8.3/LICENSE` & `manot-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `manot-0.8.3/PKG-INFO` & `manot-0.8.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: manot
-Version: 0.8.3
-Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
-Home-page: https://www.manot.ai
-Author: manot
-Author-email: manot <engineering@manot.ai>
-License: MIT
-Project-URL: Homepage, https://www.manot.ai
-Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
-Project-URL: Source, https://github.com/manotai/manot-client
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 manot
 =============
 
 [![pypi](https://img.shields.io/pypi/v/manot.svg)](https://pypi.org/project/manot)
 [![versions](https://img.shields.io/pypi/pyversions/manot.svg)]()
 [![license](https://img.shields.io/pypi/l/manot)](https://github.com/manotai/manot-client/blob/main/LICENSE)
 
@@ -48,121 +24,121 @@
 
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
-Uploading data for setup
+Uploading data for creating a project
 -------
 
 ```python
-# Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
-manot.upload_data(dir_path="/path/to/data", process="setup")
+# Upload data to manot manager S3 bucket for creating a project. The data should be in YOLO format
+manot.upload_data(dir_path="/path/to/data", process="project")
 ```
 
-Running setup 
+Running project 
 -------
 
 ```python
-# Setup process for "local","gcs" and "s3" providers
-setup = manot.setup(
+# Create a project for "local","gcs" and "s3" providers
+project = manot.create_project(
     data_provider="s3", # it must be "s3", "gcs" or "local"
     arguments={
-            "name": "setup_example",
+            "name": "project_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide ground_truths_path or detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None
             
         }
 )
 #for classification predictions should be in yolo format (txt file containing probability, classname) 
 
 # Setup process for deeplake provider
-setup = manot.setup(
+project = manot.create_project(
     data_provider="deeplake",
     arguments={
-            "name": "setup_example",
+            "name": "project_example",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "deeplake_token": "your deeplake token",
             "data_set": "user/dataset/",
             "detections_boxes_key": "deeplake key where detection boxes are stored",
             "detections_labels_key": "deeplake key where where detection labels are stored",
             "detections_score_key": "deeplake key where detections score is stored",
             "ground_truths_boxes_key": "deeplake key where ground truth boxes are stored",
             "ground_truths_labels_key": "deeplake key where ground truth labels are stored",
             "classes": "classes for deeplake",
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None   
         }
 )
-print(setup)
-# {"id": setup_id, "name": "setup_example", "status": "started"}
+print(project)
+# {"id": project_id, "name": "project_example", "status": "started"}
 
 ```
-Get setup by id 
+Get project by id 
 -------
 
 ```python
 
-setup_info = manot.get_setup(setup["id"])
-# when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
+project_info = manot.get_project(project["id"])
+# when creating a project is successfully finished, then project_info is {"id": project_id, "name": "project_example", "status": "started"}
 ```
 Upload data to get insights from 
 -------
 
 ```python
 # Upload data to manot manager S3 bucket to get insights
-manot.upload_data(dir_path="/path/to/data", process="insight")
+manot.upload_data(dir_path="/path/to/data", process="evaluation")
 ```
-Running insight on data in s3, gcs or local machine
+Running evaluation on data in s3, gcs or local machine
 -------
 
 ```python
-insight = manot.insight(
+evaluation = manot.evaluate(
     name="insight_example",
-    setup_id=setup["id"],
+    project_id=project["id"],
     data_path="/path/to/data",
     data_provider="s3",  # it must be "s3", "gcs" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
-print(insight)
-# {"id": insight_id, "name": "insight_example", "status": "started"}
+print(evaluation)
+# {"id": evaluation_id, "name": "evaluation_example", "status": "started"}
 
-insight_info = manot.get_insight(insight["id"])
-# when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
+evaluation_info = manot.get_evaluation(evaluation["id"])
+# when evaluation is successfully finished, then evaluation_info is {"id": evaluation_id, "name": "evaluation_example", "status": "finished"}
 ```
 
-Running insight on hugging face model and dataset 
+Running evaluation on hugging face model and dataset 
 -------
 
 ```python
-insight = manot.huggingface_insight(
+evaluation = manot.huggingface_evaluation(
     name='manot-huggingface',
     data_path="huggingface_dataset",
     model_path="huggingface_model",
     task="detection",
     percentage=0.5
 )
-insight_info = manot.get_insight(insight["id"])
+evaluation_info = manot.get_evaluation(evaluation["id"])
 ```
 
 ```
-scores = manot.get_score(insight['id'])
+scores = manot.get_score(evaluation['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
-manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
+manot.visualize_data_set(evaluation_info['data_set']['id'], deeplake_token,group_similar=True)
 # if group similar is set to True(default) will only return unique images 
 ```
 
 In case of detection task use this to calculate mAP on your data
 ```python
 manot.calculate_map(
     ground_truths_path="/path/to/ground_truths",
```

### Comparing `manot-0.8.3/manot.egg-info/PKG-INFO` & `manot-0.8.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manot
-Version: 0.8.3
+Version: 0.8.4
 Summary: manot AI is a model observability platform to monitor computer vision performance in real-time.
 Home-page: https://www.manot.ai
 Author: manot
 Author-email: manot <engineering@manot.ai>
 License: MIT
 Project-URL: Homepage, https://www.manot.ai
 Project-URL: Documentation, https://api.manot.ai/api-documentation/v1
@@ -48,121 +48,121 @@
 
 ```python
 from manot import manotAI
 
 manot = manotAI("manot_service_url", "token")
 ```
 
-Uploading data for setup
+Uploading data for creating a project
 -------
 
 ```python
-# Upload data to manot manager S3 bucket for Setup. The data should be in YOLO format
-manot.upload_data(dir_path="/path/to/data", process="setup")
+# Upload data to manot manager S3 bucket for creating a project. The data should be in YOLO format
+manot.upload_data(dir_path="/path/to/data", process="project")
 ```
 
-Running setup 
+Running project 
 -------
 
 ```python
-# Setup process for "local","gcs" and "s3" providers
-setup = manot.setup(
+# Create a project for "local","gcs" and "s3" providers
+project = manot.create_project(
     data_provider="s3", # it must be "s3", "gcs" or "local"
     arguments={
-            "name": "setup_example",
+            "name": "project_example",
             "images_path": "/path/to/images",
             "ground_truths_path": "/path/to/ground_truths",
             "detections_path": "/path/to/detections",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "classes_txt_path": "/path/to/classes.txt",
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide ground_truths_path or detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None
             
         }
 )
 #for classification predictions should be in yolo format (txt file containing probability, classname) 
 
 # Setup process for deeplake provider
-setup = manot.setup(
+project = manot.create_project(
     data_provider="deeplake",
     arguments={
-            "name": "setup_example",
+            "name": "project_example",
             "detections_metadata_format": "xyx2y2",  # it must be one of "xyx2y2", "xywh", or "cxcywh"
             "deeplake_token": "your deeplake token",
             "data_set": "user/dataset/",
             "detections_boxes_key": "deeplake key where detection boxes are stored",
             "detections_labels_key": "deeplake key where where detection labels are stored",
             "detections_score_key": "deeplake key where detections score is stored",
             "ground_truths_boxes_key": "deeplake key where ground truth boxes are stored",
             "ground_truths_labels_key": "deeplake key where ground truth labels are stored",
             "classes": "classes for deeplake",
             "task": 'task_type', #can be classification or detection, in case of classification you don't have to provide detections_metadata_format
             "weight_name": "yolov5s" # by default, it is None   
         }
 )
-print(setup)
-# {"id": setup_id, "name": "setup_example", "status": "started"}
+print(project)
+# {"id": project_id, "name": "project_example", "status": "started"}
 
 ```
-Get setup by id 
+Get project by id 
 -------
 
 ```python
 
-setup_info = manot.get_setup(setup["id"])
-# when setup is successfully finished, then setup_info is {"id": setup_id, "name": "setup_example", "status": "started"}
+project_info = manot.get_project(project["id"])
+# when creating a project is successfully finished, then project_info is {"id": project_id, "name": "project_example", "status": "started"}
 ```
 Upload data to get insights from 
 -------
 
 ```python
 # Upload data to manot manager S3 bucket to get insights
-manot.upload_data(dir_path="/path/to/data", process="insight")
+manot.upload_data(dir_path="/path/to/data", process="evaluation")
 ```
-Running insight on data in s3, gcs or local machine
+Running evaluation on data in s3, gcs or local machine
 -------
 
 ```python
-insight = manot.insight(
+evaluation = manot.evaluate(
     name="insight_example",
-    setup_id=setup["id"],
+    project_id=project["id"],
     data_path="/path/to/data",
     data_provider="s3",  # it must be "s3", "gcs" or "local"
     percentage="percentage" # percentage of images to be considered insight should be larger than 0 and less or equal than 100
 )
-print(insight)
-# {"id": insight_id, "name": "insight_example", "status": "started"}
+print(evaluation)
+# {"id": evaluation_id, "name": "evaluation_example", "status": "started"}
 
-insight_info = manot.get_insight(insight["id"])
-# when setup is successfully finished, then insight_info is {"id": insight_id, "name": "setup_example", "status": "started"}
+evaluation_info = manot.get_evaluation(evaluation["id"])
+# when evaluation is successfully finished, then evaluation_info is {"id": evaluation_id, "name": "evaluation_example", "status": "finished"}
 ```
 
-Running insight on hugging face model and dataset 
+Running evaluation on hugging face model and dataset 
 -------
 
 ```python
-insight = manot.huggingface_insight(
+evaluation = manot.huggingface_evaluation(
     name='manot-huggingface',
     data_path="huggingface_dataset",
     model_path="huggingface_model",
     task="detection",
     percentage=0.5
 )
-insight_info = manot.get_insight(insight["id"])
+evaluation_info = manot.get_evaluation(evaluation["id"])
 ```
 
 ```
-scores = manot.get_score(insight['id'])
+scores = manot.get_score(evaluation['id'])
 #returns list of all processed images graded by their score from 0 to 10 (higher is more impactful image)
 # if the image cannot be assigned a score it will not be showing in the list 
 ```
 
 ```python
 #in case of deeplake please also provide deeplake token 
-manot.visualize_data_set(insight_info['data_set']['id'], deeplake_token,group_similar=True)
+manot.visualize_data_set(evaluation_info['data_set']['id'], deeplake_token,group_similar=True)
 # if group similar is set to True(default) will only return unique images 
 ```
 
 In case of detection task use this to calculate mAP on your data
 ```python
 manot.calculate_map(
     ground_truths_path="/path/to/ground_truths",
```

### Comparing `manot-0.8.3/pyproject.toml` & `manot-0.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "manot"
-version = "0.8.3"
+version = "0.8.4"
 authors = [
     { name = "manot", email = "engineering@manot.ai" },
 ]
 license = {text = "MIT"}
 description = "manot AI is a model observability platform to monitor computer vision performance in real-time."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `manot-0.8.3/setup.py` & `manot-0.8.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
 setup(
     name='manot',
-    version='0.8.3',
-    description='The manot SDK is a wrapper on top of our API to make it easier to work with our model performance monitoring system. Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data, classes and model. Once the project is set up you will be able to use the insight method to extract outliers that manot has detected on the new unstructured data that the performance of the model is evaluated on.',
+    version='0.8.4',
+    description='The manot SDK is a wrapper on top of our API to make it easier to work with our model performance monitoring system. Using our SDK you can quickly set up your project by defining a few key parameters, including the paths to your data, classes and model. Once the project is set up you will be able to use the evaluation method to extract outliers that manot has detected on the new unstructured data that the performance of the model is evaluated on.',
     author='manot',
     author_email='engineering@manot.ai',
     url='https://www.manot.ai',
     packages=['manot'],
     package_dir={'manot': 'src/manot'},
     project_urls={
         'Source': 'https://github.com/manotai/manot-client',
```

### Comparing `manot-0.8.3/src/manot/logger.py` & `manot-0.8.4/src/manot/logger.py`

 * *Files identical despite different names*

### Comparing `manot-0.8.3/src/manot/manot.py` & `manot-0.8.4/src/manot/manot.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,22 +19,22 @@
 
 class manotAI:
 
     def __init__(self, url: str, token: str) -> None:
         self.__url = url.rstrip('/')
         self.__token = token
 
-    def setup(
+    def create_project(
             self,
             data_provider: Literal['s3', 'local', 'deeplake'],
             arguments: dict
     ) -> Union[bool, dict]:
         """
         :param data_provider: Provider name, it must be 's3', 'local' or 'deeplake'.
-        :param arguments: Request data to start setup process.
+        :param arguments: Request data to create project.
 
             If data_provider is 'deeplake', arguments must contain such values::
                 name: str,
                 detections_metadata_format: Literal['cxcywh', 'xywh', 'xyx2y2'],
                 deeplake_token: str,
                 data_set: str,
                 detections_boxes_key: str,
@@ -51,73 +51,73 @@
                 ground_truths_path: str,
                 detections_path: str,
                 detections_metadata_format: Literal['cxcywh', 'xywh', 'xyx2y2'],
                 classes_txt_path: str,
                 weight_name: Optional[Literal["yolov5s"]]
         """
 
-        url = f"{self.__url}/api/v1/setup/"
+        url = f"{self.__url}/api/v1/project/"
         if data_provider == "deeplake":
             url = f"{url}deeplake"
 
         arguments.update({"data_provider": data_provider})
 
         try:
             response = requests.post(url=url, data=json.dumps(arguments), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code == 201:
-            log.info("Setup process is being prepared to be started.")
-            progress_result = self.__check_progress(self.get_setup, response.json()["id"])
+            log.info("Project process is being prepared to be started.")
+            progress_result = self.__check_progress(self.get_project, response.json()["id"])
             if progress_result:
                 if progress_result['status'] == "finished":
-                    log.info("Setup process has successfully finished.")
+                    log.info("Project process has successfully finished.")
                 elif progress_result['status'] == "failure":
-                    log.error(f'There is problem setup process with id {response.json()["id"]}.')
+                    log.error(f'There is problem to create project with id {response.json()["id"]}.')
                 return progress_result
             else:
-                log.error(f'There is problem setup process with id {response.json()["id"]}.')
+                log.error(f'There is problem to create project with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
 
-    def get_setup(self, setup_id: int) -> Union[bool, None, dict]:
+    def get_project(self, project_id: int) -> Union[bool, None, dict]:
 
-        url = f"{self.__url}/api/v1/setup/{setup_id}"
+        url = f"{self.__url}/api/v1/project/{project_id}"
 
         try:
             response = requests.get(url=url, headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code != 200:
-            log.warning("Setup not found.")
+            log.warning("Project not found.")
             return None
 
         return response.json()
 
-    def insight(
+    def evaluate(
             self,
             name: str,
-            setup_id: int,
+            project_id: int,
             data_path: Union[str, List[str]],
             data_provider: Literal['s3', 'local', 'deeplake'],
             weight_name: Optional[str] = None,
             deeplake_token: Optional[str] = None,
             percentage: Optional[float] = None
     ) -> Union[bool, dict]:
 
-        url = f"{self.__url}/api/v1/insight/"
+        url = f"{self.__url}/api/v1/evaluation/"
         data = {
             "name": name,
-            "setup_id": setup_id,
+            "project_id": project_id,
             "data_path": data_path,
             "data_provider": data_provider,
             "deeplake_token": deeplake_token,
             "percentage": percentage
         }
         if weight_name:
             data["weight_name"] = weight_name
@@ -125,82 +125,82 @@
         try:
             response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code == 201:
-            log.info("Insight process is being prepared to be started.")
-            progress_result = self.__check_progress(self.get_insight, response.json()["id"])
+            log.info("Evaluation process is being prepared to be started.")
+            progress_result = self.__check_progress(self.get_evaluation, response.json()["id"])
             if progress_result:
                 if progress_result['status'] == "finished":
-                    log.info("Insight process has successfully finished.")
+                    log.info("Evaluation process has successfully finished.")
                 elif progress_result['status'] == "failure":
-                    log.error(f'There is problem insight process with id {response.json()["id"]}.')
+                    log.error(f'There is problem evaluation process with id {response.json()["id"]}.')
                 return progress_result
             else:
-                log.error(f'There is problem insight process with id {response.json()["id"]}.')
+                log.error(f'There is problem evaluation process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
 
-    def huggingface_insight(
+    def huggingface_evaluation(
             self,
             name: str,
             data_path: str,
             task: Optional[Literal['classification', 'segmentation', 'detection']] = 'detection',
             percentage: Optional[float] = None,
             model_path: Optional[str] = None,
 
 
     ) -> Union[bool, dict]:
 
-        url = f"{self.__url}/api/v1/insight/huggingface"
+        url = f"{self.__url}/api/v1/evaluation/huggingface"
         data = {
             "name": name,
             "data_path": data_path,
             "model_path": model_path,
             "task": task,
             "percentage": percentage
         }
         try:
             response = requests.post(url=url, data=json.dumps(data), headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code == 201:
-            log.info("Insight process is being prepared to be started.")
-            progress_result = self.__check_progress(self.get_insight, response.json()["id"])
+            log.info("Evaluation process is being prepared to be started.")
+            progress_result = self.__check_progress(self.get_evaluation, response.json()["id"])
             if progress_result:
                 if progress_result['status'] == "finished":
-                    log.info("Insight process has successfully finished.")
+                    log.info("Evaluation process has successfully finished.")
                 elif progress_result['status'] == "failure":
-                    log.error(f'There is problem insight process with id {response.json()["id"]}.')
+                    log.error(f'There is problem evaluation process with id {response.json()["id"]}.')
                 return progress_result
             else:
-                log.error(f'There is problem insight process with id {response.json()["id"]}.')
+                log.error(f'There is problem evaluation process with id {response.json()["id"]}.')
                 return False
 
         log.error(response.text)
         return False
 
-    def get_insight(self, insight_id: int) -> Union[bool, None, dict]:
+    def get_evaluation(self, evaluation_id: int) -> Union[bool, None, dict]:
 
-        url = f"{self.__url}/api/v1/insight/{insight_id}"
+        url = f"{self.__url}/api/v1/evaluation/{evaluation_id}"
 
         try:
             response = requests.get(url=url, headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code != 200:
-            log.warning("Insight not found.")
+            log.warning("Evaluation not found.")
             return None
 
         return response.json()
 
     def visualize_data_set(
             self,
             data_set_id: int,
@@ -223,23 +223,23 @@
 
         images = response['data_set_images']
         images_urls = []
         for file in images:
             images_urls.append(self.__process(file['id'], deeplake_token, with_inference, huggingface_model))
         return ipyplot.plot_images(images_urls, img_width=200, show_url=False, max_images=len(images_urls))
 
-    def upload_data(self, dir_path: str, process: Literal["setup", "insight"]):
+    def upload_data(self, dir_path: str, process: Literal["project", "evaluation"]):
 
         upload_manager = UploadManager(directory=dir_path, url=self.__url, token=self.__token)
-        if process == "setup":
-            return upload_manager.upload_setup_data()
-        elif process == "insight":
-            return upload_manager.upload_insight_data()
+        if process == "project":
+            return upload_manager.upload_project_data()
+        elif process == "evaluation":
+            return upload_manager.upload_evaluation_data()
         else:
-            log.error("Process must be 'setup' or 'insight'.")
+            log.error("Process must be 'project' or 'evaluation'.")
             return False
 
     def calculate_map(
             self,
             ground_truths_path: str,
             detections_path: str,
             classes_txt_path: str,
@@ -294,16 +294,16 @@
         if response.status_code == 200:
             log.info("Accuracy has successfully calculated.")
             return response.json()
 
         log.error(response.text)
         return False
 
-    def get_score(self, insight_id):
-        url = f"{self.__url}/api/v1/insight/{insight_id}/scores"
+    def get_score(self, evaluation_id):
+        url = f"{self.__url}/api/v1/evaluation/{evaluation_id}/scores"
         try:
             response = requests.get(url=url, headers={"token": self.__token})
         except Exception:
             log.error("There is problem with request.")
             return False
 
         if response.status_code != 200:
```

### Comparing `manot-0.8.3/src/manot/upload_manager.py` & `manot-0.8.4/src/manot/upload_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     def __init__(self, directory: str, url: str, token: str):
         self.directory = directory
         self.url = url
         self.token = token
         self.save_path = str(uuid.uuid4())
 
-    def upload_insight_data(self):
+    def upload_evaluation_data(self):
 
         if not self._is_exist(self.directory):
             log.error(f"No such directory: {self.directory}")
             return False
 
         correct_files = []
         for file_path in glob.glob(self.directory + "/*"):
@@ -30,15 +30,15 @@
         if not correct_files:
             log.error("There are no files to upload.")
             return False
 
         if self.upload_data(correct_files):
             return {"data_path": os.path.join(self.save_path, "images")}
 
-    def upload_setup_data(self):
+    def upload_project_data(self):
 
         images_path = os.path.join(self.directory, "images")
         detections_path = os.path.join(self.directory, "detections")
         ground_truths_path = os.path.join(self.directory, "ground_truths")
         classes_txt_path = os.path.join(self.directory, "classes.txt")
         if not self._is_exist(self.directory):
             log.error(f"No such directory: {self.directory}")
```

