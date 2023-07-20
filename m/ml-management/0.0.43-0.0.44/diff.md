# Comparing `tmp/ml-management-0.0.43.tar.gz` & `tmp/ml-management-0.0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.43.tar", last modified: Wed Jul 19 10:30:58 2023, max compression
+gzip compressed data, was "ml-management-0.0.44.tar", last modified: Thu Jul 20 08:23:45 2023, max compression
```

## Comparing `ml-management-0.0.43.tar` & `ml-management-0.0.44.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-29 11:52:32.000000 ml-management-0.0.43/MANIFEST.in
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/collectors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/collectors/collectors.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/collectors/dummy/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.546286 ml-management-0.0.43/ML_management/collectors/s3/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9711 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/collectors/topic_markers/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/dataset_loader_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4373 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/executor_template/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/executor_template/default_executors/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     6505 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/mlmanagement/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      737 2023-07-04 13:14:56.000000 ml-management-0.0.43/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    15292 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10500 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2701 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/mlmanagement/module_finder.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5001 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      316 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/models/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/models/patterns/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4865 2023-07-19 10:07:23.000000 ml-management-0.0.43/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/registry/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/registry/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2564 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/registry/exceptions.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/tests/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/tests/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9858 2023-07-11 12:32:50.000000 ml-management-0.0.43/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ML_management/uploader_data/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.43/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1914 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1430 2023-07-10 10:35:03.000000 ml-management-0.0.43/ML_management/uploader_data/utils.py
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-19 10:30:58.550286 ml-management-0.0.43/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-29 11:52:32.000000 ml-management-0.0.43/README.md
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-07-19 10:28:54.000000 ml-management-0.0.43/VERSION
-drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-19 10:30:58.550286 ml-management-0.0.43/ml_management.egg-info/
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2530 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      166 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/requires.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-07-19 10:30:58.000000 ml-management-0.0.43/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-07-19 10:30:58.550286 ml-management-0.0.43/setup.cfg
--rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1076 2023-07-10 10:35:03.000000 ml-management-0.0.43/setup.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       18 2023-06-29 11:52:32.000000 ml-management-0.0.44/MANIFEST.in
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/collectors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      120 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1092 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      456 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1318 2023-07-11 12:32:50.000000 ml-management-0.0.44/ML_management/collectors/collectors.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/collectors/dummy/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      463 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/collectors/s3/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9711 2023-07-10 10:35:03.000000 ml-management-0.0.44/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)   331440 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3167 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/dataset_loader_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4373 2023-07-19 11:55:30.000000 ml-management-0.0.44/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/executor_template/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.541493 ml-management-0.0.44/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      895 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      843 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      869 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     6505 2023-07-19 11:55:30.000000 ml-management-0.0.44/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      402 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      334 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ML_management/mlmanagement/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      737 2023-07-04 13:14:56.000000 ml-management-0.0.44/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      380 2023-07-19 16:00:17.000000 ml-management-0.0.44/ML_management/mlmanagement/base_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3392 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5054 2023-07-11 12:32:50.000000 ml-management-0.0.44/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    15292 2023-07-19 11:55:30.000000 ml-management-0.0.44/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)    10500 2023-07-19 12:00:37.000000 ml-management-0.0.44/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      201 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2701 2023-07-19 11:55:30.000000 ml-management-0.0.44/ML_management/mlmanagement/module_finder.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     5121 2023-07-19 15:58:30.000000 ml-management-0.0.44/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      316 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ML_management/models/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/models/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      949 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ML_management/models/patterns/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     4865 2023-07-19 11:55:30.000000 ml-management-0.0.44/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      561 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      445 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      457 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ML_management/registry/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/registry/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2672 2023-07-19 15:59:22.000000 ml-management-0.0.44/ML_management/registry/exceptions.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     7556 2023-07-11 12:32:50.000000 ml-management-0.0.44/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ML_management/tests/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/tests/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     3361 2023-07-11 12:32:50.000000 ml-management-0.0.44/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     9858 2023-07-11 12:32:50.000000 ml-management-0.0.44/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ML_management/uploader_data/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-06-29 11:52:32.000000 ml-management-0.0.44/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1914 2023-07-10 10:35:03.000000 ml-management-0.0.44/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1430 2023-07-10 10:35:03.000000 ml-management-0.0.44/ML_management/uploader_data/utils.py
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-20 08:23:45.545493 ml-management-0.0.44/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       56 2023-06-29 11:52:32.000000 ml-management-0.0.44/README.md
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        7 2023-07-20 08:23:43.000000 ml-management-0.0.44/VERSION
+drwxrwxr-x   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        0 2023-07-20 08:23:45.545493 ml-management-0.0.44/ml_management.egg-info/
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      367 2023-07-20 08:23:45.000000 ml-management-0.0.44/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     2576 2023-07-20 08:23:45.000000 ml-management-0.0.44/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)        1 2023-07-20 08:23:45.000000 ml-management-0.0.44/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)      166 2023-07-20 08:23:45.000000 ml-management-0.0.44/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       14 2023-07-20 08:23:45.000000 ml-management-0.0.44/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)       38 2023-07-20 08:23:45.545493 ml-management-0.0.44/setup.cfg
+-rw-rw-r--   0 ezhandrvlad  (1000) ezhandrvlad  (1000)     1076 2023-07-10 10:35:03.000000 ml-management-0.0.44/setup.py
```

### Comparing `ml-management-0.0.43/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.44/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/collectors/collectors.py` & `ml-management-0.0.44/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.44/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.44/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.44/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.44/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.44/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.44/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.44/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.44/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.44/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.44/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.44/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.44/ML_management/mlmanagement/mlmanagement.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.44/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/module_finder.py` & `ml-management-0.0.44/ML_management/mlmanagement/module_finder.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.44/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Custom exception definition for server mlflow manager graph."""
 
+from ML_management.mlmanagement.base_exceptions import ServerException
 
-class InvalidEnumType(Exception):
+
+class InvalidEnumType(ServerException):
     """Define InvalidEnumType exception."""
 
     def __init__(self, passed_enum_values, enum_type_name):
         self.passed_enum_values = passed_enum_values
         self.enum_type_name = enum_type_name
         self.message = f'Passed enum values "{", ".join(passed_enum_values)}" is invalid, ' f"must be value of Enum {enum_type_name}."
 
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (InvalidEnumType, (self.passed_enum_values, self.enum_type_name))
 
 
-class InvalidModelName(Exception):
+class InvalidModelName(ServerException):
     """Define InvalidModelName exception."""
 
     def __init__(self, passed_name, kwarg):
         self.passed_name = passed_name
         self.kwarg = kwarg
         self.message = 'Passed "{kwarg}" argument value "{passed_name}" is invalid, as this model is not registered in mlflow.'.format(
             kwarg=kwarg,
@@ -30,15 +32,15 @@
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (InvalidModelName, (self.passed_name, self.kwarg))
 
 
-class InvalidModelVersion(Exception):
+class InvalidModelVersion(ServerException):
     """Define InvalidModelVersion exception."""
 
     def __init__(self, passed_name, passed_version, name_kwarg, version_kwarg):
         self.passed_version = passed_version
         self.passed_name = passed_name
         self.name_kwarg = name_kwarg
         self.version_kwarg = version_kwarg
@@ -61,15 +63,15 @@
                 self.passed_version,
                 self.name_kwarg,
                 self.version_kwarg,
             ),
         )
 
 
-class KwargNotPassedWithUploadType(Exception):
+class KwargNotPassedWithUploadType(ServerException):
     """Define KwargNotPassedWithUploadType exception."""
 
     def __init__(self, kwarg, passed_upload_model_type):
         self.passed_upload_model_type = passed_upload_model_type
         self.kwarg = kwarg
         self.message = 'Argument "{kwarg}" cannot be ommitted with upload_model_type UploadModelType.{passed_upload_model_type}.'.format(
             kwarg=kwarg,
@@ -79,28 +81,28 @@
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (KwargNotPassedWithUploadType, (self.kwarg, self.passed_upload_model_type))
 
 
-class ModelTypeIsNotFound(Exception):
+class ModelTypeIsNotFound(ServerException):
     """Define ModelTypeIsNotFound exception."""
 
     def __init__(self):
         self.message = "Model type is not found. You must inherit the desired template."
 
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (ModelTypeIsNotFound, ())
 
 
-class ExistingModelWithOtherType(Exception):
+class ExistingModelWithOtherType(ServerException):
     """Define ExistingModelWithOtherType exception."""
 
     def __init__(self, name):
         self.name = name
         self.message = (
             f'The other model type with name "{name}" exists.'
             f"You cannot upload a model with the same name as an existing model of a different type."
@@ -109,30 +111,30 @@
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (ExistingModelWithOtherType, (self.name,))
 
 
-class InvalidExperimentName(Exception):
+class InvalidExperimentName(ServerException):
     """Define InvalidExperimentName exception."""
 
     def __init__(self, model_type, exp_name):
         self.model_type = model_type
         self.exp_name = exp_name
         self.message = f"You can't specify '{exp_name}' experiment name for model type '{model_type}' upload."
 
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (InvalidExperimentName, (self.model_type, self.exp_name))
 
 
-class InvalidUploadModelMode(Exception):
+class InvalidUploadModelMode(ServerException):
     """Define InvalidUploadModelMode exception."""
 
     def __init__(self, model_type, upload_mode):
         self.model_type = model_type
         self.upload_mode = upload_mode
         self.message = f"You can't specify upload mode '{upload_mode}' for '{model_type}' model."
```

### Comparing `ml-management-0.0.43/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.44/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.44/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.44/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/registry/exceptions.py` & `ml-management-0.0.44/ML_management/registry/exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 """Custom exception definition (necessary for RegistryManager)."""
 
+from ML_management.mlmanagement.base_exceptions import RegistyException
 
-class VersionNotFound(Exception):
+
+class VersionNotFound(RegistyException):
     """Define Version Not Found Exception."""
 
     def __init__(self, model_name: str, version: int):
         self.model_name = model_name
         self.version = version
         self.message = f'There is no version {self.version} for model "{self.model_name}"'
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (VersionNotFound, (self.model_name, self.version))
 
 
-class MetricNotLogged(Exception):
+class MetricNotLogged(RegistyException):
     """Define Metric Not Logged exception."""
 
     def __init__(self, model_name: str, metric: str):
         self.model_name = model_name
         self.metric = metric
         self.message = f'Metric "{self.metric}" is not logged for model "{self.model_name}"'
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (MetricNotLogged, (self.model_name, self.metric))
 
 
-class ModelNotRegistered(Exception):
+class ModelNotRegistered(RegistyException):
     """Define Model Not Registered exception."""
 
     def __init__(self, model_name: str, model_type: str = "model"):
         self.model_name = model_name
         self.model_type = model_type
         self.message = f'{model_type} "{model_name}" is not registered'
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (ModelNotRegistered, (self.model_name, self.model_type))
 
 
-class NoMetricProvided(Exception):
+class NoMetricProvided(RegistyException):
     """Define No Metric Provided exception."""
 
     def __init__(self, criteria: str):
         self.criteria = criteria
         self.message = f'Choice criteria "{self.criteria}" is passed, but no metric name is provided'
         super().__init__(self.message)
 
     def __reduce__(self):
         """Define reduce method to make exception picklable."""
         return (NoMetricProvided, (self.criteria))
 
 
-class UnsupportedCriteria(Exception):
+class UnsupportedCriteria(RegistyException):
     """Define Unsupported Criteria exception."""
 
     def __init__(self, criteria: str, supported_criteria: list):
         self.criteria = criteria
         self.supported_criteria = supported_criteria
         self.message = f'Choice criteria "{self.criteria}" is unsupported, must be one of: {self.supported_criteria}'
         super().__init__(self.message)
```

### Comparing `ml-management-0.0.43/ML_management/registry/registry_manager.py` & `ml-management-0.0.44/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.44/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.44/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.44/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ML_management/uploader_data/utils.py` & `ml-management-0.0.44/ML_management/uploader_data/utils.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.43/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.44/ml_management.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ML_management/executor_template/executor_pattern_to_methods_map.py
 ML_management/executor_template/upload_model_mode.py
 ML_management/executor_template/default_executors/__init__.py
 ML_management/executor_template/default_executors/finetune_executor.py
 ML_management/executor_template/default_executors/test_executor.py
 ML_management/executor_template/default_executors/train_executor.py
 ML_management/mlmanagement/__init__.py
+ML_management/mlmanagement/base_exceptions.py
 ML_management/mlmanagement/jsonschema_exceptions.py
 ML_management/mlmanagement/jsonschema_inference.py
 ML_management/mlmanagement/mlmanagement.py
 ML_management/mlmanagement/mlmanager.py
 ML_management/mlmanagement/model_type.py
 ML_management/mlmanagement/module_finder.py
 ML_management/mlmanagement/server_mlmanager_exceptions.py
```

### Comparing `ml-management-0.0.43/setup.py` & `ml-management-0.0.44/setup.py`

 * *Files identical despite different names*

