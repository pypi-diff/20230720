# Comparing `tmp/openml-0.8.0.tar.gz` & `tmp/openml-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openml-0.8.0.tar", last modified: Fri Feb 15 09:31:14 2019, max compression
+gzip compressed data, was "dist/openml-0.9.0.tar", last modified: Wed Jun  5 13:37:47 2019, max compression
```

## Comparing `openml-0.8.0.tar` & `openml-0.9.0.tar`

### file list

```diff
@@ -1,88 +1,106 @@
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/
--rw-r--r--   0 feurerm  (10328) aad       (1318)       25 2018-04-24 08:01:09.000000 openml-0.8.0/MANIFEST.in
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1117 2019-02-15 09:31:14.000000 openml-0.8.0/PKG-INFO
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1312 2018-04-24 08:01:09.000000 openml-0.8.0/README.md
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/
--rw-r--r--   0 feurerm  (10328) aad       (1318)     2102 2018-04-24 08:01:09.000000 openml-0.8.0/openml/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)      127 2019-02-15 08:39:00.000000 openml-0.8.0/openml/__version__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     5103 2019-02-15 08:39:00.000000 openml-0.8.0/openml/_api_calls.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     4036 2019-02-15 08:39:00.000000 openml-0.8.0/openml/config.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/datasets/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      419 2019-02-15 08:39:00.000000 openml-0.8.0/openml/datasets/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1736 2018-04-24 08:01:09.000000 openml-0.8.0/openml/datasets/data_feature.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    23052 2019-02-15 08:39:00.000000 openml-0.8.0/openml/datasets/dataset.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    29730 2019-02-15 08:39:00.000000 openml-0.8.0/openml/datasets/functions.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/evaluations/
--rw-r--r--   0 feurerm  (10328) aad       (1318)       81 2018-04-24 08:01:09.000000 openml-0.8.0/openml/evaluations/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1331 2019-02-15 08:39:00.000000 openml-0.8.0/openml/evaluations/evaluation.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     4382 2019-02-15 08:39:00.000000 openml-0.8.0/openml/evaluations/functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1792 2018-06-14 12:58:39.000000 openml-0.8.0/openml/exceptions.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/flows/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      380 2019-02-15 08:39:00.000000 openml-0.8.0/openml/flows/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    18292 2019-02-15 08:39:00.000000 openml-0.8.0/openml/flows/flow.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     8953 2019-02-15 08:39:00.000000 openml-0.8.0/openml/flows/functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    37081 2019-02-15 08:39:00.000000 openml-0.8.0/openml/flows/sklearn_converter.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/runs/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      547 2019-02-15 08:39:00.000000 openml-0.8.0/openml/runs/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    42311 2019-02-15 08:39:00.000000 openml-0.8.0/openml/runs/functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    19164 2019-02-15 08:39:00.000000 openml-0.8.0/openml/runs/run.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    13910 2019-02-15 08:39:00.000000 openml-0.8.0/openml/runs/trace.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/setups/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      247 2019-02-15 08:39:00.000000 openml-0.8.0/openml/setups/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     9084 2019-02-15 08:39:00.000000 openml-0.8.0/openml/setups/functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     2029 2019-02-15 08:39:00.000000 openml-0.8.0/openml/setups/setup.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/study/
--rw-r--r--   0 feurerm  (10328) aad       (1318)       64 2018-04-24 08:01:09.000000 openml-0.8.0/openml/study/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1993 2018-04-24 08:01:09.000000 openml-0.8.0/openml/study/functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1698 2018-04-24 08:01:09.000000 openml-0.8.0/openml/study/study.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml/tasks/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      513 2019-02-15 08:39:00.000000 openml-0.8.0/openml/tasks/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    14047 2019-02-15 08:39:00.000000 openml-0.8.0/openml/tasks/functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     5534 2019-02-15 08:39:00.000000 openml-0.8.0/openml/tasks/split.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     7073 2019-02-15 08:39:00.000000 openml-0.8.0/openml/tasks/task.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     4344 2019-02-15 08:39:00.000000 openml-0.8.0/openml/testing.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     7136 2019-02-15 08:39:00.000000 openml-0.8.0/openml/utils.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/openml.egg-info/
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1117 2019-02-15 09:31:14.000000 openml-0.8.0/openml.egg-info/PKG-INFO
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1843 2019-02-15 09:31:14.000000 openml-0.8.0/openml.egg-info/SOURCES.txt
--rw-r--r--   0 feurerm  (10328) aad       (1318)        1 2019-02-15 09:31:14.000000 openml-0.8.0/openml.egg-info/dependency_links.txt
--rw-r--r--   0 feurerm  (10328) aad       (1318)      195 2019-02-15 09:31:14.000000 openml-0.8.0/openml.egg-info/requires.txt
--rw-r--r--   0 feurerm  (10328) aad       (1318)       13 2019-02-15 09:31:14.000000 openml-0.8.0/openml.egg-info/top_level.txt
--rw-r--r--   0 feurerm  (10328) aad       (1318)      271 2019-02-15 09:31:14.000000 openml-0.8.0/setup.cfg
--rw-r--r--   0 feurerm  (10328) aad       (1318)     2816 2019-02-15 08:39:00.000000 openml-0.8.0/setup.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      118 2018-04-24 08:01:10.000000 openml-0.8.0/tests/__init__.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_datasets/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_datasets/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    10375 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_datasets/test_dataset.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    38652 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_datasets/test_dataset_functions.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_examples/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_examples/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     2339 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_examples/test_OpenMLDemo.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_flows/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_flows/__init__.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_flows/dummy_learn/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_flows/dummy_learn/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)      236 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_flows/dummy_learn/dummy_forest.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    19273 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_flows/test_flow.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    10620 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_flows/test_flow_functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    54225 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_flows/test_sklearn.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_openml/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_openml/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     1481 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_openml/test_openml.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_runs/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_runs/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     6859 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_runs/test_run.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)    58337 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_runs/test_run_functions.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     3348 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_runs/test_trace.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_setups/
--rw-r--r--   0 feurerm  (10328) aad       (1318)      118 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_setups/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     5962 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_setups/test_setup_functions.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_tasks/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_tasks/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     3104 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_tasks/test_split.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     2922 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_tasks/test_task.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     7097 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_tasks/test_task_functions.py
-drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-02-15 09:31:14.000000 openml-0.8.0/tests/test_utils/
--rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2018-04-24 08:01:10.000000 openml-0.8.0/tests/test_utils/__init__.py
--rw-r--r--   0 feurerm  (10328) aad       (1318)     3388 2019-02-15 08:39:00.000000 openml-0.8.0/tests/test_utils/test_utils.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      271 2019-06-05 13:37:47.000000 openml-0.9.0/setup.cfg
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml.egg-info/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1226 2019-06-05 13:37:46.000000 openml-0.9.0/openml.egg-info/PKG-INFO
+-rw-r--r--   0 feurerm  (10328) aad       (1318)       13 2019-06-05 13:37:46.000000 openml-0.9.0/openml.egg-info/top_level.txt
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        1 2019-06-05 13:37:46.000000 openml-0.9.0/openml.egg-info/dependency_links.txt
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      318 2019-06-05 13:37:46.000000 openml-0.9.0/openml.egg-info/requires.txt
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2441 2019-06-05 13:37:47.000000 openml-0.9.0/openml.egg-info/SOURCES.txt
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1226 2019-06-05 13:37:47.000000 openml-0.9.0/PKG-INFO
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_examples/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_examples/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2307 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_examples/test_OpenMLDemo.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_flows/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_flows/__init__.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_flows/dummy_learn/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_flows/dummy_learn/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      237 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_flows/dummy_learn/dummy_forest.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    19742 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_flows/test_flow.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    11395 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_flows/test_flow_functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      119 2019-06-05 13:28:33.000000 openml-0.9.0/tests/__init__.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_runs/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_runs/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     8451 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_runs/test_run.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     3341 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_runs/test_trace.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    53148 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_runs/test_run_functions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_utils/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_utils/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     3579 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_utils/test_utils.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_extensions/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_extensions/__init__.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_extensions/test_sklearn_extension/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_extensions/test_sklearn_extension/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    72237 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_extensions/test_sklearn_extension/test_sklearn_extension.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2922 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_extensions/test_functions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_setups/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      119 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_setups/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     6521 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_setups/test_setup_functions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_datasets/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_datasets/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    13905 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_datasets/test_dataset.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    47736 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_datasets/test_dataset_functions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_openml/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1440 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_openml/test_openml.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)        0 2019-03-15 15:02:49.000000 openml-0.9.0/tests/test_openml/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2502 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_openml/test_config.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/tests/test_tasks/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      166 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1556 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_clustering_task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      932 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_regression_task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1634 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_task_methods.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1170 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_classification_task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     4078 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     3285 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_split.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1167 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_learning_curve_task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      868 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_supervised_task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     8192 2019-06-05 13:28:33.000000 openml-0.9.0/tests/test_tasks/test_task_functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)       25 2019-03-15 15:02:48.000000 openml-0.9.0/MANIFEST.in
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     3750 2019-06-05 13:28:33.000000 openml-0.9.0/setup.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/evaluations/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      133 2019-06-05 13:28:33.000000 openml-0.9.0/openml/evaluations/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1507 2019-06-05 13:28:33.000000 openml-0.9.0/openml/evaluations/evaluation.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     7153 2019-06-05 13:28:33.000000 openml-0.9.0/openml/evaluations/functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2871 2019-06-05 13:28:33.000000 openml-0.9.0/openml/__init__.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/study/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      741 2019-06-05 13:28:33.000000 openml-0.9.0/openml/study/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     9956 2019-06-05 13:28:33.000000 openml-0.9.0/openml/study/study.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    19795 2019-06-05 13:28:33.000000 openml-0.9.0/openml/study/functions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/runs/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      581 2019-06-05 13:28:33.000000 openml-0.9.0/openml/runs/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    23836 2019-06-05 13:28:33.000000 openml-0.9.0/openml/runs/run.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    15460 2019-06-05 13:28:33.000000 openml-0.9.0/openml/runs/trace.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    35613 2019-06-05 13:28:33.000000 openml-0.9.0/openml/runs/functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     6478 2019-06-05 13:28:33.000000 openml-0.9.0/openml/config.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/setups/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      247 2019-03-15 15:02:48.000000 openml-0.9.0/openml/setups/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2022 2019-06-05 13:28:33.000000 openml-0.9.0/openml/setups/setup.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    11972 2019-06-05 13:28:33.000000 openml-0.9.0/openml/setups/functions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/datasets/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      479 2019-06-05 13:28:33.000000 openml-0.9.0/openml/datasets/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1553 2019-06-05 13:28:33.000000 openml-0.9.0/openml/datasets/data_feature.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    28901 2019-06-05 13:28:33.000000 openml-0.9.0/openml/datasets/dataset.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    36391 2019-06-05 13:28:33.000000 openml-0.9.0/openml/datasets/functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     5449 2019-06-05 13:28:33.000000 openml-0.9.0/openml/_api_calls.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      127 2019-06-05 13:28:33.000000 openml-0.9.0/openml/__version__.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/flows/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      219 2019-06-05 13:28:33.000000 openml-0.9.0/openml/flows/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    20436 2019-06-05 13:28:33.000000 openml-0.9.0/openml/flows/flow.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    13199 2019-06-05 13:28:33.000000 openml-0.9.0/openml/flows/functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    12159 2019-06-05 13:28:33.000000 openml-0.9.0/openml/utils.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     2098 2019-06-05 13:28:33.000000 openml-0.9.0/openml/exceptions.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/extensions/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      344 2019-06-05 13:28:33.000000 openml-0.9.0/openml/extensions/__init__.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/extensions/sklearn/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)       73 2019-06-05 13:28:33.000000 openml-0.9.0/openml/extensions/sklearn/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    68746 2019-06-05 13:28:33.000000 openml-0.9.0/openml/extensions/sklearn/extension.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     7954 2019-06-05 13:28:33.000000 openml-0.9.0/openml/extensions/extension_interface.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     3205 2019-06-05 13:28:33.000000 openml-0.9.0/openml/extensions/functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     8036 2019-06-05 13:28:33.000000 openml-0.9.0/openml/testing.py
+drwxr-xr-x   0 feurerm  (10328) aad       (1318)        0 2019-06-05 13:37:47.000000 openml-0.9.0/openml/tasks/
+-rw-r--r--   0 feurerm  (10328) aad       (1318)      601 2019-06-05 13:28:33.000000 openml-0.9.0/openml/tasks/__init__.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     5670 2019-06-05 13:28:33.000000 openml-0.9.0/openml/tasks/split.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    16513 2019-06-05 13:28:33.000000 openml-0.9.0/openml/tasks/task.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)    19119 2019-06-05 13:28:33.000000 openml-0.9.0/openml/tasks/functions.py
+-rw-r--r--   0 feurerm  (10328) aad       (1318)     1312 2019-03-15 15:02:48.000000 openml-0.9.0/README.md
```

### Comparing `openml-0.8.0/PKG-INFO` & `openml-0.9.0/openml.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: openml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python API for OpenML
 Home-page: http://openml.org/
-Author: Matthias Feurer, Andreas Müller, Farzan Majdani, Joaquin Vanschoren, Jan van Rijn and Pieter Gijsbers
+Author: Matthias Feurer, Jan van Rijn, Arlind Kadra, Andreas Müller, Pieter Gijsbers and Joaquin Vanschoren
 Author-email: feurerm@informatik.uni-freiburg.de
 Maintainer: Matthias Feurer
 Maintainer-email: feurerm@informatik.uni-freiburg.de
 License: BSD 3-clause
+Project-URL: Documentation, https://openml.github.io/openml-python/
+Project-URL: Source Code, https://github.com/openml/openml-python
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: test
+Provides-Extra: examples
```

### Comparing `openml-0.8.0/README.md` & `openml-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openml-0.8.0/openml/_api_calls.py` & `openml-0.9.0/openml/_api_calls.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,22 +5,28 @@
 import xmltodict
 
 from . import config
 from .exceptions import (OpenMLServerError, OpenMLServerException,
                          OpenMLServerNoResult)
 
 
-def _perform_api_call(call, data=None, file_elements=None):
+def _perform_api_call(call, request_method, data=None, file_elements=None):
     """
     Perform an API call at the OpenML server.
 
     Parameters
     ----------
     call : str
         The API call. For example data/list
+    request_method : str
+        The HTTP request method to perform the API call with. Legal values:
+            - get (reading functions, api key optional)
+            - post (writing functions, generaly require api key)
+            - delete (deleting functions, require api key)
+        See REST api documentation which request method is applicable.
     data : dict
         Dictionary with post-request payload.
     file_elements : dict
         Mapping of {filename: str} of strings which should be uploaded as
         files to the server.
 
     Returns
@@ -34,16 +40,19 @@
     if not url.endswith("/"):
         url += "/"
     url += call
 
     url = url.replace('=', '%3d')
 
     if file_elements is not None:
+        if request_method != 'post':
+            raise ValueError('request method must be post when file elements '
+                             'are present')
         return _read_url_files(url, data=data, file_elements=file_elements)
-    return _read_url(url, data)
+    return _read_url(url, request_method, data)
 
 
 def _file_id_to_url(file_id, filename=None):
     """
      Presents the URL how to download a given file id
      filename is optional
     """
@@ -67,44 +76,34 @@
     response = send_request(
         request_method='post',
         url=url,
         data=data,
         files=file_elements,
     )
     if response.status_code != 200:
-        raise _parse_server_exception(response, url=url)
+        raise _parse_server_exception(response, url)
     if 'Content-Encoding' not in response.headers or \
             response.headers['Content-Encoding'] != 'gzip':
-        warnings.warn('Received uncompressed content from OpenML for %s.' % url)
+        warnings.warn('Received uncompressed content from OpenML for {}.'
+                      .format(url))
     return response.text
 
 
-def _read_url(url, data=None):
-
+def _read_url(url, request_method, data=None):
     data = {} if data is None else data
     if config.apikey is not None:
         data['api_key'] = config.apikey
 
-    if len(data) == 0 or (len(data) == 1 and 'api_key' in data):
-        response = send_request(
-            request_method='get', url=url, data=data,
-        )
-
-    else:
-        # Using requests.post sets header 'Accept-encoding' automatically to
-        #  'gzip,deflate'
-        response = send_request(
-            request_method='post', url=url, data=data,
-        )
-
+    response = send_request(request_method=request_method, url=url, data=data)
     if response.status_code != 200:
-        raise _parse_server_exception(response, url=url)
+        raise _parse_server_exception(response, url)
     if 'Content-Encoding' not in response.headers or \
             response.headers['Content-Encoding'] != 'gzip':
-        warnings.warn('Received uncompressed content from OpenML for %s.' % url)
+        warnings.warn('Received uncompressed content from OpenML for {}.'
+                      .format(url))
     return response.text
 
 
 def send_request(
     request_method,
     url,
     data,
@@ -114,14 +113,16 @@
     response = None
     with requests.Session() as session:
         # Start at one to have a non-zero multiplier for the sleep
         for i in range(1, n_retries + 1):
             try:
                 if request_method == 'get':
                     response = session.get(url, params=data)
+                elif request_method == 'delete':
+                    response = session.delete(url, params=data)
                 elif request_method == 'post':
                     response = session.post(url, data=data, files=files)
                 else:
                     raise NotImplementedError()
                 break
             except (
                     requests.exceptions.ConnectionError,
@@ -132,32 +133,31 @@
                 else:
                     time.sleep(0.1 * i)
     if response is None:
         raise ValueError('This should never happen!')
     return response
 
 
-def _parse_server_exception(response, url=None):
-    # OpenML has a sopisticated error system
+def _parse_server_exception(response, url):
+    # OpenML has a sophisticated error system
     # where information about failures is provided. try to parse this
     try:
         server_exception = xmltodict.parse(response.text)
     except Exception:
-        raise OpenMLServerError(('Unexpected server error. Please '
-                                 'contact the developers!\nStatus code: '
-                                 '%d\n' % response.status_code) + response.text)
-
-    code = int(server_exception['oml:error']['oml:code'])
-    message = server_exception['oml:error']['oml:message']
-    additional = None
-    if 'oml:additional_information' in server_exception['oml:error']:
-        additional = server_exception['oml:error']['oml:additional_information']
+        raise OpenMLServerError(
+            'Unexpected server error when calling {}. Please contact the developers!\n'
+            'Status code: {}\n{}'.format(url, response.status_code, response.text))
+
+    server_error = server_exception['oml:error']
+    code = int(server_error['oml:code'])
+    message = server_error['oml:message']
+    additional_information = server_error.get('oml:additional_information')
     if code in [372, 512, 500, 482, 542, 674]:
         # 512 for runs, 372 for datasets, 500 for flows
         # 482 for tasks, 542 for evaluations, 674 for setups
-        return OpenMLServerNoResult(code, message, additional)
+        return OpenMLServerNoResult(code, message, additional_information)
     return OpenMLServerException(
         code=code,
         message=message,
-        additional=additional,
+        additional=additional_information,
         url=url
     )
```

### Comparing `openml-0.8.0/openml/datasets/data_feature.py` & `openml-0.9.0/openml/datasets/data_feature.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import six
-
 class OpenMLDataFeature(object):
     """Data Feature (a.k.a. Attribute) object.
 
        Parameters
        ----------
        index : int
             The index of this feature
@@ -26,19 +24,15 @@
                              (str(self.LEGAL_DATA_TYPES), data_type))
         if nominal_values is not None and type(nominal_values) != list:
             raise ValueError('Nominal_values is of wrong datatype')
         if type(number_missing_values) != int:
             raise ValueError('number_missing_values is of wrong datatype')
 
         self.index = index
-        # In case of python version lower than 3, change the default ASCII encoder.
-        if six.PY2:
-            self.name = str(name.encode('utf8'))
-        else:
-            self.name = str(name)
+        self.name = str(name)
         self.data_type = str(data_type)
         self.nominal_values = nominal_values
         self.number_missing_values = number_missing_values
 
     def __str__(self):
         return "[%d - %s (%s)]" % (self.index, self.name, self.data_type)
```

### Comparing `openml-0.8.0/openml/datasets/dataset.py` & `openml-0.9.0/openml/datasets/dataset.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from collections import OrderedDict
 import gzip
 import io
 import logging
 import os
-from collections import OrderedDict
+import pickle
+from typing import List, Optional, Union, Tuple, Iterable
 
 import arff
 import numpy as np
+import pandas as pd
 import scipy.sparse
 import xmltodict
-import six
-from six.moves import cPickle as pickle
 from warnings import warn
 
 import openml._api_calls
 from .data_feature import OpenMLDataFeature
 from ..exceptions import PyOpenMLError
+from ..utils import _tag_entity
 
 
 logger = logging.getLogger(__name__)
 
 
 class OpenMLDataset(object):
     """Dataset object.
@@ -32,38 +34,44 @@
     description : str
         Description of the dataset.
     format : str
         Format of the dataset which can be either 'arff' or 'sparse_arff'.
     dataset_id : int, optional
         Id autogenerated by the server.
     version : int, optional
-        Version of this dataset. '1' for original version. Auto-incremented by server.
+        Version of this dataset. '1' for original version.
+        Auto-incremented by server.
     creator : str, optional
         The person who created the dataset.
     contributor : str, optional
         People who contributed to the current version of the dataset.
     collection_date : str, optional
         The date the data was originally collected, given by the uploader.
     upload_date : str, optional
         The date-time when the dataset was uploaded, generated by server.
     language : str, optional
         Language in which the data is represented.
         Starts with 1 upper case letter, rest lower case, e.g. 'English'.
     licence : str, optional
         License of the data.
     url : str, optional
-        Valid URL, points to actual data file, on the OpenML server or another dataset repository.
+        Valid URL, points to actual data file.
+        The file can be on the OpenML server or another dataset repository.
     default_target_attribute : str, optional
-        The default target attribute, if it exists. Can have multiple values, comma separated.
+        The default target attribute, if it exists.
+        Can have multiple values, comma separated.
     row_id_attribute : str, optional
-        The attribute that represents the row-id column, if present in the dataset.
+        The attribute that represents the row-id column,
+        if present in the dataset.
     ignore_attribute : str | list, optional
-        Attributes that should be excluded in modelling, such as identifiers and indexes.
+        Attributes that should be excluded in modelling,
+        such as identifiers and indexes.
     version_label : str, optional
-        Version label provided by user, can be a date, hash, or some other type of id.
+        Version label provided by user.
+        Can be a date, hash, or some other type of id.
     citation : str, optional
         Reference(s) that should be cited when building on this data.
     tag : str, optional
         Tags, describing the algorithms.
     visibility : str, optional
         Who can see the dataset.
         Typical values: 'Everyone','All my friends','Only me'.
@@ -77,17 +85,19 @@
     status : str, optional
         Whether the dataset is active.
     md5_checksum : str, optional
         MD5 checksum to check if the dataset is downloaded without corruption.
     data_file : str, optional
         Path to where the dataset is located.
     features : dict, optional
-        A dictionary of dataset features which maps a feature index to a OpenMLDataFeature.
+        A dictionary of dataset features,
+        which maps a feature index to a OpenMLDataFeature.
     qualities : dict, optional
-        A dictionary of dataset qualities which maps a quality name to a quality value.
+        A dictionary of dataset qualities,
+        which maps a quality name to a quality value.
     dataset: string, optional
         Serialized arff dataset string.
     """
     def __init__(self, name, description, format=None,
                  data_format='arff', dataset_id=None, version=None,
                  creator=None, contributor=None, collection_date=None,
                  upload_date=None, language=None, licence=None,
@@ -117,23 +127,21 @@
         self.collection_date = collection_date
         self.upload_date = upload_date
         self.language = language
         self.licence = licence
         self.url = url
         self.default_target_attribute = default_target_attribute
         self.row_id_attribute = row_id_attribute
-        self.ignore_attributes = None
-        if isinstance(ignore_attribute, six.string_types):
+        if isinstance(ignore_attribute, str):
             self.ignore_attributes = [ignore_attribute]
-        elif isinstance(ignore_attribute, list):
+        elif isinstance(ignore_attribute, list) or ignore_attribute is None:
             self.ignore_attributes = ignore_attribute
-        elif ignore_attribute is None:
-            pass
         else:
-            raise ValueError('wrong data type for ignore_attribute. Should be list. ')
+            raise ValueError('Wrong data type for ignore_attribute. '
+                             'Should be list.')
         self.version_label = version_label
         self.citation = citation
         self.tag = tag
         self.visibility = visibility
         self.original_data_url = original_data_url
         self.paper_url = paper_url
         self.update_comment = update_comment
@@ -141,84 +149,157 @@
         self.data_file = data_file
         self.features = None
         self.qualities = None
         self._dataset = dataset
 
         if features is not None:
             self.features = {}
+            # todo add nominal values (currently not in database)
             for idx, xmlfeature in enumerate(features['oml:feature']):
+                nr_missing = xmlfeature.get('oml:number_of_missing_values', 0)
                 feature = OpenMLDataFeature(int(xmlfeature['oml:index']),
                                             xmlfeature['oml:name'],
                                             xmlfeature['oml:data_type'],
-                                            None,  # todo add nominal values (currently not in database)
-                                            int(xmlfeature.get('oml:number_of_missing_values', 0)))
+                                            xmlfeature.get('oml:nominal_value'),
+                                            int(nr_missing))
                 if idx != feature.index:
-                    raise ValueError('Data features not provided in right order')
+                    raise ValueError('Data features not provided '
+                                     'in right order')
                 self.features[feature.index] = feature
 
         self.qualities = _check_qualities(qualities)
 
         if data_file is not None:
-            if self._data_features_supported():
-                if six.PY2:
-                    self.data_pickle_file = data_file.replace('.arff', '.pkl.py2')
-                else:
-                    self.data_pickle_file = data_file.replace('.arff', '.pkl.py3')
+            self.data_pickle_file = self._data_arff_to_pickle(data_file)
+        else:
+            self.data_pickle_file = None
 
-                if os.path.exists(self.data_pickle_file):
-                    logger.debug("Data pickle file already exists.")
-                else:
-                    try:
-                        data = self._get_arff(self.format)
-                    except OSError as e:
-                        logger.critical("Please check that the data file %s is there "
-                                        "and can be read.", self.data_file)
-                        raise e
-
-                    categorical = [False if type(type_) != list else True
-                                   for name, type_ in data['attributes']]
-                    attribute_names = [name for name, type_ in data['attributes']]
-
-                    if self.format.lower() == 'sparse_arff':
-                        X = data['data']
-                        X_shape = (max(X[1]) + 1, max(X[2]) + 1)
-                        X = scipy.sparse.coo_matrix(
-                            (X[0], (X[1], X[2])), shape=X_shape, dtype=np.float32)
-                        X = X.tocsr()
-                    elif self.format.lower() == 'arff':
-                        X = np.array(data['data'], dtype=np.float32)
+    def _data_arff_to_pickle(self, data_file):
+        data_pickle_file = data_file.replace('.arff', '.pkl.py3')
+        if os.path.exists(data_pickle_file):
+            with open(data_pickle_file, "rb") as fh:
+                data, categorical, attribute_names = pickle.load(fh)
+
+            # Between v0.8 and v0.9 the format of pickled data changed from
+            # np.ndarray to pd.DataFrame. This breaks some backwards compatibility,
+            # e.g. for `run_model_on_task`. If a local file still exists with
+            # np.ndarray data, we reprocess the data file to store a pickled
+            # pd.DataFrame blob. See also #646.
+            if isinstance(data, pd.DataFrame) or scipy.sparse.issparse(data):
+                logger.debug("Data pickle file already exists.")
+                return data_pickle_file
+
+        try:
+            data = self._get_arff(self.format)
+        except OSError as e:
+            logger.critical("Please check that the data file %s is "
+                            "there and can be read.", data_file)
+            raise e
+
+        ARFF_DTYPES_TO_PD_DTYPE = {
+            'INTEGER': 'integer',
+            'REAL': 'floating',
+            'NUMERIC': 'floating',
+            'STRING': 'string'
+        }
+        attribute_dtype = {}
+        attribute_names = []
+        categories_names = {}
+        categorical = []
+        for name, type_ in data['attributes']:
+            # if the feature is nominal and the a sparse matrix is
+            # requested, the categories need to be numeric
+            if (isinstance(type_, list)
+                    and self.format.lower() == 'sparse_arff'):
+                try:
+                    np.array(type_, dtype=np.float32)
+                except ValueError:
+                    raise ValueError(
+                        "Categorical data needs to be numeric when "
+                        "using sparse ARFF."
+                    )
+            # string can only be supported with pandas DataFrame
+            elif (type_ == 'STRING'
+                  and self.format.lower() == 'sparse_arff'):
+                raise ValueError(
+                    "Dataset containing strings is not supported "
+                    "with sparse ARFF."
+                )
+
+            # infer the dtype from the ARFF header
+            if isinstance(type_, list):
+                categorical.append(True)
+                categories_names[name] = type_
+                if len(type_) == 2:
+                    type_norm = [cat.lower().capitalize()
+                                 for cat in type_]
+                    if set(['True', 'False']) == set(type_norm):
+                        categories_names[name] = [
+                            True if cat == 'True' else False
+                            for cat in type_norm
+                        ]
+                        attribute_dtype[name] = 'boolean'
                     else:
-                        raise Exception()
+                        attribute_dtype[name] = 'categorical'
+                else:
+                    attribute_dtype[name] = 'categorical'
+            else:
+                categorical.append(False)
+                attribute_dtype[name] = ARFF_DTYPES_TO_PD_DTYPE[type_]
+            attribute_names.append(name)
+
+        if self.format.lower() == 'sparse_arff':
+            X = data['data']
+            X_shape = (max(X[1]) + 1, max(X[2]) + 1)
+            X = scipy.sparse.coo_matrix(
+                (X[0], (X[1], X[2])), shape=X_shape, dtype=np.float32)
+            X = X.tocsr()
+
+        elif self.format.lower() == 'arff':
+            X = pd.DataFrame(data['data'], columns=attribute_names)
+
+            col = []
+            for column_name in X.columns:
+                if attribute_dtype[column_name] in ('categorical',
+                                                    'boolean'):
+                    col.append(self._unpack_categories(
+                        X[column_name], categories_names[column_name]))
+                else:
+                    col.append(X[column_name])
+            X = pd.concat(col, axis=1)
 
-                    with open(self.data_pickle_file, "wb") as fh:
-                        pickle.dump((X, categorical, attribute_names), fh, -1)
-                    logger.debug("Saved dataset %d: %s to file %s" %
-                                 (int(self.dataset_id or -1), self.name, self.data_pickle_file))
+        # Pickle the dataframe or the sparse matrix.
+        with open(data_pickle_file, "wb") as fh:
+            pickle.dump((X, categorical, attribute_names), fh, -1)
+        logger.debug("Saved dataset {did}: {name} to file {path}"
+                     .format(did=int(self.dataset_id or -1),
+                             name=self.name,
+                             path=data_pickle_file)
+                     )
+        return data_pickle_file
 
     def push_tag(self, tag):
         """Annotates this data set with a tag on the server.
 
         Parameters
         ----------
         tag : str
             Tag to attach to the dataset.
         """
-        data = {'data_id': self.dataset_id, 'tag': tag}
-        openml._api_calls._perform_api_call("/data/tag", data=data)
+        _tag_entity('data', self.dataset_id, tag)
 
     def remove_tag(self, tag):
         """Removes a tag from this dataset on the server.
 
         Parameters
         ----------
         tag : str
             Tag to attach to the dataset.
         """
-        data = {'data_id': self.dataset_id, 'tag': tag}
-        openml._api_calls._perform_api_call("/data/untag", data=data)
+        _tag_entity('data', self.dataset_id, tag, untag=True)
 
     def __eq__(self, other):
 
         if type(other) != OpenMLDataset:
             return False
 
         server_fields = {
@@ -236,42 +317,35 @@
         if self_keys != other_keys:
             return False
 
         # check that values of the common keys are identical
         return all(self.__dict__[key] == other.__dict__[key]
                    for key in self_keys)
 
-    def __ne__(self, other):
-        """Only needed for python 2, unnecessary in Python 3"""
-        return not self.__eq__(other)
-
     def _get_arff(self, format):
         """Read ARFF file and return decoded arff.
 
         Reads the file referenced in self.data_file.
 
         Returns
         -------
         dict
             Decoded arff.
 
         """
 
         # TODO: add a partial read method which only returns the attribute
         # headers of the corresponding .arff file!
-
-        # A random number after which we consider a file for too large on a
-        # 32 bit system...currently 120mb (just a little bit more than covtype)
         import struct
 
-        if not self._data_features_supported():
-            raise PyOpenMLError('Dataset not compatible, PyOpenML cannot handle string features')
-
         filename = self.data_file
         bits = (8 * struct.calcsize("P"))
+        # Files can be considered too large on a 32-bit system,
+        # if it exceeds 120mb (slightly more than covtype dataset size)
+        # This number is somewhat arbitrary.
         if bits != 64 and os.path.getsize(filename) > 120000000:
             return NotImplementedError("File too big")
 
         if format.lower() == 'arff':
             return_type = arff.DENSE
         elif format.lower() == 'sparse_arff':
             return_type = arff.COO
@@ -286,130 +360,194 @@
         if filename[-3:] == ".gz":
             with gzip.open(filename) as fh:
                 return decode_arff(fh)
         else:
             with io.open(filename, encoding='utf8') as fh:
                 return decode_arff(fh)
 
-    def get_data(self, target=None,
-                 include_row_id=False,
-                 include_ignore_attributes=False,
-                 return_categorical_indicator=False,
-                 return_attribute_names=False
-    ):
-        """Returns dataset content as numpy arrays / sparse matrices.
+    @staticmethod
+    def _convert_array_format(data, array_format, attribute_names):
+        """Convert a dataset to a given array format.
+
+        By default, the data are stored as a sparse matrix or a pandas
+        dataframe. One might be interested to get a pandas SparseDataFrame or a
+        NumPy array instead, respectively.
+        """
+        if array_format == "array" and not scipy.sparse.issparse(data):
+            # We encode the categories such that they are integer to be able
+            # to make a conversion to numeric for backward compatibility
+            def _encode_if_category(column):
+                if column.dtype.name == 'category':
+                    column = column.cat.codes.astype(np.float32)
+                    mask_nan = column == -1
+                    column[mask_nan] = np.nan
+                return column
+            if data.ndim == 2:
+                columns = {
+                    column_name: _encode_if_category(data.loc[:, column_name])
+                    for column_name in data.columns
+                }
+                data = pd.DataFrame(columns)
+            else:
+                data = _encode_if_category(data)
+            try:
+                return np.asarray(data, dtype=np.float32)
+            except ValueError:
+                raise PyOpenMLError(
+                    'PyOpenML cannot handle string when returning numpy'
+                    ' arrays. Use dataset_format="dataframe".'
+                )
+        if array_format == "dataframe" and scipy.sparse.issparse(data):
+            return pd.SparseDataFrame(data, columns=attribute_names)
+        return data
+
+    @staticmethod
+    def _unpack_categories(series, categories):
+        col = []
+        for x in series:
+            try:
+                col.append(categories[int(x)])
+            except (TypeError, ValueError):
+                col.append(np.nan)
+        # We require two lines to create a series of categories as detailed here:
+        # https://pandas.pydata.org/pandas-docs/version/0.24/user_guide/categorical.html#series-creation  # noqa E501
+        raw_cat = pd.Categorical(col, ordered=True, categories=categories)
+        return pd.Series(raw_cat, index=series.index, name=series.name)
+
+    def _download_data(self) -> None:
+        """ Download ARFF data file to standard cache directory. Set `self.data_file`. """
+        # import required here to avoid circular import.
+        from .functions import _get_dataset_arff
+        self.data_file = _get_dataset_arff(self)
+
+    def get_data(
+            self,
+            target: Optional[Union[List[str], str]] = None,
+            include_row_id: bool = False,
+            include_ignore_attributes: bool = False,
+            dataset_format: str = "dataframe",
+    ) -> Tuple[
+            Union[np.ndarray, pd.DataFrame, scipy.sparse.csr_matrix],
+            Optional[Union[np.ndarray, pd.DataFrame]],
+            List[bool],
+            List[str]
+    ]:
+        """ Returns dataset content as dataframes or sparse matrices.
 
         Parameters
         ----------
-
+        target : string, List[str] or None (default=None)
+            Name of target column to separate from the data.
+            Splitting multiple columns is currently not supported.
+        include_row_id : boolean (default=False)
+            Whether to include row ids in the returned dataset.
+        include_ignore_attributes : boolean (default=False)
+            Whether to include columns that are marked as "ignore"
+            on the server in the dataset.
+        dataset_format : string (default='dataframe')
+            The format of returned dataset.
+            If ``array``, the returned dataset will be a NumPy array or a SciPy sparse matrix.
+            If ``dataframe``, the returned dataset will be a Pandas DataFrame or SparseDataFrame.
 
         Returns
         -------
-
+        X : ndarray, dataframe, or sparse matrix, shape (n_samples, n_columns)
+            Dataset
+        y : ndarray or pd.Series, shape (n_samples, ) or None
+            Target column
+        categorical_indicator : boolean ndarray
+            Mask that indicate categorical features.
+        attribute_names : List[str]
+            List of attribute names.
         """
-        rval = []
-
-        if not self._data_features_supported():
-            raise PyOpenMLError(
-                'Dataset %d not compatible, PyOpenML cannot handle string '
-                'features' % self.dataset_id
-            )
+        if self.data_pickle_file is None:
+            if self.data_file is None:
+                self._download_data()
+            self.data_pickle_file = self._data_arff_to_pickle(self.data_file)
 
         path = self.data_pickle_file
         if not os.path.exists(path):
             raise ValueError("Cannot find a pickle file for dataset %s at "
                              "location %s " % (self.name, path))
         else:
             with open(path, "rb") as fh:
                 data, categorical, attribute_names = pickle.load(fh)
 
         to_exclude = []
-        if include_row_id is False:
-            if not self.row_id_attribute:
-                pass
-            else:
-                if isinstance(self.row_id_attribute, six.string_types):
-                    to_exclude.append(self.row_id_attribute)
-                else:
-                    to_exclude.extend(self.row_id_attribute)
-
-        if include_ignore_attributes is False:
-            if not self.ignore_attributes:
-                pass
-            else:
-                if isinstance(self.ignore_attributes, six.string_types):
-                    to_exclude.append(self.ignore_attributes)
-                else:
-                    to_exclude.extend(self.ignore_attributes)
+        if not include_row_id and self.row_id_attribute is not None:
+            if isinstance(self.row_id_attribute, str):
+                to_exclude.append(self.row_id_attribute)
+            elif isinstance(self.row_id_attribute, Iterable):
+                to_exclude.extend(self.row_id_attribute)
+
+        if not include_ignore_attributes and self.ignore_attributes is not None:
+            if isinstance(self.ignore_attributes, str):
+                to_exclude.append(self.ignore_attributes)
+            elif isinstance(self.ignore_attributes, Iterable):
+                to_exclude.extend(self.ignore_attributes)
 
         if len(to_exclude) > 0:
             logger.info("Going to remove the following attributes:"
                         " %s" % to_exclude)
             keep = np.array([True if column not in to_exclude else False
                              for column in attribute_names])
-            data = data[:, keep]
+            if hasattr(data, 'iloc'):
+                data = data.iloc[:, keep]
+            else:
+                data = data[:, keep]
             categorical = [cat for cat, k in zip(categorical, keep) if k]
             attribute_names = [att for att, k in
                                zip(attribute_names, keep) if k]
 
         if target is None:
-            rval.append(data)
+            data = self._convert_array_format(data, dataset_format,
+                                              attribute_names)
+            targets = None
         else:
-            if isinstance(target, six.string_types):
+            if isinstance(target, str):
                 if ',' in target:
                     target = target.split(',')
                 else:
                     target = [target]
             targets = np.array([True if column in target else False
                                 for column in attribute_names])
             if np.sum(targets) > 1:
                 raise NotImplementedError(
                     "Number of requested targets %d is not implemented." %
                     np.sum(targets)
                 )
             target_categorical = [
-                cat for cat, column in
-                six.moves.zip(categorical, attribute_names)
+                cat for cat, column in zip(categorical, attribute_names)
                 if column in target
             ]
             target_dtype = int if target_categorical[0] else float
 
-            try:
+            if hasattr(data, 'iloc'):
+                x = data.iloc[:, ~targets]
+                y = data.iloc[:, targets]
+            else:
                 x = data[:, ~targets]
                 y = data[:, targets].astype(target_dtype)
 
-                if len(y.shape) == 2 and y.shape[1] == 1:
-                    y = y[:, 0]
-
-                categorical = [cat for cat, t in
-                               zip(categorical, targets) if not t]
-                attribute_names = [att for att, k in
-                                   zip(attribute_names, targets) if not k]
-            except KeyError as e:
-                import sys
-                sys.stdout.flush()
-                raise e
+            categorical = [cat for cat, t in zip(categorical, targets)
+                           if not t]
+            attribute_names = [att for att, k in zip(attribute_names, targets)
+                               if not k]
 
+            x = self._convert_array_format(x, dataset_format, attribute_names)
             if scipy.sparse.issparse(y):
                 y = np.asarray(y.todense()).astype(target_dtype).flatten()
+            y = y.squeeze()
+            y = self._convert_array_format(y, dataset_format, attribute_names)
+            y = y.astype(target_dtype) if dataset_format == 'array' else y
+            data, targets = x, y
 
-            rval.append(x)
-            rval.append(y)
-
-        if return_categorical_indicator:
-            rval.append(categorical)
-        if return_attribute_names:
-            rval.append(attribute_names)
-
-        if len(rval) == 1:
-            return rval[0]
-        else:
-            return rval
+        return data, targets, categorical, attribute_names
 
-    def retrieve_class_labels(self, target_name='class'):
+    def retrieve_class_labels(self, target_name: str = 'class') -> Union[None, List[str]]:
         """Reads the datasets arff to determine the class-labels.
 
         If the task has no class labels (for example a regression problem)
         it returns None. Necessary because the data returned by get_data
         only contains the indices of the classes, while OpenML needs the real
         classname when uploading the results of a run.
 
@@ -418,41 +556,25 @@
         target_name : str
             Name of the target attribute
 
         Returns
         -------
         list
         """
-
-        # TODO improve performance, currently reads the whole file
-        # Should make a method that only reads the attributes
-        arffFileName = self.data_file
-
-        if self.format.lower() == 'arff':
-            return_type = arff.DENSE
-        elif self.format.lower() == 'sparse_arff':
-            return_type = arff.COO
-        else:
-            raise ValueError('Unknown data format %s' % self.format)
-
-        with io.open(arffFileName, encoding='utf8') as fh:
-            arffData = arff.ArffDecoder().decode(fh, return_type=return_type)
-
-        dataAttributes = dict(arffData['attributes'])
-        if target_name in dataAttributes:
-            return dataAttributes[target_name]
-        else:
-            return None
+        for feature in self.features.values():
+            if (feature.name == target_name) and (feature.data_type == 'nominal'):
+                return feature.nominal_values
+        return None
 
     def get_features_by_type(self, data_type, exclude=None,
                              exclude_ignore_attributes=True,
                              exclude_row_id_attribute=True):
         """
-        Returns indices of features of a given type, e.g., all nominal features.
-        Can use additional parameters to exclude various features by index or ontology.
+        Return indices of features of a given type, e.g. all nominal features.
+        Optional parameters to exclude various features by index or ontology.
 
         Parameters
         ----------
         data_type : str
             The data type to return (e.g., nominal, numeric, date, string)
         exclude : list(int)
             Indices to exclude (and adapt the return values as if these indices
@@ -471,38 +593,40 @@
         """
         if data_type not in OpenMLDataFeature.LEGAL_DATA_TYPES:
             raise TypeError("Illegal feature type requested")
         if self.ignore_attributes is not None:
             if not isinstance(self.ignore_attributes, list):
                 raise TypeError("ignore_attributes should be a list")
         if self.row_id_attribute is not None:
-            if not isinstance(self.row_id_attribute, six.string_types):
+            if not isinstance(self.row_id_attribute, str):
                 raise TypeError("row id attribute should be a str")
         if exclude is not None:
             if not isinstance(exclude, list):
                 raise TypeError("Exclude should be a list")
-            # assert all(isinstance(elem, str) for elem in exclude), "Exclude should be a list of strings"
+            # assert all(isinstance(elem, str) for elem in exclude),
+            #            "Exclude should be a list of strings"
         to_exclude = []
         if exclude is not None:
             to_exclude.extend(exclude)
         if exclude_ignore_attributes and self.ignore_attributes is not None:
             to_exclude.extend(self.ignore_attributes)
         if exclude_row_id_attribute and self.row_id_attribute is not None:
             to_exclude.append(self.row_id_attribute)
 
         result = []
         offset = 0
-        # this function assumes that everything in to_exclude will be 'excluded' from the dataset (hence the offset)
+        # this function assumes that everything in to_exclude will
+        # be 'excluded' from the dataset (hence the offset)
         for idx in self.features:
             name = self.features[idx].name
             if name in to_exclude:
                 offset += 1
             else:
                 if self.features[idx].data_type == data_type:
-                    result.append(idx-offset)
+                    result.append(idx - offset)
         return result
 
     def publish(self):
         """Publish the dataset on the OpenML server.
 
         Upload the dataset description and dataset content to openml.
 
@@ -518,48 +642,51 @@
             file_elements['dataset'] = self._dataset
         else:
             # the path to the arff dataset is given
             if self.data_file is not None:
                 path = os.path.abspath(self.data_file)
                 if os.path.exists(path):
                     try:
-                        # check if arff is valid
-                        decoder = arff.ArffDecoder()
+
                         with io.open(path, encoding='utf8') as fh:
+                            # check if arff is valid
+                            decoder = arff.ArffDecoder()
                             decoder.decode(fh, encode_nominal=True)
                     except arff.ArffException:
-                        raise ValueError("The file you have provided is not a valid arff file")
+                        raise ValueError("The file you have provided is not "
+                                         "a valid arff file.")
 
-                    file_elements['dataset'] = open(path, 'rb')
+                    with open(path, 'rb') as fp:
+                        file_elements['dataset'] = fp.read()
             else:
                 if self.url is None:
-                    raise ValueError("No path/url to the dataset file was given")
+                    raise ValueError("No url/path to the data file was given")
 
         return_value = openml._api_calls._perform_api_call(
-            "data/",
+            "data/", 'post',
             file_elements=file_elements,
         )
-        self.dataset_id = int(xmltodict.parse(return_value)['oml:upload_data_set']['oml:id'])
+        response = xmltodict.parse(return_value)
+        self.dataset_id = int(response['oml:upload_data_set']['oml:id'])
         return self.dataset_id
 
-
     def _to_xml(self):
-        """Serialize object to xml for upload
+        """ Serialize object to xml for upload
 
         Returns
         -------
         xml_dataset : str
             XML description of the data.
         """
         props = ['id', 'name', 'version', 'description', 'format', 'creator',
                  'contributor', 'collection_date', 'upload_date', 'language',
                  'licence', 'url', 'default_target_attribute',
                  'row_id_attribute', 'ignore_attribute', 'version_label',
                  'citation', 'tag', 'visibility', 'original_data_url',
-                 'paper_url', 'update_comment', 'md5_checksum']  # , 'data_file']
+                 'paper_url', 'update_comment', 'md5_checksum']
 
         data_container = OrderedDict()
         data_dict = OrderedDict([('@xmlns:oml', 'http://openml.org/openml')])
         data_container['oml:data_set_description'] = data_dict
 
         for prop in props:
             content = getattr(self, prop, None)
@@ -571,22 +698,14 @@
             pretty=True,
         )
         # A flow may not be uploaded with the xml encoding specification:
         # <?xml version="1.0" encoding="utf-8"?>
         xml_string = xml_string.split('\n', 1)[-1]
         return xml_string
 
-    def _data_features_supported(self):
-        if self.features is not None:
-            for idx in self.features:
-                if self.features[idx].data_type not in ['numeric', 'nominal']:
-                    return False
-            return True
-        return True
-
 
 def _check_qualities(qualities):
     if qualities is not None:
         qualities_ = {}
         for xmlquality in qualities:
             name = xmlquality['oml:name']
             if xmlquality.get('oml:value', None) is None:
```

### Comparing `openml-0.8.0/openml/datasets/functions.py` & `openml-0.9.0/openml/datasets/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,50 +1,44 @@
-import hashlib
 import io
 import os
 import re
+from typing import List, Dict, Union, Optional
 
 import numpy as np
-import six
 import arff
 import pandas as pd
 
 import xmltodict
 from scipy.sparse import coo_matrix
-from oslo_concurrency import lockutils
 from collections import OrderedDict
-from warnings import warn
 
 import openml.utils
 import openml._api_calls
 from .dataset import OpenMLDataset
 from ..exceptions import (
     OpenMLCacheException,
     OpenMLHashException,
     OpenMLServerException,
-    PrivateDatasetError,
+    OpenMLPrivateDatasetError,
 )
 from ..utils import (
     _create_cache_directory,
     _remove_cache_dir_for_id,
-    _create_cache_directory_for_id,
-    _create_lockfiles_dir,
+    _create_cache_directory_for_id
 )
 
 
 DATASETS_CACHE_DIR_NAME = 'datasets'
 
-
-
 ############################################################################
 # Local getters/accessors to the cache directory
 
 
 def _list_cached_datasets():
-    """Return list with ids of all cached datasets
+    """ Return list with ids of all cached datasets.
 
     Returns
     -------
     list
         List with IDs of all cached datasets.
     """
     datasets = []
@@ -62,16 +56,16 @@
 
         dataset_id = int(directory_name)
 
         directory_name = os.path.join(dataset_cache_dir,
                                       directory_name)
         dataset_directory_content = os.listdir(directory_name)
 
-        if ("dataset.arff" in dataset_directory_content and
-                "description.xml" in dataset_directory_content):
+        if ("dataset.arff" in dataset_directory_content
+           and "description.xml" in dataset_directory_content):
             if dataset_id not in datasets:
                 datasets.append(dataset_id)
 
     datasets.sort()
     return datasets
 
 
@@ -84,26 +78,31 @@
 
     for dataset_id in dataset_list:
         datasets[dataset_id] = _get_cached_dataset(dataset_id)
 
     return datasets
 
 
-def _get_cached_dataset(dataset_id):
+def _get_cached_dataset(
+    dataset_id: int
+) -> OpenMLDataset:
     """Get cached dataset for ID.
 
     Returns
     -------
     OpenMLDataset
     """
     description = _get_cached_dataset_description(dataset_id)
     arff_file = _get_cached_dataset_arff(dataset_id)
     features = _get_cached_dataset_features(dataset_id)
     qualities = _get_cached_dataset_qualities(dataset_id)
-    dataset = _create_dataset_from_description(description, features, qualities, arff_file)
+    dataset = _create_dataset_from_description(description,
+                                               features,
+                                               qualities,
+                                               arff_file)
 
     return dataset
 
 
 def _get_cached_dataset_description(dataset_id):
     did_cache_dir = _create_cache_directory_for_id(
         DATASETS_CACHE_DIR_NAME, dataset_id,
@@ -121,31 +120,30 @@
 
 def _get_cached_dataset_features(dataset_id):
     did_cache_dir = _create_cache_directory_for_id(
         DATASETS_CACHE_DIR_NAME, dataset_id,
     )
     features_file = os.path.join(did_cache_dir, "features.xml")
     try:
-        with io.open(features_file, encoding='utf8') as fh:
-            features_xml = fh.read()
-            return xmltodict.parse(features_xml)["oml:data_features"]
+        return _load_features_from_file(features_file)
     except (IOError, OSError):
         raise OpenMLCacheException("Dataset features for dataset id %d not "
                                    "cached" % dataset_id)
 
 
 def _get_cached_dataset_qualities(dataset_id):
     did_cache_dir = _create_cache_directory_for_id(
         DATASETS_CACHE_DIR_NAME, dataset_id,
     )
     qualities_file = os.path.join(did_cache_dir, "qualities.xml")
     try:
         with io.open(qualities_file, encoding='utf8') as fh:
             qualities_xml = fh.read()
-            return xmltodict.parse(qualities_xml)["oml:data_qualities"]['oml:quality']
+            qualities_dict = xmltodict.parse(qualities_xml)
+            return qualities_dict["oml:data_qualities"]['oml:quality']
     except (IOError, OSError):
         raise OpenMLCacheException("Dataset qualities for dataset id %d not "
                                    "cached" % dataset_id)
 
 
 def _get_cached_dataset_arff(dataset_id):
     did_cache_dir = _create_cache_directory_for_id(
@@ -158,215 +156,338 @@
             pass
         return output_file
     except (OSError, IOError):
         raise OpenMLCacheException("ARFF file for dataset id %d not "
                                    "cached" % dataset_id)
 
 
-def list_datasets(offset=None, size=None, status=None, tag=None, **kwargs):
+def _get_cache_directory(dataset: OpenMLDataset) -> str:
+    """ Return the cache directory of the OpenMLDataset """
+    return _create_cache_directory_for_id(DATASETS_CACHE_DIR_NAME, dataset.dataset_id)
+
+
+def list_datasets(
+    offset: Optional[int] = None,
+    size: Optional[int] = None,
+    status: Optional[str] = None,
+    tag: Optional[str] = None,
+    output_format: str = 'dict',
+    **kwargs
+) -> Union[Dict, pd.DataFrame]:
 
     """
-    Return a list of all dataset which are on OpenML. (Supports large amount of results)
+    Return a list of all dataset which are on OpenML.
+    Supports large amount of results.
 
     Parameters
     ----------
     offset : int, optional
         The number of datasets to skip, starting from the first.
     size : int, optional
         The maximum number of datasets to show.
     status : str, optional
         Should be {active, in_preparation, deactivated}. By
         default active datasets are returned, but also datasets
         from another status can be requested.
     tag : str, optional
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
     kwargs : dict, optional
         Legal filter operators (keys in the dict):
         data_name, data_version, number_instances,
         number_features, number_classes, number_missing_values.
 
     Returns
     -------
-    datasets : dict of dicts
-        A mapping from dataset ID to dict.
-
-        Every dataset is represented by a dictionary containing
-        the following information:
-        - dataset id
-        - name
-        - format
-        - status
-
-        If qualities are calculated for the dataset, some of
-        these are also returned.
-    """
-
-    return openml.utils._list_all(_list_datasets, offset=offset, size=size, status=status, tag=tag, **kwargs)
+    datasets : dict of dicts, or dataframe
+        - If output_format='dict'
+            A mapping from dataset ID to dict.
+
+            Every dataset is represented by a dictionary containing
+            the following information:
+            - dataset id
+            - name
+            - format
+            - status
+            If qualities are calculated for the dataset, some of
+            these are also returned.
+
+        - If output_format='dataframe'
+            Each row maps to a dataset
+            Each column contains the following information:
+            - dataset id
+            - name
+            - format
+            - status
+            If qualities are calculated for the dataset, some of
+            these are also included as columns.
+    """
+    if output_format not in ['dataframe', 'dict']:
+        raise ValueError("Invalid output format selected. "
+                         "Only 'dict' or 'dataframe' applicable.")
+
+    return openml.utils._list_all(output_format=output_format,
+                                  listing_call=_list_datasets,
+                                  offset=offset,
+                                  size=size,
+                                  status=status,
+                                  tag=tag,
+                                  **kwargs)
 
 
-def _list_datasets(**kwargs):
-
+def _list_datasets(output_format='dict', **kwargs):
     """
     Perform api call to return a list of all datasets.
 
     Parameters
     ----------
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
     kwargs : dict, optional
         Legal filter operators (keys in the dict):
-        {tag, status, limit, offset, data_name, data_version, number_instances,
+        tag, status, limit, offset, data_name, data_version, number_instances,
         number_features, number_classes, number_missing_values.
 
     Returns
     -------
-    datasets : dict of dicts
+    datasets : dict of dicts, or dataframe
     """
 
     api_call = "data/list"
 
     if kwargs is not None:
         for operator, value in kwargs.items():
             api_call += "/%s/%s" % (operator, value)
-    return __list_datasets(api_call)
+    return __list_datasets(api_call=api_call, output_format=output_format)
 
 
-def __list_datasets(api_call):
+def __list_datasets(api_call, output_format='dict'):
 
-    xml_string = openml._api_calls._perform_api_call(api_call)
+    xml_string = openml._api_calls._perform_api_call(api_call, 'get')
     datasets_dict = xmltodict.parse(xml_string, force_list=('oml:dataset',))
 
     # Minimalistic check if the XML is useful
     assert type(datasets_dict['oml:data']['oml:dataset']) == list, \
         type(datasets_dict['oml:data'])
     assert datasets_dict['oml:data']['@xmlns:oml'] == \
         'http://openml.org/openml', datasets_dict['oml:data']['@xmlns:oml']
 
     datasets = dict()
     for dataset_ in datasets_dict['oml:data']['oml:dataset']:
-        did = int(dataset_['oml:did'])
-        dataset = {'did': did,
-                   'name': dataset_['oml:name'],
-                   'format': dataset_['oml:format'],
-                   'status': dataset_['oml:status']}
+        ignore_attributes = ['oml:file_id', 'oml:quality']
+        dataset = {k.replace('oml:', ''): v
+                   for (k, v) in dataset_.items()
+                   if k not in ignore_attributes}
+        dataset['did'] = int(dataset['did'])
+        dataset['version'] = int(dataset['version'])
 
         # The number of qualities can range from 0 to infinity
         for quality in dataset_.get('oml:quality', list()):
-            quality['#text'] = float(quality['#text'])
-            if abs(int(quality['#text']) - quality['#text']) < 0.0000001:
-                quality['#text'] = int(quality['#text'])
-            dataset[quality['@name']] = quality['#text']
-        datasets[did] = dataset
+            try:
+                dataset[quality['@name']] = int(quality['#text'])
+            except ValueError:
+                dataset[quality['@name']] = float(quality['#text'])
+        datasets[dataset['did']] = dataset
+
+    if output_format == 'dataframe':
+        datasets = pd.DataFrame.from_dict(datasets, orient='index')
 
     return datasets
 
 
-def check_datasets_active(dataset_ids):
-    """Check if the dataset ids provided are active.
+def _load_features_from_file(features_file: str) -> Dict:
+    with io.open(features_file, encoding='utf8') as fh:
+        features_xml = fh.read()
+        xml_dict = xmltodict.parse(features_xml,
+                                   force_list=('oml:feature', 'oml:nominal_value'))
+        return xml_dict["oml:data_features"]
+
+
+def check_datasets_active(dataset_ids: List[int]) -> Dict[int, bool]:
+    """
+    Check if the dataset ids provided are active.
 
     Parameters
     ----------
-    dataset_ids : iterable
-        Integers representing dataset ids.
+    dataset_ids : List[int]
+        A list of integers representing dataset ids.
 
     Returns
     -------
     dict
         A dictionary with items {did: bool}
     """
-    dataset_list = list_datasets()
-    dataset_ids = sorted(dataset_ids)
+    dataset_list = list_datasets(status='all')
     active = {}
 
-    for dataset in dataset_list:
-        active[dataset['did']] = dataset['status'] == 'active'
-
     for did in dataset_ids:
-        if did not in active:
-            raise ValueError('Could not find dataset %d in OpenML dataset list.'
-                             % did)
-
-    active = {did: active[did] for did in dataset_ids}
+        dataset = dataset_list.get(did, None)
+        if dataset is None:
+            raise ValueError('Could not find dataset {} in OpenML dataset list.'.format(did))
+        else:
+            active[did] = (dataset['status'] == 'active')
 
     return active
 
 
-def get_datasets(dataset_ids):
+def _name_to_id(
+    dataset_name: str,
+    version: Optional[int] = None,
+    error_if_multiple: bool = False
+) -> int:
+    """ Attempt to find the dataset id of the dataset with the given name.
+
+    If multiple datasets with the name exist, and ``error_if_multiple`` is ``False``,
+    then return the least recent still active dataset.
+
+    Raises an error if no dataset with the name is found.
+    Raises an error if a version is specified but it could not be found.
+
+    Parameters
+    ----------
+    dataset_name : str
+        The name of the dataset for which to find its id.
+    version : int
+        Version to retrieve. If not specified, the oldest active version is returned.
+    error_if_multiple : bool (default=False)
+        If `False`, if multiple datasets match, return the least recent active dataset.
+        If `True`, if multiple datasets match, raise an error.
+
+    Returns
+    -------
+    int
+       The id of the dataset.
+    """
+    status = None if version is not None else 'active'
+    candidates = list_datasets(data_name=dataset_name, status=status, data_version=version)
+    if error_if_multiple and len(candidates) > 1:
+        raise ValueError("Multiple active datasets exist with name {}".format(dataset_name))
+    if len(candidates) == 0:
+        no_dataset_for_name = "No active datasets exist with name {}".format(dataset_name)
+        and_version = " and version {}".format(version) if version is not None else ""
+        raise RuntimeError(no_dataset_for_name + and_version)
+
+    # Dataset ids are chronological so we can just sort based on ids (instead of version)
+    return sorted(candidates)[0]
+
+
+def get_datasets(
+    dataset_ids: List[Union[str, int]],
+    download_data: bool = True,
+) -> List[OpenMLDataset]:
     """Download datasets.
 
     This function iterates :meth:`openml.datasets.get_dataset`.
 
     Parameters
     ----------
     dataset_ids : iterable
-        Integers representing dataset ids.
+        Integers or strings representing dataset ids or dataset names.
+        If dataset names are specified, the least recent still active dataset version is returned.
+    download_data : bool, optional
+        If True, also download the data file. Beware that some datasets are large and it might
+        make the operation noticeably slower. Metadata is also still retrieved.
+        If False, create the OpenMLDataset and only populate it with the metadata.
+        The data may later be retrieved through the `OpenMLDataset.get_data` method.
 
     Returns
     -------
     datasets : list of datasets
         A list of dataset objects.
     """
     datasets = []
     for dataset_id in dataset_ids:
-        datasets.append(get_dataset(dataset_id))
+        datasets.append(get_dataset(dataset_id, download_data))
     return datasets
 
 
-def get_dataset(dataset_id):
-    """Download a dataset.
-
-    TODO: explain caching!
+@openml.utils.thread_safe_if_oslo_installed
+def get_dataset(
+    dataset_id: Union[int, str],
+    download_data: bool = True,
+    version: int = None,
+    error_if_multiple: bool = False
+) -> OpenMLDataset:
+    """ Download the OpenML dataset representation, optionally also download actual data file.
 
     This function is thread/multiprocessing safe.
+    This function uses caching. A check will be performed to determine if the information has
+    previously been downloaded, and if so be loaded from disk instead of retrieved from the server.
+
+    If dataset is retrieved by name, a version may be specified.
+    If no version is specified and multiple versions of the dataset exist,
+    the earliest version of the dataset that is still active will be returned.
+    This scenario will raise an error instead if `exception_if_multiple` is `True`.
 
     Parameters
     ----------
-    dataset_id : int
+    dataset_id : int or str
         Dataset ID of the dataset to download
+    download_data : bool, optional (default=True)
+        If True, also download the data file. Beware that some datasets are large and it might
+        make the operation noticeably slower. Metadata is also still retrieved.
+        If False, create the OpenMLDataset and only populate it with the metadata.
+        The data may later be retrieved through the `OpenMLDataset.get_data` method.
+    version : int, optional (default=None)
+        Specifies the version if `dataset_id` is specified by name.
+        If no version is specified, retrieve the least recent still active version.
+    error_if_multiple : bool, optional (default=False)
+        If `True` raise an error if multiple datasets are found with matching criteria.
 
     Returns
     -------
     dataset : :class:`openml.OpenMLDataset`
-        The downloaded dataset."""
-    try:
-        dataset_id = int(dataset_id)
-    except:
-        raise ValueError("Dataset ID is neither an Integer nor can be "
-                         "cast to an Integer.")
-
-    with lockutils.external_lock(
-        name='datasets.functions.get_dataset:%d' % dataset_id,
-        lock_path=_create_lockfiles_dir(),
-    ):
-        did_cache_dir = _create_cache_directory_for_id(
-            DATASETS_CACHE_DIR_NAME, dataset_id,
-        )
-
+        The downloaded dataset.
+    """
+    if isinstance(dataset_id, str):
         try:
-            remove_dataset_cache = True
-            description = _get_dataset_description(did_cache_dir, dataset_id)
-            arff_file = _get_dataset_arff(did_cache_dir, description)
-            features = _get_dataset_features(did_cache_dir, dataset_id)
-            qualities = _get_dataset_qualities(did_cache_dir, dataset_id)
-            remove_dataset_cache = False
-        except OpenMLServerException as e:
-            # if there was an exception, check if the user had access to the dataset
-            if e.code == 112:
-                six.raise_from(PrivateDatasetError(e.message), None)
-            else:
-                raise e
-        finally:
-            if remove_dataset_cache:
-                _remove_cache_dir_for_id(DATASETS_CACHE_DIR_NAME, did_cache_dir)
+            dataset_id = int(dataset_id)
+        except ValueError:
+            dataset_id = _name_to_id(dataset_id, version, error_if_multiple)  # type: ignore
+    elif not isinstance(dataset_id, int):
+        raise TypeError("`dataset_id` must be one of `str` or `int`, not {}."
+                        .format(type(dataset_id)))
 
-        dataset = _create_dataset_from_description(
-            description, features, qualities, arff_file
-        )
+    did_cache_dir = _create_cache_directory_for_id(
+        DATASETS_CACHE_DIR_NAME, dataset_id,
+    )
+
+    try:
+        remove_dataset_cache = True
+        description = _get_dataset_description(did_cache_dir, dataset_id)
+        features = _get_dataset_features(did_cache_dir, dataset_id)
+        qualities = _get_dataset_qualities(did_cache_dir, dataset_id)
+
+        arff_file = _get_dataset_arff(description) if download_data else None
+
+        remove_dataset_cache = False
+    except OpenMLServerException as e:
+        # if there was an exception,
+        # check if the user had access to the dataset
+        if e.code == 112:
+            raise OpenMLPrivateDatasetError(e.message) from None
+        else:
+            raise e
+    finally:
+        if remove_dataset_cache:
+            _remove_cache_dir_for_id(DATASETS_CACHE_DIR_NAME,
+                                     did_cache_dir)
+
+    dataset = _create_dataset_from_description(
+        description, features, qualities, arff_file
+    )
     return dataset
 
 
 def attributes_arff_from_df(df):
-    """Create the attributes as specified by the ARFF format using a dataframe.
+    """ Describe attributes of the dataframe according to ARFF specification.
 
     Parameters
     ----------
     df : DataFrame, shape (n_samples, n_features)
         The dataframe containing the data set.
 
     Returns
@@ -383,15 +504,15 @@
     for column_name in df:
         # skipna=True does not infer properly the dtype. The NA values are
         # dropped before the inference instead.
         column_dtype = pd.api.types.infer_dtype(df[column_name].dropna())
 
         if column_dtype == 'categorical':
             # for categorical feature, arff expects a list string. However, a
-            # categorical column can contain mixed type and we should therefore
+            # categorical column can contain mixed type and should therefore
             # raise an error asking to convert all entries to string.
             categories = df[column_name].cat.categories
             categories_dtype = pd.api.types.infer_dtype(categories)
             if categories_dtype not in ('string', 'unicode'):
                 raise ValueError("The column '{}' of the dataframe is of "
                                  "'category' dtype. Therefore, all values in "
                                  "this columns should be string. Please "
@@ -456,27 +577,30 @@
         providing a dataframe, the attribute names and type can be inferred by
         passing ``attributes='auto'``.
         The target feature is indicated as meta-data of the dataset.
     default_target_attribute : str
         The default target attribute, if it exists.
         Can have multiple values, comma separated.
     ignore_attribute : str | list
-        Attributes that should be excluded in modelling, such as identifiers and indexes.
+        Attributes that should be excluded in modelling,
+        such as identifiers and indexes.
     citation : str
         Reference(s) that should be cited when building on this data.
     version_label : str, optional
-        Version label provided by user, can be a date, hash, or some other type of id.
+        Version label provided by user.
+         Can be a date, hash, or some other type of id.
     row_id_attribute : str, optional
         The attribute that represents the row-id column, if present in the
         dataset. If ``data`` is a dataframe and ``row_id_attribute`` is not
         specified, the index of the dataframe will be used as the
         ``row_id_attribute``. If the name of the index is ``None``, it will
         be discarded.
+
         .. versionadded: 0.8
-           Inference of ``row_id_attribute`` from a dataframe.
+            Inference of ``row_id_attribute`` from a dataframe.
     original_data_url : str, optional
         For derived data, the url to the original dataset.
     paper_url : str, optional
         Link to a paper describing the dataset.
     update_comment : str, optional
         An explanation for when the dataset is uploaded.
 
@@ -485,22 +609,22 @@
     class:`openml.OpenMLDataset`
         Dataset description."""
 
     if isinstance(data, (pd.DataFrame, pd.SparseDataFrame)):
         # infer the row id from the index of the dataset
         if row_id_attribute is None:
             row_id_attribute = data.index.name
-        # When calling data.values, the index will be skipped. We need to reset
-        # the index such that it is part of the data.
+        # When calling data.values, the index will be skipped.
+        # We need to reset the index such that it is part of the data.
         if data.index.name is not None:
             data = data.reset_index()
 
     if attributes == 'auto' or isinstance(attributes, dict):
         if not hasattr(data, "columns"):
-            raise ValueError("Automatically inferring the attributes required "
+            raise ValueError("Automatically inferring attributes requires "
                              "a pandas DataFrame or SparseDataFrame. "
                              "A {!r} was given instead.".format(data))
         # infer the type of data for each column of the DataFrame
         attributes_ = attributes_arff_from_df(data)
         if isinstance(attributes, dict):
             # override the attributes which was specified by the user
             for attr_idx in range(len(attributes_)):
@@ -574,16 +698,16 @@
             return_type=return_type
         )
     except arff.ArffException:
         raise ValueError("The arguments you have provided \
                              do not construct a valid ARFF file")
 
     return OpenMLDataset(
-        name,
-        description,
+        name=name,
+        description=description,
         data_format=data_format,
         creator=creator,
         contributor=contributor,
         collection_date=collection_date,
         language=language,
         licence=licence,
         default_target_attribute=default_target_attribute,
@@ -596,17 +720,17 @@
         update_comment=update_comment,
         dataset=arff_dataset,
     )
 
 
 def status_update(data_id, status):
     """
-    Updates the status of a dataset to either 'active' or 'deactivated'. Please
-    see the OpenML API documentation for a description of the status and all
-    legal status transitions:
+    Updates the status of a dataset to either 'active' or 'deactivated'.
+    Please see the OpenML API documentation for a description of the status
+    and all legal status transitions:
     https://docs.openml.org/#dataset-status
 
     Parameters
     ----------
     data_id : int
         The data id of the dataset
     status : str,
@@ -614,14 +738,15 @@
     """
     legal_status = {'active', 'deactivated'}
     if status not in legal_status:
         raise ValueError('Illegal status value. '
                          'Legal values: %s' % legal_status)
     data = {'data_id': data_id, 'status': status}
     result_xml = openml._api_calls._perform_api_call("data/status/update",
+                                                     'post',
                                                      data=data)
     result = xmltodict.parse(result_xml)
     server_data_id = result['oml:data_status_update']['oml:id']
     server_status = result['oml:data_status_update']['oml:status']
     if status != server_status or int(data_id) != int(server_data_id):
         # This should never happen
         raise ValueError('Data id/status does not collide')
@@ -643,83 +768,82 @@
     Returns
     -------
     dict
         XML Dataset description parsed to a dict.
 
     """
 
-    # TODO implement a cache for this that invalidates itself after some
-    # time
+    # TODO implement a cache for this that invalidates itself after some time
     # This can be saved on disk, but cannot be cached properly, because
     # it contains the information on whether a dataset is active.
     description_file = os.path.join(did_cache_dir, "description.xml")
 
     try:
         return _get_cached_dataset_description(dataset_id)
     except OpenMLCacheException:
-        dataset_xml = openml._api_calls._perform_api_call("data/%d" % dataset_id)
+        url_extension = "data/{}".format(dataset_id)
+        dataset_xml = openml._api_calls._perform_api_call(url_extension, 'get')
         with io.open(description_file, "w", encoding='utf8') as fh:
             fh.write(dataset_xml)
 
     description = xmltodict.parse(dataset_xml)[
         "oml:data_set_description"]
 
     return description
 
 
-def _get_dataset_arff(did_cache_dir, description):
-    """Get the filepath to the dataset ARFF
-
-    Checks if the file is in the cache, if yes, return the path to the file. If
-    not, downloads the file and caches it, then returns the file path.
+def _get_dataset_arff(description: Union[Dict, OpenMLDataset],
+                      cache_directory: str = None) -> str:
+    """ Return the path to the local arff file of the dataset. If is not cached, it is downloaded.
+
+    Checks if the file is in the cache, if yes, return the path to the file.
+    If not, downloads the file and caches it, then returns the file path.
+    The cache directory is generated based on dataset information, but can also be specified.
 
     This function is NOT thread/multiprocessing safe.
 
     Parameters
     ----------
-    did_cache_dir : str
-        Cache subdirectory for this dataset.
+    description : dictionary or OpenMLDataset
+        Either a dataset description as dict or OpenMLDataset.
 
-    description : dictionary
-        Dataset description dict.
+    cache_directory: str, optional (default=None)
+        Folder to store the arff file in.
+        If None, use the default cache directory for the dataset.
 
     Returns
     -------
     output_filename : string
         Location of ARFF file.
     """
-    output_file_path = os.path.join(did_cache_dir, "dataset.arff")
-    md5_checksum_fixture = description.get("oml:md5_checksum")
-    did = description.get("oml:id")
+    if isinstance(description, dict):
+        md5_checksum_fixture = description.get("oml:md5_checksum")
+        url = description['oml:url']
+        did = description.get('oml:id')
+    elif isinstance(description, OpenMLDataset):
+        md5_checksum_fixture = description.md5_checksum
+        url = description.url
+        did = description.dataset_id
+    else:
+        raise TypeError("`description` should be either OpenMLDataset or Dict.")
 
-    # This means the file is still there; whether it is useful is up to
-    # the user and not checked by the program.
-    try:
-        with io.open(output_file_path, encoding='utf8'):
-            pass
-        return output_file_path
-    except (OSError, IOError):
-        pass
+    if cache_directory is None:
+        cache_directory = _create_cache_directory_for_id(DATASETS_CACHE_DIR_NAME, did)
+    output_file_path = os.path.join(cache_directory, "dataset.arff")
 
-    url = description['oml:url']
-    arff_string = openml._api_calls._read_url(url)
-    md5 = hashlib.md5()
-    md5.update(arff_string.encode('utf-8'))
-    md5_checksum = md5.hexdigest()
-    if md5_checksum != md5_checksum_fixture:
-        raise OpenMLHashException(
-            'Checksum %s of downloaded dataset %d is unequal to the checksum '
-            '%s sent by the server.' % (
-                md5_checksum, int(did), md5_checksum_fixture
-            )
+    try:
+        openml.utils._download_text_file(
+            source=url,
+            output_path=output_file_path,
+            md5_checksum=md5_checksum_fixture
         )
-
-    with io.open(output_file_path, "w", encoding='utf8') as fh:
-        fh.write(arff_string)
-    del arff_string
+    except OpenMLHashException as e:
+        additional_info = " Raised when downloading dataset {}.".format(did)
+        e.args = (e.args[0] + additional_info,)
+        raise
 
     return output_file_path
 
 
 def _get_dataset_features(did_cache_dir, dataset_id):
     """API call to get dataset features (cached)
 
@@ -740,26 +864,21 @@
     -------
     features : dict
         Dictionary containing dataset feature descriptions, parsed from XML.
     """
     features_file = os.path.join(did_cache_dir, "features.xml")
 
     # Dataset features aren't subject to change...
-    try:
-        with io.open(features_file, encoding='utf8') as fh:
-            features_xml = fh.read()
-    except (OSError, IOError):
-        features_xml = openml._api_calls._perform_api_call("data/features/%d" % dataset_id)
-
+    if not os.path.isfile(features_file):
+        url_extension = "data/features/{}".format(dataset_id)
+        features_xml = openml._api_calls._perform_api_call(url_extension, 'get')
         with io.open(features_file, "w", encoding='utf8') as fh:
             fh.write(features_xml)
 
-    features = xmltodict.parse(features_xml, force_list=('oml:feature',))["oml:data_features"]
-
-    return features
+    return _load_features_from_file(features_file)
 
 
 def _get_dataset_qualities(did_cache_dir, dataset_id):
     """API call to get dataset qualities (cached)
 
     Features are metafeatures (number of features, number of classes, ...)
 
@@ -780,70 +899,78 @@
     """
     # Dataset qualities are subject to change and must be fetched every time
     qualities_file = os.path.join(did_cache_dir, "qualities.xml")
     try:
         with io.open(qualities_file, encoding='utf8') as fh:
             qualities_xml = fh.read()
     except (OSError, IOError):
-        qualities_xml = openml._api_calls._perform_api_call("data/qualities/%d" % dataset_id)
+        url_extension = "data/qualities/{}".format(dataset_id)
+        qualities_xml = openml._api_calls._perform_api_call(url_extension, 'get')
 
         with io.open(qualities_file, "w", encoding='utf8') as fh:
             fh.write(qualities_xml)
 
-    qualities = xmltodict.parse(qualities_xml, force_list=('oml:quality',))['oml:data_qualities']['oml:quality']
+    xml_as_dict = xmltodict.parse(qualities_xml, force_list=('oml:quality',))
+    qualities = xml_as_dict['oml:data_qualities']['oml:quality']
 
     return qualities
 
 
-def _create_dataset_from_description(description, features, qualities, arff_file):
+def _create_dataset_from_description(
+        description: Dict[str, str],
+        features: Dict,
+        qualities: List,
+        arff_file: str = None,
+) -> OpenMLDataset:
     """Create a dataset object from a description dict.
 
     Parameters
     ----------
     description : dict
         Description of a dataset in xml dict.
-    arff_file : string
+    features : dict
+        Description of a dataset features.
+    qualities : list
+        Description of a dataset qualities.
+    arff_file : string, optional
         Path of dataset ARFF file.
 
     Returns
     -------
     dataset : dataset object
         Dataset object from dict and ARFF.
     """
-    dataset = OpenMLDataset(
+    return OpenMLDataset(
         description["oml:name"],
         description.get("oml:description"),
         data_format=description["oml:format"],
         dataset_id=description["oml:id"],
         version=description["oml:version"],
         creator=description.get("oml:creator"),
         contributor=description.get("oml:contributor"),
         collection_date=description.get("oml:collection_date"),
         upload_date=description.get("oml:upload_date"),
         language=description.get("oml:language"),
         licence=description.get("oml:licence"),
         url=description["oml:url"],
-        default_target_attribute=description.get(
-            "oml:default_target_attribute"
-        ),
+        default_target_attribute=description.get("oml:default_target_attribute"),
         row_id_attribute=description.get("oml:row_id_attribute"),
         ignore_attribute=description.get("oml:ignore_attribute"),
         version_label=description.get("oml:version_label"),
         citation=description.get("oml:citation"),
         tag=description.get("oml:tag"),
         visibility=description.get("oml:visibility"),
         original_data_url=description.get("oml:original_data_url"),
         paper_url=description.get("oml:paper_url"),
         update_comment=description.get("oml:update_comment"),
         md5_checksum=description.get("oml:md5_checksum"),
         data_file=arff_file,
         features=features,
         qualities=qualities,
     )
-    return dataset
 
 
 def _get_online_dataset_arff(dataset_id):
     """Download the ARFF file for a given dataset id
     from the OpenML website.
 
     Parameters
@@ -852,19 +979,21 @@
         A dataset id.
 
     Returns
     -------
     str
         A string representation of an ARFF file.
     """
-    dataset_xml = openml._api_calls._perform_api_call("data/%d" % dataset_id)
+    dataset_xml = openml._api_calls._perform_api_call("data/%d" % dataset_id,
+                                                      'get')
     # build a dict from the xml.
     # use the url from the dataset description and return the ARFF string
     return openml._api_calls._read_url(
-        xmltodict.parse(dataset_xml)['oml:data_set_description']['oml:url']
+        xmltodict.parse(dataset_xml)['oml:data_set_description']['oml:url'],
+        request_method='get'
     )
 
 
 def _get_online_dataset_format(dataset_id):
     """Get the dataset format for a given dataset id
     from the OpenML website.
 
@@ -874,12 +1003,13 @@
         A dataset id.
 
     Returns
     -------
     str
         Dataset format.
     """
-    dataset_xml = openml._api_calls._perform_api_call("data/%d" % dataset_id)
+    dataset_xml = openml._api_calls._perform_api_call("data/%d" % dataset_id,
+                                                      'get')
     # build a dict from the xml and get the format from the dataset description
     return xmltodict\
         .parse(dataset_xml)['oml:data_set_description']['oml:format']\
         .lower()
```

### Comparing `openml-0.8.0/openml/evaluations/evaluation.py` & `openml-0.9.0/openml/evaluations/evaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,37 +3,38 @@
     """
     Contains all meta-information about a run / evaluation combination,
     according to the evaluation/list function
 
     Parameters
     ----------
     run_id : int
-    
+        Refers to the run.
     task_id : int
-    
+        Refers to the task.
     setup_id : int
-    
+        Refers to the setup.
     flow_id : int
-    
+        Refers to the flow.
     flow_name : str
-    
+        Name of the referred flow.
     data_id : int
-    
+        Refers to the dataset.
     data_name : str
-        the name of the dataset
+        The name of the dataset.
     function : str
-        the evaluation function of this item (e.g., accuracy)
+        The evaluation metric of this item (e.g., accuracy).
     upload_time : str
-        the time of evaluation
+        The time of evaluation.
     value : float
-        the value of this evaluation
+        The value (score) of this evaluation.
     values : List[float]
-        the values per repeat and fold (if requested)
+        The values (scores) per repeat and fold (if requested)
     array_data : str
-        list of information per class (e.g., in case of precision, auroc, recall)
+        list of information per class.
+        (e.g., in case of precision, auroc, recall)
     """
     def __init__(self, run_id, task_id, setup_id, flow_id, flow_name,
                  data_id, data_name, function, upload_time, value, values,
                  array_data=None):
         self.run_id = run_id
         self.task_id = task_id
         self.setup_id = setup_id
```

### Comparing `openml-0.8.0/openml/flows/flow.py` & `openml-0.9.0/openml/flows/flow.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections import OrderedDict
+import os
+from typing import Dict, List, Union  # noqa: F401
 
-import six
 import xmltodict
 
-import openml._api_calls
-from ..utils import extract_xml_tags
+from ..extensions import get_extension_by_flow
+from ..utils import extract_xml_tags, _tag_entity
 
 
 class OpenMLFlow(object):
     """OpenML Flow. Stores machine learning models.
 
     Flows should not be generated manually, but by the function
     :meth:`openml.flows.create_flow_from_model`. Using this helper function
@@ -125,15 +126,17 @@
         self.binary_md5 = binary_md5
         self.version = version
         self.upload_date = upload_date
         self.language = language
         self.dependencies = dependencies
         self.flow_id = flow_id
 
-    def _to_xml(self):
+        self.extension = get_extension_by_flow(self)
+
+    def _to_xml(self) -> str:
         """Generate xml representation of self for upload to server.
 
         Returns
         -------
         str
             Flow represented as XML string.
         """
@@ -141,15 +144,15 @@
         flow_xml = xmltodict.unparse(flow_dict, pretty=True)
 
         # A flow may not be uploaded with the xml encoding specification:
         # <?xml version="1.0" encoding="utf-8"?>
         flow_xml = flow_xml.split('\n', 1)[-1]
         return flow_xml
 
-    def _to_dict(self):
+    def _to_dict(self) -> dict:
         """ Helper function used by _to_xml and itself.
 
         Creates a dictionary representation of self which can be serialized
         to xml by the function _to_xml. Since a flow can contain subflows
         (components) this helper function calls itself recursively to also
         serialize these flows to dictionaries.
 
@@ -160,16 +163,16 @@
 
         Returns
         -------
         OrderedDict
             Flow represented as OrderedDict.
 
         """
-        flow_container = OrderedDict()
-        flow_dict = OrderedDict([('@xmlns:oml', 'http://openml.org/openml')])
+        flow_container = OrderedDict()  # type: 'OrderedDict[str, OrderedDict]'
+        flow_dict = OrderedDict([('@xmlns:oml', 'http://openml.org/openml')])  # type: 'OrderedDict[str, Union[List, str]]'  # noqa E501
         flow_container['oml:flow'] = flow_dict
         _add_if_nonempty(flow_dict, 'oml:id', self.flow_id)
 
         for required in ["name", "external_version"]:
             if getattr(self, required) is None:
                 raise ValueError("self.{} is required but None".format(
                     required))
@@ -177,49 +180,49 @@
                           "version", "external_version", "description",
                           "upload_date", "language", "dependencies"]:
             _add_if_nonempty(flow_dict, 'oml:{}'.format(attribute),
                              getattr(self, attribute))
 
         flow_parameters = []
         for key in self.parameters:
-            param_dict = OrderedDict()
+            param_dict = OrderedDict()  # type: 'OrderedDict[str, str]'
             param_dict['oml:name'] = key
             meta_info = self.parameters_meta_info[key]
 
             _add_if_nonempty(param_dict, 'oml:data_type',
                              meta_info['data_type'])
             param_dict['oml:default_value'] = self.parameters[key]
             _add_if_nonempty(param_dict, 'oml:description',
                              meta_info['description'])
 
             for key_, value in param_dict.items():
-                if key_ is not None and not isinstance(key_, six.string_types):
+                if key_ is not None and not isinstance(key_, str):
                     raise ValueError('Parameter name %s cannot be serialized '
                                      'because it is of type %s. Only strings '
                                      'can be serialized.' % (key_, type(key_)))
-                if value is not None and not isinstance(value, six.string_types):
+                if value is not None and not isinstance(value, str):
                     raise ValueError('Parameter value %s cannot be serialized '
                                      'because it is of type %s. Only strings '
-                                     'can be serialized.' % (value, type(value)))
+                                     'can be serialized.'
+                                     % (value, type(value)))
 
             flow_parameters.append(param_dict)
 
         flow_dict['oml:parameter'] = flow_parameters
 
         components = []
         for key in self.components:
-            component_dict = OrderedDict()
+            component_dict = OrderedDict()  # type: 'OrderedDict[str, Dict]'
             component_dict['oml:identifier'] = key
-            component_dict['oml:flow'] = \
-                self.components[key]._to_dict()['oml:flow']
+            component_dict['oml:flow'] = self.components[key]._to_dict()['oml:flow']
 
             for key_ in component_dict:
                 # We only need to check if the key is a string, because the
                 # value is a flow. The flow itself is valid by recursion
-                if key_ is not None and not isinstance(key_, six.string_types):
+                if key_ is not None and not isinstance(key_, str):
                     raise ValueError('Parameter name %s cannot be serialized '
                                      'because it is of type %s. Only strings '
                                      'can be serialized.' % (key_, type(key_)))
 
             components.append(component_dict)
 
         flow_dict['oml:component'] = components
@@ -308,56 +311,93 @@
         arguments['tags'] = extract_xml_tags('oml:tag', dic)
 
         arguments['model'] = None
         flow = cls(**arguments)
 
         return flow
 
-    def publish(self):
-        """Publish flow to OpenML server.
+    def to_filesystem(self, output_directory: str) -> None:
+        os.makedirs(output_directory, exist_ok=True)
+        if 'flow.xml' in os.listdir(output_directory):
+            raise ValueError('Output directory already contains a flow.xml file.')
+
+        run_xml = self._to_xml()
+        with open(os.path.join(output_directory, 'flow.xml'), 'w') as f:
+            f.write(run_xml)
+
+    @classmethod
+    def from_filesystem(cls, input_directory) -> 'OpenMLFlow':
+        with open(os.path.join(input_directory, 'flow.xml'), 'r') as f:
+            xml_string = f.read()
+        return OpenMLFlow._from_dict(xmltodict.parse(xml_string))
+
+    def publish(self, raise_error_if_exists: bool = False) -> 'OpenMLFlow':
+        """ Publish this flow to OpenML server.
+
+        Raises a PyOpenMLError if the flow exists on the server, but
+        `self.flow_id` does not match the server known flow id.
+
+        Parameters
+        ----------
+        raise_error_if_exists : bool, optional (default=False)
+            If True, raise PyOpenMLError if the flow exists on the server.
+            If False, update the local flow to match the server flow.
 
         Returns
         -------
         self : OpenMLFlow
 
         """
         # Import at top not possible because of cyclic dependencies. In
         # particular, flow.py tries to import functions.py in order to call
         # get_flow(), while functions.py tries to import flow.py in order to
         # instantiate an OpenMLFlow.
         import openml.flows.functions
 
-        xml_description = self._to_xml()
+        flow_id = openml.flows.functions.flow_exists(self.name, self.external_version)
+        if not flow_id:
+            if self.flow_id:
+                raise openml.exceptions.PyOpenMLError("Flow does not exist on the server, "
+                                                      "but 'flow.flow_id' is not None.")
+            xml_description = self._to_xml()
+            file_elements = {'description': xml_description}
+            return_value = openml._api_calls._perform_api_call(
+                "flow/",
+                'post',
+                file_elements=file_elements,
+            )
+            server_response = xmltodict.parse(return_value)
+            flow_id = int(server_response['oml:upload_flow']['oml:id'])
+        elif raise_error_if_exists:
+            error_message = "This OpenMLFlow already exists with id: {}.".format(flow_id)
+            raise openml.exceptions.PyOpenMLError(error_message)
+        elif self.flow_id is not None and self.flow_id != flow_id:
+            raise openml.exceptions.PyOpenMLError("Local flow_id does not match server flow_id: "
+                                                  "'{}' vs '{}'".format(self.flow_id, flow_id))
 
-        file_elements = {'description': xml_description}
-        return_value = openml._api_calls._perform_api_call(
-            "flow/",
-            file_elements=file_elements,
-        )
-        flow_id = int(xmltodict.parse(return_value)['oml:upload_flow']['oml:id'])
         flow = openml.flows.functions.get_flow(flow_id)
         _copy_server_fields(flow, self)
         try:
             openml.flows.functions.assert_flows_equal(
                 self, flow, flow.upload_date, ignore_parameter_values=True
             )
         except ValueError as e:
             message = e.args[0]
             raise ValueError("Flow was not stored correctly on the server. "
                              "New flow ID is %d. Please check manually and "
                              "remove the flow if necessary! Error is:\n'%s'" %
                              (flow_id, message))
         return self
 
-    def get_structure(self, key_item):
+    def get_structure(self, key_item: str) -> Dict[str, List[str]]:
         """
-        Returns for each sub-component of the flow the path of identifiers that
-        should be traversed to reach this component. The resulting dict maps a
-        key (identifying a flow by either its id, name or fullname) to the
-        parameter prefix.
+        Returns for each sub-component of the flow the path of identifiers
+        that should be traversed to reach this component. The resulting dict
+        maps a key (identifying a flow by either its id, name or fullname) to
+        the parameter prefix.
 
         Parameters
         ----------
         key_item: str
             The flow attribute that will be used to identify flows in the
             structure. Allowed values {flow_id, name}
 
@@ -409,27 +449,25 @@
         """Annotates this flow with a tag on the server.
 
         Parameters
         ----------
         tag : str
             Tag to attach to the flow.
         """
-        data = {'flow_id': self.flow_id, 'tag': tag}
-        openml._api_calls._perform_api_call("/flow/tag", data=data)
+        _tag_entity('flow', self.flow_id, tag)
 
     def remove_tag(self, tag):
         """Removes a tag from this flow on the server.
 
         Parameters
         ----------
         tag : str
             Tag to attach to the flow.
         """
-        data = {'flow_id': self.flow_id, 'tag': tag}
-        openml._api_calls._perform_api_call("/flow/untag", data=data)
+        _tag_entity('flow', self.flow_id, tag, untag=True)
 
 
 def _copy_server_fields(source_flow, target_flow):
     fields_added_by_the_server = ['flow_id', 'uploader', 'version',
                                   'upload_date']
     for field in fields_added_by_the_server:
         setattr(target_flow, field, getattr(source_flow, field))
```

### Comparing `openml-0.8.0/openml/runs/__init__.py` & `openml-0.9.0/openml/runs/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from .functions import (
     run_model_on_task,
     run_flow_on_task,
     get_run,
     list_runs,
     get_runs,
     get_run_trace,
+    run_exists,
     initialize_model_from_run,
     initialize_model_from_trace,
 )
 
 __all__ = [
     'OpenMLRun',
     'OpenMLRunTrace',
     'OpenMLTraceIteration',
     'run_model_on_task',
     'run_flow_on_task',
     'get_run',
     'list_runs',
     'get_runs',
     'get_run_trace',
+    'run_exists',
     'initialize_model_from_run',
     'initialize_model_from_trace'
 ]
```

### Comparing `openml-0.8.0/openml/runs/functions.py` & `openml-0.9.0/openml/runs/functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,300 +1,360 @@
-import collections
+from collections import OrderedDict
 import io
-import json
+import itertools
 import os
-import sys
-import time
+from typing import Any, List, Dict, Optional, Set, Tuple, Union, TYPE_CHECKING  # noqa F401
 import warnings
 
-import numpy as np
-import sklearn.pipeline
-import six
-import xmltodict
 import sklearn.metrics
+import xmltodict
+import pandas as pd
 
 import openml
 import openml.utils
 import openml._api_calls
-from ..exceptions import PyOpenMLError
-from .. import config
-from openml.flows.sklearn_converter import _check_n_jobs
+from openml.exceptions import PyOpenMLError
+from openml.extensions import get_extension_by_model
+from openml import config
 from openml.flows.flow import _copy_server_fields
-from ..flows import sklearn_to_flow, get_flow, flow_exists, OpenMLFlow
+from ..flows import get_flow, flow_exists, OpenMLFlow
 from ..setups import setup_exists, initialize_model
-from ..exceptions import OpenMLCacheException, OpenMLServerException
-from ..tasks import OpenMLTask
-from .run import OpenMLRun, _get_version_information
+from ..exceptions import OpenMLCacheException, OpenMLServerException, OpenMLRunsExistError
+from ..tasks import OpenMLTask, OpenMLClassificationTask, OpenMLClusteringTask, \
+    OpenMLRegressionTask, OpenMLSupervisedTask, OpenMLLearningCurveTask
+from .run import OpenMLRun
 from .trace import OpenMLRunTrace
+from ..tasks import TaskTypeEnum
 
-# _get_version_info, _get_dict and _create_setup_string are in run.py to avoid
-# circular imports
+# Avoid import cycles: https://mypy.readthedocs.io/en/latest/common_issues.html#import-cycles
+if TYPE_CHECKING:
+    from openml.extensions.extension_interface import Extension
+
+# get_dict is in run.py to avoid circular imports
 
 RUNS_CACHE_DIR_NAME = 'runs'
 
 
-def run_model_on_task(model, task, avoid_duplicate_runs=True, flow_tags=None,
-                      seed=None, add_local_measures=True):
-    """See ``run_flow_on_task for a documentation``."""
-    # TODO: At some point in the future do not allow for arguments in old order (order changed 6-2018).
-    if isinstance(model, OpenMLTask) and hasattr(task, 'fit') and hasattr(task, 'predict'):
-        warnings.warn("The old argument order (task, model) is deprecated and will not be supported in the future. "
-                      "Please use the order (model, task).", DeprecationWarning)
+def run_model_on_task(
+    model: Any,
+    task: OpenMLTask,
+    avoid_duplicate_runs: bool = True,
+    flow_tags: List[str] = None,
+    seed: int = None,
+    add_local_measures: bool = True,
+    upload_flow: bool = False,
+    return_flow: bool = False,
+) -> Union[OpenMLRun, Tuple[OpenMLRun, OpenMLFlow]]:
+    """Run the model on the dataset defined by the task.
+
+    Parameters
+    ----------
+    model : sklearn model
+        A model which has a function fit(X,Y) and predict(X),
+        all supervised estimators of scikit learn follow this definition of a model [1]
+        [1](http://scikit-learn.org/stable/tutorial/statistical_inference/supervised_learning.html)
+    task : OpenMLTask
+        Task to perform. This may be a model instead if the first argument is an OpenMLTask.
+    avoid_duplicate_runs : bool, optional (default=True)
+        If True, the run will throw an error if the setup/task combination is already present on
+        the server. This feature requires an internet connection.
+    flow_tags : List[str], optional (default=None)
+        A list of tags that the flow should have at creation.
+    seed: int, optional (default=None)
+        Models that are not seeded will get this seed.
+    add_local_measures : bool, optional (default=True)
+        Determines whether to calculate a set of evaluation measures locally,
+        to later verify server behaviour.
+    upload_flow : bool (default=False)
+        If True, upload the flow to OpenML if it does not exist yet.
+        If False, do not upload the flow to OpenML.
+    return_flow : bool (default=False)
+        If True, returns the OpenMLFlow generated from the model in addition to the OpenMLRun.
+
+    Returns
+    -------
+    run : OpenMLRun
+        Result of the run.
+    flow : OpenMLFlow (optional, only if `return_flow` is True).
+        Flow generated from the model.
+    """
+
+    extension = get_extension_by_model(model, raise_if_no_extension=True)
+    if extension is None:
+        # This should never happen and is only here to please mypy will be gone soon once the
+        # whole function is removed
+        raise TypeError(extension)
+
+    # TODO: At some point in the future do not allow for arguments in old order (6-2018).
+    # Flexibility currently still allowed due to code-snippet in OpenML100 paper (3-2019).
+    # When removing this please also remove the method `is_estimator` from the extension
+    # interface as it is only used here (MF, 3-2019)
+    if isinstance(model, OpenMLTask) and extension.is_estimator(model):
+        warnings.warn("The old argument order (task, model) is deprecated and "
+                      "will not be supported in the future. Please use the "
+                      "order (model, task).", DeprecationWarning)
         task, model = model, task
 
-    flow = sklearn_to_flow(model)
+    flow = extension.model_to_flow(model)
 
-    return run_flow_on_task(task=task, flow=flow,
-                            avoid_duplicate_runs=avoid_duplicate_runs,
-                            flow_tags=flow_tags, seed=seed,
-                            add_local_measures=add_local_measures)
+    run = run_flow_on_task(
+        task=task,
+        flow=flow,
+        avoid_duplicate_runs=avoid_duplicate_runs,
+        flow_tags=flow_tags,
+        seed=seed,
+        add_local_measures=add_local_measures,
+        upload_flow=upload_flow,
+    )
+    if return_flow:
+        return run, flow
+    return run
 
 
-def run_flow_on_task(flow, task, avoid_duplicate_runs=True, flow_tags=None,
-                     seed=None, add_local_measures=True):
+def run_flow_on_task(
+    flow: OpenMLFlow,
+    task: OpenMLTask,
+    avoid_duplicate_runs: bool = True,
+    flow_tags: List[str] = None,
+    seed: int = None,
+    add_local_measures: bool = True,
+    upload_flow: bool = False,
+) -> OpenMLRun:
+
     """Run the model provided by the flow on the dataset defined by task.
 
-    Takes the flow and repeat information into account. In case a flow is not
-    yet published, it is published after executing the run (requires
-    internet connection).
+    Takes the flow and repeat information into account.
+    The Flow may optionally be published.
 
     Parameters
     ----------
-    model : sklearn model
-        A model which has a function fit(X,Y) and predict(X),
+    flow : OpenMLFlow
+        A flow wraps a machine learning model together with relevant information.
+        The model has a function fit(X,Y) and predict(X),
         all supervised estimators of scikit learn follow this definition of a model [1]
         [1](http://scikit-learn.org/stable/tutorial/statistical_inference/supervised_learning.html)
     task : OpenMLTask
-        Task to perform. This may be an OpenMLFlow instead if the second argument is an OpenMLTask.
-    avoid_duplicate_runs : bool
-        If this flag is set to True, the run will throw an error if the
-        setup/task combination is already present on the server. Works only
-        if the flow is already published on the server. This feature requires an
-        internet connection.
-        This may be an OpenMLTask instead if the first argument is the OpenMLFlow.
-    flow_tags : list(str)
+        Task to perform. This may be an OpenMLFlow instead if the first argument is an OpenMLTask.
+    avoid_duplicate_runs : bool, optional (default=True)
+        If True, the run will throw an error if the setup/task combination is already present on
+        the server. This feature requires an internet connection.
+    avoid_duplicate_runs : bool, optional (default=True)
+        If True, the run will throw an error if the setup/task combination is already present on
+        the server. This feature requires an internet connection.
+    flow_tags : List[str], optional (default=None)
         A list of tags that the flow should have at creation.
-    seed: int
-        Models that are not seeded will be automatically seeded by a RNG. The
-        RBG will be seeded with this seed.
-    add_local_measures : bool
+    seed: int, optional (default=None)
+        Models that are not seeded will get this seed.
+    add_local_measures : bool, optional (default=True)
         Determines whether to calculate a set of evaluation measures locally,
-        to later verify server behaviour. Defaults to True
+        to later verify server behaviour.
+    upload_flow : bool (default=False)
+        If True, upload the flow to OpenML if it does not exist yet.
+        If False, do not upload the flow to OpenML.
 
     Returns
     -------
     run : OpenMLRun
         Result of the run.
     """
     if flow_tags is not None and not isinstance(flow_tags, list):
-        raise ValueError("flow_tags should be list")
+        raise ValueError("flow_tags should be a list")
+
+    if task.task_id is None:
+        raise ValueError("The task should be published at OpenML")
 
-    # TODO: At some point in the future do not allow for arguments in old order (order changed 6-2018).
+    # TODO: At some point in the future do not allow for arguments in old order (changed 6-2018).
+    # Flexibility currently still allowed due to code-snippet in OpenML100 paper (3-2019).
     if isinstance(flow, OpenMLTask) and isinstance(task, OpenMLFlow):
         # We want to allow either order of argument (to avoid confusion).
-        warnings.warn("The old argument order (Flow, model) is deprecated and will not be supported in the future. "
-                      "Please use the order (model, Flow).", DeprecationWarning)
+        warnings.warn("The old argument order (Flow, model) is deprecated and "
+                      "will not be supported in the future. Please use the "
+                      "order (model, Flow).", DeprecationWarning)
         task, flow = flow, task
 
-    flow.model = _get_seeded_model(flow.model, seed=seed)
+    flow.model = flow.extension.seed_model(flow.model, seed=seed)
 
-    # skips the run if it already exists and the user opts for this in the config file.
-    # also, if the flow is not present on the server, the check is not needed.
-    flow_id = flow_exists(flow.name, flow.external_version)
-    if avoid_duplicate_runs and flow_id:
-        flow_from_server = get_flow(flow_id)
-        flow_from_server.model = flow.model
-        setup_id = setup_exists(flow_from_server)
-        ids = _run_exists(task.task_id, setup_id)
-        if ids:
-            raise PyOpenMLError("Run already exists in server. Run id(s): %s" % str(ids))
-        _copy_server_fields(flow_from_server, flow)
+    # We only need to sync with the server right now if we want to upload the flow,
+    # or ensure no duplicate runs exist. Otherwise it can be synced at upload time.
+    flow_id = None
+    if upload_flow or avoid_duplicate_runs:
+        flow_id = flow_exists(flow.name, flow.external_version)
+        if isinstance(flow.flow_id, int) and flow_id != flow.flow_id:
+            if flow_id:
+                raise PyOpenMLError("Local flow_id does not match server flow_id: "
+                                    "'{}' vs '{}'".format(flow.flow_id, flow_id))
+            else:
+                raise PyOpenMLError("Flow does not exist on the server, "
+                                    "but 'flow.flow_id' is not None.")
 
-    dataset = task.get_dataset()
+        if upload_flow and not flow_id:
+            flow.publish()
+            flow_id = flow.flow_id
+        elif flow_id:
+            flow_from_server = get_flow(flow_id)
+            _copy_server_fields(flow_from_server, flow)
+            if avoid_duplicate_runs:
+                flow_from_server.model = flow.model
+                setup_id = setup_exists(flow_from_server)
+                ids = run_exists(task.task_id, setup_id)
+                if ids:
+                    error_message = ("One or more runs of this setup were "
+                                     "already performed on the task.")
+                    raise OpenMLRunsExistError(ids, error_message)
+        else:
+            # Flow does not exist on server and we do not want to upload it.
+            # No sync with the server happens.
+            flow_id = None
+            pass
 
-    if task.class_labels is None:
-        raise ValueError('The task has no class labels. This method currently '
-                         'only works for tasks with class labels.')
+    dataset = task.get_dataset()
 
-    run_environment = _get_version_information()
+    run_environment = flow.extension.get_version_information()
     tags = ['openml-python', run_environment[1]]
 
     # execute the run
-    res = _run_task_get_arffcontent(flow.model, task, add_local_measures=add_local_measures)
-
-    # in case the flow not exists, flow_id will be False (as returned by
-    # flow_exists). Also check whether there are no illegal flow.flow_id values
-    # (compared to result of openml.flows.flow_exists)
-    if flow_id is False:
-        if flow.flow_id is not None:
-            raise ValueError('flow.flow_id is not None, but the flow does not'
-                             'exist on the server according to flow_exists')
-        _publish_flow_if_necessary(flow)
-        # if the flow was published successfully
-        # and has an id
-        if flow.flow_id is not None:
-            flow_id = flow.flow_id
-
+    res = _run_task_get_arffcontent(
+        flow=flow,
+        model=flow.model,
+        task=task,
+        extension=flow.extension,
+        add_local_measures=add_local_measures,
+    )
 
     data_content, trace, fold_evaluations, sample_evaluations = res
-    if not isinstance(flow.flow_id, int):
-        # This is the usual behaviour, where the flow object was initiated off
-        # line and requires some additional information (flow_id, input_id for
-        # each hyperparameter) to be usable by this library
-        server_flow = get_flow(flow_id)
-        openml.flows.flow._copy_server_fields(server_flow, flow)
-        openml.flows.assert_flows_equal(flow, server_flow,
-                                        ignore_parameter_values=True)
-    else:
-        # This can only happen when the function is called directly, and not
-        # through "run_model_on_task"
-        if flow.flow_id != flow_id:
-            # This should never happen, unless user made a flow-creation fault
-            raise ValueError(
-                "Result from API call flow_exists and flow.flow_id are not "
-                "same: '%s' vs '%s'" % (str(flow.flow_id), str(flow_id))
-            )
 
     run = OpenMLRun(
         task_id=task.task_id,
-        flow_id=flow.flow_id,
+        flow_id=flow_id,
         dataset_id=dataset.dataset_id,
         model=flow.model,
         flow_name=flow.name,
         tags=tags,
         trace=trace,
         data_content=data_content,
+        flow=flow,
+        setup_string=flow.extension.create_setup_string(flow.model),
     )
-    # TODO: currently hard-coded sklearn assumption.
-    run.parameter_settings = openml.flows.obtain_parameter_values(flow)
+
+    if (upload_flow or avoid_duplicate_runs) and flow.flow_id is not None:
+        # We only extract the parameter settings if a sync happened with the server.
+        # I.e. when the flow was uploaded or we found it in the avoid_duplicate check.
+        # Otherwise, we will do this at upload time.
+        run.parameter_settings = flow.extension.obtain_parameter_values(flow)
 
     # now we need to attach the detailed evaluations
-    if task.task_type_id == 3:
+    if task.task_type_id == TaskTypeEnum.LEARNING_CURVE:
         run.sample_evaluations = sample_evaluations
     else:
         run.fold_evaluations = fold_evaluations
 
-    config.logger.info('Executed Task %d with Flow id: %d' % (task.task_id, run.flow_id))
+    if flow_id:
+        message = 'Executed Task {} with Flow id:{}'.format(task.task_id, run.flow_id)
+    else:
+        message = 'Executed Task {} on local Flow with name {}.'.format(task.task_id, flow.name)
+    config.logger.info(message)
 
     return run
 
 
-def _publish_flow_if_necessary(flow):
-    # try publishing the flow if one has to assume it doesn't exist yet. It
-    # might fail because it already exists, then the flow is currently not
-    # reused
-    try:
-        flow.publish()
-    except OpenMLServerException as e:
-        if e.message == "flow already exists":
-            # TODO: JvR: the following lines of code can be replaced by
-            # a pass (after changing the unit tests) as run_flow_on_task does
-            # not longer rely on it
-            flow_id = openml.flows.flow_exists(flow.name,
-                                               flow.external_version)
-            server_flow = get_flow(flow_id)
-            openml.flows.flow._copy_server_fields(server_flow, flow)
-            openml.flows.assert_flows_equal(flow, server_flow,
-                                            ignore_parameter_values=True)
-        else:
-            raise e
-
-
-def get_run_trace(run_id):
+def get_run_trace(run_id: int) -> OpenMLRunTrace:
     """
     Get the optimization trace object for a given run id.
 
     Parameters
     ----------
     run_id : int
 
     Returns
     -------
     openml.runs.OpenMLTrace
     """
-    trace_xml = openml._api_calls._perform_api_call('run/trace/%d' % run_id)
+    trace_xml = openml._api_calls._perform_api_call('run/trace/%d' % run_id,
+                                                    'get')
     run_trace = OpenMLRunTrace.trace_from_xml(trace_xml)
     return run_trace
 
 
-def initialize_model_from_run(run_id):
+def initialize_model_from_run(run_id: int) -> Any:
     """
     Initialized a model based on a run_id (i.e., using the exact
     same parameter settings)
 
     Parameters
-        ----------
-        run_id : int
-            The Openml run_id
-
-        Returns
-        -------
-        model : sklearn model
-            the scikitlearn model with all parameters initailized
+    ----------
+    run_id : int
+        The Openml run_id
+
+    Returns
+    -------
+    model
     """
     run = get_run(run_id)
     return initialize_model(run.setup_id)
 
 
-def initialize_model_from_trace(run_id, repeat, fold, iteration=None):
+def initialize_model_from_trace(
+    run_id: int,
+    repeat: int,
+    fold: int,
+    iteration: Optional[int] = None,
+) -> Any:
     """
     Initialize a model based on the parameters that were set
     by an optimization procedure (i.e., using the exact same
     parameter settings)
 
     Parameters
     ----------
     run_id : int
         The Openml run_id. Should contain a trace file,
         otherwise a OpenMLServerException is raised
 
-    repeat: int
+    repeat : int
         The repeat nr (column in trace file)
 
-    fold: int
+    fold : int
         The fold nr (column in trace file)
 
-    iteration: int
+    iteration : int
         The iteration nr (column in trace file). If None, the
         best (selected) iteration will be searched (slow),
         according to the selection criteria implemented in
         OpenMLRunTrace.get_selected_iteration
 
     Returns
     -------
-    model : sklearn model
-        the scikit-learn model with all parameters initailized
+    model
     """
+    run = get_run(run_id)
+    flow = get_flow(run.flow_id)
     run_trace = get_run_trace(run_id)
 
     if iteration is None:
         iteration = run_trace.get_selected_iteration(repeat, fold)
 
     request = (repeat, fold, iteration)
     if request not in run_trace.trace_iterations:
-        raise ValueError('Combination repeat, fold, iteration not availavle')
+        raise ValueError('Combination repeat, fold, iteration not available')
     current = run_trace.trace_iterations[(repeat, fold, iteration)]
 
     search_model = initialize_model_from_run(run_id)
-    if not isinstance(search_model, sklearn.model_selection._search.BaseSearchCV):
-        raise ValueError('Deserialized flow not instance of ' \
-                         'sklearn.model_selection._search.BaseSearchCV')
-    base_estimator = search_model.estimator
-    base_estimator.set_params(**current.get_parameters())
-    return base_estimator
+    model = flow.extension.instantiate_model_from_hpo_class(search_model, current)
+    return model
 
 
-def _run_exists(task_id, setup_id):
-    """Checks whether a task/setup combination is already present on the server.
+def run_exists(task_id: int, setup_id: int) -> Set[int]:
+    """Checks whether a task/setup combination is already present on the
+    server.
 
     Parameters
     ----------
-    task_id: int
+    task_id : int
 
-    setup_id: int
+    setup_id : int
 
     Returns
     -------
         Set run ids for runs where flow setup_id was run on task_id. Empty
         set if it wasn't run yet.
     """
     if setup_id <= 0:
@@ -304,409 +364,178 @@
     try:
         result = list_runs(task=[task_id], setup=[setup_id])
         if len(result) > 0:
             return set(result.keys())
         else:
             return set()
     except OpenMLServerException as exception:
-        # error code 512 implies no results. This means the run does not exist yet
-        assert(exception.code == 512)
+        # error code 512 implies no results. The run does not exist yet
+        assert (exception.code == 512)
         return set()
 
 
-def _get_seeded_model(model, seed=None):
-    """Sets all the non-seeded components of a model with a seed.
-       Models that are already seeded will maintain the seed. In
-       this case, only integer seeds are allowed (An exception
-       is thrown when a RandomState was used as seed)
-
-        Parameters
-        ----------
-        model : sklearn model
-            The model to be seeded
-        seed : int
-            The seed to initialize the RandomState with. Unseeded subcomponents
-            will be seeded with a random number from the RandomState.
-
-        Returns
-        -------
-        model : sklearn model
-            a version of the model where all (sub)components have
-            a seed
-    """
-
-    def _seed_current_object(current_value):
-        if isinstance(current_value, int):  # acceptable behaviour
-            return False
-        elif isinstance(current_value, np.random.RandomState):
-            raise ValueError(
-                'Models initialized with a RandomState object are not supported. Please seed with an integer. ')
-        elif current_value is not None:
-            raise ValueError(
-                'Models should be seeded with int or None (this should never happen). ')
-        else:
-            return True
-
-    rs = np.random.RandomState(seed)
-    model_params = model.get_params()
-    random_states = {}
-    for param_name in sorted(model_params):
-        if 'random_state' in param_name:
-            currentValue = model_params[param_name]
-            # important to draw the value at this point (and not in the if statement)
-            # this way we guarantee that if a different set of subflows is seeded,
-            # the same number of the random generator is used
-            newValue = rs.randint(0, 2**16)
-            if _seed_current_object(currentValue):
-                random_states[param_name] = newValue
-
-        # Also seed CV objects!
-        elif isinstance(model_params[param_name],
-                        sklearn.model_selection.BaseCrossValidator):
-            if not hasattr(model_params[param_name], 'random_state'):
-                continue
-
-            currentValue = model_params[param_name].random_state
-            newValue = rs.randint(0, 2 ** 16)
-            if _seed_current_object(currentValue):
-                model_params[param_name].random_state = newValue
-
-    model.set_params(**random_states)
-    return model
-
-
-def _prediction_to_row(rep_no, fold_no, sample_no, row_id, correct_label,
-                       predicted_label, predicted_probabilities, class_labels,
-                       model_classes_mapping):
-    """Util function that turns probability estimates of a classifier for a given
-        instance into the right arff format to upload to openml.
-
-        Parameters
-        ----------
-        rep_no : int
-            The repeat of the experiment (0-based; in case of 1 time CV, always 0)
-        fold_no : int
-            The fold nr of the experiment (0-based; in case of holdout, always 0)
-        sample_no : int
-            In case of learning curves, the index of the subsample (0-based; in case of no learning curve, always 0)
-        row_id : int
-            row id in the initial dataset
-        correct_label : str
-            original label of the instance
-        predicted_label : str
-            the label that was predicted
-        predicted_probabilities : array (size=num_classes)
-            probabilities per class
-        class_labels : array (size=num_classes)
-        model_classes_mapping : list
-            A list of classes the model produced.
-            Obtained by BaseEstimator.classes_
-
-        Returns
-        -------
-        arff_line : list
-            representation of the current prediction in OpenML format
-        """
-    if not isinstance(rep_no, (int, np.integer)): raise ValueError('rep_no should be int')
-    if not isinstance(fold_no, (int, np.integer)): raise ValueError('fold_no should be int')
-    if not isinstance(sample_no, (int, np.integer)): raise ValueError('sample_no should be int')
-    if not isinstance(row_id, (int, np.integer)): raise ValueError('row_id should be int')
-    if not len(predicted_probabilities) == len(model_classes_mapping):
-        raise ValueError('len(predicted_probabilities) != len(class_labels)')
-
-    arff_line = [rep_no, fold_no, sample_no, row_id]
-    for class_label_idx in range(len(class_labels)):
-        if class_label_idx in model_classes_mapping:
-            index = np.where(model_classes_mapping == class_label_idx)[0][0]  # TODO: WHY IS THIS 2D???
-            arff_line.append(predicted_probabilities[index])
-        else:
-            arff_line.append(0.0)
-
-    arff_line.append(class_labels[predicted_label])
-    arff_line.append(correct_label)
-    return arff_line
-
-
-def _run_task_get_arffcontent(model, task, add_local_measures):
-
-    def _prediction_to_probabilities(y, model_classes):
-        # y: list or numpy array of predictions
-        # model_classes: sklearn classifier mapping from original array id to prediction index id
-        if not isinstance(model_classes, list):
-            raise ValueError('please convert model classes to list prior to calling this fn')
-        result = np.zeros((len(y), len(model_classes)), dtype=np.float32)
-        for obs, prediction_idx in enumerate(y):
-            array_idx = model_classes.index(prediction_idx)
-            result[obs][array_idx] = 1.0
-        return result
-
-    arff_datacontent = []
-    arff_tracecontent = []
+def _run_task_get_arffcontent(
+    flow: OpenMLFlow,
+    model: Any,
+    task: OpenMLTask,
+    extension: 'Extension',
+    add_local_measures: bool,
+) -> Tuple[
+    List[List],
+    Optional[OpenMLRunTrace],
+    'OrderedDict[str, OrderedDict]',
+    'OrderedDict[str, OrderedDict]',
+]:
+    arff_datacontent = []  # type: List[List]
+    traces = []  # type: List[OpenMLRunTrace]
     # stores fold-based evaluation measures. In case of a sample based task,
     # this information is multiple times overwritten, but due to the ordering
     # of tne loops, eventually it contains the information based on the full
     # dataset size
-    user_defined_measures_per_fold = collections.OrderedDict()
+    user_defined_measures_per_fold = OrderedDict()  # type: 'OrderedDict[str, OrderedDict]'
     # stores sample-based evaluation measures (sublevel of fold-based)
     # will also be filled on a non sample-based task, but the information
     # is the same as the fold-based measures, and disregarded in that case
-    user_defined_measures_per_sample = collections.OrderedDict()
+    user_defined_measures_per_sample = OrderedDict()  # type: 'OrderedDict[str, OrderedDict]'
 
-    # sys.version_info returns a tuple, the following line compares the entry of tuples
-    # https://docs.python.org/3.6/reference/expressions.html#value-comparisons
-    can_measure_runtime = sys.version_info[:2] >= (3, 3) and _check_n_jobs(model)
     # TODO use different iterator to only provide a single iterator (less
     # methods, less maintenance, less confusion)
     num_reps, num_folds, num_samples = task.get_split_dimensions()
 
-    for rep_no in range(num_reps):
-        for fold_no in range(num_folds):
-            for sample_no in range(num_samples):
-                model_fold = sklearn.base.clone(model, safe=True)
-                res = _run_model_on_fold(model_fold, task, rep_no, fold_no, sample_no,
-                                         can_measure_runtime=can_measure_runtime,
-                                         add_local_measures=add_local_measures)
-                arff_datacontent_fold, arff_tracecontent_fold, user_defined_measures_fold, model_fold = res
-
-                arff_datacontent.extend(arff_datacontent_fold)
-                arff_tracecontent.extend(arff_tracecontent_fold)
-
-                for measure in user_defined_measures_fold:
-
-                    if measure not in user_defined_measures_per_fold:
-                        user_defined_measures_per_fold[measure] = collections.OrderedDict()
-                    if rep_no not in user_defined_measures_per_fold[measure]:
-                        user_defined_measures_per_fold[measure][rep_no] = collections.OrderedDict()
-
-                    if measure not in user_defined_measures_per_sample:
-                        user_defined_measures_per_sample[measure] = collections.OrderedDict()
-                    if rep_no not in user_defined_measures_per_sample[measure]:
-                        user_defined_measures_per_sample[measure][rep_no] = collections.OrderedDict()
-                    if fold_no not in user_defined_measures_per_sample[measure][rep_no]:
-                        user_defined_measures_per_sample[measure][rep_no][fold_no] = collections.OrderedDict()
-
-                    user_defined_measures_per_fold[measure][rep_no][fold_no] = user_defined_measures_fold[measure]
-                    user_defined_measures_per_sample[measure][rep_no][fold_no][sample_no] = user_defined_measures_fold[measure]
-
-    # Note that we need to use a fitted model (i.e., model_fold, and not model) here,
-    # to ensure it contains the hyperparameter data (in cv_results_)
-    if isinstance(model_fold, sklearn.model_selection._search.BaseSearchCV):
-        # arff_tracecontent is already set
-        arff_trace_attributes = _extract_arfftrace_attributes(model_fold)
-        trace = OpenMLRunTrace.generate(
-            arff_trace_attributes,
-            arff_tracecontent,
+    for n_fit, (rep_no, fold_no, sample_no) in enumerate(itertools.product(
+        range(num_reps),
+        range(num_folds),
+        range(num_samples),
+    ), start=1):
+
+        train_indices, test_indices = task.get_train_test_split_indices(
+            repeat=rep_no, fold=fold_no, sample=sample_no)
+        if isinstance(task, OpenMLSupervisedTask):
+            x, y = task.get_X_and_y(dataset_format='array')
+            train_x = x[train_indices]
+            train_y = y[train_indices]
+            test_x = x[test_indices]
+            test_y = y[test_indices]
+        elif isinstance(task, OpenMLClusteringTask):
+            x = task.get_X(dataset_format='array')
+            train_x = x[train_indices]
+            train_y = None
+            test_x = None
+            test_y = None
+        else:
+            raise NotImplementedError(task.task_type)
+
+        config.logger.info(
+            "Going to execute flow '%s' on task %d for repeat %d fold %d sample %d.",
+            flow.name, task.task_id, rep_no, fold_no, sample_no,
+        )
+
+        (
+            pred_y,
+            proba_y,
+            user_defined_measures_fold,
+            trace,
+        ) = extension._run_model_on_fold(
+            model=model,
+            task=task,
+            X_train=train_x,
+            y_train=train_y,
+            rep_no=rep_no,
+            fold_no=fold_no,
+            X_test=test_x,
         )
+        if trace is not None:
+            traces.append(trace)
+
+        # add client-side calculated metrics. These is used on the server as
+        # consistency check, only useful for supervised tasks
+        def _calculate_local_measure(sklearn_fn, openml_name):
+            user_defined_measures_fold[openml_name] = sklearn_fn(test_y, pred_y)
+
+        if isinstance(task, (OpenMLClassificationTask, OpenMLLearningCurveTask)):
+
+            for i, tst_idx in enumerate(test_indices):
+
+                arff_line = [rep_no, fold_no, sample_no, tst_idx]  # type: List[Any]
+                if task.class_labels is not None:
+                    for j, class_label in enumerate(task.class_labels):
+                        arff_line.append(proba_y[i][j])
+
+                    arff_line.append(task.class_labels[pred_y[i]])
+                    arff_line.append(task.class_labels[test_y[i]])
+                else:
+                    raise ValueError('The task has no class labels')
+
+                arff_datacontent.append(arff_line)
+
+            if add_local_measures:
+                _calculate_local_measure(
+                    sklearn.metrics.accuracy_score,
+                    'predictive_accuracy',
+                )
+
+        elif isinstance(task, OpenMLRegressionTask):
+
+            for i in range(0, len(test_indices)):
+                arff_line = [rep_no, fold_no, test_indices[i], pred_y[i], test_y[i]]
+                arff_datacontent.append(arff_line)
+
+            if add_local_measures:
+                _calculate_local_measure(
+                    sklearn.metrics.mean_absolute_error,
+                    'mean_absolute_error',
+                )
+
+        elif isinstance(task, OpenMLClusteringTask):
+            for i in range(0, len(test_indices)):
+                arff_line = [test_indices[i], pred_y[i]]  # row_id, cluster ID
+                arff_datacontent.append(arff_line)
+
+        else:
+            raise TypeError(type(task))
+
+        for measure in user_defined_measures_fold:
+
+            if measure not in user_defined_measures_per_fold:
+                user_defined_measures_per_fold[measure] = OrderedDict()
+            if rep_no not in user_defined_measures_per_fold[measure]:
+                user_defined_measures_per_fold[measure][rep_no] = OrderedDict()
+
+            if measure not in user_defined_measures_per_sample:
+                user_defined_measures_per_sample[measure] = OrderedDict()
+            if rep_no not in user_defined_measures_per_sample[measure]:
+                user_defined_measures_per_sample[measure][rep_no] = OrderedDict()
+            if fold_no not in user_defined_measures_per_sample[measure][rep_no]:
+                user_defined_measures_per_sample[measure][rep_no][fold_no] = OrderedDict()
+
+            user_defined_measures_per_fold[measure][rep_no][fold_no] = (
+                user_defined_measures_fold[measure]
+            )
+            user_defined_measures_per_sample[measure][rep_no][fold_no][sample_no] = (
+                user_defined_measures_fold[measure]
+            )
+
+    if len(traces) > 0:
+        if len(traces) != n_fit:
+            raise ValueError(
+                'Did not find enough traces (expected {}, found {})'.format(n_fit, len(traces))
+            )
+        else:
+            trace = OpenMLRunTrace.merge_traces(traces)
     else:
         trace = None
 
     return (
         arff_datacontent,
         trace,
         user_defined_measures_per_fold,
         user_defined_measures_per_sample,
     )
 
 
-def _run_model_on_fold(model, task, rep_no, fold_no, sample_no, can_measure_runtime, add_local_measures):
-    """Internal function that executes a model on a fold (and possibly
-       subsample) of the dataset. It returns the data that is necessary
-       to construct the OpenML Run object (potentially over more than
-       one folds). Is used by run_task_get_arff_content. Do not use this
-       function unless you know what you are doing.
-
-        Parameters
-        ----------
-        model : sklearn model
-            The UNTRAINED model to run
-        task : OpenMLTask
-            The task to run the model on
-        rep_no : int
-            The repeat of the experiment (0-based; in case of 1 time CV,
-            always 0)
-        fold_no : int
-            The fold nr of the experiment (0-based; in case of holdout,
-            always 0)
-        sample_no : int
-            In case of learning curves, the index of the subsample (0-based;
-            in case of no learning curve, always 0)
-        can_measure_runtime : bool
-            Wether we are allowed to measure runtime (requires: Single node
-            computation and Python >= 3.3)
-        add_local_measures : bool
-            Determines whether to calculate a set of measures (i.e., predictive
-            accuracy) locally, to later verify server behaviour
-
-        Returns
-        -------
-        arff_datacontent : List[List]
-            Arff representation (list of lists) of the predictions that were
-            generated by this fold (for putting in predictions.arff)
-        arff_tracecontent :  List[List]
-            Arff representation (list of lists) of the trace data that was
-            generated by this fold (for putting in trace.arff)
-        user_defined_measures : Dict[float]
-            User defined measures that were generated on this fold
-        model : sklearn model
-            The model trained on this fold
-    """
-    def _prediction_to_probabilities(y, model_classes):
-        # y: list or numpy array of predictions
-        # model_classes: sklearn classifier mapping from original array id to prediction index id
-        if not isinstance(model_classes, list):
-            raise ValueError('please convert model classes to list prior to calling this fn')
-        result = np.zeros((len(y), len(model_classes)), dtype=np.float32)
-        for obs, prediction_idx in enumerate(y):
-            array_idx = model_classes.index(prediction_idx)
-            result[obs][array_idx] = 1.0
-        return result
-
-    # TODO: if possible, give a warning if model is already fitted (acceptable in case of custom experimentation,
-    # but not desirable if we want to upload to OpenML).
-
-    train_indices, test_indices = task.get_train_test_split_indices(repeat=rep_no,
-                                                                    fold=fold_no,
-                                                                    sample=sample_no)
-
-    X, Y = task.get_X_and_y()
-    trainX = X[train_indices]
-    trainY = Y[train_indices]
-    testX = X[test_indices]
-    testY = Y[test_indices]
-    user_defined_measures = collections.OrderedDict()
-
-    try:
-        # for measuring runtime. Only available since Python 3.3
-        if can_measure_runtime:
-            modelfit_starttime = time.process_time()
-        model.fit(trainX, trainY)
-
-        if can_measure_runtime:
-            modelfit_duration = (time.process_time() - modelfit_starttime) * 1000
-            user_defined_measures['usercpu_time_millis_training'] = modelfit_duration
-    except AttributeError as e:
-        # typically happens when training a regressor on classification task
-        raise PyOpenMLError(str(e))
-
-    # extract trace, if applicable
-    arff_tracecontent = []
-    if isinstance(model, sklearn.model_selection._search.BaseSearchCV):
-        arff_tracecontent.extend(_extract_arfftrace(model, rep_no, fold_no))
-
-    # search for model classes_ (might differ depending on modeltype)
-    # first, pipelines are a special case (these don't have a classes_
-    # object, but rather borrows it from the last step. We do this manually,
-    # because of the BaseSearch check)
-    if isinstance(model, sklearn.pipeline.Pipeline):
-        used_estimator = model.steps[-1][-1]
-    else:
-        used_estimator = model
-
-    if isinstance(used_estimator, sklearn.model_selection._search.BaseSearchCV):
-        model_classes = used_estimator.best_estimator_.classes_
-    else:
-        model_classes = used_estimator.classes_
-
-    if can_measure_runtime:
-        modelpredict_starttime = time.process_time()
-
-    PredY = model.predict(testX)
-    try:
-        ProbaY = model.predict_proba(testX)
-    except AttributeError:
-        ProbaY = _prediction_to_probabilities(PredY, list(model_classes))
-
-    if can_measure_runtime:
-        modelpredict_duration = (time.process_time() - modelpredict_starttime) * 1000
-        user_defined_measures['usercpu_time_millis_testing'] = modelpredict_duration
-        user_defined_measures['usercpu_time_millis'] = modelfit_duration + modelpredict_duration
-
-    if ProbaY.shape[1] != len(task.class_labels):
-        warnings.warn("Repeat %d Fold %d: estimator only predicted for %d/%d classes!" % (rep_no, fold_no, ProbaY.shape[1], len(task.class_labels)))
-
-    # add client-side calculated metrics. These might be used on the server as consistency check
-    def _calculate_local_measure(sklearn_fn, openml_name):
-        user_defined_measures[openml_name] = sklearn_fn(testY, PredY)
-
-    if add_local_measures:
-        _calculate_local_measure(sklearn.metrics.accuracy_score, 'predictive_accuracy')
-
-    arff_datacontent = []
-    for i in range(0, len(test_indices)):
-        arff_line = _prediction_to_row(rep_no, fold_no, sample_no,
-                                       test_indices[i], task.class_labels[testY[i]],
-                                       PredY[i], ProbaY[i], task.class_labels, model_classes)
-        arff_datacontent.append(arff_line)
-    return arff_datacontent, arff_tracecontent, user_defined_measures, model
-
-
-def _extract_arfftrace(model, rep_no, fold_no):
-    if not isinstance(model, sklearn.model_selection._search.BaseSearchCV):
-        raise ValueError('model should be instance of'\
-                         ' sklearn.model_selection._search.BaseSearchCV')
-    if not hasattr(model, 'cv_results_'):
-        raise ValueError('model should contain `cv_results_`')
-
-    arff_tracecontent = []
-    for itt_no in range(0, len(model.cv_results_['mean_test_score'])):
-        # we use the string values for True and False, as it is defined in this way by the OpenML server
-        selected = 'false'
-        if itt_no == model.best_index_:
-            selected = 'true'
-        test_score = model.cv_results_['mean_test_score'][itt_no]
-        arff_line = [rep_no, fold_no, itt_no, test_score, selected]
-        for key in model.cv_results_:
-            if key.startswith('param_'):
-                value = model.cv_results_[key][itt_no]
-                if value is not np.ma.masked:
-                    serialized_value = json.dumps(value)
-                else:
-                    serialized_value = np.nan
-                arff_line.append(serialized_value)
-        arff_tracecontent.append(arff_line)
-    return arff_tracecontent
-
-
-def _extract_arfftrace_attributes(model):
-    if not isinstance(model, sklearn.model_selection._search.BaseSearchCV):
-        raise ValueError('model should be instance of'\
-                         ' sklearn.model_selection._search.BaseSearchCV')
-    if not hasattr(model, 'cv_results_'):
-        raise ValueError('model should contain `cv_results_`')
-
-    # attributes that will be in trace arff, regardless of the model
-    trace_attributes = [('repeat', 'NUMERIC'),
-                        ('fold', 'NUMERIC'),
-                        ('iteration', 'NUMERIC'),
-                        ('evaluation', 'NUMERIC'),
-                        ('selected', ['true', 'false'])]
-
-    # model dependent attributes for trace arff
-    for key in model.cv_results_:
-        if key.startswith('param_'):
-            # supported types should include all types, including bool, int float
-            supported_basic_types = (bool, int, float, six.string_types)
-            for param_value in model.cv_results_[key]:
-                if isinstance(param_value, supported_basic_types) or param_value is None or param_value is np.ma.masked:
-                    # basic string values
-                    type = 'STRING'
-                elif isinstance(param_value, list) and all(isinstance(i, int) for i in param_value):
-                    # list of integers
-                    type = 'STRING'
-                else:
-                    raise TypeError('Unsupported param type in param grid: %s' %key)
-
-            # we renamed the attribute param to parameter, as this is a required
-            # OpenML convention - this also guards against name collisions
-            # with the required trace attributes
-            attribute = (openml.runs.trace.PREFIX + key[6:], type)
-            trace_attributes.append(attribute)
-    return trace_attributes
-
-
 def get_runs(run_ids):
     """Gets all runs in run_ids list.
 
     Parameters
     ----------
     run_ids : list of ints
 
@@ -718,160 +547,188 @@
 
     runs = []
     for run_id in run_ids:
         runs.append(get_run(run_id))
     return runs
 
 
-def get_run(run_id):
+@openml.utils.thread_safe_if_oslo_installed
+def get_run(run_id: int, ignore_cache: bool = False) -> OpenMLRun:
     """Gets run corresponding to run_id.
 
     Parameters
     ----------
     run_id : int
 
+    ignore_cache : bool
+        Whether to ignore the cache. If ``true`` this will download and overwrite the run xml
+        even if the requested run is already cached.
+
+    ignore_cache
+
     Returns
     -------
     run : OpenMLRun
         Run corresponding to ID, fetched from the server.
     """
-    run_dir = openml.utils._create_cache_directory_for_id(RUNS_CACHE_DIR_NAME, run_id)
+    run_dir = openml.utils._create_cache_directory_for_id(RUNS_CACHE_DIR_NAME,
+                                                          run_id)
     run_file = os.path.join(run_dir, "description.xml")
 
     if not os.path.exists(run_dir):
         os.makedirs(run_dir)
 
     try:
-        return _get_cached_run(run_id)
+        if not ignore_cache:
+            return _get_cached_run(run_id)
+        else:
+            raise OpenMLCacheException(message='dummy')
 
-    except (OpenMLCacheException):
-        run_xml = openml._api_calls._perform_api_call("run/%d" % run_id)
+    except OpenMLCacheException:
+        run_xml = openml._api_calls._perform_api_call("run/%d" % run_id, 'get')
         with io.open(run_file, "w", encoding='utf8') as fh:
             fh.write(run_xml)
 
     run = _create_run_from_xml(run_xml)
 
     return run
 
 
 def _create_run_from_xml(xml, from_server=True):
     """Create a run object from xml returned from server.
 
     Parameters
     ----------
-    run_xml : string
+    xml : string
         XML describing a run.
 
+    from_server : bool, optional (default=True)
+        If True, an AttributeError is raised if any of the fields required by the server is not
+        present in the xml. If False, those absent fields will be treated as None.
+
     Returns
     -------
     run : OpenMLRun
         New run object representing run_xml.
     """
 
     def obtain_field(xml_obj, fieldname, from_server, cast=None):
-        # this function can be used to check whether a field is present in an object.
-        # if it is not present, either returns None or throws an error (this is
-        # usually done if the xml comes from the server)
+        # this function can be used to check whether a field is present in an
+        # object. if it is not present, either returns None or throws an error
+        # (this is usually done if the xml comes from the server)
         if fieldname in xml_obj:
             if cast is not None:
                 return cast(xml_obj[fieldname])
             return xml_obj[fieldname]
         elif not from_server:
             return None
         else:
-            raise AttributeError('Run XML does not contain required (server) field: ', fieldname)
+            raise AttributeError('Run XML does not contain required (server) '
+                                 'field: ', fieldname)
 
-    run = xmltodict.parse(xml, force_list=['oml:file', 'oml:evaluation', 'oml:parameter_setting'])["oml:run"]
+    run = xmltodict.parse(xml, force_list=['oml:file', 'oml:evaluation',
+                                           'oml:parameter_setting'])["oml:run"]
     run_id = obtain_field(run, 'oml:run_id', from_server, cast=int)
     uploader = obtain_field(run, 'oml:uploader', from_server, cast=int)
     uploader_name = obtain_field(run, 'oml:uploader_name', from_server)
     task_id = int(run['oml:task_id'])
     task_type = obtain_field(run, 'oml:task_type', from_server)
 
     # even with the server requirement this field may be empty.
     if 'oml:task_evaluation_measure' in run:
         task_evaluation_measure = run['oml:task_evaluation_measure']
     else:
         task_evaluation_measure = None
 
-    flow_id = int(run['oml:flow_id'])
+    if not from_server and run['oml:flow_id'] is None:
+        # This can happen for a locally stored run of which the flow is not yet published.
+        flow_id = None
+        parameters = None
+    else:
+        flow_id = obtain_field(run, 'oml:flow_id', from_server, cast=int)
+        # parameters are only properly formatted once the flow is established on the server.
+        # thus they are also not stored for runs with local flows.
+        parameters = []
+        if 'oml:parameter_setting' in run:
+            obtained_parameter_settings = run['oml:parameter_setting']
+            for parameter_dict in obtained_parameter_settings:
+                current_parameter = OrderedDict()
+                current_parameter['oml:name'] = parameter_dict['oml:name']
+                current_parameter['oml:value'] = parameter_dict['oml:value']
+                if 'oml:component' in parameter_dict:
+                    current_parameter['oml:component'] = \
+                        parameter_dict['oml:component']
+                parameters.append(current_parameter)
+
     flow_name = obtain_field(run, 'oml:flow_name', from_server)
     setup_id = obtain_field(run, 'oml:setup_id', from_server, cast=int)
     setup_string = obtain_field(run, 'oml:setup_string', from_server)
 
-    parameters = []
-    if 'oml:parameter_setting' in run:
-        obtained_parameter_settings = run['oml:parameter_setting']
-        for parameter_dict in obtained_parameter_settings:
-            current_parameter = collections.OrderedDict()
-            current_parameter['oml:name'] = parameter_dict['oml:name']
-            current_parameter['oml:value'] = parameter_dict['oml:value']
-            if 'oml:component' in parameter_dict:
-                current_parameter['oml:component'] = parameter_dict['oml:component']
-            parameters.append(current_parameter)
-
     if 'oml:input_data' in run:
         dataset_id = int(run['oml:input_data']['oml:dataset']['oml:did'])
     elif not from_server:
         dataset_id = None
 
-    files = collections.OrderedDict()
-    evaluations = collections.OrderedDict()
-    fold_evaluations = collections.OrderedDict()
-    sample_evaluations = collections.OrderedDict()
+    files = OrderedDict()
+    evaluations = OrderedDict()
+    fold_evaluations = OrderedDict()
+    sample_evaluations = OrderedDict()
     if 'oml:output_data' not in run:
         if from_server:
-            raise ValueError('Run does not contain output_data (OpenML server error?)')
+            raise ValueError('Run does not contain output_data '
+                             '(OpenML server error?)')
     else:
         output_data = run['oml:output_data']
         if 'oml:file' in output_data:
             # multiple files, the normal case
             for file_dict in output_data['oml:file']:
-                    files[file_dict['oml:name']] = int(file_dict['oml:file_id'])
+                files[file_dict['oml:name']] = int(file_dict['oml:file_id'])
         if 'oml:evaluation' in output_data:
             # in normal cases there should be evaluations, but in case there
             # was an error these could be absent
             for evaluation_dict in output_data['oml:evaluation']:
                 key = evaluation_dict['oml:name']
                 if 'oml:value' in evaluation_dict:
                     value = float(evaluation_dict['oml:value'])
                 elif 'oml:array_data' in evaluation_dict:
                     value = evaluation_dict['oml:array_data']
                 else:
-                    raise ValueError('Could not find keys "value" or "array_data" '
-                                     'in %s' % str(evaluation_dict.keys()))
-                if '@repeat' in evaluation_dict and '@fold' in evaluation_dict and '@sample' in evaluation_dict:
+                    raise ValueError('Could not find keys "value" or '
+                                     '"array_data" in %s' %
+                                     str(evaluation_dict.keys()))
+                if '@repeat' in evaluation_dict and '@fold' in \
+                        evaluation_dict and '@sample' in evaluation_dict:
                     repeat = int(evaluation_dict['@repeat'])
                     fold = int(evaluation_dict['@fold'])
                     sample = int(evaluation_dict['@sample'])
                     if key not in sample_evaluations:
-                        sample_evaluations[key] = collections.OrderedDict()
+                        sample_evaluations[key] = OrderedDict()
                     if repeat not in sample_evaluations[key]:
-                        sample_evaluations[key][repeat] = collections.OrderedDict()
+                        sample_evaluations[key][repeat] = OrderedDict()
                     if fold not in sample_evaluations[key][repeat]:
-                        sample_evaluations[key][repeat][fold] = collections.OrderedDict()
+                        sample_evaluations[key][repeat][fold] = OrderedDict()
                     sample_evaluations[key][repeat][fold][sample] = value
                 elif '@repeat' in evaluation_dict and '@fold' in evaluation_dict:
                     repeat = int(evaluation_dict['@repeat'])
                     fold = int(evaluation_dict['@fold'])
                     if key not in fold_evaluations:
-                        fold_evaluations[key] = collections.OrderedDict()
+                        fold_evaluations[key] = OrderedDict()
                     if repeat not in fold_evaluations[key]:
-                        fold_evaluations[key][repeat] = collections.OrderedDict()
+                        fold_evaluations[key][repeat] = OrderedDict()
                     fold_evaluations[key][repeat][fold] = value
                 else:
                     evaluations[key] = value
 
     if 'description' not in files and from_server is True:
         raise ValueError('No description file for run %d in run '
                          'description XML' % run_id)
 
     if 'predictions' not in files and from_server is True:
         task = openml.tasks.get_task(task_id)
-        if task.task_type_id == 8:
+        if task.task_type_id == TaskTypeEnum.SUBGROUP_DISCOVERY:
             raise NotImplementedError(
                 'Subgroup discovery tasks are not yet supported.'
             )
         else:
             # JvR: actually, I am not sure whether this error should be raised.
             # a run can consist without predictions. But for now let's keep it
             # Matthias: yes, it should stay as long as we do not really handle
@@ -891,17 +748,14 @@
                      dataset_id=dataset_id, output_files=files,
                      evaluations=evaluations,
                      fold_evaluations=fold_evaluations,
                      sample_evaluations=sample_evaluations,
                      tags=tags)
 
 
-
-
-
 def _get_cached_run(run_id):
     """Load a run from the cache."""
     run_cache_dir = openml.utils._create_cache_directory_for_id(
         RUNS_CACHE_DIR_NAME, run_id,
     )
     try:
         run_file = os.path.join(run_cache_dir, "description.xml")
@@ -910,17 +764,27 @@
         return run
 
     except (OSError, IOError):
         raise OpenMLCacheException("Run file for run id %d not "
                                    "cached" % run_id)
 
 
-def list_runs(offset=None, size=None, id=None, task=None, setup=None,
-              flow=None, uploader=None, tag=None, display_errors=False, **kwargs):
-
+def list_runs(
+    offset: Optional[int] = None,
+    size: Optional[int] = None,
+    id: Optional[List] = None,
+    task: Optional[List[int]] = None,
+    setup: Optional[List] = None,
+    flow: Optional[List] = None,
+    uploader: Optional[List] = None,
+    tag: Optional[str] = None,
+    display_errors: bool = False,
+    output_format: str = 'dict',
+    **kwargs
+) -> Union[Dict, pd.DataFrame]:
     """
     List all runs matching all of the given filters.
     (Supports large amount of results)
 
     Parameters
     ----------
     offset : int, optional
@@ -940,30 +804,65 @@
 
     tag : str, optional
 
     display_errors : bool, optional (default=None)
         Whether to list runs which have an error (for example a missing
         prediction file).
 
-    kwargs: dict, optional
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
+
+    kwargs : dict, optional
         Legal filter operators: task_type.
 
     Returns
     -------
-    dict
-        List of found runs.
+    dict of dicts, or dataframe
     """
-
-    return openml.utils._list_all(_list_runs, offset=offset, size=size, id=id, task=task, setup=setup,
-                                  flow=flow, uploader=uploader, tag=tag, display_errors=display_errors, **kwargs)
-
-
-def _list_runs(id=None, task=None, setup=None,
-               flow=None, uploader=None, display_errors=False, **kwargs):
-
+    if output_format not in ['dataframe', 'dict']:
+        raise ValueError("Invalid output format selected. "
+                         "Only 'dict' or 'dataframe' applicable.")
+
+    if id is not None and (not isinstance(id, list)):
+        raise TypeError('id must be of type list.')
+    if task is not None and (not isinstance(task, list)):
+        raise TypeError('task must be of type list.')
+    if setup is not None and (not isinstance(setup, list)):
+        raise TypeError('setup must be of type list.')
+    if flow is not None and (not isinstance(flow, list)):
+        raise TypeError('flow must be of type list.')
+    if uploader is not None and (not isinstance(uploader, list)):
+        raise TypeError('uploader must be of type list.')
+
+    return openml.utils._list_all(output_format=output_format,
+                                  listing_call=_list_runs,
+                                  offset=offset,
+                                  size=size,
+                                  id=id,
+                                  task=task,
+                                  setup=setup,
+                                  flow=flow,
+                                  uploader=uploader,
+                                  tag=tag,
+                                  display_errors=display_errors,
+                                  **kwargs)
+
+
+def _list_runs(
+    id: Optional[List] = None,
+    task: Optional[List] = None,
+    setup: Optional[List] = None,
+    flow: Optional[List] = None,
+    uploader: Optional[List] = None,
+    display_errors: bool = False,
+    output_format: str = 'dict',
+    **kwargs
+) -> Union[Dict, pd.DataFrame]:
     """
     Perform API call `/run/list/{filters}'
     <https://www.openml.org/api_docs/#!/run/get_run_list_filters>`
 
     Parameters
     ----------
     The arguments that are lists are separated from the single value
@@ -981,20 +880,25 @@
 
     uploader : list, optional
 
     display_errors : bool, optional (default=None)
         Whether to list runs which have an error (for example a missing
         prediction file).
 
-    kwargs: dict, optional
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
+
+    kwargs : dict, optional
         Legal filter operators: task_type.
 
     Returns
     -------
-    dict
+    dict, or dataframe
         List of found runs.
     """
 
     api_call = "run/list"
     if kwargs is not None:
         for operator, value in kwargs.items():
             api_call += "/%s/%s" % (operator, value)
@@ -1006,20 +910,20 @@
         api_call += "/setup/%s" % ','.join([str(int(i)) for i in setup])
     if flow is not None:
         api_call += "/flow/%s" % ','.join([str(int(i)) for i in flow])
     if uploader is not None:
         api_call += "/uploader/%s" % ','.join([str(int(i)) for i in uploader])
     if display_errors:
         api_call += "/show_errors/true"
-    return __list_runs(api_call)
+    return __list_runs(api_call=api_call, output_format=output_format)
 
 
-def __list_runs(api_call):
+def __list_runs(api_call, output_format='dict'):
     """Helper function to parse API calls which are lists of runs"""
-    xml_string = openml._api_calls._perform_api_call(api_call)
+    xml_string = openml._api_calls._perform_api_call(api_call, 'get')
     runs_dict = xmltodict.parse(xml_string, force_list=('oml:run',))
     # Minimalistic check if the XML is useful
     if 'oml:runs' not in runs_dict:
         raise ValueError('Error in return XML, does not contain "oml:runs": %s'
                          % str(runs_dict))
     elif '@xmlns:oml' not in runs_dict['oml:runs']:
         raise ValueError('Error in return XML, does not contain '
@@ -1030,19 +934,24 @@
                          '"oml:runs"/@xmlns:oml is not '
                          '"http://openml.org/openml": %s'
                          % str(runs_dict))
 
     assert type(runs_dict['oml:runs']['oml:run']) == list, \
         type(runs_dict['oml:runs'])
 
-    runs = collections.OrderedDict()
+    runs = OrderedDict()
     for run_ in runs_dict['oml:runs']['oml:run']:
         run_id = int(run_['oml:run_id'])
         run = {'run_id': run_id,
                'task_id': int(run_['oml:task_id']),
                'setup_id': int(run_['oml:setup_id']),
                'flow_id': int(run_['oml:flow_id']),
-               'uploader': int(run_['oml:uploader'])}
+               'uploader': int(run_['oml:uploader']),
+               'upload_time': str(run_['oml:upload_time']),
+               'error_message': str((run_['oml:error_message']) or '')}
 
         runs[run_id] = run
 
+    if output_format == 'dataframe':
+        runs = pd.DataFrame.from_dict(runs, orient='index')
+
     return runs
```

### Comparing `openml-0.8.0/openml/runs/run.py` & `openml-0.9.0/openml/runs/run.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from collections import OrderedDict
-import errno
-import json
 import pickle
-import sys
 import time
-import numpy as np
+from typing import Any, IO, TextIO  # noqa F401
+import os
 
 import arff
-import os
+import numpy as np
 import xmltodict
 
 import openml
 import openml._api_calls
-from ..tasks import get_task
 from ..exceptions import PyOpenMLError
+from ..flows import get_flow
+from ..tasks import (get_task,
+                     TaskTypeEnum,
+                     OpenMLClassificationTask,
+                     OpenMLLearningCurveTask,
+                     OpenMLClusteringTask,
+                     OpenMLRegressionTask
+                     )
+from ..utils import _tag_entity
 
 
 class OpenMLRun(object):
     """OpenML Run: result of running a model on an openml dataset.
 
-    Parameters
-    ----------
-    FIXME
-
+       Parameters
+       ----------
+       task_id : int
+           Refers to the task.
+       flow_id : int
+           Refers to the flow.
+       dataset_id: int
+           Refers to the data.
     """
+
     def __init__(self, task_id, flow_id, dataset_id, setup_string=None,
-                 output_files=None, setup_id=None, tags=None, uploader=None, uploader_name=None,
-                 evaluations=None, fold_evaluations=None, sample_evaluations=None,
-                 data_content=None, trace=None,
-                 model=None, task_type=None, task_evaluation_measure=None, flow_name=None,
-                 parameter_settings=None, predictions_url=None, task=None,
-                 flow=None, run_id=None):
+                 output_files=None, setup_id=None, tags=None, uploader=None,
+                 uploader_name=None, evaluations=None, fold_evaluations=None,
+                 sample_evaluations=None, data_content=None, trace=None,
+                 model=None, task_type=None, task_evaluation_measure=None,
+                 flow_name=None, parameter_settings=None, predictions_url=None,
+                 task=None, flow=None, run_id=None):
         self.uploader = uploader
         self.uploader_name = uploader_name
         self.task_id = task_id
         self.task_type = task_type
         self.task_evaluation_measure = task_evaluation_measure
         self.flow_id = flow_id
         self.flow_name = flow_name
@@ -64,269 +75,392 @@
         return "[run id: {}, task id: {}, flow id: {}, flow name: {}]".format(
             self.run_id, self.task_id, self.flow_id, flow_name)
 
     def _repr_pretty_(self, pp, cycle):
         pp.text(str(self))
 
     @classmethod
-    def from_filesystem(cls, folder, expect_model=True):
+    def from_filesystem(cls, directory: str, expect_model: bool = True) -> 'OpenMLRun':
         """
         The inverse of the to_filesystem method. Instantiates an OpenMLRun
         object based on files stored on the file system.
 
         Parameters
         ----------
-        folder : str
+        directory : str
             a path leading to the folder where the results
             are stored
 
         expect_model : bool
             if True, it requires the model pickle to be present, and an error
             will be thrown if not. Otherwise, the model might or might not
             be present.
 
         Returns
         -------
         run : OpenMLRun
             the re-instantiated run object
         """
-        if not os.path.isdir(folder):
+
+        # Avoiding cyclic imports
+        import openml.runs.functions
+
+        if not os.path.isdir(directory):
             raise ValueError('Could not find folder')
 
-        description_path = os.path.join(folder, 'description.xml')
-        predictions_path = os.path.join(folder, 'predictions.arff')
-        trace_path = os.path.join(folder, 'trace.arff')
-        model_path = os.path.join(folder, 'model.pkl')
+        description_path = os.path.join(directory, 'description.xml')
+        predictions_path = os.path.join(directory, 'predictions.arff')
+        trace_path = os.path.join(directory, 'trace.arff')
+        model_path = os.path.join(directory, 'model.pkl')
 
         if not os.path.isfile(description_path):
             raise ValueError('Could not find description.xml')
         if not os.path.isfile(predictions_path):
             raise ValueError('Could not find predictions.arff')
         if not os.path.isfile(model_path) and expect_model:
             raise ValueError('Could not find model.pkl')
 
-        with open(description_path, 'r') as fp:
-            xml_string = fp.read()
-            run = openml.runs.functions._create_run_from_xml(xml_string, from_server=False)
+        with open(description_path, 'r') as fht:
+            xml_string = fht.read()
+        run = openml.runs.functions._create_run_from_xml(xml_string, from_server=False)
+
+        if run.flow_id is None:
+            flow = openml.flows.OpenMLFlow.from_filesystem(directory)
+            run.flow = flow
+            run.flow_name = flow.name
 
-        with open(predictions_path, 'r') as fp:
-            predictions = arff.load(fp)
+        with open(predictions_path, 'r') as fht:
+            predictions = arff.load(fht)
             run.data_content = predictions['data']
 
         if os.path.isfile(model_path):
-            # note that it will load the model if the file exists, even if expect_model is False
-            with open(model_path, 'rb') as fp:
-                run.model = pickle.load(fp)
+            # note that it will load the model if the file exists, even if
+            # expect_model is False
+            with open(model_path, 'rb') as fhb:
+                run.model = pickle.load(fhb)
 
         if os.path.isfile(trace_path):
             run.trace = openml.runs.OpenMLRunTrace._from_filesystem(trace_path)
 
         return run
 
-    def to_filesystem(self, output_directory, store_model=True):
+    def to_filesystem(
+        self,
+        directory: str,
+        store_model: bool = True,
+    ) -> None:
         """
         The inverse of the from_filesystem method. Serializes a run
         on the filesystem, to be uploaded later.
 
         Parameters
         ----------
-        output_directory : str
+        directory : str
             a path leading to the folder where the results
             will be stored. Should be empty
 
-        store_model : bool
+        store_model : bool, optional (default=True)
             if True, a model will be pickled as well. As this is the most
             storage expensive part, it is often desirable to not store the
             model.
         """
         if self.data_content is None or self.model is None:
-            raise ValueError('Run should have been executed (and contain model / predictions)')
-
-        try:
-            os.makedirs(output_directory)
-        except OSError as e:
-            if e.errno == errno.EEXIST:
-                pass
-            else:
-                raise e
+            raise ValueError('Run should have been executed (and contain '
+                             'model / predictions)')
 
-        if not os.listdir(output_directory) == []:
-            raise ValueError('Output directory should be empty')
+        os.makedirs(directory, exist_ok=True)
+        if not os.listdir(directory) == []:
+            raise ValueError(
+                'Output directory {} should be empty'.format(os.path.abspath(directory))
+            )
 
         run_xml = self._create_description_xml()
         predictions_arff = arff.dumps(self._generate_arff_dict())
 
-        with open(os.path.join(output_directory, 'description.xml'), 'w') as f:
-            f.write(run_xml)
-        with open(os.path.join(output_directory, 'predictions.arff'), 'w') as f:
-            f.write(predictions_arff)
+        # It seems like typing does not allow to define the same variable multiple times
+        with open(os.path.join(directory, 'description.xml'), 'w') as fh:  # type: TextIO
+            fh.write(run_xml)
+        with open(os.path.join(directory, 'predictions.arff'), 'w') as fh:
+            fh.write(predictions_arff)
         if store_model:
-            with open(os.path.join(output_directory, 'model.pkl'), 'wb') as f:
-                pickle.dump(self.model, f)
+            with open(os.path.join(directory, 'model.pkl'), 'wb') as fh_b:  # type: IO[bytes]
+                pickle.dump(self.model, fh_b)
+
+        if self.flow_id is None:
+            self.flow.to_filesystem(directory)
 
         if self.trace is not None:
-            self.trace._to_filesystem(output_directory)
+            self.trace._to_filesystem(directory)
 
-    def _generate_arff_dict(self):
-        """Generates the arff dictionary for uploading predictions to the server.
+    def _generate_arff_dict(self) -> 'OrderedDict[str, Any]':
+        """Generates the arff dictionary for uploading predictions to the
+        server.
 
         Assumes that the run has been executed.
 
         Returns
         -------
         arf_dict : dict
             Dictionary representation of the ARFF file that will be uploaded.
             Contains predictions and information about the run environment.
         """
         if self.data_content is None:
             raise ValueError('Run has not been executed.')
+        if self.flow is None:
+            self.flow = get_flow(self.flow_id)
 
-        run_environment = (_get_version_information() +
-                           [time.strftime("%c")] + ['Created by run_task()'])
+        run_environment = (self.flow.extension.get_version_information()
+                           + [time.strftime("%c")]
+                           + ['Created by run_task()'])
         task = get_task(self.task_id)
-        class_labels = task.class_labels
 
-        arff_dict = OrderedDict()
-        arff_dict['attributes'] = [('repeat', 'NUMERIC'),  # lowercase 'numeric' gives an error
-                                   ('fold', 'NUMERIC'),
-                                   ('sample', 'NUMERIC'),
-                                   ('row_id', 'NUMERIC')] + \
-            [('confidence.' + class_labels[i], 'NUMERIC') for i in range(len(class_labels))] +\
-            [('prediction', class_labels),
-             ('correct', class_labels)]
+        arff_dict = OrderedDict()  # type: 'OrderedDict[str, Any]'
         arff_dict['data'] = self.data_content
         arff_dict['description'] = "\n".join(run_environment)
-        arff_dict['relation'] = 'openml_task_' + str(task.task_id) + '_predictions'
+        arff_dict['relation'] =\
+            'openml_task_{}_predictions'.format(task.task_id)
+
+        if isinstance(task, OpenMLLearningCurveTask):
+            class_labels = task.class_labels
+            instance_specifications = [
+                ('repeat', 'NUMERIC'),
+                ('fold', 'NUMERIC'),
+                ('sample', 'NUMERIC'),
+                ('row_id', 'NUMERIC')
+            ]
+
+            arff_dict['attributes'] = instance_specifications
+            if class_labels is not None:
+                arff_dict['attributes'] = arff_dict['attributes'] + \
+                    [('confidence.' + class_labels[i],
+                      'NUMERIC')
+                     for i in range(len(class_labels))] + \
+                    [('prediction', class_labels),
+                     ('correct', class_labels)]
+            else:
+                raise ValueError('The task has no class labels')
+
+        elif isinstance(task, OpenMLClassificationTask):
+            class_labels = task.class_labels
+            instance_specifications = [('repeat', 'NUMERIC'),
+                                       ('fold', 'NUMERIC'),
+                                       ('sample', 'NUMERIC'),  # Legacy
+                                       ('row_id', 'NUMERIC')]
+
+            arff_dict['attributes'] = instance_specifications
+            if class_labels is not None:
+                prediction_confidences = [('confidence.' + class_labels[i],
+                                           'NUMERIC')
+                                          for i in range(len(class_labels))]
+                prediction_and_true = [('prediction', class_labels),
+                                       ('correct', class_labels)]
+                arff_dict['attributes'] = arff_dict['attributes'] + \
+                    prediction_confidences + \
+                    prediction_and_true
+            else:
+                raise ValueError('The task has no class labels')
+
+        elif isinstance(task, OpenMLRegressionTask):
+            arff_dict['attributes'] = [('repeat', 'NUMERIC'),
+                                       ('fold', 'NUMERIC'),
+                                       ('row_id', 'NUMERIC'),
+                                       ('prediction', 'NUMERIC'),
+                                       ('truth', 'NUMERIC')]
+
+        elif isinstance(task, OpenMLClusteringTask):
+            arff_dict['attributes'] = [('repeat', 'NUMERIC'),
+                                       ('fold', 'NUMERIC'),
+                                       ('row_id', 'NUMERIC'),
+                                       ('cluster', 'NUMERIC')]
+
+        else:
+            raise NotImplementedError(
+                'Task type %s is not yet supported.' % str(task.task_type)
+            )
+
         return arff_dict
 
-    def get_metric_fn(self, sklearn_fn, kwargs={}):
+    def get_metric_fn(self, sklearn_fn, kwargs=None):
         """Calculates metric scores based on predicted values. Assumes the
         run has been executed locally (and contains run_data). Furthermore,
-        it assumes that the 'correct' attribute is specified in the arff
-        (which is an optional field, but always the case for openml-python
-        runs)
+        it assumes that the 'correct' or 'truth' attribute is specified in
+        the arff (which is an optional field, but always the case for
+        openml-python runs)
 
         Parameters
         ----------
         sklearn_fn : function
             a function pointer to a sklearn function that
             accepts ``y_true``, ``y_pred`` and ``**kwargs``
 
         Returns
         -------
         scores : list
             a list of floats, of length num_folds * num_repeats
         """
+        kwargs = kwargs if kwargs else dict()
         if self.data_content is not None and self.task_id is not None:
             predictions_arff = self._generate_arff_dict()
         elif 'predictions' in self.output_files:
             predictions_file_url = openml._api_calls._file_id_to_url(
                 self.output_files['predictions'], 'predictions.arff',
             )
-            predictions_arff = arff.loads(openml._api_calls._read_url(predictions_file_url))
+            response = openml._api_calls._read_url(predictions_file_url,
+                                                   request_method='get')
+            predictions_arff = arff.loads(response)
             # TODO: make this a stream reader
         else:
-            raise ValueError('Run should have been locally executed or contain outputfile reference.')
+            raise ValueError('Run should have been locally executed or '
+                             'contain outputfile reference.')
+
+        # Need to know more about the task to compute scores correctly
+        task = get_task(self.task_id)
 
         attribute_names = [att[0] for att in predictions_arff['attributes']]
-        if 'correct' not in attribute_names:
-            raise ValueError('Attribute "correct" should be set')
-        if 'prediction' not in attribute_names:
-            raise ValueError('Attribute "predict" should be set')
+        if (task.task_type_id in [TaskTypeEnum.SUPERVISED_CLASSIFICATION,
+                                  TaskTypeEnum.LEARNING_CURVE]
+                and 'correct' not in attribute_names):
+            raise ValueError('Attribute "correct" should be set for '
+                             'classification task runs')
+        if (task.task_type_id == TaskTypeEnum.SUPERVISED_REGRESSION
+                and 'truth' not in attribute_names):
+            raise ValueError('Attribute "truth" should be set for '
+                             'regression task runs')
+        if (task.task_type_id != TaskTypeEnum.CLUSTERING
+                and 'prediction' not in attribute_names):
+            raise ValueError('Attribute "predict" should be set for '
+                             'supervised task runs')
 
         def _attribute_list_to_dict(attribute_list):
-            # convenience function: Creates a mapping to map from the name of attributes
-            # present in the arff prediction file to their index. This is necessary
-            # because the number of classes can be different for different tasks.
+            # convenience function: Creates a mapping to map from the name of
+            # attributes present in the arff prediction file to their index.
+            # This is necessary because the number of classes can be different
+            # for different tasks.
             res = OrderedDict()
             for idx in range(len(attribute_list)):
                 res[attribute_list[idx][0]] = idx
             return res
-        attribute_dict = _attribute_list_to_dict(predictions_arff['attributes'])
 
-        # might throw KeyError!
-        predicted_idx = attribute_dict['prediction']
-        correct_idx = attribute_dict['correct']
+        attribute_dict = \
+            _attribute_list_to_dict(predictions_arff['attributes'])
+
         repeat_idx = attribute_dict['repeat']
         fold_idx = attribute_dict['fold']
-        sample_idx = attribute_dict['sample'] # TODO: this one might be zero
+        predicted_idx = attribute_dict['prediction']  # Assume supervised task
+
+        if task.task_type_id == TaskTypeEnum.SUPERVISED_CLASSIFICATION or \
+                task.task_type_id == TaskTypeEnum.LEARNING_CURVE:
+            correct_idx = attribute_dict['correct']
+        elif task.task_type_id == TaskTypeEnum.SUPERVISED_REGRESSION:
+            correct_idx = attribute_dict['truth']
+        has_samples = False
+        if 'sample' in attribute_dict:
+            sample_idx = attribute_dict['sample']
+            has_samples = True
 
-        if predictions_arff['attributes'][predicted_idx][1] != predictions_arff['attributes'][correct_idx][1]:
+        if predictions_arff['attributes'][predicted_idx][1] != \
+                predictions_arff['attributes'][correct_idx][1]:
             pred = predictions_arff['attributes'][predicted_idx][1]
             corr = predictions_arff['attributes'][correct_idx][1]
-            raise ValueError('Predicted and Correct do not have equal values: %s Vs. %s' %(str(pred), str(corr)))
+            raise ValueError('Predicted and Correct do not have equal values:'
+                             ' %s Vs. %s' % (str(pred), str(corr)))
 
         # TODO: these could be cached
         values_predict = {}
         values_correct = {}
         for line_idx, line in enumerate(predictions_arff['data']):
             rep = line[repeat_idx]
             fold = line[fold_idx]
-            samp = line[sample_idx]
+            if has_samples:
+                samp = line[sample_idx]
+            else:
+                samp = 0  # No learning curve sample, always 0
 
-            # TODO: can be sped up bt preprocessing index, but OK for now.
-            prediction = predictions_arff['attributes'][predicted_idx][1].index(line[predicted_idx])
-            correct = predictions_arff['attributes'][predicted_idx][1].index(line[correct_idx])
+            if task.task_type_id in [TaskTypeEnum.SUPERVISED_CLASSIFICATION,
+                                     TaskTypeEnum.LEARNING_CURVE]:
+                prediction = predictions_arff['attributes'][predicted_idx][
+                    1].index(line[predicted_idx])
+                correct = predictions_arff['attributes'][predicted_idx][1]. \
+                    index(line[correct_idx])
+            elif task.task_type_id == TaskTypeEnum.SUPERVISED_REGRESSION:
+                prediction = line[predicted_idx]
+                correct = line[correct_idx]
             if rep not in values_predict:
                 values_predict[rep] = OrderedDict()
                 values_correct[rep] = OrderedDict()
             if fold not in values_predict[rep]:
                 values_predict[rep][fold] = OrderedDict()
                 values_correct[rep][fold] = OrderedDict()
             if samp not in values_predict[rep][fold]:
                 values_predict[rep][fold][samp] = []
                 values_correct[rep][fold][samp] = []
 
-            values_predict[line[repeat_idx]][line[fold_idx]][line[sample_idx]].append(prediction)
-            values_correct[line[repeat_idx]][line[fold_idx]][line[sample_idx]].append(correct)
+            values_predict[rep][fold][samp].append(prediction)
+            values_correct[rep][fold][samp].append(correct)
 
         scores = []
         for rep in values_predict.keys():
             for fold in values_predict[rep].keys():
                 last_sample = len(values_predict[rep][fold]) - 1
                 y_pred = values_predict[rep][fold][last_sample]
                 y_true = values_correct[rep][fold][last_sample]
                 scores.append(sklearn_fn(y_true, y_pred, **kwargs))
         return np.array(scores)
 
-    def publish(self):
-        """Publish a run to the OpenML server.
+    def publish(self) -> 'OpenMLRun':
+        """ Publish a run (and if necessary, its flow) to the OpenML server.
 
         Uploads the results of a run to OpenML.
-        Sets the run_id on self
+        If the run is of an unpublished OpenMLFlow, the flow will be uploaded too.
+        Sets the run_id on self.
 
         Returns
         -------
         self : OpenMLRun
         """
         if self.model is None:
             raise PyOpenMLError(
                 "OpenMLRun obj does not contain a model. "
                 "(This should never happen.) "
             )
         if self.flow_id is None:
-            raise PyOpenMLError(
-                "OpenMLRun obj does not contain a flow id. "
-                "(Should have been added while executing the task.) "
+            if self.flow is None:
+                raise PyOpenMLError(
+                    "OpenMLRun object does not contain a flow id or reference to OpenMLFlow "
+                    "(these should have been added while executing the task). "
+                )
+            else:
+                # publish the linked Flow before publishing the run.
+                self.flow.publish()
+                self.flow_id = self.flow.flow_id
+
+        if self.parameter_settings is None:
+            if self.flow is None:
+                self.flow = openml.flows.get_flow(self.flow_id)
+            self.parameter_settings = self.flow.extension.obtain_parameter_values(
+                self.flow,
+                self.model,
             )
 
         description_xml = self._create_description_xml()
         file_elements = {'description': ("description.xml", description_xml)}
 
         if self.error_message is None:
             predictions = arff.dumps(self._generate_arff_dict())
             file_elements['predictions'] = ("predictions.arff", predictions)
 
         if self.trace is not None:
             trace_arff = arff.dumps(self.trace.trace_to_arff())
             file_elements['trace'] = ("trace.arff", trace_arff)
 
-        return_value = openml._api_calls._perform_api_call("/run/", file_elements=file_elements)
-        run_id = int(xmltodict.parse(return_value)['oml:upload_run']['oml:run_id'])
-        self.run_id = run_id
+        return_value = openml._api_calls._perform_api_call(
+            "/run/", 'post', file_elements=file_elements
+        )
+        result = xmltodict.parse(return_value)
+        self.run_id = int(result['oml:upload_run']['oml:run_id'])
         return self
 
     def _create_description_xml(self):
         """Create xml representation of run for upload.
 
         Returns
         -------
@@ -337,128 +471,103 @@
         # as a tag, it must be of the form ([a-zA-Z0-9_\-\.])+
         # so we format time from 'mm/dd/yy hh:mm:ss' to 'mm-dd-yy_hh.mm.ss'
         # well_formatted_time = time.strftime("%c").replace(
         #     ' ', '_').replace('/', '-').replace(':', '.')
         # tags = run_environment + [well_formatted_time] + ['run_task'] + \
         #     [self.model.__module__ + "." + self.model.__class__.__name__]
         description = _to_dict(taskid=self.task_id, flow_id=self.flow_id,
-                               setup_string=_create_setup_string(self.model),
+                               setup_string=self.setup_string,
                                parameter_settings=self.parameter_settings,
                                error_message=self.error_message,
                                fold_evaluations=self.fold_evaluations,
                                sample_evaluations=self.sample_evaluations,
                                tags=self.tags)
         description_xml = xmltodict.unparse(description, pretty=True)
         return description_xml
 
-    def push_tag(self, tag):
+    def push_tag(self, tag: str) -> None:
         """Annotates this run with a tag on the server.
 
         Parameters
         ----------
         tag : str
             Tag to attach to the run.
         """
-        data = {'run_id': self.run_id, 'tag': tag}
-        openml._api_calls._perform_api_call("/run/tag", data=data)
+        _tag_entity('run', self.run_id, tag)
 
-    def remove_tag(self, tag):
+    def remove_tag(self, tag: str) -> None:
         """Removes a tag from this run on the server.
 
         Parameters
         ----------
         tag : str
             Tag to attach to the run.
         """
-        data = {'run_id': self.run_id, 'tag': tag}
-        openml._api_calls._perform_api_call("/run/untag", data=data)
+        _tag_entity('run', self.run_id, tag, untag=True)
 
 
-################################################################################
+###############################################################################
 # Functions which cannot be in runs/functions due to circular imports
 
-
-# This can possibly be done by a package such as pyxb, but I could not get
-# it to work properly.
-def _get_version_information():
-    """Gets versions of python, sklearn, numpy and scipy, returns them in an array,
-
-    Returns
-    -------
-    result : an array with version information of the above packages
-    """
-    import sklearn
-    import scipy
-    import numpy
-
-    major, minor, micro, _, _ = sys.version_info
-    python_version = 'Python_{}.'.format(
-        ".".join([str(major), str(minor), str(micro)]))
-    sklearn_version = 'Sklearn_{}.'.format(sklearn.__version__)
-    numpy_version = 'NumPy_{}.'.format(numpy.__version__)
-    scipy_version = 'SciPy_{}.'.format(scipy.__version__)
-
-    return [python_version, sklearn_version, numpy_version, scipy_version]
-
-
 def _to_dict(taskid, flow_id, setup_string, error_message, parameter_settings,
              tags=None, fold_evaluations=None, sample_evaluations=None):
     """ Creates a dictionary corresponding to the desired xml desired by openML
 
     Parameters
     ----------
     taskid : int
         the identifier of the task
     setup_string : string
-        a CLI string which can invoke the learning with the correct parameter settings
+        a CLI string which can invoke the learning with the correct parameter
+        settings
     parameter_settings : array of dicts
-        each dict containing keys name, value and component, one per parameter setting
+        each dict containing keys name, value and component, one per parameter
+        setting
     tags : array of strings
         information that give a description of the run, must conform to
         regex ``([a-zA-Z0-9_\-\.])+``
-    fold_evaluations : dict mapping from evaluation measure to a dict mapping repeat_nr
-        to a dict mapping from fold nr to a value (double)
-    sample_evaluations : dict mapping from evaluation measure to a dict mapping repeat_nr
-        to a dict mapping from fold nr to a dict mapping to a sample nr to a value (double)
+    fold_evaluations : dict mapping from evaluation measure to a dict mapping
+        repeat_nr to a dict mapping from fold nr to a value (double)
+    sample_evaluations : dict mapping from evaluation measure to a dict
+        mapping repeat_nr to a dict mapping from fold nr to a dict mapping to
+        a sample nr to a value (double)
     sample_evaluations :
     Returns
     -------
     result : an array with version information of the above packages
-    """
+    """  # noqa: W605
     description = OrderedDict()
     description['oml:run'] = OrderedDict()
     description['oml:run']['@xmlns:oml'] = 'http://openml.org/openml'
     description['oml:run']['oml:task_id'] = taskid
     description['oml:run']['oml:flow_id'] = flow_id
     if error_message is not None:
         description['oml:run']['oml:error_message'] = error_message
     description['oml:run']['oml:parameter_setting'] = parameter_settings
     if tags is not None:
         description['oml:run']['oml:tag'] = tags  # Tags describing the run
     if (fold_evaluations is not None and len(fold_evaluations) > 0) or \
-       (sample_evaluations is not None and len(sample_evaluations) > 0):
+            (sample_evaluations is not None and len(sample_evaluations) > 0):
         description['oml:run']['oml:output_data'] = OrderedDict()
         description['oml:run']['oml:output_data']['oml:evaluation'] = list()
     if fold_evaluations is not None:
         for measure in fold_evaluations:
             for repeat in fold_evaluations[measure]:
                 for fold, value in fold_evaluations[measure][repeat].items():
-                    current = OrderedDict([('@repeat', str(repeat)), ('@fold', str(fold)),
-                                           ('oml:name', measure), ('oml:value', str(value))])
-                    description['oml:run']['oml:output_data']['oml:evaluation'].append(current)
+                    current = OrderedDict([
+                        ('@repeat', str(repeat)), ('@fold', str(fold)),
+                        ('oml:name', measure), ('oml:value', str(value))])
+                    description['oml:run']['oml:output_data'][
+                        'oml:evaluation'].append(current)
     if sample_evaluations is not None:
         for measure in sample_evaluations:
             for repeat in sample_evaluations[measure]:
                 for fold in sample_evaluations[measure][repeat]:
-                    for sample, value in sample_evaluations[measure][repeat][fold].items():
-                        current = OrderedDict([('@repeat', str(repeat)), ('@fold', str(fold)),
-                                               ('@sample', str(sample)), ('oml:name', measure),
-                                               ('oml:value', str(value))])
-                        description['oml:run']['oml:output_data']['oml:evaluation'].append(current)
+                    for sample, value in sample_evaluations[measure][repeat][
+                            fold].items():
+                        current = OrderedDict([
+                            ('@repeat', str(repeat)), ('@fold', str(fold)),
+                            ('@sample', str(sample)), ('oml:name', measure),
+                            ('oml:value', str(value))])
+                        description['oml:run']['oml:output_data'][
+                            'oml:evaluation'].append(current)
     return description
-
-
-def _create_setup_string(model):
-    """Create a string representing the model"""
-    run_environment = " ".join(_get_version_information())
-    # fixme str(model) might contain (...)
-    return run_environment + " " + str(model)
```

### Comparing `openml-0.8.0/openml/runs/trace.py` & `openml-0.9.0/openml/runs/trace.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import arff
+from collections import OrderedDict
 import json
 import os
+from typing import List, Tuple  # noqa F401
+
+import arff
 import xmltodict
-from collections import OrderedDict
 
 PREFIX = 'parameter_'
 REQUIRED_ATTRIBUTES = [
     'repeat',
     'fold',
     'iteration',
     'evaluation',
@@ -28,29 +30,29 @@
 
     """
 
     def __init__(self, run_id, trace_iterations):
         self.run_id = run_id
         self.trace_iterations = trace_iterations
 
-    def get_selected_iteration(self, fold, repeat):
+    def get_selected_iteration(self, fold: int, repeat: int) -> int:
         """
         Returns the trace iteration that was marked as selected. In
         case multiple are marked as selected (should not happen) the
         first of these is returned
 
         Parameters
         ----------
         fold: int
 
         repeat: int
 
         Returns
         ----------
-        OpenMLTraceIteration
+        int
             The trace iteration from the given fold and repeat that was
             selected as the best iteration by the search procedure
         """
         for (r, f, i) in self.trace_iterations:
             if (
                 r == repeat
                 and f == fold
@@ -100,15 +102,15 @@
             attributes=attributes,
             content=content,
             error_message='setup_string not allowed when constructing a '
                           'trace object from run results.'
         )
 
     @classmethod
-    def _from_filesystem(cls, file_path):
+    def _from_filesystem(cls, file_path: str) -> 'OpenMLRunTrace':
         """
         Logic to deserialize the trace from the filesystem.
 
         Parameters
         ----------
         file_path: str
             File path where the trace arff is stored.
@@ -277,15 +279,15 @@
             current = OpenMLTraceIteration(
                 repeat=repeat,
                 fold=fold,
                 iteration=iteration,
                 setup_string=None,
                 evaluation=evaluation,
                 selected=selected,
-                paramaters=parameters,
+                parameters=parameters,
             )
             trace[(repeat, fold, iteration)] = current
 
         return cls(None, trace)
 
     @classmethod
     def trace_from_xml(cls, xml):
@@ -342,20 +344,56 @@
                 evaluation,
                 selected,
             )
             trace[(repeat, fold, iteration)] = current
 
         return cls(run_id, trace)
 
+    @classmethod
+    def merge_traces(cls, traces: List['OpenMLRunTrace']) -> 'OpenMLRunTrace':
+
+        merged_trace = OrderedDict()  # type: OrderedDict[Tuple[int, int, int], OpenMLTraceIteration]  # noqa E501
+
+        previous_iteration = None
+        for trace in traces:
+            for iteration in trace:
+                key = (iteration.repeat, iteration.fold, iteration.iteration)
+                if previous_iteration is not None:
+                    if (
+                        list(merged_trace[previous_iteration].parameters.keys())
+                        != list(iteration.parameters.keys())
+                    ):
+                        raise ValueError(
+                            'Cannot merge traces because the parameters are not equal: {} vs {}'.
+                            format(
+                                list(merged_trace[previous_iteration].parameters.keys()),
+                                list(iteration.parameters.keys()),
+                            )
+                        )
+
+                if key in merged_trace:
+                    raise ValueError(
+                        "Cannot merge traces because key '{}' was encountered twice".format(key)
+                    )
+
+                merged_trace[key] = iteration
+                previous_iteration = key
+
+        return cls(None, merged_trace)
+
     def __str__(self):
-        return '[Run id: %d, %d trace iterations]' % (
-            self.run_id,
+        return '[Run id: %d, %d trace iterations]'.format(
+            -1 if self.run_id is None else self.run_id,
             len(self.trace_iterations),
         )
 
+    def __iter__(self):
+        for val in self.trace_iterations.values():
+            yield val
+
 
 class OpenMLTraceIteration(object):
     """OpenML Trace Iteration: parsed output from Run Trace call
 
     Parameters
     ----------
     repeat : int
@@ -386,42 +424,42 @@
         self,
         repeat,
         fold,
         iteration,
         setup_string,
         evaluation,
         selected,
-        paramaters=None,
+        parameters=None,
     ):
 
         if not isinstance(selected, bool):
             raise TypeError(type(selected))
-        if setup_string and paramaters:
+        if setup_string and parameters:
             raise ValueError(
                 'Can only be instantiated with either '
                 'setup_string or parameters argument.'
             )
-        elif not setup_string and not paramaters:
+        elif not setup_string and not parameters:
             raise ValueError(
                 'Either setup_string or parameters needs to be passed as '
                 'argument.'
             )
-        if paramaters is not None and not isinstance(paramaters, OrderedDict):
+        if parameters is not None and not isinstance(parameters, OrderedDict):
             raise TypeError(
                 'argument parameters is not an instance of OrderedDict, but %s'
-                % str(type(paramaters))
+                % str(type(parameters))
             )
 
         self.repeat = repeat
         self.fold = fold
         self.iteration = iteration
         self.setup_string = setup_string
         self.evaluation = evaluation
         self.selected = selected
-        self.parameters = paramaters
+        self.parameters = parameters
 
     def get_parameters(self):
         result = {}
         # parameters have prefix 'parameter_'
 
         if self.setup_string:
             for param in self.setup_string:
```

### Comparing `openml-0.8.0/openml/setups/functions.py` & `openml-0.9.0/openml/setups/functions.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from collections import OrderedDict
-
 import io
-import openml
 import os
+from typing import Any, Union, List, Dict, Optional
+
 import xmltodict
+import pandas as pd
 
+import openml
 from .. import config
 from .setup import OpenMLSetup, OpenMLParameter
 from openml.flows import flow_exists
-from openml.exceptions import OpenMLServerNoResult
+import openml.exceptions
 import openml.utils
 
 
-def setup_exists(flow):
+def setup_exists(flow) -> int:
     """
     Checks whether a hyperparameter configuration already exists on the server.
 
     Parameters
     ----------
     flow : flow
         The openml flow object. Should have flow id present for the main flow
@@ -27,29 +29,30 @@
     -------
     setup_id : int
         setup id iff exists, False otherwise
     """
     # sadly, this api call relies on a run object
     openml.flows.functions._check_flow_for_server_id(flow)
     if flow.model is None:
-        raise ValueError('Flow should have model field set with the actual '
-                         'model. ')
+        raise ValueError('Flow should have model field set with the actual model.')
+    if flow.extension is None:
+        raise ValueError('Flow should have model field set with the correct extension.')
 
     # checks whether the flow exists on the server and flow ids align
     exists = flow_exists(flow.name, flow.external_version)
     if exists != flow.flow_id:
         raise ValueError('This should not happen!')
 
-    # TODO: currently hard-coded sklearn assumption
-    openml_param_settings = openml.flows.obtain_parameter_values(flow)
+    openml_param_settings = flow.extension.obtain_parameter_values(flow)
     description = xmltodict.unparse(_to_dict(flow.flow_id,
                                              openml_param_settings),
                                     pretty=True)
     file_elements = {'description': ('description.arff', description)}
     result = openml._api_calls._perform_api_call('/setup/exists/',
+                                                 'post',
                                                  file_elements=file_elements)
     result_dict = xmltodict.parse(result)
     setup_id = int(result_dict['oml:setup_exists']['oml:id'])
     if setup_id > 0:
         return setup_id
     else:
         return False
@@ -59,206 +62,260 @@
     """Load a run from the cache."""
     cache_dir = config.get_cache_directory()
     setup_cache_dir = os.path.join(cache_dir, "setups", str(setup_id))
     try:
         setup_file = os.path.join(setup_cache_dir, "description.xml")
         with io.open(setup_file, encoding='utf8') as fh:
             setup_xml = xmltodict.parse(fh.read())
-            setup = _create_setup_from_xml(setup_xml)
+            setup = _create_setup_from_xml(setup_xml, output_format='object')
         return setup
 
     except (OSError, IOError):
-        raise openml.exceptions.OpenMLCacheException("Setup file for setup id %d not cached" % setup_id)
+        raise openml.exceptions.OpenMLCacheException(
+            "Setup file for setup id %d not cached" % setup_id)
 
 
 def get_setup(setup_id):
     """
      Downloads the setup (configuration) description from OpenML
      and returns a structured object
 
     Parameters
     ----------
     setup_id : int
         The Openml setup_id
 
     Returns
     -------
-    OpenMLSetup
-        an initialized openml setup object
+    dict or OpenMLSetup(an initialized openml setup object)
     """
-    setup_dir = os.path.join(config.get_cache_directory(), "setups", str(setup_id))
+    setup_dir = os.path.join(config.get_cache_directory(),
+                             "setups",
+                             str(setup_id))
     setup_file = os.path.join(setup_dir, "description.xml")
 
     if not os.path.exists(setup_dir):
         os.makedirs(setup_dir)
 
     try:
         return _get_cached_setup(setup_id)
-
     except (openml.exceptions.OpenMLCacheException):
-        setup_xml = openml._api_calls._perform_api_call('/setup/%d' % setup_id)
+        url_suffix = '/setup/%d' % setup_id
+        setup_xml = openml._api_calls._perform_api_call(url_suffix, 'get')
         with io.open(setup_file, "w", encoding='utf8') as fh:
             fh.write(setup_xml)
 
     result_dict = xmltodict.parse(setup_xml)
-    return _create_setup_from_xml(result_dict)
+    return _create_setup_from_xml(result_dict, output_format='object')
 
 
-def list_setups(offset=None, size=None, flow=None, tag=None, setup=None):
+def list_setups(
+    offset: Optional[int] = None,
+    size: Optional[int] = None,
+    flow: Optional[int] = None,
+    tag: Optional[str] = None,
+    setup: Optional[List] = None,
+    output_format: str = 'object'
+) -> Union[Dict, pd.DataFrame]:
     """
     List all setups matching all of the given filters.
 
     Parameters
     ----------
     offset : int, optional
     size : int, optional
     flow : int, optional
     tag : str, optional
     setup : list(int), optional
+    output_format: str, optional (default='object')
+        The parameter decides the format of the output.
+        - If 'object' the output is a dict of OpenMLSetup objects
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
 
     Returns
     -------
-    dict
-        """
-
-    return openml.utils._list_all(_list_setups, offset=offset, size=size,
-                                  flow=flow, tag=tag, setup=setup, batch_size=1000)  #batch size for setups is lower
+    dict or dataframe
+    """
+    if output_format not in ['dataframe', 'dict', 'object']:
+        raise ValueError("Invalid output format selected. "
+                         "Only 'dict', 'object', or 'dataframe' applicable.")
+
+    batch_size = 1000  # batch size for setups is lower
+    return openml.utils._list_all(output_format=output_format,
+                                  listing_call=_list_setups,
+                                  offset=offset,
+                                  size=size,
+                                  flow=flow,
+                                  tag=tag,
+                                  setup=setup,
+                                  batch_size=batch_size)
 
 
-def _list_setups(setup=None, **kwargs):
+def _list_setups(setup=None, output_format='object', **kwargs):
     """
     Perform API call `/setup/list/{filters}`
 
     Parameters
     ----------
     The setup argument that is a list is separated from the single value
     filters which are put into the kwargs.
 
     setup : list(int), optional
 
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
+
     kwargs: dict, optional
         Legal filter operators: flow, setup, limit, offset, tag.
 
     Returns
     -------
-    dict
+    dict or dataframe
         """
 
     api_call = "setup/list"
     if setup is not None:
         api_call += "/setup/%s" % ','.join([str(int(i)) for i in setup])
     if kwargs is not None:
         for operator, value in kwargs.items():
             api_call += "/%s/%s" % (operator, value)
 
-    return __list_setups(api_call)
+    return __list_setups(api_call=api_call, output_format=output_format)
 
 
-def __list_setups(api_call):
+def __list_setups(api_call, output_format='object'):
     """Helper function to parse API calls which are lists of setups"""
-    xml_string = openml._api_calls._perform_api_call(api_call)
+    xml_string = openml._api_calls._perform_api_call(api_call, 'get')
     setups_dict = xmltodict.parse(xml_string, force_list=('oml:setup',))
+    openml_uri = 'http://openml.org/openml'
     # Minimalistic check if the XML is useful
     if 'oml:setups' not in setups_dict:
-        raise ValueError('Error in return XML, does not contain "oml:setups": %s'
-                         % str(setups_dict))
+        raise ValueError('Error in return XML, does not contain "oml:setups":'
+                         ' %s' % str(setups_dict))
     elif '@xmlns:oml' not in setups_dict['oml:setups']:
         raise ValueError('Error in return XML, does not contain '
                          '"oml:setups"/@xmlns:oml: %s'
                          % str(setups_dict))
-    elif setups_dict['oml:setups']['@xmlns:oml'] != 'http://openml.org/openml':
+    elif setups_dict['oml:setups']['@xmlns:oml'] != openml_uri:
         raise ValueError('Error in return XML, value of  '
                          '"oml:seyups"/@xmlns:oml is not '
-                         '"http://openml.org/openml": %s'
-                         % str(setups_dict))
+                         '"%s": %s'
+                         % (openml_uri, str(setups_dict)))
 
     assert type(setups_dict['oml:setups']['oml:setup']) == list, \
         type(setups_dict['oml:setups'])
 
     setups = dict()
     for setup_ in setups_dict['oml:setups']['oml:setup']:
         # making it a dict to give it the right format
-        current = _create_setup_from_xml({'oml:setup_parameters': setup_})
-        setups[current.setup_id] = current
+        current = _create_setup_from_xml({'oml:setup_parameters': setup_},
+                                         output_format=output_format)
+        if output_format == 'object':
+            setups[current.setup_id] = current
+        else:
+            setups[current['setup_id']] = current
+
+    if output_format == 'dataframe':
+        setups = pd.DataFrame.from_dict(setups, orient='index')
 
     return setups
 
 
-def initialize_model(setup_id):
+def initialize_model(setup_id: int) -> Any:
     """
     Initialized a model based on a setup_id (i.e., using the exact
     same parameter settings)
 
     Parameters
     ----------
     setup_id : int
         The Openml setup_id
 
     Returns
     -------
-    model : sklearn model
-        the scikitlearn model with all parameters initialized
+    model
     """
     setup = get_setup(setup_id)
     flow = openml.flows.get_flow(setup.flow_id)
 
-    # instead of using scikit-learns "set_params" function, we override the
+    # instead of using scikit-learns or any other library's "set_params" function, we override the
     # OpenMLFlow objects default parameter value so we can utilize the
-    # flow_to_sklearn function to reinitialize the flow with the set defaults.
+    # Extension.flow_to_model() function to reinitialize the flow with the set defaults.
     for hyperparameter in setup.parameters.values():
         structure = flow.get_structure('flow_id')
         if len(structure[hyperparameter.flow_id]) > 0:
             subflow = flow.get_subflow(structure[hyperparameter.flow_id])
         else:
             subflow = flow
         subflow.parameters[hyperparameter.parameter_name] = \
             hyperparameter.value
 
-    model = openml.flows.flow_to_sklearn(flow)
+    model = flow.extension.flow_to_model(flow)
     return model
 
 
 def _to_dict(flow_id, openml_parameter_settings):
     # for convenience, this function (ab)uses the run object.
     xml = OrderedDict()
     xml['oml:run'] = OrderedDict()
     xml['oml:run']['@xmlns:oml'] = 'http://openml.org/openml'
     xml['oml:run']['oml:flow_id'] = flow_id
     xml['oml:run']['oml:parameter_setting'] = openml_parameter_settings
 
     return xml
 
 
-def _create_setup_from_xml(result_dict):
+def _create_setup_from_xml(result_dict, output_format='object'):
     """
-    Turns an API xml result into a OpenMLSetup object
+    Turns an API xml result into a OpenMLSetup object (or dict)
     """
     setup_id = int(result_dict['oml:setup_parameters']['oml:setup_id'])
     flow_id = int(result_dict['oml:setup_parameters']['oml:flow_id'])
     parameters = {}
     if 'oml:parameter' not in result_dict['oml:setup_parameters']:
         parameters = None
     else:
         # basically all others
         xml_parameters = result_dict['oml:setup_parameters']['oml:parameter']
         if isinstance(xml_parameters, dict):
             id = int(xml_parameters['oml:id'])
-            parameters[id] = _create_setup_parameter_from_xml(xml_parameters)
+            parameters[id] = _create_setup_parameter_from_xml(result_dict=xml_parameters,
+                                                              output_format=output_format)
         elif isinstance(xml_parameters, list):
             for xml_parameter in xml_parameters:
                 id = int(xml_parameter['oml:id'])
-                parameters[id] = _create_setup_parameter_from_xml(xml_parameter)
+                parameters[id] = \
+                    _create_setup_parameter_from_xml(result_dict=xml_parameter,
+                                                     output_format=output_format)
         else:
-            raise ValueError('Expected None, list or dict, received someting else: %s' %str(type(xml_parameters)))
+            raise ValueError('Expected None, list or dict, received '
+                             'something else: %s' % str(type(xml_parameters)))
 
+    if output_format in ['dataframe', 'dict']:
+        return_dict = {'setup_id': setup_id, 'flow_id': flow_id}
+        return_dict['parameters'] = parameters
+        return(return_dict)
     return OpenMLSetup(setup_id, flow_id, parameters)
 
 
-def _create_setup_parameter_from_xml(result_dict):
-    return OpenMLParameter(input_id=int(result_dict['oml:id']),
-                           flow_id=int(result_dict['oml:flow_id']),
-                           flow_name=result_dict['oml:flow_name'],
-                           full_name=result_dict['oml:full_name'],
-                           parameter_name=result_dict['oml:parameter_name'],
-                           data_type=result_dict['oml:data_type'],
-                           default_value=result_dict['oml:default_value'],
-                           value=result_dict['oml:value'])
+def _create_setup_parameter_from_xml(result_dict, output_format='object'):
+    if output_format == 'object':
+        return OpenMLParameter(input_id=int(result_dict['oml:id']),
+                               flow_id=int(result_dict['oml:flow_id']),
+                               flow_name=result_dict['oml:flow_name'],
+                               full_name=result_dict['oml:full_name'],
+                               parameter_name=result_dict['oml:parameter_name'],
+                               data_type=result_dict['oml:data_type'],
+                               default_value=result_dict['oml:default_value'],
+                               value=result_dict['oml:value'])
+    else:
+        return({'input_id': int(result_dict['oml:id']),
+                'flow_id': int(result_dict['oml:flow_id']),
+                'flow_name': result_dict['oml:flow_name'],
+                'full_name': result_dict['oml:full_name'],
+                'parameter_name': result_dict['oml:parameter_name'],
+                'data_type': result_dict['oml:data_type'],
+                'default_value': result_dict['oml:default_value'],
+                'value': result_dict['oml:value']})
```

### Comparing `openml-0.8.0/openml/setups/setup.py` & `openml-0.9.0/openml/setups/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
        ----------
        setup_id : int
             The OpenML setup id
        flow_id : int
             The flow that it is build upon
         parameters : dict
             The setting of the parameters
-           """
+    """
 
     def __init__(self, setup_id, flow_id, parameters):
         if not isinstance(setup_id, int):
             raise ValueError('setup id should be int')
         if not isinstance(flow_id, int):
             raise ValueError('flow id should be int')
         if parameters is not None:
```

### Comparing `openml-0.8.0/openml/tasks/__init__.py` & `openml-0.9.0/openml/tasks/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from .task import (
     OpenMLTask,
     OpenMLSupervisedTask,
     OpenMLClassificationTask,
     OpenMLRegressionTask,
     OpenMLClusteringTask,
     OpenMLLearningCurveTask,
+    TaskTypeEnum,
 )
 from .split import OpenMLSplit
-from .functions import (get_task, get_tasks, list_tasks)
+from .functions import (
+    create_task,
+    get_task,
+    get_tasks,
+    list_tasks,
+)
 
 __all__ = [
     'OpenMLTask',
     'OpenMLSupervisedTask',
     'OpenMLClusteringTask',
     'OpenMLRegressionTask',
     'OpenMLClassificationTask',
     'OpenMLLearningCurveTask',
+    'create_task',
     'get_task',
     'get_tasks',
     'list_tasks',
     'OpenMLSplit',
+    'TaskTypeEnum'
 ]
```

### Comparing `openml-0.8.0/openml/tasks/functions.py` & `openml-0.9.0/openml/tasks/functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from collections import OrderedDict
 import io
 import re
 import os
+from typing import Union, Dict, Optional
 
-from oslo_concurrency import lockutils
+import pandas as pd
 import xmltodict
 
 from ..exceptions import OpenMLCacheException
 from ..datasets import get_dataset
 from .task import (
     OpenMLClassificationTask,
     OpenMLClusteringTask,
     OpenMLLearningCurveTask,
+    TaskTypeEnum,
     OpenMLRegressionTask,
-    OpenMLSupervisedTask
+    OpenMLSupervisedTask,
+    OpenMLTask
 )
 import openml.utils
 import openml._api_calls
 
+
 TASKS_CACHE_DIR_NAME = 'tasks'
 
+
 def _get_cached_tasks():
     """Return a dict of all the tasks which are cached locally.
     Returns
     -------
     tasks : OrderedDict
         A dict of all the cached tasks. Each task is an instance of
         OpenMLTask.
@@ -42,16 +47,15 @@
 
         tid = int(filename)
         tasks[tid] = _get_cached_task(tid)
 
     return tasks
 
 
-
-def _get_cached_task(tid):
+def _get_cached_task(tid: int) -> OpenMLTask:
     """Return a cached task based on the given id.
 
     Parameters
     ----------
     tid : int
         Id of the task.
 
@@ -61,63 +65,76 @@
     """
     tid_cache_dir = openml.utils._create_cache_directory_for_id(
         TASKS_CACHE_DIR_NAME,
         tid
     )
 
     try:
-        with io.open(os.path.join(tid_cache_dir, "task.xml"), encoding='utf8') as fh:
+        with io.open(os.path.join(tid_cache_dir, "task.xml"), encoding='utf8')\
+                as fh:
             return _create_task_from_xml(fh.read())
     except (OSError, IOError):
-        openml.utils._remove_cache_dir_for_id(TASKS_CACHE_DIR_NAME, tid_cache_dir)
+        openml.utils._remove_cache_dir_for_id(TASKS_CACHE_DIR_NAME,
+                                              tid_cache_dir)
         raise OpenMLCacheException("Task file for tid %d not "
                                    "cached" % tid)
 
 
 def _get_estimation_procedure_list():
     """Return a list of all estimation procedures which are on OpenML.
     Returns
     -------
     procedures : list
         A list of all estimation procedures. Every procedure is represented by
         a dictionary containing the following information: id, task type id,
         name, type, repeats, folds, stratified.
     """
+    url_suffix = "estimationprocedure/list"
+    xml_string = openml._api_calls._perform_api_call(url_suffix,
+                                                     'get')
 
-    xml_string = openml._api_calls._perform_api_call("estimationprocedure/list")
     procs_dict = xmltodict.parse(xml_string)
     # Minimalistic check if the XML is useful
     if 'oml:estimationprocedures' not in procs_dict:
         raise ValueError('Error in return XML, does not contain tag '
                          'oml:estimationprocedures.')
     elif '@xmlns:oml' not in procs_dict['oml:estimationprocedures']:
         raise ValueError('Error in return XML, does not contain tag '
                          '@xmlns:oml as a child of oml:estimationprocedures.')
     elif procs_dict['oml:estimationprocedures']['@xmlns:oml'] != \
             'http://openml.org/openml':
         raise ValueError('Error in return XML, value of '
                          'oml:estimationprocedures/@xmlns:oml is not '
                          'http://openml.org/openml, but %s' %
-                         str(procs_dict['oml:estimationprocedures']['@xmlns:oml']))
+                         str(procs_dict['oml:estimationprocedures'][
+                             '@xmlns:oml']))
 
     procs = []
-    for proc_ in procs_dict['oml:estimationprocedures']['oml:estimationprocedure']:
+    for proc_ in procs_dict['oml:estimationprocedures'][
+            'oml:estimationprocedure']:
         procs.append(
             {
                 'id': int(proc_['oml:id']),
                 'task_type_id': int(proc_['oml:ttid']),
                 'name': proc_['oml:name'],
                 'type': proc_['oml:type'],
             }
         )
 
     return procs
 
 
-def list_tasks(task_type_id=None, offset=None, size=None, tag=None, **kwargs):
+def list_tasks(
+    task_type_id: Optional[int] = None,
+    offset: Optional[int] = None,
+    size: Optional[int] = None,
+    tag: Optional[str] = None,
+    output_format: str = 'dict',
+    **kwargs
+) -> Union[Dict, pd.DataFrame]:
     """
     Return a number of tasks having the given tag and task_type_id
     Parameters
     ----------
     Filter task_type_id is separated from the other filters because
     it is used as task_type_id in the task description, but it is named
     type when used as a filter in list tasks call.
@@ -134,29 +151,49 @@
         - Subgroup Discovery: 8
     offset : int, optional
         the number of tasks to skip, starting from the first
     size : int, optional
         the maximum number of tasks to show
     tag : str, optional
         the tag to include
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
     kwargs: dict, optional
-        Legal filter operators: data_tag, status, data_id, data_name, number_instances, number_features,
+        Legal filter operators: data_tag, status, data_id, data_name,
+        number_instances, number_features,
         number_classes, number_missing_values.
+
     Returns
     -------
     dict
         All tasks having the given task_type_id and the give tag. Every task is
         represented by a dictionary containing the following information:
         task id, dataset id, task_type and status. If qualities are calculated
         for the associated dataset, some of these are also returned.
+    dataframe
+        All tasks having the given task_type_id and the give tag. Every task is
+        represented by a row in the data frame containing the following information
+        as columns: task id, dataset id, task_type and status. If qualities are
+        calculated for the associated dataset, some of these are also returned.
     """
-    return openml.utils._list_all(_list_tasks, task_type_id=task_type_id, offset=offset, size=size, tag=tag, **kwargs)
+    if output_format not in ['dataframe', 'dict']:
+        raise ValueError("Invalid output format selected. "
+                         "Only 'dict' or 'dataframe' applicable.")
+    return openml.utils._list_all(output_format=output_format,
+                                  listing_call=_list_tasks,
+                                  task_type_id=task_type_id,
+                                  offset=offset,
+                                  size=size,
+                                  tag=tag,
+                                  **kwargs)
 
 
-def _list_tasks(task_type_id=None, **kwargs):
+def _list_tasks(task_type_id=None, output_format='dict', **kwargs):
     """
     Perform the api call to return a number of tasks having the given filters.
     Parameters
     ----------
     Filter task_type_id is separated from the other filters because
     it is used as task_type_id in the task description, but it is named
     type when used as a filter in list tasks call.
@@ -167,37 +204,42 @@
         - Supervised regression: 2
         - Learning curve: 3
         - Supervised data stream classification: 4
         - Clustering: 5
         - Machine Learning Challenge: 6
         - Survival Analysis: 7
         - Subgroup Discovery: 8
+    output_format: str, optional (default='dict')
+        The parameter decides the format of the output.
+        - If 'dict' the output is a dict of dict
+        - If 'dataframe' the output is a pandas DataFrame
     kwargs: dict, optional
         Legal filter operators: tag, task_id (list), data_tag, status, limit,
         offset, data_id, data_name, number_instances, number_features,
         number_classes, number_missing_values.
+
     Returns
     -------
-    dict
+    dict or dataframe
     """
     api_call = "task/list"
     if task_type_id is not None:
         api_call += "/type/%d" % int(task_type_id)
     if kwargs is not None:
         for operator, value in kwargs.items():
             if operator == 'task_id':
                 value = ','.join([str(int(i)) for i in value])
             api_call += "/%s/%s" % (operator, value)
-    return __list_tasks(api_call)
+    return __list_tasks(api_call=api_call, output_format=output_format)
 
 
-def __list_tasks(api_call):
-
-    xml_string = openml._api_calls._perform_api_call(api_call)
-    tasks_dict = xmltodict.parse(xml_string, force_list=('oml:task', 'oml:input'))
+def __list_tasks(api_call, output_format='dict'):
+    xml_string = openml._api_calls._perform_api_call(api_call, 'get')
+    tasks_dict = xmltodict.parse(xml_string, force_list=('oml:task',
+                                                         'oml:input'))
     # Minimalistic check if the XML is useful
     if 'oml:tasks' not in tasks_dict:
         raise ValueError('Error in return XML, does not contain "oml:runs": %s'
                          % str(tasks_dict))
     elif '@xmlns:oml' not in tasks_dict['oml:tasks']:
         raise ValueError('Error in return XML, does not contain '
                          '"oml:runs"/@xmlns:oml: %s'
@@ -225,93 +267,119 @@
                     'name': task_['oml:name'],
                     'task_type': task_['oml:task_type'],
                     'status': task_['oml:status']}
 
             # Other task inputs
             for input in task_.get('oml:input', list()):
                 if input['@name'] == 'estimation_procedure':
-                    task[input['@name']] = proc_dict[int(input['#text'])]['name']
+                    task[input['@name']] = \
+                        proc_dict[int(input['#text'])]['name']
                 else:
                     value = input.get('#text')
                     task[input['@name']] = value
 
             # The number of qualities can range from 0 to infinity
             for quality in task_.get('oml:quality', list()):
                 if '#text' not in quality:
                     quality_value = 0.0
                 else:
                     quality['#text'] = float(quality['#text'])
-                    if abs(int(quality['#text']) - quality['#text']) < 0.0000001:
+                    if abs(int(quality['#text']) - quality['#text']) \
+                            < 0.0000001:
                         quality['#text'] = int(quality['#text'])
                     quality_value = quality['#text']
                 task[quality['@name']] = quality_value
             tasks[tid] = task
         except KeyError as e:
             if tid is not None:
                 raise KeyError(
                     "Invalid xml for task %d: %s\nFrom %s" % (
                         tid, e, task_
                     )
                 )
             else:
                 raise KeyError('Could not find key %s in %s!' % (e, task_))
 
+    if output_format == 'dataframe':
+        tasks = pd.DataFrame.from_dict(tasks, orient='index')
+
     return tasks
 
 
-def get_tasks(task_ids):
+def get_tasks(task_ids, download_data=True):
     """Download tasks.
+
     This function iterates :meth:`openml.tasks.get_task`.
+
     Parameters
     ----------
     task_ids : iterable
-        Integers representing task ids.
+        Integers/Strings representing task ids.
+    download_data : bool
+        Option to trigger download of data along with the meta data.
+
     Returns
     -------
     list
     """
     tasks = []
     for task_id in task_ids:
-        tasks.append(get_task(task_id))
+        tasks.append(get_task(task_id, download_data))
     return tasks
 
 
-def get_task(task_id):
-    """Download the OpenML task for a given task ID.
+@openml.utils.thread_safe_if_oslo_installed
+def get_task(task_id: int, download_data: bool = True) -> OpenMLTask:
+    """Download OpenML task for a given task ID.
+
+    Downloads the task representation, while the data splits can be
+    downloaded optionally based on the additional parameter. Else,
+    splits will either way be downloaded when the task is being used.
+
     Parameters
     ----------
-    task_id : int
+    task_id : int or str
         The OpenML task id.
+    download_data : bool
+        Option to trigger download of data along with the meta data.
+
+    Returns
+    -------
+    task
     """
-    task_id = int(task_id)
+    try:
+        task_id = int(task_id)
+    except (ValueError, TypeError):
+        raise ValueError("Dataset ID is neither an Integer nor can be "
+                         "cast to an Integer.")
 
-    with lockutils.external_lock(
-            name='task.functions.get_task:%d' % task_id,
-            lock_path=openml.utils._create_lockfiles_dir(),
-    ):
-        tid_cache_dir = openml.utils._create_cache_directory_for_id(
-            TASKS_CACHE_DIR_NAME, task_id,
-        )
+    tid_cache_dir = openml.utils._create_cache_directory_for_id(
+        TASKS_CACHE_DIR_NAME, task_id,
+    )
 
-        try:
-            task = _get_task_description(task_id)
-            dataset = get_dataset(task.dataset_id)
-            # Clustering tasks do not have class labels
-            # and do not offer download_split
+    try:
+        task = _get_task_description(task_id)
+        dataset = get_dataset(task.dataset_id, download_data)
+        # List of class labels availaible in dataset description
+        # Including class labels as part of task meta data handles
+        #   the case where data download was initially disabled
+        if isinstance(task, OpenMLClassificationTask):
+            task.class_labels = \
+                dataset.retrieve_class_labels(task.target_name)
+        # Clustering tasks do not have class labels
+        # and do not offer download_split
+        if download_data:
             if isinstance(task, OpenMLSupervisedTask):
                 task.download_split()
-                if isinstance(task, OpenMLClassificationTask):
-                    task.class_labels = \
-                        dataset.retrieve_class_labels(task.target_name)
-        except Exception as e:
-            openml.utils._remove_cache_dir_for_id(
-                TASKS_CACHE_DIR_NAME,
-                tid_cache_dir,
-            )
-            raise e
+    except Exception as e:
+        openml.utils._remove_cache_dir_for_id(
+            TASKS_CACHE_DIR_NAME,
+            tid_cache_dir,
+        )
+        raise e
 
     return task
 
 
 def _get_task_description(task_id):
 
     try:
@@ -320,15 +388,16 @@
         xml_file = os.path.join(
             openml.utils._create_cache_directory_for_id(
                 TASKS_CACHE_DIR_NAME,
                 task_id,
             ),
             "task.xml",
         )
-        task_xml = openml._api_calls._perform_api_call("task/%d" % task_id)
+        task_xml = openml._api_calls._perform_api_call("task/%d" % task_id,
+                                                       'get')
 
         with io.open(xml_file, "w", encoding='utf8') as fh:
             fh.write(task_xml)
         return _create_task_from_xml(task_xml)
 
 
 def _create_task_from_xml(xml):
@@ -361,47 +430,114 @@
         inputs[name] = dic["oml:input"]
 
     evaluation_measures = None
     if 'evaluation_measures' in inputs:
         evaluation_measures = inputs["evaluation_measures"][
             "oml:evaluation_measures"]["oml:evaluation_measure"]
 
-    task_type = dic["oml:task_type"]
+    task_type_id = int(dic["oml:task_type_id"])
     common_kwargs = {
         'task_id': dic["oml:task_id"],
-        'task_type': task_type,
+        'task_type': dic["oml:task_type"],
         'task_type_id': dic["oml:task_type_id"],
         'data_set_id': inputs["source_data"][
             "oml:data_set"]["oml:data_set_id"],
         'evaluation_measure': evaluation_measures,
     }
-    if task_type in (
-        "Supervised Classification",
-        "Supervised Regression",
-        "Learning Curve"
+    if task_type_id in (
+        TaskTypeEnum.SUPERVISED_CLASSIFICATION,
+        TaskTypeEnum.SUPERVISED_REGRESSION,
+        TaskTypeEnum.LEARNING_CURVE
     ):
         # Convert some more parameters
         for parameter in \
                 inputs["estimation_procedure"]["oml:estimation_procedure"][
                     "oml:parameter"]:
             name = parameter["@name"]
             text = parameter.get("#text", "")
             estimation_parameters[name] = text
 
         common_kwargs['estimation_procedure_type'] = inputs[
             "estimation_procedure"][
             "oml:estimation_procedure"]["oml:type"]
         common_kwargs['estimation_parameters'] = estimation_parameters
         common_kwargs['target_name'] = inputs[
-                "source_data"]["oml:data_set"]["oml:target_feature"]
+            "source_data"]["oml:data_set"]["oml:target_feature"]
         common_kwargs['data_splits_url'] = inputs["estimation_procedure"][
-                "oml:estimation_procedure"]["oml:data_splits_url"]
+            "oml:estimation_procedure"]["oml:data_splits_url"]
 
     cls = {
-        "Supervised Classification": OpenMLClassificationTask,
-        "Supervised Regression": OpenMLRegressionTask,
-        "Clustering": OpenMLClusteringTask,
-        "Learning Curve": OpenMLLearningCurveTask,
-    }.get(task_type)
+        TaskTypeEnum.SUPERVISED_CLASSIFICATION: OpenMLClassificationTask,
+        TaskTypeEnum.SUPERVISED_REGRESSION: OpenMLRegressionTask,
+        TaskTypeEnum.CLUSTERING: OpenMLClusteringTask,
+        TaskTypeEnum.LEARNING_CURVE: OpenMLLearningCurveTask,
+    }.get(task_type_id)
     if cls is None:
-        raise NotImplementedError('Task type %s not supported.')
+        raise NotImplementedError('Task type %s not supported.' %
+                                  common_kwargs['task_type'])
     return cls(**common_kwargs)
+
+
+def create_task(
+        task_type_id: int,
+        dataset_id: int,
+        estimation_procedure_id: int,
+        target_name: Optional[str] = None,
+        evaluation_measure: Optional[str] = None,
+        **kwargs
+) -> Union[
+    OpenMLClassificationTask, OpenMLRegressionTask,
+    OpenMLLearningCurveTask, OpenMLClusteringTask
+]:
+    """Create a task based on different given attributes.
+
+    Builds a task object with the function arguments as
+    attributes. The type of the task object built is
+    determined from the task type id.
+    More information on how the arguments (task attributes),
+    relate to the different possible tasks can be found in
+    the individual task objects at the openml.tasks.task
+    module.
+
+    Parameters
+    ----------
+    task_type_id : int
+        Id of the task type.
+    dataset_id : int
+        The id of the dataset for the task.
+    target_name : str, optional
+        The name of the feature used as a target.
+        At the moment, only optional for the clustering tasks.
+    estimation_procedure_id : int
+        The id of the estimation procedure.
+    evaluation_measure : str, optional
+        The name of the evaluation measure.
+    kwargs : dict, optional
+        Other task attributes that are not mandatory
+        for task upload.
+
+    Returns
+    -------
+    OpenMLClassificationTask, OpenMLRegressionTask,
+    OpenMLLearningCurveTask, OpenMLClusteringTask
+    """
+    task_cls = {
+        TaskTypeEnum.SUPERVISED_CLASSIFICATION: OpenMLClassificationTask,
+        TaskTypeEnum.SUPERVISED_REGRESSION: OpenMLRegressionTask,
+        TaskTypeEnum.CLUSTERING: OpenMLClusteringTask,
+        TaskTypeEnum.LEARNING_CURVE: OpenMLLearningCurveTask,
+    }.get(task_type_id)
+
+    if task_cls is None:
+        raise NotImplementedError(
+            'Task type {0:d} not supported.'.format(task_type_id)
+        )
+    else:
+        return task_cls(
+            task_type_id=task_type_id,
+            task_type=None,
+            data_set_id=dataset_id,
+            target_name=target_name,
+            estimation_procedure_id=estimation_procedure_id,
+            evaluation_measure=evaluation_measure,
+            **kwargs
+        )
```

### Comparing `openml-0.8.0/openml/tasks/split.py` & `openml-0.9.0/openml/tasks/split.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,101 +1,110 @@
 from collections import namedtuple, OrderedDict
 import os
-import six
+import pickle
 
 import numpy as np
-import scipy.io.arff
-from six.moves import cPickle as pickle
+import arff
 
 
 Split = namedtuple("Split", ["train", "test"])
 
 
-if six.PY2:
-    FileNotFoundError = IOError
-
-
 class OpenMLSplit(object):
+    """OpenML Split object.
+
+       Parameters
+       ----------
+       name : int or str
+       description : str
+       split : dict
+    """
 
     def __init__(self, name, description, split):
         self.description = description
         self.name = name
         self.split = dict()
 
         # Add splits according to repetition
         for repetition in split:
             repetition = int(repetition)
             self.split[repetition] = OrderedDict()
             for fold in split[repetition]:
                 self.split[repetition][fold] = OrderedDict()
                 for sample in split[repetition][fold]:
-                    self.split[repetition][fold][sample] = split[repetition][fold][sample]
+                    self.split[repetition][fold][sample] = split[
+                        repetition][fold][sample]
 
         self.repeats = len(self.split)
         if any([len(self.split[0]) != len(self.split[i])
                 for i in range(self.repeats)]):
             raise ValueError('')
         self.folds = len(self.split[0])
         self.samples = len(self.split[0][0])
 
     def __eq__(self, other):
-        if type(self) != type(other):
-            return False
-        elif self.name != other.name:
+        if (type(self) != type(other)
+                or self.name != other.name
+                or self.description != other.description
+                or self.split.keys() != other.split.keys()):
             return False
-        elif self.description != other.description:
-            return False
-        elif self.split.keys() != other.split.keys():
+
+        if any(self.split[repetition].keys() != other.split[repetition].keys()
+                for repetition in self.split):
             return False
-        else:
-            for repetition in self.split:
-                if self.split[repetition].keys() != other.split[repetition].keys():
-                    return False
-                else:
-                    for fold in self.split[repetition]:
-                        for sample in self.split[repetition][fold]:
-                            if np.all(self.split[repetition][fold][sample].test !=
-                                      other.split[repetition][fold][sample].test)\
-                                    and \
-                                    np.all(self.split[repetition][fold][sample].train
-                                           != other.split[repetition][fold][sample].train):
-                                return False
+
+        samples = [(repetition, fold, sample)
+                   for repetition in self.split
+                   for fold in self.split[repetition]
+                   for sample in self.split[repetition][fold]]
+
+        for repetition, fold, sample in samples:
+            self_train, self_test = self.split[repetition][fold][sample]
+            other_train, other_test = other.split[repetition][fold][sample]
+            if not (np.all(self_train == other_train)
+                    and np.all(self_test == other_test)):
+                return False
         return True
 
     @classmethod
-    def _from_arff_file(cls, filename):
+    def _from_arff_file(cls, filename: str) -> 'OpenMLSplit':
 
         repetitions = None
 
-        if six.PY2:
-            pkl_filename = filename.replace(".arff", ".pkl.py2")
-        else:
-            pkl_filename = filename.replace(".arff", ".pkl.py3")
+        pkl_filename = filename.replace(".arff", ".pkl.py3")
 
         if os.path.exists(pkl_filename):
             with open(pkl_filename, "rb") as fh:
                 _ = pickle.load(fh)
             repetitions = _["repetitions"]
             name = _["name"]
 
         # Cache miss
         if repetitions is None:
             # Faster than liac-arff and sufficient in this situation!
             if not os.path.exists(filename):
-                raise FileNotFoundError('Split arff %s does not exist!' % filename)
-            splits, meta = scipy.io.arff.loadarff(filename)
-            name = meta.name
+                raise FileNotFoundError(
+                    'Split arff %s does not exist!' % filename
+                )
+            file_data = arff.load(open(filename), return_type=arff.DENSE_GEN)
+            splits = file_data['data']
+            name = file_data['relation']
+            attrnames = [attr[0] for attr in file_data['attributes']]
 
             repetitions = OrderedDict()
 
-            type_idx = meta._attrnames.index('type')
-            rowid_idx = meta._attrnames.index('rowid')
-            repeat_idx = meta._attrnames.index('repeat')
-            fold_idx = meta._attrnames.index('fold')
-            sample_idx = (meta._attrnames.index('sample') if 'sample' in meta._attrnames else None) # can be None
+            type_idx = attrnames.index('type')
+            rowid_idx = attrnames.index('rowid')
+            repeat_idx = attrnames.index('repeat')
+            fold_idx = attrnames.index('fold')
+            sample_idx = (
+                attrnames.index('sample')
+                if 'sample' in attrnames
+                else None
+            )
 
             for line in splits:
                 # A line looks like type, rowid, repeat, fold
                 repetition = int(line[repeat_idx])
                 fold = int(line[fold_idx])
                 sample = 0
                 if sample_idx is not None:
@@ -103,29 +112,32 @@
 
                 if repetition not in repetitions:
                     repetitions[repetition] = OrderedDict()
                 if fold not in repetitions[repetition]:
                     repetitions[repetition][fold] = OrderedDict()
                 if sample not in repetitions[repetition][fold]:
                     repetitions[repetition][fold][sample] = ([], [])
+                split = repetitions[repetition][fold][sample]
 
-                type_ = line[type_idx].decode('utf-8')
+                type_ = line[type_idx]
                 if type_ == 'TRAIN':
-                    repetitions[repetition][fold][sample][0].append(line[rowid_idx])
+                    split[0].append(line[rowid_idx])
                 elif type_ == 'TEST':
-                    repetitions[repetition][fold][sample][1].append(line[rowid_idx])
+                    split[1].append(line[rowid_idx])
                 else:
                     raise ValueError(type_)
 
             for repetition in repetitions:
                 for fold in repetitions[repetition]:
                     for sample in repetitions[repetition][fold]:
                         repetitions[repetition][fold][sample] = Split(
-                            np.array(repetitions[repetition][fold][sample][0], dtype=np.int32),
-                            np.array(repetitions[repetition][fold][sample][1], dtype=np.int32))
+                            np.array(repetitions[repetition][fold][sample][0],
+                                     dtype=np.int32),
+                            np.array(repetitions[repetition][fold][sample][1],
+                                     dtype=np.int32))
 
             with open(pkl_filename, "wb") as fh:
                 pickle.dump({"name": name, "repetitions": repetitions}, fh,
                             protocol=2)
 
         return cls(name, '', repetitions)
```

### Comparing `openml-0.8.0/openml.egg-info/PKG-INFO` & `openml-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: openml
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python API for OpenML
 Home-page: http://openml.org/
-Author: Matthias Feurer, Andreas Müller, Farzan Majdani, Joaquin Vanschoren, Jan van Rijn and Pieter Gijsbers
+Author: Matthias Feurer, Jan van Rijn, Arlind Kadra, Andreas Müller, Pieter Gijsbers and Joaquin Vanschoren
 Author-email: feurerm@informatik.uni-freiburg.de
 Maintainer: Matthias Feurer
 Maintainer-email: feurerm@informatik.uni-freiburg.de
 License: BSD 3-clause
+Project-URL: Documentation, https://openml.github.io/openml-python/
+Project-URL: Source Code, https://github.com/openml/openml-python
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: test
+Provides-Extra: examples
```

### Comparing `openml-0.8.0/openml.egg-info/SOURCES.txt` & `openml-0.9.0/openml.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -17,18 +17,22 @@
 openml/datasets/__init__.py
 openml/datasets/data_feature.py
 openml/datasets/dataset.py
 openml/datasets/functions.py
 openml/evaluations/__init__.py
 openml/evaluations/evaluation.py
 openml/evaluations/functions.py
+openml/extensions/__init__.py
+openml/extensions/extension_interface.py
+openml/extensions/functions.py
+openml/extensions/sklearn/__init__.py
+openml/extensions/sklearn/extension.py
 openml/flows/__init__.py
 openml/flows/flow.py
 openml/flows/functions.py
-openml/flows/sklearn_converter.py
 openml/runs/__init__.py
 openml/runs/functions.py
 openml/runs/run.py
 openml/runs/trace.py
 openml/setups/__init__.py
 openml/setups/functions.py
 openml/setups/setup.py
@@ -41,27 +45,37 @@
 openml/tasks/task.py
 tests/__init__.py
 tests/test_datasets/__init__.py
 tests/test_datasets/test_dataset.py
 tests/test_datasets/test_dataset_functions.py
 tests/test_examples/__init__.py
 tests/test_examples/test_OpenMLDemo.py
+tests/test_extensions/__init__.py
+tests/test_extensions/test_functions.py
+tests/test_extensions/test_sklearn_extension/__init__.py
+tests/test_extensions/test_sklearn_extension/test_sklearn_extension.py
 tests/test_flows/__init__.py
 tests/test_flows/test_flow.py
 tests/test_flows/test_flow_functions.py
-tests/test_flows/test_sklearn.py
 tests/test_flows/dummy_learn/__init__.py
 tests/test_flows/dummy_learn/dummy_forest.py
 tests/test_openml/__init__.py
+tests/test_openml/test_config.py
 tests/test_openml/test_openml.py
 tests/test_runs/__init__.py
 tests/test_runs/test_run.py
 tests/test_runs/test_run_functions.py
 tests/test_runs/test_trace.py
 tests/test_setups/__init__.py
 tests/test_setups/test_setup_functions.py
 tests/test_tasks/__init__.py
+tests/test_tasks/test_classification_task.py
+tests/test_tasks/test_clustering_task.py
+tests/test_tasks/test_learning_curve_task.py
+tests/test_tasks/test_regression_task.py
 tests/test_tasks/test_split.py
+tests/test_tasks/test_supervised_task.py
 tests/test_tasks/test_task.py
 tests/test_tasks/test_task_functions.py
+tests/test_tasks/test_task_methods.py
 tests/test_utils/__init__.py
 tests/test_utils/test_utils.py
```

### Comparing `openml-0.8.0/tests/test_datasets/test_dataset.py` & `openml-0.9.0/tests/test_datasets/test_dataset.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,126 +1,205 @@
 from time import time
+from warnings import filterwarnings, catch_warnings
 
 import numpy as np
-import six
+import pandas as pd
+import pytest
 from scipy import sparse
-from warnings import filterwarnings, catch_warnings
 
 import openml
 from openml.testing import TestBase
+from openml.exceptions import PyOpenMLError
 
 
 class OpenMLDatasetTest(TestBase):
     _multiprocess_can_split_ = True
 
     def setUp(self):
         super(OpenMLDatasetTest, self).setUp()
         openml.config.server = self.production_server
 
         # Load dataset id 2 - dataset 2 is interesting because it contains
         # missing values, categorical features etc.
-        self.dataset = openml.datasets.get_dataset(2)
+        self.dataset = openml.datasets.get_dataset(2, download_data=False)
+        # titanic as missing values, categories, and string
+        self.titanic = openml.datasets.get_dataset(40945, download_data=False)
+        # these datasets have some boolean features
+        self.pc4 = openml.datasets.get_dataset(1049, download_data=False)
+        self.jm1 = openml.datasets.get_dataset(1053, download_data=False)
 
-    def test_get_data(self):
+    def test_get_data_array(self):
         # Basic usage
-        rval = self.dataset.get_data()
+        rval, _, categorical, attribute_names = self.dataset.get_data(dataset_format='array')
         self.assertIsInstance(rval, np.ndarray)
         self.assertEqual(rval.dtype, np.float32)
         self.assertEqual((898, 39), rval.shape)
-        rval, categorical = self.dataset.get_data(
-            return_categorical_indicator=True)
         self.assertEqual(len(categorical), 39)
         self.assertTrue(all([isinstance(cat, bool) for cat in categorical]))
-        rval, attribute_names = self.dataset.get_data(
-            return_attribute_names=True)
         self.assertEqual(len(attribute_names), 39)
-        self.assertTrue(all([isinstance(att, six.string_types)
+        self.assertTrue(all([isinstance(att, str)
                              for att in attribute_names]))
+        self.assertIsNone(_)
+
+        # check that an error is raised when the dataset contains string
+        err_msg = "PyOpenML cannot handle string when returning numpy arrays"
+        with pytest.raises(PyOpenMLError, match=err_msg):
+            self.titanic.get_data(dataset_format='array')
+
+    def test_get_data_pandas(self):
+        data, _, _, _ = self.titanic.get_data(dataset_format='dataframe')
+        self.assertTrue(isinstance(data, pd.DataFrame))
+        self.assertEqual(data.shape[1], len(self.titanic.features))
+        self.assertEqual(data.shape[0], 1309)
+        col_dtype = {
+            'pclass': 'float64',
+            'survived': 'category',
+            'name': 'object',
+            'sex': 'category',
+            'age': 'float64',
+            'sibsp': 'float64',
+            'parch': 'float64',
+            'ticket': 'object',
+            'fare': 'float64',
+            'cabin': 'object',
+            'embarked': 'category',
+            'boat': 'object',
+            'body': 'float64',
+            'home.dest': 'object'
+        }
+        for col_name in data.columns:
+            self.assertTrue(data[col_name].dtype.name == col_dtype[col_name])
+
+        X, y, _, _ = self.titanic.get_data(
+            dataset_format='dataframe',
+            target=self.titanic.default_target_attribute)
+        self.assertTrue(isinstance(X, pd.DataFrame))
+        self.assertTrue(isinstance(y, pd.Series))
+        self.assertEqual(X.shape, (1309, 13))
+        self.assertEqual(y.shape, (1309,))
+        for col_name in X.columns:
+            self.assertTrue(X[col_name].dtype.name == col_dtype[col_name])
+        self.assertTrue(y.dtype.name == col_dtype['survived'])
+
+    def test_get_data_boolean_pandas(self):
+        # test to check that we are converting properly True and False even
+        # with some inconsistency when dumping the data on openml
+        data, _, _, _ = self.jm1.get_data()
+        self.assertTrue(data['defects'].dtype.name == 'category')
+        self.assertTrue(set(data['defects'].cat.categories) == {True, False})
+
+        data, _, _, _ = self.pc4.get_data()
+        self.assertTrue(data['c'].dtype.name == 'category')
+        self.assertTrue(set(data['c'].cat.categories) == {True, False})
+
+    def test_get_data_no_str_data_for_nparrays(self):
+        # check that an error is raised when the dataset contains string
+        err_msg = "PyOpenML cannot handle string when returning numpy arrays"
+        with pytest.raises(PyOpenMLError, match=err_msg):
+            self.titanic.get_data(dataset_format='array')
 
     def test_get_data_with_rowid(self):
         self.dataset.row_id_attribute = "condition"
-        rval, categorical = self.dataset.get_data(
-            include_row_id=True, return_categorical_indicator=True)
-        self.assertEqual(rval.dtype, np.float32)
+        rval, _, categorical, _ = self.dataset.get_data(include_row_id=True)
+        self.assertIsInstance(rval, pd.DataFrame)
+        for (dtype, is_cat) in zip(rval.dtypes, categorical):
+            expected_type = 'category' if is_cat else 'float64'
+            self.assertEqual(dtype.name, expected_type)
         self.assertEqual(rval.shape, (898, 39))
         self.assertEqual(len(categorical), 39)
-        rval, categorical = self.dataset.get_data(
-            include_row_id=False, return_categorical_indicator=True)
-        self.assertEqual(rval.dtype, np.float32)
+
+        rval, _, categorical, _ = self.dataset.get_data()
+        self.assertIsInstance(rval, pd.DataFrame)
+        for (dtype, is_cat) in zip(rval.dtypes, categorical):
+            expected_type = 'category' if is_cat else 'float64'
+            self.assertEqual(dtype.name, expected_type)
         self.assertEqual(rval.shape, (898, 38))
         self.assertEqual(len(categorical), 38)
 
-    def test_get_data_with_target(self):
-        X, y = self.dataset.get_data(target="class")
+    def test_get_data_with_target_array(self):
+        X, y, _, attribute_names = self.dataset.get_data(dataset_format='array', target="class")
         self.assertIsInstance(X, np.ndarray)
         self.assertEqual(X.dtype, np.float32)
-        self.assertIn(y.dtype, [np.int32, np.int64])
         self.assertEqual(X.shape, (898, 38))
-        X, y, attribute_names = self.dataset.get_data(
-            target="class",
-            return_attribute_names=True
-        )
+        self.assertIn(y.dtype, [np.int32, np.int64])
+        self.assertEqual(y.shape, (898, ))
         self.assertEqual(len(attribute_names), 38)
         self.assertNotIn("class", attribute_names)
+
+    def test_get_data_with_target_pandas(self):
+        X, y, categorical, attribute_names = self.dataset.get_data(target="class")
+        self.assertIsInstance(X, pd.DataFrame)
+        for (dtype, is_cat) in zip(X.dtypes, categorical):
+            expected_type = 'category' if is_cat else 'float64'
+            self.assertEqual(dtype.name, expected_type)
+        self.assertIsInstance(y, pd.Series)
+        self.assertEqual(y.dtype.name, 'category')
+
+        self.assertEqual(X.shape, (898, 38))
+        self.assertEqual(len(attribute_names), 38)
         self.assertEqual(y.shape, (898, ))
 
+        self.assertNotIn("class", attribute_names)
+
     def test_get_data_rowid_and_ignore_and_target(self):
         self.dataset.ignore_attributes = ["condition"]
         self.dataset.row_id_attribute = ["hardness"]
-        X, y = self.dataset.get_data(
-            target="class",
-            include_row_id=False,
-            include_ignore_attributes=False
-        )
-        self.assertEqual(X.dtype, np.float32)
-        self.assertIn(y.dtype, [np.int32, np.int64])
+        X, y, categorical, names = self.dataset.get_data(target="class")
         self.assertEqual(X.shape, (898, 36))
-        X, y, categorical = self.dataset.get_data(
-            target="class",
-            return_categorical_indicator=True,
-        )
         self.assertEqual(len(categorical), 36)
-        self.assertListEqual(categorical, [True] * 3 + [False] + [True] * 2 + [
-            False] + [True] * 23 + [False] * 3 + [True] * 3)
+        cats = [True] * 3 + [False, True, True, False] + [True] * 23 + [False] * 3 + [True] * 3
+        self.assertListEqual(categorical, cats)
         self.assertEqual(y.shape, (898, ))
 
     def test_get_data_with_ignore_attributes(self):
         self.dataset.ignore_attributes = ["condition"]
-        rval = self.dataset.get_data(include_ignore_attributes=True)
-        self.assertEqual(rval.dtype, np.float32)
+        rval, _, categorical, _ = self.dataset.get_data(include_ignore_attributes=True)
+        for (dtype, is_cat) in zip(rval.dtypes, categorical):
+            expected_type = 'category' if is_cat else 'float64'
+            self.assertEqual(dtype.name, expected_type)
         self.assertEqual(rval.shape, (898, 39))
-        rval, categorical = self.dataset.get_data(
-            include_ignore_attributes=True, return_categorical_indicator=True)
         self.assertEqual(len(categorical), 39)
-        rval = self.dataset.get_data(include_ignore_attributes=False)
-        self.assertEqual(rval.dtype, np.float32)
+
+        rval, _, categorical, _ = self.dataset.get_data(include_ignore_attributes=False)
+        for (dtype, is_cat) in zip(rval.dtypes, categorical):
+            expected_type = 'category' if is_cat else 'float64'
+            self.assertEqual(dtype.name, expected_type)
         self.assertEqual(rval.shape, (898, 38))
-        rval, categorical = self.dataset.get_data(
-            include_ignore_attributes=False, return_categorical_indicator=True)
         self.assertEqual(len(categorical), 38)
-        # TODO test multiple ignore attributes!
 
     def test_dataset_format_constructor(self):
 
         with catch_warnings():
             filterwarnings('error')
             self.assertRaises(
                 DeprecationWarning,
                 openml.OpenMLDataset,
                 'Test',
                 'Test',
                 format='arff'
             )
 
+    def test_get_data_with_nonexisting_class(self):
+        # This class is using the anneal dataset with labels [1, 2, 3, 4, 5, 'U']. However,
+        # label 4 does not exist and we test that the features 5 and 'U' are correctly mapped to
+        # indices 4 and 5, and that nothing is mapped to index 3.
+        _, y, _, _ = self.dataset.get_data('class', dataset_format='dataframe')
+        self.assertEqual(list(y.dtype.categories), ['1', '2', '3', '4', '5', 'U'])
+        _, y, _, _ = self.dataset.get_data('class', dataset_format='array')
+        self.assertEqual(np.min(y), 0)
+        self.assertEqual(np.max(y), 5)
+        # Check that no label is mapped to 3, since it is reserved for label '4'.
+        self.assertEqual(np.sum(y == 3), 0)
+
 
 class OpenMLDatasetTestOnTestServer(TestBase):
     def setUp(self):
         super(OpenMLDatasetTestOnTestServer, self).setUp()
         # longley, really small dataset
-        self.dataset = openml.datasets.get_dataset(125)
+        self.dataset = openml.datasets.get_dataset(125, download_data=False)
 
     def test_tagging(self):
         tag = "testing_tag_{}_{}".format(self.id(), time())
         ds_list = openml.datasets.list_datasets(tag=tag)
         self.assertEqual(len(ds_list), 0)
         self.dataset.push_tag(tag)
         ds_list = openml.datasets.list_datasets(tag=tag)
@@ -134,102 +213,100 @@
 class OpenMLDatasetTestSparse(TestBase):
     _multiprocess_can_split_ = True
 
     def setUp(self):
         super(OpenMLDatasetTestSparse, self).setUp()
         openml.config.server = self.production_server
 
-        self.sparse_dataset = openml.datasets.get_dataset(4136)
+        self.sparse_dataset = openml.datasets.get_dataset(4136, download_data=False)
 
     def test_get_sparse_dataset_with_target(self):
-        X, y = self.sparse_dataset.get_data(target="class")
+        X, y, _, attribute_names = self.sparse_dataset.get_data(
+            dataset_format='array', target="class"
+        )
+
         self.assertTrue(sparse.issparse(X))
         self.assertEqual(X.dtype, np.float32)
+        self.assertEqual(X.shape, (600, 20000))
+
         self.assertIsInstance(y, np.ndarray)
         self.assertIn(y.dtype, [np.int32, np.int64])
-        self.assertEqual(X.shape, (600, 20000))
-        X, y, attribute_names = self.sparse_dataset.get_data(
-            target="class",
-            return_attribute_names=True,
-        )
-        self.assertTrue(sparse.issparse(X))
+        self.assertEqual(y.shape, (600, ))
+
         self.assertEqual(len(attribute_names), 20000)
         self.assertNotIn("class", attribute_names)
-        self.assertEqual(y.shape, (600, ))
 
     def test_get_sparse_dataset(self):
-        rval = self.sparse_dataset.get_data()
+        rval, _, categorical, attribute_names = self.sparse_dataset.get_data(dataset_format='array')
         self.assertTrue(sparse.issparse(rval))
         self.assertEqual(rval.dtype, np.float32)
         self.assertEqual((600, 20001), rval.shape)
-        rval, categorical = self.sparse_dataset.get_data(
-            return_categorical_indicator=True)
-        self.assertTrue(sparse.issparse(rval))
+
         self.assertEqual(len(categorical), 20001)
         self.assertTrue(all([isinstance(cat, bool) for cat in categorical]))
-        rval, attribute_names = self.sparse_dataset.get_data(
-            return_attribute_names=True)
-        self.assertTrue(sparse.issparse(rval))
+
         self.assertEqual(len(attribute_names), 20001)
-        self.assertTrue(all([isinstance(att, six.string_types)
-                             for att in attribute_names]))
+        self.assertTrue(all([isinstance(att, str) for att in attribute_names]))
+
+    def test_get_sparse_dataframe(self):
+        rval, *_ = self.sparse_dataset.get_data()
+        self.assertTrue(isinstance(rval, pd.SparseDataFrame))
+        self.assertEqual((600, 20001), rval.shape)
 
     def test_get_sparse_dataset_with_rowid(self):
         self.sparse_dataset.row_id_attribute = ["V256"]
-        rval, categorical = self.sparse_dataset.get_data(
-            include_row_id=True, return_categorical_indicator=True)
+        rval, _, categorical, _ = self.sparse_dataset.get_data(
+            dataset_format='array', include_row_id=True
+        )
         self.assertTrue(sparse.issparse(rval))
         self.assertEqual(rval.dtype, np.float32)
         self.assertEqual(rval.shape, (600, 20001))
         self.assertEqual(len(categorical), 20001)
-        rval, categorical = self.sparse_dataset.get_data(
-            include_row_id=False, return_categorical_indicator=True)
+
+        rval, _, categorical, _ = self.sparse_dataset.get_data(
+            dataset_format='array', include_row_id=False
+        )
         self.assertTrue(sparse.issparse(rval))
         self.assertEqual(rval.dtype, np.float32)
         self.assertEqual(rval.shape, (600, 20000))
         self.assertEqual(len(categorical), 20000)
 
     def test_get_sparse_dataset_with_ignore_attributes(self):
         self.sparse_dataset.ignore_attributes = ["V256"]
-        rval = self.sparse_dataset.get_data(include_ignore_attributes=True)
+        rval, _, categorical, _ = self.sparse_dataset.get_data(
+            dataset_format='array', include_ignore_attributes=True
+        )
         self.assertTrue(sparse.issparse(rval))
         self.assertEqual(rval.dtype, np.float32)
         self.assertEqual(rval.shape, (600, 20001))
-        rval, categorical = self.sparse_dataset.get_data(
-            include_ignore_attributes=True, return_categorical_indicator=True)
-        self.assertTrue(sparse.issparse(rval))
+
         self.assertEqual(len(categorical), 20001)
-        rval = self.sparse_dataset.get_data(include_ignore_attributes=False)
+        rval, _, categorical, _ = self.sparse_dataset.get_data(
+            dataset_format='array', include_ignore_attributes=False
+        )
         self.assertTrue(sparse.issparse(rval))
         self.assertEqual(rval.dtype, np.float32)
         self.assertEqual(rval.shape, (600, 20000))
-        rval, categorical = self.sparse_dataset.get_data(
-            include_ignore_attributes=False, return_categorical_indicator=True)
-        self.assertTrue(sparse.issparse(rval))
         self.assertEqual(len(categorical), 20000)
-        # TODO test multiple ignore attributes!
 
     def test_get_sparse_dataset_rowid_and_ignore_and_target(self):
         # TODO: re-add row_id and ignore attributes
         self.sparse_dataset.ignore_attributes = ["V256"]
         self.sparse_dataset.row_id_attribute = ["V512"]
-        X, y = self.sparse_dataset.get_data(
+        X, y, categorical, _ = self.sparse_dataset.get_data(
+            dataset_format='array',
             target="class",
             include_row_id=False,
             include_ignore_attributes=False,
         )
         self.assertTrue(sparse.issparse(X))
         self.assertEqual(X.dtype, np.float32)
         self.assertIn(y.dtype, [np.int32, np.int64])
         self.assertEqual(X.shape, (600, 19998))
-        X, y, categorical = self.sparse_dataset.get_data(
-            target="class",
-            return_categorical_indicator=True,
-        )
-        self.assertTrue(sparse.issparse(X))
+
         self.assertEqual(len(categorical), 19998)
         self.assertListEqual(categorical, [False] * 19998)
         self.assertEqual(y.shape, (600, ))
 
 
 class OpenMLDatasetQualityTest(TestBase):
     def test__check_qualities(self):
```

### Comparing `openml-0.8.0/tests/test_datasets/test_dataset_functions.py` & `openml-0.9.0/tests/test_datasets/test_dataset_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,24 @@
-import unittest
 import os
-import sys
 import random
 from itertools import product
-if sys.version_info[0] >= 3:
-    from unittest import mock
-else:
-    import mock
+from unittest import mock
 
 import arff
-import six
 
 import pytest
 import numpy as np
 import pandas as pd
 import scipy.sparse
 from oslo_concurrency import lockutils
-from warnings import filterwarnings, catch_warnings
 
 import openml
 from openml import OpenMLDataset
-from openml.exceptions import OpenMLCacheException, PyOpenMLError, \
-    OpenMLHashException, PrivateDatasetError
+from openml.exceptions import OpenMLCacheException, OpenMLHashException, \
+    OpenMLPrivateDatasetError
 from openml.testing import TestBase
 from openml.utils import _tag_entity, _create_cache_directory_for_id
 from openml.datasets.functions import (create_dataset,
                                        attributes_arff_from_df,
                                        _get_cached_dataset,
                                        _get_cached_dataset_features,
                                        _get_cached_dataset_qualities,
@@ -56,15 +49,16 @@
                     name='datasets.functions.get_dataset:%s' % did,
                     lock_path=os.path.join(openml.config.get_cache_directory(), 'locks'),
             ):
                 pickle_path = os.path.join(cache_dir, 'datasets', did,
                                            'dataset.pkl')
                 try:
                     os.remove(pickle_path)
-                except:
+                except (OSError, FileNotFoundError):
+                    #  Replaced a bare except. Not sure why either of these would be acceptable.
                     pass
 
     def _get_empty_param_for_dataset(self):
 
         return {
             'name': None,
             'description': None,
@@ -110,60 +104,64 @@
     def test_get_cached_dataset_description(self):
         openml.config.cache_directory = self.static_cache_dir
         description = openml.datasets.functions._get_cached_dataset_description(2)
         self.assertIsInstance(description, dict)
 
     def test_get_cached_dataset_description_not_cached(self):
         openml.config.cache_directory = self.static_cache_dir
-        self.assertRaisesRegexp(OpenMLCacheException, "Dataset description for "
-                                                      "dataset id 3 not cached",
-                                openml.datasets.functions._get_cached_dataset_description,
-                                3)
+        self.assertRaisesRegex(OpenMLCacheException,
+                               "Dataset description for dataset id 3 not cached",
+                               openml.datasets.functions._get_cached_dataset_description,
+                               dataset_id=3)
 
     def test_get_cached_dataset_arff(self):
         openml.config.cache_directory = self.static_cache_dir
-        description = openml.datasets.functions._get_cached_dataset_arff(
-            dataset_id=2)
+        description = openml.datasets.functions._get_cached_dataset_arff(dataset_id=2)
         self.assertIsInstance(description, str)
 
     def test_get_cached_dataset_arff_not_cached(self):
         openml.config.cache_directory = self.static_cache_dir
-        self.assertRaisesRegexp(OpenMLCacheException, "ARFF file for "
-                                                      "dataset id 3 not cached",
-                                openml.datasets.functions._get_cached_dataset_arff,
-                                3)
+        self.assertRaisesRegex(OpenMLCacheException,
+                               "ARFF file for dataset id 3 not cached",
+                               openml.datasets.functions._get_cached_dataset_arff,
+                               dataset_id=3)
 
     def _check_dataset(self, dataset):
-            self.assertEqual(type(dataset), dict)
-            self.assertGreaterEqual(len(dataset), 2)
-            self.assertIn('did', dataset)
-            self.assertIsInstance(dataset['did'], int)
-            self.assertIn('status', dataset)
-            self.assertIsInstance(dataset['status'], six.string_types)
-            self.assertIn(dataset['status'], ['in_preparation', 'active',
-                                              'deactivated'])
+        self.assertEqual(type(dataset), dict)
+        self.assertGreaterEqual(len(dataset), 2)
+        self.assertIn('did', dataset)
+        self.assertIsInstance(dataset['did'], int)
+        self.assertIn('status', dataset)
+        self.assertIsInstance(dataset['status'], str)
+        self.assertIn(dataset['status'], ['in_preparation', 'active', 'deactivated'])
+
     def _check_datasets(self, datasets):
         for did in datasets:
             self._check_dataset(datasets[did])
 
     def test_tag_untag_dataset(self):
-        tag = 'test_tag_%d' %random.randint(1, 1000000)
+        tag = 'test_tag_%d' % random.randint(1, 1000000)
         all_tags = _tag_entity('data', 1, tag)
         self.assertTrue(tag in all_tags)
         all_tags = _tag_entity('data', 1, tag, untag=True)
         self.assertTrue(tag not in all_tags)
 
     def test_list_datasets(self):
         # We can only perform a smoke test here because we test on dynamic
         # data from the internet...
         datasets = openml.datasets.list_datasets()
         # 1087 as the number of datasets on openml.org
         self.assertGreaterEqual(len(datasets), 100)
         self._check_datasets(datasets)
 
+    def test_list_datasets_output_format(self):
+        datasets = openml.datasets.list_datasets(output_format='dataframe')
+        self.assertIsInstance(datasets, pd.DataFrame)
+        self.assertGreaterEqual(len(datasets), 100)
+
     def test_list_datasets_by_tag(self):
         datasets = openml.datasets.list_datasets(tag='study_14')
         self.assertGreaterEqual(len(datasets), 100)
         self._check_datasets(datasets)
 
     def test_list_datasets_by_size(self):
         datasets = openml.datasets.list_datasets(size=10050)
@@ -187,15 +185,17 @@
 
     def test_list_datasets_by_number_missing_values(self):
         datasets = openml.datasets.list_datasets(number_missing_values="5..100")
         self.assertGreaterEqual(len(datasets), 5)
         self._check_datasets(datasets)
 
     def test_list_datasets_combined_filters(self):
-        datasets = openml.datasets.list_datasets(tag='study_14', number_instances="100..1000", number_missing_values="800..1000")
+        datasets = openml.datasets.list_datasets(tag='study_14',
+                                                 number_instances="100..1000",
+                                                 number_missing_values="800..1000")
         self.assertGreaterEqual(len(datasets), 1)
         self._check_datasets(datasets)
 
     def test_list_datasets_paginate(self):
         size = 10
         max = 100
         for i in range(0, max, size):
@@ -206,107 +206,232 @@
     def test_list_datasets_empty(self):
         datasets = openml.datasets.list_datasets(tag='NoOneWouldUseThisTagAnyway')
         if len(datasets) > 0:
             raise ValueError('UnitTest Outdated, tag was already used (please remove)')
 
         self.assertIsInstance(datasets, dict)
 
-    @unittest.skip('See https://github.com/openml/openml-python/issues/149')
     def test_check_datasets_active(self):
-        active = openml.datasets.check_datasets_active([1, 17])
-        self.assertTrue(active[1])
+        # Have to test on live because there is no deactivated dataset on the test server.
+        openml.config.server = self.production_server
+        active = openml.datasets.check_datasets_active([2, 17])
+        self.assertTrue(active[2])
         self.assertFalse(active[17])
-        self.assertRaisesRegexp(ValueError, 'Could not find dataset 79 in OpenML'
-                                            ' dataset list.',
-                                openml.datasets.check_datasets_active, [79])
+        self.assertRaisesRegex(
+            ValueError,
+            'Could not find dataset 79 in OpenML dataset list.',
+            openml.datasets.check_datasets_active,
+            [79],
+        )
+        openml.config.server = self.test_server
+
+    def _datasets_retrieved_successfully(self, dids, metadata_only=True):
+        """ Checks that all files for the given dids have been downloaded.
+
+        This includes:
+            - description
+            - qualities
+            - features
+            - absence of data arff if metadata_only, else it must be present too.
+        """
+        for did in dids:
+            self.assertTrue(os.path.exists(os.path.join(
+                openml.config.get_cache_directory(), "datasets", str(did), "description.xml")))
+            self.assertTrue(os.path.exists(os.path.join(
+                openml.config.get_cache_directory(), "datasets", str(did), "qualities.xml")))
+            self.assertTrue(os.path.exists(os.path.join(
+                openml.config.get_cache_directory(), "datasets", str(did), "features.xml")))
+
+            data_assert = self.assertFalse if metadata_only else self.assertTrue
+            data_assert(os.path.exists(os.path.join(
+                openml.config.get_cache_directory(), "datasets", str(did), "dataset.arff")))
+
+    def test__name_to_id_with_deactivated(self):
+        """ Check that an activated dataset is returned if an earlier deactivated one exists. """
+        openml.config.server = self.production_server
+        # /d/1 was deactivated
+        self.assertEqual(openml.datasets.functions._name_to_id('anneal'), 2)
+        openml.config.server = self.test_server
+
+    def test__name_to_id_with_multiple_active(self):
+        """ With multiple active datasets, retrieve the least recent active. """
+        openml.config.server = self.production_server
+        self.assertEqual(openml.datasets.functions._name_to_id('iris'), 61)
+
+    def test__name_to_id_with_version(self):
+        """ With multiple active datasets, retrieve the least recent active. """
+        openml.config.server = self.production_server
+        self.assertEqual(openml.datasets.functions._name_to_id('iris', version=3), 969)
+
+    def test__name_to_id_with_multiple_active_error(self):
+        """ With multiple active datasets, retrieve the least recent active. """
+        self.assertRaisesRegex(
+            ValueError,
+            "Multiple active datasets exist with name iris",
+            openml.datasets.functions._name_to_id,
+            dataset_name='iris',
+            error_if_multiple=True
+        )
+
+    def test__name_to_id_name_does_not_exist(self):
+        """ With multiple active datasets, retrieve the least recent active. """
+        self.assertRaisesRegex(
+            RuntimeError,
+            "No active datasets exist with name does_not_exist",
+            openml.datasets.functions._name_to_id,
+            dataset_name='does_not_exist'
+        )
+
+    def test__name_to_id_version_does_not_exist(self):
+        """ With multiple active datasets, retrieve the least recent active. """
+        self.assertRaisesRegex(
+            RuntimeError,
+            "No active datasets exist with name iris and version 100000",
+            openml.datasets.functions._name_to_id,
+            dataset_name='iris',
+            version=100000
+        )
+
+    def test_get_datasets_by_name(self):
+        # did 1 and 2 on the test server:
+        dids = ['anneal', 'kr-vs-kp']
+        datasets = openml.datasets.get_datasets(dids, download_data=False)
+        self.assertEqual(len(datasets), 2)
+        self._datasets_retrieved_successfully([1, 2])
+
+    def test_get_datasets_by_mixed(self):
+        # did 1 and 2 on the test server:
+        dids = ['anneal', 2]
+        datasets = openml.datasets.get_datasets(dids, download_data=False)
+        self.assertEqual(len(datasets), 2)
+        self._datasets_retrieved_successfully([1, 2])
 
     def test_get_datasets(self):
         dids = [1, 2]
         datasets = openml.datasets.get_datasets(dids)
         self.assertEqual(len(datasets), 2)
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "description.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "2", "description.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "dataset.arff")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "2", "dataset.arff")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "features.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "2", "features.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "qualities.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "2", "qualities.xml")))
+        self._datasets_retrieved_successfully([1, 2], metadata_only=False)
+
+    def test_get_datasets_lazy(self):
+        dids = [1, 2]
+        datasets = openml.datasets.get_datasets(dids, download_data=False)
+        self.assertEqual(len(datasets), 2)
+        self._datasets_retrieved_successfully([1, 2], metadata_only=True)
+
+        datasets[0].get_data()
+        datasets[1].get_data()
+        self._datasets_retrieved_successfully([1, 2], metadata_only=False)
+
+    def test_get_dataset_by_name(self):
+        dataset = openml.datasets.get_dataset('anneal')
+        self.assertEqual(type(dataset), OpenMLDataset)
+        self.assertEqual(dataset.dataset_id, 1)
+        self._datasets_retrieved_successfully([1], metadata_only=False)
+
+        self.assertGreater(len(dataset.features), 1)
+        self.assertGreater(len(dataset.qualities), 4)
+
+        # Issue324 Properly handle private datasets when trying to access them
+        openml.config.server = self.production_server
+        self.assertRaises(OpenMLPrivateDatasetError, openml.datasets.get_dataset, 45)
 
     def test_get_dataset(self):
+        # This is the only non-lazy load to ensure default behaviour works.
         dataset = openml.datasets.get_dataset(1)
         self.assertEqual(type(dataset), OpenMLDataset)
         self.assertEqual(dataset.name, 'anneal')
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "description.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "dataset.arff")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "features.xml")))
-        self.assertTrue(os.path.exists(os.path.join(
-            openml.config.get_cache_directory(), "datasets", "1", "qualities.xml")))
+        self._datasets_retrieved_successfully([1], metadata_only=False)
 
         self.assertGreater(len(dataset.features), 1)
         self.assertGreater(len(dataset.qualities), 4)
 
         # Issue324 Properly handle private datasets when trying to access them
         openml.config.server = self.production_server
-        self.assertRaises(PrivateDatasetError, openml.datasets.get_dataset, 45)
+        self.assertRaises(OpenMLPrivateDatasetError, openml.datasets.get_dataset, 45)
+
+    def test_get_dataset_lazy(self):
+        dataset = openml.datasets.get_dataset(1, download_data=False)
+        self.assertEqual(type(dataset), OpenMLDataset)
+        self.assertEqual(dataset.name, 'anneal')
+        self._datasets_retrieved_successfully([1], metadata_only=True)
+
+        self.assertGreater(len(dataset.features), 1)
+        self.assertGreater(len(dataset.qualities), 4)
 
+        dataset.get_data()
+        self._datasets_retrieved_successfully([1], metadata_only=False)
 
-    def test_get_dataset_with_string(self):
-        dataset = openml.datasets.get_dataset(101)
-        self.assertRaises(PyOpenMLError, dataset._get_arff, 'arff')
-        self.assertRaises(PyOpenMLError, dataset.get_data)
+        # Issue324 Properly handle private datasets when trying to access them
+        openml.config.server = self.production_server
+        self.assertRaises(OpenMLPrivateDatasetError, openml.datasets.get_dataset, 45, False)
+
+    def test_get_dataset_lazy_all_functions(self):
+        """ Test that all expected functionality is available without downloading the dataset. """
+        dataset = openml.datasets.get_dataset(1, download_data=False)
+        # We only tests functions as general integrity is tested by test_get_dataset_lazy
+
+        def ensure_absence_of_real_data():
+            self.assertFalse(os.path.exists(os.path.join(
+                openml.config.get_cache_directory(), "datasets", "1", "dataset.arff")))
+
+        tag = 'test_lazy_tag_%d' % random.randint(1, 1000000)
+        dataset.push_tag(tag)
+        ensure_absence_of_real_data()
+
+        dataset.remove_tag(tag)
+        ensure_absence_of_real_data()
+
+        nominal_indices = dataset.get_features_by_type('nominal')
+        correct = [0, 1, 2, 5, 6, 7, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19,
+                   20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31, 35, 36, 37, 38]
+        self.assertEqual(nominal_indices, correct)
+        ensure_absence_of_real_data()
+
+        classes = dataset.retrieve_class_labels()
+        self.assertEqual(classes, ['1', '2', '3', '4', '5', 'U'])
+        ensure_absence_of_real_data()
 
     def test_get_dataset_sparse(self):
-        dataset = openml.datasets.get_dataset(102)
-        X = dataset.get_data()
+        dataset = openml.datasets.get_dataset(102, download_data=False)
+        X, *_ = dataset.get_data(dataset_format='array')
         self.assertIsInstance(X, scipy.sparse.csr_matrix)
 
     def test_download_rowid(self):
         # Smoke test which checks that the dataset has the row-id set correctly
         did = 44
-        dataset = openml.datasets.get_dataset(did)
+        dataset = openml.datasets.get_dataset(did, download_data=False)
         self.assertEqual(dataset.row_id_attribute, 'Counter')
 
     def test__get_dataset_description(self):
         description = _get_dataset_description(self.workdir, 2)
         self.assertIsInstance(description, dict)
         description_xml_path = os.path.join(self.workdir,
                                             'description.xml')
         self.assertTrue(os.path.exists(description_xml_path))
 
     def test__getarff_path_dataset_arff(self):
         openml.config.cache_directory = self.static_cache_dir
         description = openml.datasets.functions._get_cached_dataset_description(2)
-        arff_path = _get_dataset_arff(self.workdir, description)
+        arff_path = _get_dataset_arff(description, cache_directory=self.workdir)
         self.assertIsInstance(arff_path, str)
         self.assertTrue(os.path.exists(arff_path))
 
     def test__getarff_md5_issue(self):
         description = {
             'oml:id': 5,
             'oml:md5_checksum': 'abc',
             'oml:url': 'https://www.openml.org/data/download/61',
         }
-        self.assertRaisesRegexp(
+        self.assertRaisesRegex(
             OpenMLHashException,
-            'Checksum ad484452702105cbf3d30f8deaba39a9 of downloaded dataset 5 '
-            'is unequal to the checksum abc sent by the server.',
+            'Checksum ad484452702105cbf3d30f8deaba39a9 of downloaded file '
+            'is unequal to the expected checksum abc. '
+            'Raised when downloading dataset 5.',
             _get_dataset_arff,
-            self.workdir, description,
+            description,
         )
 
     def test__get_dataset_features(self):
         features = _get_dataset_features(self.workdir, 2)
         self.assertIsInstance(features, dict)
         features_xml_path = os.path.join(self.workdir, 'features.xml')
         self.assertTrue(os.path.exists(features_xml_path))
@@ -328,23 +453,22 @@
         self.assertFalse(os.path.exists(did_cache_dir))
 
     # Use _get_dataset_arff to load the description, trigger an exception in the
     # test target and have a slightly higher coverage
     @mock.patch('openml.datasets.functions._get_dataset_arff')
     def test_deletion_of_cache_dir_faulty_download(self, patch):
         patch.side_effect = Exception('Boom!')
-        self.assertRaisesRegexp(Exception, 'Boom!', openml.datasets.get_dataset,
-                                1)
+        self.assertRaisesRegex(Exception, 'Boom!', openml.datasets.get_dataset, dataset_id=1)
         datasets_cache_dir = os.path.join(
             self.workdir, 'org', 'openml', 'test', 'datasets'
         )
         self.assertEqual(len(os.listdir(datasets_cache_dir)), 0)
 
     def test_publish_dataset(self):
-
+        # lazy loading not possible as we need the arff-file.
         openml.datasets.get_dataset(3)
         file_path = os.path.join(openml.config.get_cache_directory(),
                                  "datasets", "3", "dataset.arff")
         dataset = OpenMLDataset(
             "anneal",
             "test",
             data_format="arff",
@@ -354,17 +478,17 @@
             data_file=file_path,
         )
         dataset.publish()
         self.assertIsInstance(dataset.dataset_id, int)
 
     def test__retrieve_class_labels(self):
         openml.config.cache_directory = self.static_cache_dir
-        labels = openml.datasets.get_dataset(2).retrieve_class_labels()
+        labels = openml.datasets.get_dataset(2, download_data=False).retrieve_class_labels()
         self.assertEqual(labels, ['1', '2', '3', '4', '5', 'U'])
-        labels = openml.datasets.get_dataset(2).retrieve_class_labels(
+        labels = openml.datasets.get_dataset(2, download_data=False).retrieve_class_labels(
             target_name='product-type')
         self.assertEqual(labels, ['C', 'H', 'G'])
 
     def test_upload_dataset_with_url(self):
 
         dataset = OpenMLDataset(
             "%s-UploadTestWithURL" % self._get_sentinel(),
@@ -441,15 +565,15 @@
         df = pd.DataFrame([[1], ['2'], [3.]])
         df[0] = df[0].astype('category')
         err_msg = "The column '0' of the dataframe is of 'category' dtype."
         with pytest.raises(ValueError, match=err_msg):
             attributes_arff_from_df(df)
 
     def test_attributes_arff_from_df_unknown_dtype(self):
-        # check that an error is raised when the dtype is not supported by
+        # check that an error is raised when the dtype is not supptagorted by
         # liac-arff
         data = [
             [[1], ['2'], [3.]],
             [pd.Timestamp('2012-05-01'), pd.Timestamp('2012-05-02')],
         ]
         dtype = [
             'mixed-integer',
@@ -681,17 +805,16 @@
         self.assertRaises(
             ValueError,
             create_dataset,
             **param
         )
 
     def test_get_online_dataset_arff(self):
-
-        # Australian dataset
-        dataset_id = 100
+        dataset_id = 100  # Australian
+        # lazy loading not used as arff file is checked.
         dataset = openml.datasets.get_dataset(dataset_id)
         decoder = arff.ArffDecoder()
         # check if the arff from the dataset is
         # the same as the arff from _get_arff function
         d_format = (dataset.format).lower()
 
         self.assertEqual(
@@ -705,15 +828,15 @@
             "ARFF files are not equal"
         )
 
     def test_get_online_dataset_format(self):
 
         # Phoneme dataset
         dataset_id = 77
-        dataset = openml.datasets.get_dataset(dataset_id)
+        dataset = openml.datasets.get_dataset(dataset_id, download_data=False)
 
         self.assertEqual(
             (dataset.format).lower(),
             _get_online_dataset_format(dataset_id),
             "The format of the ARFF files is different"
         )
 
@@ -837,14 +960,107 @@
             downloaded_data,
             dataset._dataset,
             "Uploaded ARFF does not match original one"
         )
         self.assertTrue(
             '@ATTRIBUTE rnd_str {a, b, c, d, e, f, g}' in downloaded_data)
 
+    def test_ignore_attributes_dataset(self):
+        data = [
+            ['a', 'sunny', 85.0, 85.0, 'FALSE', 'no'],
+            ['b', 'sunny', 80.0, 90.0, 'TRUE', 'no'],
+            ['c', 'overcast', 83.0, 86.0, 'FALSE', 'yes'],
+            ['d', 'rainy', 70.0, 96.0, 'FALSE', 'yes'],
+            ['e', 'rainy', 68.0, 80.0, 'FALSE', 'yes']
+        ]
+        column_names = ['rnd_str', 'outlook', 'temperature', 'humidity',
+                        'windy', 'play']
+        df = pd.DataFrame(data, columns=column_names)
+        # enforce the type of each column
+        df['outlook'] = df['outlook'].astype('category')
+        df['windy'] = df['windy'].astype('bool')
+        df['play'] = df['play'].astype('category')
+        # meta-information
+        name = '%s-pandas_testing_dataset' % self._get_sentinel()
+        description = 'Synthetic dataset created from a Pandas DataFrame'
+        creator = 'OpenML tester'
+        collection_date = '01-01-2018'
+        language = 'English'
+        licence = 'MIT'
+        default_target_attribute = 'play'
+        citation = 'None'
+        original_data_url = 'http://openml.github.io/openml-python'
+        paper_url = 'http://openml.github.io/openml-python'
+
+        # we use the create_dataset function which call the OpenMLDataset
+        # constructor
+        # pass a string to ignore_attribute
+        dataset = openml.datasets.functions.create_dataset(
+            name=name,
+            description=description,
+            creator=creator,
+            contributor=None,
+            collection_date=collection_date,
+            language=language,
+            licence=licence,
+            default_target_attribute=default_target_attribute,
+            row_id_attribute=None,
+            ignore_attribute='outlook',
+            citation=citation,
+            attributes='auto',
+            data=df,
+            version_label='test',
+            original_data_url=original_data_url,
+            paper_url=paper_url
+        )
+        self.assertEqual(dataset.ignore_attributes, ['outlook'])
+
+        # pass a list to ignore_attribute
+        dataset = openml.datasets.functions.create_dataset(
+            name=name,
+            description=description,
+            creator=creator,
+            contributor=None,
+            collection_date=collection_date,
+            language=language,
+            licence=licence,
+            default_target_attribute=default_target_attribute,
+            row_id_attribute=None,
+            ignore_attribute=['outlook', 'windy'],
+            citation=citation,
+            attributes='auto',
+            data=df,
+            version_label='test',
+            original_data_url=original_data_url,
+            paper_url=paper_url
+        )
+        self.assertEqual(dataset.ignore_attributes, ['outlook', 'windy'])
+
+        # raise an error if unknown type
+        err_msg = 'Wrong data type for ignore_attribute. Should be list.'
+        with pytest.raises(ValueError, match=err_msg):
+            openml.datasets.functions.create_dataset(
+                name=name,
+                description=description,
+                creator=creator,
+                contributor=None,
+                collection_date=collection_date,
+                language=language,
+                licence=licence,
+                default_target_attribute=default_target_attribute,
+                row_id_attribute=None,
+                ignore_attribute=tuple(['outlook', 'windy']),
+                citation=citation,
+                attributes='auto',
+                data=df,
+                version_label='test',
+                original_data_url=original_data_url,
+                paper_url=paper_url
+            )
+
     def test_create_dataset_row_id_attribute_error(self):
         # meta-information
         name = '%s-pandas_testing_dataset' % self._get_sentinel()
         description = 'Synthetic dataset created from a Pandas DataFrame'
         creator = 'OpenML tester'
         collection_date = '01-01-2018'
         language = 'English'
@@ -950,15 +1166,15 @@
         collection_date = '01-01-2018'
         language = 'English'
         licence = 'MIT'
         default_target_attribute = 'col_{}'.format(data.shape[1] - 1)
         citation = 'None'
         original_data_url = 'http://openml.github.io/openml-python'
         paper_url = 'http://openml.github.io/openml-python'
-        err_msg = "Automatically inferring the attributes required a pandas"
+        err_msg = "Automatically inferring attributes requires a pandas"
         with pytest.raises(ValueError, match=err_msg):
             openml.datasets.functions.create_dataset(
                 name=name,
                 description=description,
                 creator=creator,
                 contributor=None,
                 collection_date=collection_date,
```

### Comparing `openml-0.8.0/tests/test_examples/test_OpenMLDemo.py` & `openml-0.9.0/tests/test_examples/test_OpenMLDemo.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 import sys
 
 import matplotlib
 matplotlib.use('AGG')
 import nbformat
 from nbconvert.exporters import export
 from nbconvert.exporters.python import PythonExporter
-import six
 
-if six.PY2:
-    import mock
-else:
-    import unittest.mock as mock
+import unittest.mock as mock
 
 from unittest import skip
 import openml._api_calls
 import openml.config
 from openml.testing import TestBase
 
 _perform_api_call = openml._api_calls._perform_api_call
@@ -30,20 +26,20 @@
         self.kernel_name = 'python%d' % python_version
         self.this_file_directory = os.path.dirname(__file__)
         self.notebook_output_directory = os.path.join(
             self.this_file_directory, '.out')
 
         try:
             shutil.rmtree(self.notebook_output_directory)
-        except:
+        except OSError:
             pass
 
         try:
             os.makedirs(self.notebook_output_directory)
-        except:
+        except OSError:
             pass
 
     def _tst_notebook(self, notebook_name):
 
         notebook_filename = os.path.abspath(os.path.join(
             self.this_file_directory, '..', '..', 'examples', notebook_name))
 
@@ -79,8 +75,8 @@
         openml.config.server = self.production_server
         self._tst_notebook('OpenML_Tutorial.ipynb')
         self.assertGreater(patch.call_count, 100)
 
     @skip("Deleted tutorial file")
     def test_tutorial_dataset(self):
 
-        self._tst_notebook('Dataset_import.ipynb')
+        self._tst_notebook('Dataset_import.ipynb')
```

### Comparing `openml-0.8.0/tests/test_flows/test_flow.py` & `openml-0.9.0/tests/test_flows/test_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import collections
 import copy
+from distutils.version import LooseVersion
 import hashlib
 import re
-import sys
 import time
-from distutils.version import LooseVersion
-
-if sys.version_info[0] >= 3:
-    from unittest import mock
-else:
-    import mock
+from unittest import mock
 
 import scipy.stats
 import sklearn
 import sklearn.datasets
 import sklearn.decomposition
 import sklearn.dummy
 import sklearn.ensemble
@@ -27,25 +22,29 @@
 if LooseVersion(sklearn.__version__) < "0.20":
     from sklearn.preprocessing import Imputer
 else:
     from sklearn.impute import SimpleImputer as Imputer
 
 import xmltodict
 
-from openml.testing import TestBase
-from openml._api_calls import _perform_api_call
 import openml
-import openml.utils
-from openml.flows.sklearn_converter import _format_external_version
+from openml._api_calls import _perform_api_call
 import openml.exceptions
+import openml.extensions.sklearn
+from openml.testing import TestBase
+import openml.utils
 
 
 class TestFlow(TestBase):
     _multiprocess_can_split_ = True
 
+    def setUp(self):
+        super().setUp()
+        self.extension = openml.extensions.sklearn.SklearnExtension()
+
     def test_get_flow(self):
         # We need to use the production server here because 4024 is not the
         # test server
         openml.config.server = self.production_server
 
         flow = openml.flows.get_flow(4024)
         self.assertIsInstance(flow, openml.OpenMLFlow)
@@ -111,170 +110,201 @@
         self.assertIn(flow_id, flow_list)
         flow.remove_tag(tag)
         flow_list = openml.flows.list_flows(tag=tag)
         self.assertEqual(len(flow_list), 0)
 
     def test_from_xml_to_xml(self):
         # Get the raw xml thing
-        # TODO maybe get this via get_flow(), which would have to be refactored to allow getting only the xml dictionary
+        # TODO maybe get this via get_flow(), which would have to be refactored
+        # to allow getting only the xml dictionary
         # TODO: no sklearn flows.
         for flow_id in [3, 5, 7, 9, ]:
-            flow_xml = _perform_api_call("flow/%d" % flow_id)
+            flow_xml = _perform_api_call("flow/%d" % flow_id,
+                                         request_method='get')
             flow_dict = xmltodict.parse(flow_xml)
 
             flow = openml.OpenMLFlow._from_dict(flow_dict)
             new_xml = flow._to_xml()
 
-            flow_xml = flow_xml.replace('  ', '').replace('\t', '').strip().replace('\n\n', '\n').replace('&quot;', '"')
+            flow_xml = (
+                flow_xml.replace('  ', '').replace('\t', '').
+                strip().replace('\n\n', '\n').replace('&quot;', '"')
+            )
             flow_xml = re.sub(r'^$', '', flow_xml)
-            new_xml = new_xml.replace('  ', '').replace('\t', '').strip().replace('\n\n', '\n').replace('&quot;', '"')
+            new_xml = (
+                new_xml.replace('  ', '').replace('\t', '').
+                strip().replace('\n\n', '\n').replace('&quot;', '"')
+            )
             new_xml = re.sub(r'^$', '', new_xml)
 
             self.assertEqual(new_xml, flow_xml)
 
     def test_to_xml_from_xml(self):
         scaler = sklearn.preprocessing.StandardScaler(with_mean=False)
         boosting = sklearn.ensemble.AdaBoostClassifier(
             base_estimator=sklearn.tree.DecisionTreeClassifier())
         model = sklearn.pipeline.Pipeline(steps=(
             ('scaler', scaler), ('boosting', boosting)))
-        flow = openml.flows.sklearn_to_flow(model)
+        flow = self.extension.model_to_flow(model)
         flow.flow_id = -234
         # end of setup
 
         xml = flow._to_xml()
         xml_dict = xmltodict.parse(xml)
         new_flow = openml.flows.OpenMLFlow._from_dict(xml_dict)
 
         # Would raise exception if they are not legal
         openml.flows.functions.assert_flows_equal(new_flow, flow)
         self.assertIsNot(new_flow, flow)
 
     def test_publish_flow(self):
-        flow = openml.OpenMLFlow(name='sklearn.dummy.DummyClassifier',
-                                 class_name='sklearn.dummy.DummyClassifier',
-                                 description="test description",
-                                 model=sklearn.dummy.DummyClassifier(),
-                                 components=collections.OrderedDict(),
-                                 parameters=collections.OrderedDict(),
-                                 parameters_meta_info=collections.OrderedDict(),
-                                 external_version=_format_external_version(
-                                     'sklearn', sklearn.__version__),
-                                 tags=[],
-                                 language='English',
-                                 dependencies=None)
+        flow = openml.OpenMLFlow(
+            name='sklearn.dummy.DummyClassifier',
+            class_name='sklearn.dummy.DummyClassifier',
+            description="test description",
+            model=sklearn.dummy.DummyClassifier(),
+            components=collections.OrderedDict(),
+            parameters=collections.OrderedDict(),
+            parameters_meta_info=collections.OrderedDict(),
+            external_version=self.extension._format_external_version(
+                'sklearn',
+                sklearn.__version__,
+            ),
+            tags=[],
+            language='English',
+            dependencies=None,
+        )
 
         flow, _ = self._add_sentinel_to_flow_name(flow, None)
 
         flow.publish()
         self.assertIsInstance(flow.flow_id, int)
 
-    def test_publish_existing_flow(self):
+    @mock.patch('openml.flows.functions.flow_exists')
+    def test_publish_existing_flow(self, flow_exists_mock):
         clf = sklearn.tree.DecisionTreeClassifier(max_depth=2)
-        flow = openml.flows.sklearn_to_flow(clf)
-        flow, _ = self._add_sentinel_to_flow_name(flow, None)
-        flow.publish()
-        self.assertRaisesRegexp(openml.exceptions.OpenMLServerException,
-                                'flow already exists', flow.publish)
+        flow = self.extension.model_to_flow(clf)
+        flow_exists_mock.return_value = 1
+
+        with self.assertRaises(openml.exceptions.PyOpenMLError) as context_manager:
+            flow.publish(raise_error_if_exists=True)
+
+        self.assertTrue('OpenMLFlow already exists' in context_manager.exception.message)
 
     def test_publish_flow_with_similar_components(self):
-        clf = sklearn.ensemble.VotingClassifier(
-            [('lr', sklearn.linear_model.LogisticRegression())])
-        flow = openml.flows.sklearn_to_flow(clf)
+        clf = sklearn.ensemble.VotingClassifier([
+            ('lr', sklearn.linear_model.LogisticRegression(solver='lbfgs')),
+        ])
+        flow = self.extension.model_to_flow(clf)
         flow, _ = self._add_sentinel_to_flow_name(flow, None)
         flow.publish()
         # For a flow where both components are published together, the upload
         # date should be equal
-        self.assertEqual(flow.upload_date,
-                         flow.components['lr'].upload_date,
-                         (flow.name, flow.flow_id,
-                          flow.components['lr'].name, flow.components['lr'].flow_id))
+        self.assertEqual(
+            flow.upload_date,
+            flow.components['lr'].upload_date,
+            msg=(
+                flow.name,
+                flow.flow_id,
+                flow.components['lr'].name, flow.components['lr'].flow_id,
+            ),
+        )
 
         clf1 = sklearn.tree.DecisionTreeClassifier(max_depth=2)
-        flow1 = openml.flows.sklearn_to_flow(clf1)
+        flow1 = self.extension.model_to_flow(clf1)
         flow1, sentinel = self._add_sentinel_to_flow_name(flow1, None)
         flow1.publish()
 
         # In order to assign different upload times to the flows!
         time.sleep(1)
 
         clf2 = sklearn.ensemble.VotingClassifier(
             [('dt', sklearn.tree.DecisionTreeClassifier(max_depth=2))])
-        flow2 = openml.flows.sklearn_to_flow(clf2)
+        flow2 = self.extension.model_to_flow(clf2)
         flow2, _ = self._add_sentinel_to_flow_name(flow2, sentinel)
         flow2.publish()
         # If one component was published before the other, the components in
         # the flow should have different upload dates
         self.assertNotEqual(flow2.upload_date,
                             flow2.components['dt'].upload_date)
 
         clf3 = sklearn.ensemble.AdaBoostClassifier(
             sklearn.tree.DecisionTreeClassifier(max_depth=3))
-        flow3 = openml.flows.sklearn_to_flow(clf3)
+        flow3 = self.extension.model_to_flow(clf3)
         flow3, _ = self._add_sentinel_to_flow_name(flow3, sentinel)
         # Child flow has different parameter. Check for storing the flow
         # correctly on the server should thus not check the child's parameters!
         flow3.publish()
 
     def test_semi_legal_flow(self):
         # TODO: Test if parameters are set correctly!
-        # should not throw error as it contains two differentiable forms of Bagging
-        # i.e., Bagging(Bagging(J48)) and Bagging(J48)
+        # should not throw error as it contains two differentiable forms of
+        # Bagging i.e., Bagging(Bagging(J48)) and Bagging(J48)
         semi_legal = sklearn.ensemble.BaggingClassifier(
             base_estimator=sklearn.ensemble.BaggingClassifier(
                 base_estimator=sklearn.tree.DecisionTreeClassifier()))
-        flow = openml.flows.sklearn_to_flow(semi_legal)
+        flow = self.extension.model_to_flow(semi_legal)
         flow, _ = self._add_sentinel_to_flow_name(flow, None)
 
         flow.publish()
 
     @mock.patch('openml.flows.functions.get_flow')
+    @mock.patch('openml.flows.functions.flow_exists')
     @mock.patch('openml._api_calls._perform_api_call')
-    def test_publish_error(self, api_call_mock, get_flow_mock):
+    def test_publish_error(self, api_call_mock, flow_exists_mock, get_flow_mock):
         model = sklearn.ensemble.RandomForestClassifier()
-        flow = openml.flows.sklearn_to_flow(model)
+        flow = self.extension.model_to_flow(model)
         api_call_mock.return_value = "<oml:upload_flow>\n" \
                                      "    <oml:id>1</oml:id>\n" \
                                      "</oml:upload_flow>"
+        flow_exists_mock.return_value = False
         get_flow_mock.return_value = flow
 
         flow.publish()
         self.assertEqual(api_call_mock.call_count, 1)
         self.assertEqual(get_flow_mock.call_count, 1)
+        self.assertEqual(flow_exists_mock.call_count, 1)
 
         flow_copy = copy.deepcopy(flow)
         flow_copy.name = flow_copy.name[:-1]
         get_flow_mock.return_value = flow_copy
+        flow_exists_mock.return_value = 1
 
         with self.assertRaises(ValueError) as context_manager:
             flow.publish()
 
-        fixture = "Flow was not stored correctly on the server. " \
-                  "New flow ID is 1. Please check manually and remove " \
-                  "the flow if necessary! Error is:\n" \
-                  "'Flow sklearn.ensemble.forest.RandomForestClassifier: values for attribute 'name' differ: " \
-                  "'sklearn.ensemble.forest.RandomForestClassifier'" \
-                  "\nvs\n'sklearn.ensemble.forest.RandomForestClassifie'.'"
+        fixture = (
+            "Flow was not stored correctly on the server. "
+            "New flow ID is 1. Please check manually and remove "
+            "the flow if necessary! Error is:\n"
+            "'Flow sklearn.ensemble.forest.RandomForestClassifier: "
+            "values for attribute 'name' differ: "
+            "'sklearn.ensemble.forest.RandomForestClassifier'"
+            "\nvs\n'sklearn.ensemble.forest.RandomForestClassifie'.'"
+        )
 
         self.assertEqual(context_manager.exception.args[0], fixture)
-        self.assertEqual(api_call_mock.call_count, 2)
         self.assertEqual(get_flow_mock.call_count, 2)
 
     def test_illegal_flow(self):
         # should throw error as it contains two imputers
-        illegal = sklearn.pipeline.Pipeline(steps=[('imputer1', Imputer()),
-                                                   ('imputer2', Imputer()),
-                                                   ('classif', sklearn.tree.DecisionTreeClassifier())])
-        self.assertRaises(ValueError, openml.flows.sklearn_to_flow, illegal)
+        illegal = sklearn.pipeline.Pipeline(
+            steps=[
+                ('imputer1', Imputer()),
+                ('imputer2', Imputer()),
+                ('classif', sklearn.tree.DecisionTreeClassifier())
+            ]
+        )
+        self.assertRaises(ValueError, self.extension.model_to_flow, illegal)
 
     def test_nonexisting_flow_exists(self):
         def get_sentinel():
-            # Create a unique prefix for the flow. Necessary because the flow is
-            # identified by its name and external version online. Having a unique
-            #  name allows us to publish the same flow in each test run
+            # Create a unique prefix for the flow. Necessary because the flow
+            # is identified by its name and external version online. Having a
+            # unique name allows us to publish the same flow in each test run
             md5 = hashlib.md5()
             md5.update(str(time.time()).encode('utf-8'))
             sentinel = md5.hexdigest()[:10]
             sentinel = 'TEST%s' % sentinel
             return sentinel
 
         name = get_sentinel() + get_sentinel()
@@ -286,31 +316,39 @@
     def test_existing_flow_exists(self):
         # create a flow
         nb = sklearn.naive_bayes.GaussianNB()
 
         ohe_params = {'sparse': False, 'handle_unknown': 'ignore'}
         if LooseVersion(sklearn.__version__) >= '0.20':
             ohe_params['categories'] = 'auto'
-        steps = [('imputation', Imputer(strategy='median')),
-                 ('hotencoding', sklearn.preprocessing.OneHotEncoder(**ohe_params)),
-                 ('variencethreshold', sklearn.feature_selection.VarianceThreshold()),
-                 ('classifier', sklearn.tree.DecisionTreeClassifier())]
+        steps = [
+            ('imputation', Imputer(strategy='median')),
+            ('hotencoding', sklearn.preprocessing.OneHotEncoder(**ohe_params)),
+            (
+                'variencethreshold',
+                sklearn.feature_selection.VarianceThreshold(),
+            ),
+            ('classifier', sklearn.tree.DecisionTreeClassifier())
+        ]
         complicated = sklearn.pipeline.Pipeline(steps=steps)
 
         for classifier in [nb, complicated]:
-            flow = openml.flows.sklearn_to_flow(classifier)
+            flow = self.extension.model_to_flow(classifier)
             flow, _ = self._add_sentinel_to_flow_name(flow, None)
             # publish the flow
             flow = flow.publish()
             # redownload the flow
             flow = openml.flows.get_flow(flow.flow_id)
 
             # check if flow exists can find it
             flow = openml.flows.get_flow(flow.flow_id)
-            downloaded_flow_id = openml.flows.flow_exists(flow.name, flow.external_version)
+            downloaded_flow_id = openml.flows.flow_exists(
+                flow.name,
+                flow.external_version,
+            )
             self.assertEqual(downloaded_flow_id, flow.flow_id)
 
     def test_sklearn_to_upload_to_flow(self):
         iris = sklearn.datasets.load_iris()
         X = iris.data
         y = iris.target
 
@@ -323,24 +361,32 @@
         pca = sklearn.decomposition.TruncatedSVD()
         fs = sklearn.feature_selection.SelectPercentile(
             score_func=sklearn.feature_selection.f_classif, percentile=30)
         fu = sklearn.pipeline.FeatureUnion(transformer_list=[
             ('pca', pca), ('fs', fs)])
         boosting = sklearn.ensemble.AdaBoostClassifier(
             base_estimator=sklearn.tree.DecisionTreeClassifier())
-        model = sklearn.pipeline.Pipeline(steps=[('ohe', ohe), ('scaler', scaler),
-                                                 ('fu', fu), ('boosting', boosting)])
-        parameter_grid = {'boosting__n_estimators': [1, 5, 10, 100],
-                          'boosting__learning_rate': scipy.stats.uniform(0.01, 0.99),
-                          'boosting__base_estimator__max_depth': scipy.stats.randint(1, 10)}
+        model = sklearn.pipeline.Pipeline(
+            steps=[
+                ('ohe', ohe),
+                ('scaler', scaler),
+                ('fu', fu),
+                ('boosting', boosting),
+            ]
+        )
+        parameter_grid = {
+            'boosting__n_estimators': [1, 5, 10, 100],
+            'boosting__learning_rate': scipy.stats.uniform(0.01, 0.99),
+            'boosting__base_estimator__max_depth': scipy.stats.randint(1, 10),
+        }
         cv = sklearn.model_selection.StratifiedKFold(n_splits=5, shuffle=True)
         rs = sklearn.model_selection.RandomizedSearchCV(
             estimator=model, param_distributions=parameter_grid, cv=cv)
         rs.fit(X, y)
-        flow = openml.flows.sklearn_to_flow(rs)
+        flow = self.extension.model_to_flow(rs)
         # Tags may be sorted in any order (by the server). Just using one tag
         # makes sure that the xml comparison does not fail because of that.
         subflows = [flow]
         while len(subflows) > 0:
             f = subflows.pop()
             f.tags = []
             subflows.extend(list(f.components.values()))
@@ -349,49 +395,57 @@
 
         flow.publish()
         self.assertIsInstance(flow.flow_id, int)
 
         # Check whether we can load the flow again
         # Remove the sentinel from the name again so that we can reinstantiate
         # the object again
-        new_flow = openml.flows.get_flow(flow_id=flow.flow_id,
-                                         reinstantiate=True)
+        new_flow = openml.flows.get_flow(flow_id=flow.flow_id, reinstantiate=True)
 
         local_xml = flow._to_xml()
         server_xml = new_flow._to_xml()
 
         for i in range(10):
             # Make sure that we replace all occurences of two newlines
             local_xml = local_xml.replace(sentinel, '')
-            local_xml = local_xml.replace('  ', '').replace('\t', '').strip().replace('\n\n', '\n').replace('&quot;', '"')
+            local_xml = (
+                local_xml.replace('  ', '').replace('\t', '').
+                strip().replace('\n\n', '\n').replace('&quot;', '"')
+            )
             local_xml = re.sub(r'(^$)', '', local_xml)
             server_xml = server_xml.replace(sentinel, '')
-            server_xml = server_xml.replace('  ', '').replace('\t', '').strip().replace('\n\n', '\n').replace('&quot;', '"')
+            server_xml = (
+                server_xml.replace('  ', '').replace('\t', '').
+                strip().replace('\n\n', '\n').replace('&quot;', '"')
+            )
             server_xml = re.sub(r'^$', '', server_xml)
 
         self.assertEqual(server_xml, local_xml)
 
         # Would raise exception if they are not equal!
         openml.flows.functions.assert_flows_equal(new_flow, flow)
         self.assertIsNot(new_flow, flow)
 
         # OneHotEncoder was moved to _encoders module in 0.20
         module_name_encoder = ('_encoders'
                                if LooseVersion(sklearn.__version__) >= "0.20"
                                else 'data')
-        fixture_name = '%ssklearn.model_selection._search.RandomizedSearchCV(' \
-                       'estimator=sklearn.pipeline.Pipeline(' \
-                       'ohe=sklearn.preprocessing.%s.OneHotEncoder,' \
-                       'scaler=sklearn.preprocessing.data.StandardScaler,' \
-                       'fu=sklearn.pipeline.FeatureUnion(' \
-                       'pca=sklearn.decomposition.truncated_svd.TruncatedSVD,' \
-                       'fs=sklearn.feature_selection.univariate_selection.SelectPercentile),' \
-                       'boosting=sklearn.ensemble.weight_boosting.AdaBoostClassifier(' \
-                       'base_estimator=sklearn.tree.tree.DecisionTreeClassifier)))' \
-                        % (sentinel, module_name_encoder)
+        fixture_name = (
+            '%ssklearn.model_selection._search.RandomizedSearchCV('
+            'estimator=sklearn.pipeline.Pipeline('
+            'ohe=sklearn.preprocessing.%s.OneHotEncoder,'
+            'scaler=sklearn.preprocessing.data.StandardScaler,'
+            'fu=sklearn.pipeline.FeatureUnion('
+            'pca=sklearn.decomposition.truncated_svd.TruncatedSVD,'
+            'fs='
+            'sklearn.feature_selection.univariate_selection.SelectPercentile),'
+            'boosting=sklearn.ensemble.weight_boosting.AdaBoostClassifier('
+            'base_estimator=sklearn.tree.tree.DecisionTreeClassifier)))'
+            % (sentinel, module_name_encoder)
+        )
         self.assertEqual(new_flow.name, fixture_name)
         new_flow.model.fit(X, y)
 
     def test_extract_tags(self):
         flow_xml = "<oml:tag>study_14</oml:tag>"
         flow_dict = xmltodict.parse(flow_xml)
         tags = openml.utils.extract_xml_tags('oml:tag', flow_dict)
```

### Comparing `openml-0.8.0/tests/test_flows/test_flow_functions.py` & `openml-0.9.0/tests/test_flows/test_flow_functions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 from collections import OrderedDict
 import copy
 import unittest
 
-import six
+from distutils.version import LooseVersion
+import sklearn
+import pandas as pd
 
 import openml
 from openml.testing import TestBase
+import openml.extensions.sklearn
 
 
 class TestFlowFunctions(TestBase):
     _multiprocess_can_split_ = True
 
     def _check_flow(self, flow):
         self.assertEqual(type(flow), dict)
         self.assertEqual(len(flow), 6)
         self.assertIsInstance(flow['id'], int)
-        self.assertIsInstance(flow['name'], six.string_types)
-        self.assertIsInstance(flow['full_name'], six.string_types)
-        self.assertIsInstance(flow['version'], six.string_types)
-        # There are some runs on openml.org that can have an empty external
-        # version
-        self.assertTrue(isinstance(flow['external_version'], six.string_types) or
-                        flow['external_version'] is None)
+        self.assertIsInstance(flow['name'], str)
+        self.assertIsInstance(flow['full_name'], str)
+        self.assertIsInstance(flow['version'], str)
+        # There are some runs on openml.org that can have an empty external version
+        ext_version_str_or_none = (isinstance(flow['external_version'], str)
+                                   or flow['external_version'] is None)
+        self.assertTrue(ext_version_str_or_none)
 
     def test_list_flows(self):
         openml.config.server = self.production_server
         # We can only perform a smoke test here because we test on dynamic
         # data from the internet...
         flows = openml.flows.list_flows()
         # 3000 as the number of flows on openml.org
         self.assertGreaterEqual(len(flows), 1500)
         for fid in flows:
             self._check_flow(flows[fid])
 
+    def test_list_flows_output_format(self):
+        openml.config.server = self.production_server
+        # We can only perform a smoke test here because we test on dynamic
+        # data from the internet...
+        flows = openml.flows.list_flows(output_format='dataframe')
+        self.assertIsInstance(flows, pd.DataFrame)
+        self.assertGreaterEqual(len(flows), 1500)
+
     def test_list_flows_empty(self):
         openml.config.server = self.production_server
         flows = openml.flows.list_flows(tag='NoOneEverUsesThisTag123')
         if len(flows) > 0:
-            raise ValueError('UnitTest Outdated, got somehow results (please adapt)')
+            raise ValueError(
+                'UnitTest Outdated, got somehow results (please adapt)'
+            )
 
         self.assertIsInstance(flows, dict)
 
     def test_list_flows_by_tag(self):
         openml.config.server = self.production_server
         flows = openml.flows.list_flows(tag='weka')
         self.assertGreaterEqual(len(flows), 5)
         for did in flows:
             self._check_flow(flows[did])
 
     def test_list_flows_paginate(self):
         openml.config.server = self.production_server
         size = 10
-        max = 100
-        for i in range(0, max, size):
+        maximum = 100
+        for i in range(0, maximum, size):
             flows = openml.flows.list_flows(offset=i, size=size)
             self.assertGreaterEqual(size, len(flows))
             for did in flows:
                 self._check_flow(flows[did])
 
     def test_are_flows_equal(self):
         flow = openml.flows.OpenMLFlow(name='Test',
@@ -79,32 +92,42 @@
                                      ('external_version', '2'),
                                      ('language', 'english'),
                                      ('dependencies', 'ab'),
                                      ('class_name', 'Tes'),
                                      ('custom_name', 'Tes')]:
             new_flow = copy.deepcopy(flow)
             setattr(new_flow, attribute, new_value)
-            self.assertNotEqual(getattr(flow, attribute), getattr(new_flow, attribute))
-            self.assertRaises(ValueError, openml.flows.functions.assert_flows_equal,
-                              flow, new_flow)
+            self.assertNotEqual(
+                getattr(flow, attribute),
+                getattr(new_flow, attribute),
+            )
+            self.assertRaises(
+                ValueError,
+                openml.flows.functions.assert_flows_equal,
+                flow,
+                new_flow,
+            )
 
         # Test that the API ignores several keys when comparing flows
         openml.flows.functions.assert_flows_equal(flow, flow)
         for attribute, new_value in [('flow_id', 1),
                                      ('uploader', 1),
                                      ('version', 1),
                                      ('upload_date', '18.12.1988'),
                                      ('binary_url', 'openml.org'),
                                      ('binary_format', 'gzip'),
                                      ('binary_md5', '12345'),
                                      ('model', []),
                                      ('tags', ['abc', 'de'])]:
             new_flow = copy.deepcopy(flow)
             setattr(new_flow, attribute, new_value)
-            self.assertNotEqual(getattr(flow, attribute), getattr(new_flow, attribute))
+            self.assertNotEqual(
+                getattr(flow, attribute),
+                getattr(new_flow, attribute),
+            )
             openml.flows.functions.assert_flows_equal(flow, new_flow)
 
         # Now test for parameters
         flow.parameters['abc'] = 1.0
         flow.parameters['def'] = 2.0
         openml.flows.functions.assert_flows_equal(flow, flow)
         new_flow = copy.deepcopy(flow)
@@ -126,84 +149,110 @@
                           openml.flows.functions.assert_flows_equal,
                           parent_flow, new_flow)
 
     def test_are_flows_equal_ignore_parameter_values(self):
         paramaters = OrderedDict((('a', 5), ('b', 6)))
         parameters_meta_info = OrderedDict((('a', None), ('b', None)))
 
-        flow = openml.flows.OpenMLFlow(name='Test',
-                                       description='Test flow',
-                                       model=None,
-                                       components=OrderedDict(),
-                                       parameters=paramaters,
-                                       parameters_meta_info=parameters_meta_info,
-                                       external_version='1',
-                                       tags=['abc', 'def'],
-                                       language='English',
-                                       dependencies='abc',
-                                       class_name='Test',
-                                       custom_name='Test')
+        flow = openml.flows.OpenMLFlow(
+            name='Test',
+            description='Test flow',
+            model=None,
+            components=OrderedDict(),
+            parameters=paramaters,
+            parameters_meta_info=parameters_meta_info,
+            external_version='1',
+            tags=['abc', 'def'],
+            language='English',
+            dependencies='abc',
+            class_name='Test',
+            custom_name='Test',
+        )
 
         openml.flows.functions.assert_flows_equal(flow, flow)
         openml.flows.functions.assert_flows_equal(flow, flow,
                                                   ignore_parameter_values=True)
 
         new_flow = copy.deepcopy(flow)
         new_flow.parameters['a'] = 7
-        self.assertRaisesRegexp(ValueError, "values for attribute 'parameters' "
-                                            "differ: 'OrderedDict\(\[\('a', "
-                                            "5\), \('b', 6\)\]\)'\nvs\n"
-                                            "'OrderedDict\(\[\('a', 7\), "
-                                            "\('b', 6\)\]\)'",
-                                openml.flows.functions.assert_flows_equal,
-                                flow, new_flow)
+        self.assertRaisesRegex(
+            ValueError,
+            r"values for attribute 'parameters' differ: "
+            r"'OrderedDict\(\[\('a', 5\), \('b', 6\)\]\)'\nvs\n"
+            r"'OrderedDict\(\[\('a', 7\), \('b', 6\)\]\)'",
+            openml.flows.functions.assert_flows_equal,
+            flow, new_flow,
+        )
         openml.flows.functions.assert_flows_equal(flow, new_flow,
                                                   ignore_parameter_values=True)
 
         del new_flow.parameters['a']
-        self.assertRaisesRegexp(ValueError, "values for attribute 'parameters' "
-                                            "differ: 'OrderedDict\(\[\('a', "
-                                            "5\), \('b', 6\)\]\)'\nvs\n"
-                                            "'OrderedDict\(\[\('b', 6\)\]\)'",
-                                openml.flows.functions.assert_flows_equal,
-                                flow, new_flow)
-        self.assertRaisesRegexp(ValueError, "Flow Test: parameter set of flow "
-                                            "differs from the parameters stored "
-                                            "on the server.",
-                                openml.flows.functions.assert_flows_equal,
-                                flow, new_flow, ignore_parameter_values=True)
+        self.assertRaisesRegex(
+            ValueError,
+            r"values for attribute 'parameters' differ: "
+            r"'OrderedDict\(\[\('a', 5\), \('b', 6\)\]\)'\nvs\n"
+            r"'OrderedDict\(\[\('b', 6\)\]\)'",
+            openml.flows.functions.assert_flows_equal,
+            flow, new_flow,
+        )
+        self.assertRaisesRegex(
+            ValueError,
+            r"Flow Test: parameter set of flow differs from the parameters "
+            r"stored on the server.",
+            openml.flows.functions.assert_flows_equal,
+            flow, new_flow, ignore_parameter_values=True,
+        )
 
     def test_are_flows_equal_ignore_if_older(self):
         paramaters = OrderedDict((('a', 5), ('b', 6)))
         parameters_meta_info = OrderedDict((('a', None), ('b', None)))
+        flow_upload_date = '2017-01-31T12-01-01'
+        assert_flows_equal = openml.flows.functions.assert_flows_equal
 
         flow = openml.flows.OpenMLFlow(name='Test',
                                        description='Test flow',
                                        model=None,
                                        components=OrderedDict(),
                                        parameters=paramaters,
                                        parameters_meta_info=parameters_meta_info,
                                        external_version='1',
                                        tags=['abc', 'def'],
                                        language='English',
                                        dependencies='abc',
                                        class_name='Test',
                                        custom_name='Test',
-                                       upload_date='2017-01-31T12-01-01')
+                                       upload_date=flow_upload_date)
 
-        openml.flows.functions.assert_flows_equal(flow, flow,
-                                                  ignore_parameter_values_on_older_children='2017-01-31T12-01-01')
-        openml.flows.functions.assert_flows_equal(flow, flow,
-                                                  ignore_parameter_values_on_older_children=None)
+        assert_flows_equal(flow, flow, ignore_parameter_values_on_older_children=flow_upload_date)
+        assert_flows_equal(flow, flow, ignore_parameter_values_on_older_children=None)
         new_flow = copy.deepcopy(flow)
         new_flow.parameters['a'] = 7
-        self.assertRaises(ValueError, openml.flows.functions.assert_flows_equal,
-                          flow, new_flow, ignore_parameter_values_on_older_children='2017-01-31T12-01-01')
-        self.assertRaises(ValueError, openml.flows.functions.assert_flows_equal,
-                          flow, new_flow, ignore_parameter_values_on_older_children=None)
+        self.assertRaises(ValueError, assert_flows_equal, flow, new_flow,
+                          ignore_parameter_values_on_older_children=flow_upload_date)
+        self.assertRaises(ValueError, assert_flows_equal, flow, new_flow,
+                          ignore_parameter_values_on_older_children=None)
 
         new_flow.upload_date = '2016-01-31T12-01-01'
-        self.assertRaises(ValueError, openml.flows.functions.assert_flows_equal,
-                          flow, new_flow,
-                          ignore_parameter_values_on_older_children='2017-01-31T12-01-01')
-        openml.flows.functions.assert_flows_equal(flow, flow,
-                                                  ignore_parameter_values_on_older_children=None)
+        self.assertRaises(ValueError, assert_flows_equal, flow, new_flow,
+                          ignore_parameter_values_on_older_children=flow_upload_date)
+        assert_flows_equal(flow, flow, ignore_parameter_values_on_older_children=None)
+
+    @unittest.skipIf(LooseVersion(sklearn.__version__) < "0.20",
+                     reason="OrdinalEncoder introduced in 0.20. "
+                            "No known models with list of lists parameters in older versions.")
+    def test_sklearn_to_flow_list_of_lists(self):
+        from sklearn.preprocessing import OrdinalEncoder
+        ordinal_encoder = OrdinalEncoder(categories=[[0, 1], [0, 1]])
+
+        extension = openml.extensions.sklearn.SklearnExtension()
+
+        # Test serialization works
+        flow = extension.model_to_flow(ordinal_encoder)
+
+        # Test flow is accepted by server
+        self._add_sentinel_to_flow_name(flow)
+        flow.publish()
+
+        # Test deserialization works
+        server_flow = openml.flows.get_flow(flow.flow_id, reinstantiate=True)
+        self.assertEqual(server_flow.parameters['categories'], '[[0, 1], [0, 1]]')
+        self.assertEqual(server_flow.model.categories, flow.model.categories)
```

### Comparing `openml-0.8.0/tests/test_runs/test_run.py` & `openml-0.9.0/tests/test_runs/test_run.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import numpy as np
 import random
 import os
 from time import time
 
 from sklearn.dummy import DummyClassifier
 from sklearn.tree import DecisionTreeClassifier
-from sklearn.ensemble import RandomForestClassifier, AdaBoostClassifier
-from sklearn.linear_model import LogisticRegression
-from sklearn.model_selection import GridSearchCV, RandomizedSearchCV, StratifiedKFold
+from sklearn.model_selection import GridSearchCV
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import Imputer
 
 from openml.testing import TestBase
-from openml.flows.sklearn_converter import sklearn_to_flow
-from openml import OpenMLRun
 import openml
+import openml.extensions.sklearn
 
 
 class TestRun(TestBase):
     # Splitting not helpful, these test's don't rely on the server and take
     # less than 1 seconds
 
     def test_tagging(self):
@@ -34,29 +31,33 @@
         self.assertEqual(len(run_list), 1)
         self.assertIn(run_id, run_list)
         run.remove_tag(tag)
         run_list = openml.runs.list_runs(tag=tag)
         self.assertEqual(len(run_list), 0)
 
     def _test_run_obj_equals(self, run, run_prime):
-        for dictionary in ['evaluations', 'fold_evaluations', 'sample_evaluations']:
+        for dictionary in ['evaluations', 'fold_evaluations',
+                           'sample_evaluations']:
             if getattr(run, dictionary) is not None:
-                self.assertDictEqual(getattr(run, dictionary), getattr(run_prime, dictionary))
+                self.assertDictEqual(getattr(run, dictionary),
+                                     getattr(run_prime, dictionary))
             else:
                 # should be none or empty
                 other = getattr(run_prime, dictionary)
                 if other is not None:
                     self.assertDictEqual(other, dict())
-        self.assertEqual(run._create_description_xml(), run_prime._create_description_xml())
+        self.assertEqual(run._create_description_xml(),
+                         run_prime._create_description_xml())
 
-        numeric_part = np.array(np.array(run.data_content)[:, 0:-2], dtype=float)
-        numeric_part_prime = np.array(np.array(run_prime.data_content)[:, 0:-2], dtype=float)
+        numeric_part = \
+            np.array(np.array(run.data_content)[:, 0:-2], dtype=float)
+        numeric_part_prime = \
+            np.array(np.array(run_prime.data_content)[:, 0:-2], dtype=float)
         string_part = np.array(run.data_content)[:, -2:]
         string_part_prime = np.array(run_prime.data_content)[:, -2:]
-        # JvR: Python 2.7 requires an almost equal check, rather than an equals check
         np.testing.assert_array_almost_equal(numeric_part, numeric_part_prime)
         np.testing.assert_array_equal(string_part, string_part_prime)
 
         if run.trace is not None:
             run_trace_content = run.trace.trace_to_arff()['data']
         else:
             run_trace_content = None
@@ -88,93 +89,144 @@
             bool_part = [line[4] for line in run_trace_content]
             bool_part_prime = [line[4] for line in run_prime_trace_content]
             for bp, bpp in zip(bool_part, bool_part_prime):
                 self.assertIn(bp, ['true', 'false'])
                 self.assertIn(bpp, ['true', 'false'])
             string_part = np.array(run_trace_content)[:, 5:]
             string_part_prime = np.array(run_prime_trace_content)[:, 5:]
-            # JvR: Python 2.7 requires an almost equal check, rather than an
-            # equals check
+
             np.testing.assert_array_almost_equal(int_part, int_part_prime)
             np.testing.assert_array_almost_equal(float_part, float_part_prime)
             self.assertEqual(bool_part, bool_part_prime)
             np.testing.assert_array_equal(string_part, string_part_prime)
         else:
             self.assertIsNone(run_prime_trace_content)
 
     def test_to_from_filesystem_vanilla(self):
+
         model = Pipeline([
             ('imputer', Imputer(strategy='mean')),
             ('classifier', DecisionTreeClassifier(max_depth=1)),
         ])
         task = openml.tasks.get_task(119)
         run = openml.runs.run_model_on_task(
             model=model,
             task=task,
             add_local_measures=False,
+            avoid_duplicate_runs=False,
+            upload_flow=True
         )
 
         cache_path = os.path.join(
             self.workdir,
             'runs',
             str(random.getrandbits(128)),
         )
         run.to_filesystem(cache_path)
 
         run_prime = openml.runs.OpenMLRun.from_filesystem(cache_path)
+        # The flow has been uploaded to server, so only the reference flow_id should be present
+        self.assertTrue(run_prime.flow_id is not None)
+        self.assertTrue(run_prime.flow is None)
         self._test_run_obj_equals(run, run_prime)
         run_prime.publish()
 
     def test_to_from_filesystem_search(self):
+
         model = Pipeline([
             ('imputer', Imputer(strategy='mean')),
             ('classifier', DecisionTreeClassifier(max_depth=1)),
         ])
         model = GridSearchCV(
             estimator=model,
             param_grid={
                 "classifier__max_depth": [1, 2, 3, 4, 5],
                 "imputer__strategy": ['mean', 'median'],
             }
         )
 
         task = openml.tasks.get_task(119)
         run = openml.runs.run_model_on_task(
-            model,
-            task,
+            model=model,
+            task=task,
             add_local_measures=False,
+            avoid_duplicate_runs=False,
         )
 
         cache_path = os.path.join(
             self.workdir,
             'runs',
             str(random.getrandbits(128)),
         )
         run.to_filesystem(cache_path)
 
         run_prime = openml.runs.OpenMLRun.from_filesystem(cache_path)
         self._test_run_obj_equals(run, run_prime)
         run_prime.publish()
 
     def test_to_from_filesystem_no_model(self):
+
         model = Pipeline([
             ('imputer', Imputer(strategy='mean')),
             ('classifier', DummyClassifier()),
         ])
         task = openml.tasks.get_task(119)
         run = openml.runs.run_model_on_task(
-            task,
-            model,
+            model=model,
+            task=task,
             add_local_measures=False,
         )
 
         cache_path = os.path.join(
             self.workdir,
             'runs',
             str(random.getrandbits(128)),
         )
         run.to_filesystem(cache_path, store_model=False)
         # obtain run from filesystem
         openml.runs.OpenMLRun.from_filesystem(cache_path, expect_model=False)
         # assert default behaviour is throwing an error
         with self.assertRaises(ValueError, msg='Could not find model.pkl'):
             openml.runs.OpenMLRun.from_filesystem(cache_path)
+
+    def test_publish_with_local_loaded_flow(self):
+        """
+        Publish a run tied to a local flow after it has first been saved to
+         and loaded from disk.
+        """
+        extension = openml.extensions.sklearn.SklearnExtension()
+
+        model = Pipeline([
+            ('imputer', Imputer(strategy='mean')),
+            ('classifier', DummyClassifier()),
+        ])
+        task = openml.tasks.get_task(119)
+
+        # Make sure the flow does not exist on the server yet.
+        flow = extension.model_to_flow(model)
+        self._add_sentinel_to_flow_name(flow)
+        self.assertFalse(openml.flows.flow_exists(flow.name, flow.external_version))
+
+        run = openml.runs.run_flow_on_task(
+            flow=flow,
+            task=task,
+            add_local_measures=False,
+            avoid_duplicate_runs=False,
+            upload_flow=False
+        )
+
+        # Make sure that the flow has not been uploaded as requested.
+        self.assertFalse(openml.flows.flow_exists(flow.name, flow.external_version))
+
+        cache_path = os.path.join(
+            self.workdir,
+            'runs',
+            str(random.getrandbits(128)),
+        )
+        run.to_filesystem(cache_path)
+        # obtain run from filesystem
+        loaded_run = openml.runs.OpenMLRun.from_filesystem(cache_path)
+        loaded_run.publish()
+
+        # make sure the flow is published as part of publishing the run.
+        self.assertTrue(openml.flows.flow_exists(flow.name, flow.external_version))
+        openml.runs.get_run(loaded_run.run_id)
```

### Comparing `openml-0.8.0/tests/test_runs/test_run_functions.py` & `openml-0.9.0/tests/test_runs/test_run_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,114 +1,134 @@
 import arff
-import collections
 from distutils.version import LooseVersion
-import json
 import os
 import random
 import time
 import sys
+import unittest.mock
 
 import numpy as np
 
 import openml
 import openml.exceptions
 import openml._api_calls
 import sklearn
 import unittest
+import warnings
+import pandas as pd
 
+import openml.extensions.sklearn
 from openml.testing import TestBase
-from openml.runs.functions import _run_task_get_arffcontent, \
-    _get_seeded_model, _run_exists, _extract_arfftrace, \
-    _extract_arfftrace_attributes, _prediction_to_row, _check_n_jobs
-from openml.flows.sklearn_converter import sklearn_to_flow
+from openml.runs.functions import (
+    _run_task_get_arffcontent,
+    run_exists,
+)
 from openml.runs.trace import OpenMLRunTrace
+from openml.tasks import TaskTypeEnum
 
 from sklearn.naive_bayes import GaussianNB
 from sklearn.model_selection._search import BaseSearchCV
-from sklearn.tree import DecisionTreeClassifier, ExtraTreeClassifier
+from sklearn.tree import DecisionTreeClassifier
 from sklearn.preprocessing.imputation import Imputer
 from sklearn.dummy import DummyClassifier
 from sklearn.preprocessing import StandardScaler
 from sklearn.feature_selection import VarianceThreshold
 from sklearn.linear_model import LogisticRegression, SGDClassifier, \
     LinearRegression
-from sklearn.neural_network import MLPClassifier
 from sklearn.ensemble import RandomForestClassifier, BaggingClassifier
-from sklearn.svm import SVC, LinearSVC
+from sklearn.svm import SVC
 from sklearn.model_selection import RandomizedSearchCV, GridSearchCV, \
     StratifiedKFold
 from sklearn.pipeline import Pipeline
 
 
-class HardNaiveBayes(GaussianNB):
-    # class for testing a naive bayes classifier that does not allow soft predictions
-    def __init__(self, priors=None):
-        super(HardNaiveBayes, self).__init__(priors)
-
-    def predict_proba(*args, **kwargs):
-        raise AttributeError('predict_proba is not available when  probability=False')
-
-
 class TestRun(TestBase):
     _multiprocess_can_split_ = True
     # diabetis dataset, 768 observations, 0 missing vals, 33% holdout set
     # (253 test obs), no nominal attributes, all numeric attributes
     TEST_SERVER_TASK_SIMPLE = (119, 0, 253, list(), list(range(8)))
-    # creadit-a dataset, 690 observations, 67 missing vals, 33% holdout set
+    TEST_SERVER_TASK_REGRESSION = (738, 0, 718, list(), list(range(8)))
+    # credit-a dataset, 690 observations, 67 missing vals, 33% holdout set
     # (227 test obs)
     TEST_SERVER_TASK_MISSING_VALS = (96, 67, 227,
                                      [0, 3, 4, 5, 6, 8, 9, 11, 12],
                                      [1, 2, 7, 10, 13, 14])
 
+    # Suppress warnings to facilitate testing
+    hide_warnings = True
+    if hide_warnings:
+        warnings.filterwarnings("ignore", category=DeprecationWarning)
+        warnings.filterwarnings("ignore", category=FutureWarning)
+        warnings.filterwarnings("ignore", category=UserWarning)
+
+    def setUp(self):
+        super().setUp()
+        self.extension = openml.extensions.sklearn.SklearnExtension()
+
     def _wait_for_processed_run(self, run_id, max_waiting_time_seconds):
-        # it can take a while for a run to be processed on the OpenML (test) server
-        # however, sometimes it is good to wait (a bit) for this, to properly test
-        # a function. In this case, we wait for max_waiting_time_seconds on this
-        # to happen, probing the server every 10 seconds to speed up the process
+        # it can take a while for a run to be processed on the OpenML (test)
+        # server however, sometimes it is good to wait (a bit) for this, to
+        # properly test a function. In this case, we wait for max_waiting_time_
+        # seconds on this to happen, probing the server every 10 seconds to
+        # speed up the process
 
         # time.time() works in seconds
         start_time = time.time()
         while time.time() - start_time < max_waiting_time_seconds:
-            run = openml.runs.get_run(run_id)
+            run = openml.runs.get_run(run_id, ignore_cache=True)
             if len(run.evaluations) > 0:
                 return
             else:
                 time.sleep(10)
+        raise RuntimeError('Could not find any evaluations! Please check whether run {} was '
+                           'evaluated correctly on the server'.format(run_id))
 
     def _compare_predictions(self, predictions, predictions_prime):
         self.assertEqual(np.array(predictions_prime['data']).shape,
                          np.array(predictions['data']).shape)
 
         # The original search model does not submit confidence
         # bounds, so we can not compare the arff line
         compare_slice = [0, 1, 2, -1, -2]
         for idx in range(len(predictions['data'])):
             # depends on the assumption "predictions are in same order"
             # that does not necessarily hold.
             # But with the current code base, it holds.
             for col_idx in compare_slice:
-                self.assertEqual(predictions['data'][idx][col_idx],
-                                 predictions_prime['data'][idx][col_idx])
+                val_1 = predictions['data'][idx][col_idx]
+                val_2 = predictions_prime['data'][idx][col_idx]
+                if type(val_1) == float or type(val_2) == float:
+                    self.assertAlmostEqual(
+                        float(val_1),
+                        float(val_2),
+                        places=6,
+                    )
+                else:
+                    self.assertEqual(val_1, val_2)
 
         return True
 
     def _rerun_model_and_compare_predictions(self, run_id, model_prime, seed):
         run = openml.runs.get_run(run_id)
         task = openml.tasks.get_task(run.task_id)
 
         # TODO: assert holdout task
 
         # downloads the predictions of the old task
         file_id = run.output_files['predictions']
         predictions_url = openml._api_calls._file_id_to_url(file_id)
-        predictions = arff.loads(openml._api_calls._read_url(predictions_url))
-
-        run_prime = openml.runs.run_model_on_task(model_prime, task,
-                                                  avoid_duplicate_runs=False,
-                                                  seed=seed)
+        response = openml._api_calls._read_url(predictions_url,
+                                               request_method='get')
+        predictions = arff.loads(response)
+        run_prime = openml.runs.run_model_on_task(
+            model=model_prime,
+            task=task,
+            avoid_duplicate_runs=False,
+            seed=seed,
+        )
         predictions_prime = run_prime._generate_arff_dict()
 
         self._compare_predictions(predictions, predictions_prime)
 
     def _perform_run(self, task_id, num_instances, n_missing_vals, clf,
                      flow_expected_rsv=None, seed=1, check_setup=True,
                      sentinel=None):
@@ -146,32 +166,39 @@
         Returns:
         --------
         run: OpenMLRun
             The performed run (with run id)
         """
         classes_without_random_state = \
             ['sklearn.model_selection._search.GridSearchCV',
-             'sklearn.pipeline.Pipeline']
+             'sklearn.pipeline.Pipeline',
+             'sklearn.linear_model.base.LinearRegression',
+             ]
 
         def _remove_random_state(flow):
             if 'random_state' in flow.parameters:
                 del flow.parameters['random_state']
             for component in flow.components.values():
                 _remove_random_state(component)
 
-        flow = sklearn_to_flow(clf)
+        flow = self.extension.model_to_flow(clf)
         flow, _ = self._add_sentinel_to_flow_name(flow, sentinel)
         if not openml.flows.flow_exists(flow.name, flow.external_version):
             flow.publish()
 
         task = openml.tasks.get_task(task_id)
+
         X, y = task.get_X_and_y()
         self.assertEqual(np.count_nonzero(np.isnan(X)), n_missing_vals)
-        run = openml.runs.run_flow_on_task(flow, task, seed=seed,
-                                           avoid_duplicate_runs=openml.config.avoid_duplicate_runs)
+        run = openml.runs.run_flow_on_task(
+            flow=flow,
+            task=task,
+            seed=seed,
+            avoid_duplicate_runs=openml.config.avoid_duplicate_runs,
+        )
         run_ = run.publish()
         self.assertEqual(run_, run)
         self.assertIsInstance(run.dataset_id, int)
 
         # This is only a smoke check right now
         # TODO add a few asserts here
         run._create_description_xml()
@@ -183,217 +210,192 @@
         # check arff output
         self.assertEqual(len(run.data_content), num_instances)
 
         if check_setup:
             # test the initialize setup function
             run_id = run_.run_id
             run_server = openml.runs.get_run(run_id)
-            clf_server = openml.setups.initialize_model(run_server.setup_id)
-            flow_local = openml.flows.sklearn_to_flow(clf)
-            flow_server = openml.flows.sklearn_to_flow(clf_server)
+            clf_server = openml.setups.initialize_model(
+                setup_id=run_server.setup_id,
+            )
+            flow_local = self.extension.model_to_flow(clf)
+            flow_server = self.extension.model_to_flow(clf_server)
 
             if flow.class_name not in classes_without_random_state:
-                error_msg = 'Flow class %s (id=%d) does not have a random state parameter' % (flow.class_name, flow.flow_id)
+                error_msg = 'Flow class %s (id=%d) does not have a random ' \
+                            'state parameter' % (flow.class_name, flow.flow_id)
                 self.assertIn('random_state', flow.parameters, error_msg)
-                # If the flow is initialized from a model without a random state,
-                # the flow is on the server without any random state
+                # If the flow is initialized from a model without a random
+                # state, the flow is on the server without any random state
                 self.assertEqual(flow.parameters['random_state'], 'null')
                 # As soon as a flow is run, a random state is set in the model.
                 # If a flow is re-instantiated
                 self.assertEqual(flow_local.parameters['random_state'],
                                  flow_expected_rsv)
                 self.assertEqual(flow_server.parameters['random_state'],
                                  flow_expected_rsv)
             _remove_random_state(flow_local)
             _remove_random_state(flow_server)
             openml.flows.assert_flows_equal(flow_local, flow_server)
 
             # and test the initialize setup from run function
-            clf_server2 = openml.runs.initialize_model_from_run(run_server.run_id)
-            flow_server2 = openml.flows.sklearn_to_flow(clf_server2)
+            clf_server2 = openml.runs.initialize_model_from_run(
+                run_id=run_server.run_id,
+            )
+            flow_server2 = self.extension.model_to_flow(clf_server2)
             if flow.class_name not in classes_without_random_state:
                 self.assertEqual(flow_server2.parameters['random_state'],
                                  flow_expected_rsv)
 
             _remove_random_state(flow_server2)
             openml.flows.assert_flows_equal(flow_local, flow_server2)
 
             # self.assertEqual(clf.get_params(), clf_prime.get_params())
             # self.assertEqual(clf, clf_prime)
 
         downloaded = openml.runs.get_run(run_.run_id)
-        assert('openml-python' in downloaded.tags)
+        assert ('openml-python' in downloaded.tags)
 
         # TODO make sure that these attributes are instantiated when
         # downloading a run? Or make sure that the trace object is created when
         # running a flow on a task (and not only the arff object is created,
         # so that the two objects can actually be compared):
         # downloaded_run_trace = downloaded._generate_trace_arff_dict()
         # self.assertEqual(run_trace, downloaded_run_trace)
         return run
 
-    def _check_fold_evaluations(self, fold_evaluations, num_repeats, num_folds, max_time_allowed=60000):
+    def _check_sample_evaluations(self, sample_evaluations, num_repeats,
+                                  num_folds, num_samples,
+                                  max_time_allowed=60000):
         """
-        Checks whether the right timing measures are attached to the run (before upload).
-        Test is only performed for versions >= Python3.3
+        Checks whether the right timing measures are attached to the run
+        (before upload). Test is only performed for versions >= Python3.3
 
-        In case of check_n_jobs(clf) == false, please do not perform this check (check this
-        condition outside of this function. )
-        default max_time_allowed (per fold, in milli seconds) = 1 minute, quite pessimistic
+        In case of check_n_jobs(clf) == false, please do not perform this
+        check (check this condition outside of this function. )
+        default max_time_allowed (per fold, in milli seconds) = 1 minute,
+        quite pessimistic
         """
 
-        # a dict mapping from openml measure to a tuple with the minimum and maximum allowed value
-        check_measures = {'usercpu_time_millis_testing': (0, max_time_allowed),
-                          'usercpu_time_millis_training': (0, max_time_allowed),  # should take at least one millisecond (?)
-                          'usercpu_time_millis': (0, max_time_allowed),
-                          'predictive_accuracy': (0, 1)}
-
-        self.assertIsInstance(fold_evaluations, dict)
-        if sys.version_info[:2] >= (3, 3):
-            # this only holds if we are allowed to record time (otherwise some are missing)
-            self.assertEqual(set(fold_evaluations.keys()), set(check_measures.keys()))
-
-        for measure in check_measures.keys():
-            if measure in fold_evaluations:
-                num_rep_entrees = len(fold_evaluations[measure])
-                self.assertEqual(num_rep_entrees, num_repeats)
-                min_val = check_measures[measure][0]
-                max_val = check_measures[measure][1]
-                for rep in range(num_rep_entrees):
-                    num_fold_entrees = len(fold_evaluations[measure][rep])
-                    self.assertEqual(num_fold_entrees, num_folds)
-                    for fold in range(num_fold_entrees):
-                        evaluation = fold_evaluations[measure][rep][fold]
-                        self.assertIsInstance(evaluation, float)
-                        self.assertGreaterEqual(evaluation, min_val)
-                        self.assertLessEqual(evaluation, max_val)
-
-    def _check_sample_evaluations(self, sample_evaluations, num_repeats, num_folds, num_samples, max_time_allowed=60000):
-        """
-        Checks whether the right timing measures are attached to the run (before upload).
-        Test is only performed for versions >= Python3.3
-
-        In case of check_n_jobs(clf) == false, please do not perform this check (check this
-        condition outside of this function. )
-        default max_time_allowed (per fold, in milli seconds) = 1 minute, quite pessimistic
-        """
-
-        # a dict mapping from openml measure to a tuple with the minimum and maximum allowed value
-        check_measures = {'usercpu_time_millis_testing': (0, max_time_allowed),
-                          'usercpu_time_millis_training': (0, max_time_allowed),  # should take at least one millisecond (?)
-                          'usercpu_time_millis': (0, max_time_allowed),
-                          'predictive_accuracy': (0, 1)}
+        # a dict mapping from openml measure to a tuple with the minimum and
+        # maximum allowed value
+        check_measures = {
+            # should take at least one millisecond (?)
+            'usercpu_time_millis_testing': (0, max_time_allowed),
+            'usercpu_time_millis_training': (0, max_time_allowed),
+            'usercpu_time_millis': (0, max_time_allowed),
+            'wall_clock_time_millis_training': (0, max_time_allowed),
+            'wall_clock_time_millis_testing': (0, max_time_allowed),
+            'wall_clock_time_millis': (0, max_time_allowed),
+            'predictive_accuracy': (0, 1)
+        }
 
         self.assertIsInstance(sample_evaluations, dict)
         if sys.version_info[:2] >= (3, 3):
-            # this only holds if we are allowed to record time (otherwise some are missing)
-            self.assertEqual(set(sample_evaluations.keys()), set(check_measures.keys()))
+            # this only holds if we are allowed to record time (otherwise some
+            # are missing)
+            self.assertEqual(set(sample_evaluations.keys()),
+                             set(check_measures.keys()))
 
         for measure in check_measures.keys():
             if measure in sample_evaluations:
                 num_rep_entrees = len(sample_evaluations[measure])
                 self.assertEqual(num_rep_entrees, num_repeats)
                 for rep in range(num_rep_entrees):
                     num_fold_entrees = len(sample_evaluations[measure][rep])
                     self.assertEqual(num_fold_entrees, num_folds)
                     for fold in range(num_fold_entrees):
-                        num_sample_entrees = len(sample_evaluations[measure][rep][fold])
+                        num_sample_entrees = len(
+                            sample_evaluations[measure][rep][fold])
                         self.assertEqual(num_sample_entrees, num_samples)
                         for sample in range(num_sample_entrees):
-                            evaluation = sample_evaluations[measure][rep][fold][sample]
+                            evaluation = sample_evaluations[measure][rep][
+                                fold][sample]
                             self.assertIsInstance(evaluation, float)
                             if not os.environ.get('CI_WINDOWS'):
                                 # Either Appveyor is much faster than Travis
                                 # and/or measurements are not as accurate.
-                                # Either way, windows seems to get an eval-time of 0 sometimes.
+                                # Either way, windows seems to get an eval-time
+                                # of 0 sometimes.
                                 self.assertGreater(evaluation, 0)
                             self.assertLess(evaluation, max_time_allowed)
 
     def test_run_regression_on_classif_task(self):
         task_id = 115
 
         clf = LinearRegression()
         task = openml.tasks.get_task(task_id)
-        self.assertRaises(AttributeError, openml.runs.run_model_on_task,
-                          model=clf, task=task, avoid_duplicate_runs=False)
+        with self.assertRaises(AttributeError):
+            openml.runs.run_model_on_task(
+                model=clf,
+                task=task,
+                avoid_duplicate_runs=False,
+            )
 
     def test_check_erronous_sklearn_flow_fails(self):
         task_id = 115
         task = openml.tasks.get_task(task_id)
 
         # Invalid parameter values
-        clf = LogisticRegression(C='abc')
-        self.assertRaisesRegexp(ValueError,
-                                "Penalty term must be positive; got "
-                                # u? for 2.7/3.4-6 compability
-                                "\(C=u?'abc'\)",
-                                openml.runs.run_model_on_task, task=task,
-                                model=clf)
-
-    def test__publish_flow_if_necessary(self):
-        task_id = 115
-        task = openml.tasks.get_task(task_id)
+        clf = LogisticRegression(C='abc', solver='lbfgs')
+        with self.assertRaisesRegex(
+            ValueError,
+            r"Penalty term must be positive; got \(C=u?'abc'\)",  # u? for 2.7/3.4-6 compability
+        ):
+            openml.runs.run_model_on_task(
+                task=task,
+                model=clf,
+            )
 
-        clf = LogisticRegression()
-        flow = sklearn_to_flow(clf)
-        flow, sentinel = self._add_sentinel_to_flow_name(flow, None)
-        openml.runs.functions._publish_flow_if_necessary(flow)
-        self.assertIsNotNone(flow.flow_id)
-
-        flow2 = sklearn_to_flow(clf)
-        flow2, _ = self._add_sentinel_to_flow_name(flow2, sentinel)
-        openml.runs.functions._publish_flow_if_necessary(flow2)
-        self.assertEqual(flow2.flow_id, flow.flow_id)
-
-    ############################################################################
-    # These unit tests are ment to test the following functions, using a varity
-    #  of flows:
+    ###########################################################################
+    # These unit tests are meant to test the following functions, using a
+    # variety of flows:
     # - openml.runs.run_task()
     # - openml.runs.OpenMLRun.publish()
     # - openml.runs.initialize_model()
     # - [implicitly] openml.setups.initialize_model()
     # - openml.runs.initialize_model_from_trace()
     # They're split among several actual functions to allow for parallel
     # execution of the unit tests without the need to add an additional module
     # like unittest2
 
     def _run_and_upload(self, clf, task_id, n_missing_vals, n_test_obs,
-                        flow_expected_rsv, sentinel=None):
+                        flow_expected_rsv, num_folds=1, num_iterations=5,
+                        seed=1, metric=sklearn.metrics.accuracy_score,
+                        metric_name='predictive_accuracy',
+                        task_type=TaskTypeEnum.SUPERVISED_CLASSIFICATION,
+                        sentinel=None):
         def determine_grid_size(param_grid):
             if isinstance(param_grid, dict):
                 grid_iterations = 1
                 for param in param_grid:
                     grid_iterations *= len(param_grid[param])
                 return grid_iterations
             elif isinstance(param_grid, list):
                 grid_iterations = 0
                 for sub_grid in param_grid:
                     grid_iterations += determine_grid_size(sub_grid)
                 return grid_iterations
             else:
                 raise TypeError('Param Grid should be of type list '
                                 '(GridSearch only) or dict')
-        seed = 1
-        num_folds = 1  # because of holdout
-        num_iterations = 5  # for base search classifiers
 
         run = self._perform_run(task_id, n_test_obs, n_missing_vals, clf,
                                 flow_expected_rsv=flow_expected_rsv, seed=seed,
                                 sentinel=sentinel)
 
-        # obtain accuracy scores using get_metric_score:
-        accuracy_scores = run.get_metric_fn(sklearn.metrics.accuracy_score)
+        # obtain scores using get_metric_score:
+        scores = run.get_metric_fn(metric)
         # compare with the scores in user defined measures
-        accuracy_scores_provided = []
-        for rep in run.fold_evaluations['predictive_accuracy'].keys():
-            for fold in run.fold_evaluations['predictive_accuracy'][rep].keys():
-                accuracy_scores_provided.append(
-                    run.fold_evaluations['predictive_accuracy'][rep][fold])
-
-        self.assertEqual(sum(accuracy_scores_provided), sum(accuracy_scores))
+        scores_provided = []
+        for rep in run.fold_evaluations[metric_name].keys():
+            for fold in run.fold_evaluations[metric_name][rep].keys():
+                scores_provided.append(
+                    run.fold_evaluations[metric_name][rep][fold])
+        self.assertEqual(sum(scores_provided), sum(scores))
 
         if isinstance(clf, BaseSearchCV):
             trace_content = run.trace.trace_to_arff()['data']
             if isinstance(clf, GridSearchCV):
                 grid_iterations = determine_grid_size(clf.param_grid)
                 self.assertEqual(len(trace_content),
                                  grid_iterations * num_folds)
@@ -404,48 +406,109 @@
             # downloads the best model based on the optimization trace
             # suboptimal (slow), and not guaranteed to work if evaluation
             # engine is behind.
             # TODO: mock this? We have the arff already on the server
             self._wait_for_processed_run(run.run_id, 200)
             try:
                 model_prime = openml.runs.initialize_model_from_trace(
-                    run.run_id, 0, 0)
+                    run_id=run.run_id,
+                    repeat=0,
+                    fold=0,
+                )
             except openml.exceptions.OpenMLServerException as e:
                 e.additional = "%s; run_id %d" % (e.additional, run.run_id)
                 raise e
 
             self._rerun_model_and_compare_predictions(run.run_id, model_prime,
                                                       seed)
         else:
             run_downloaded = openml.runs.get_run(run.run_id)
             sid = run_downloaded.setup_id
             model_prime = openml.setups.initialize_model(sid)
             self._rerun_model_and_compare_predictions(run.run_id,
                                                       model_prime, seed)
 
         # todo: check if runtime is present
-        self._check_fold_evaluations(run.fold_evaluations, 1, num_folds)
-        pass
+        self._check_fold_timing_evaluations(run.fold_evaluations, 1, num_folds,
+                                            task_type=task_type)
+        return run
+
+    def _run_and_upload_classification(self, clf, task_id, n_missing_vals,
+                                       n_test_obs, flow_expected_rsv,
+                                       sentinel=None):
+        num_folds = 1  # because of holdout
+        num_iterations = 5  # for base search algorithms
+        metric = sklearn.metrics.accuracy_score  # metric class
+        metric_name = 'predictive_accuracy'  # openml metric name
+        task_type = TaskTypeEnum.SUPERVISED_CLASSIFICATION  # task type
+
+        return self._run_and_upload(
+            clf=clf,
+            task_id=task_id,
+            n_missing_vals=n_missing_vals,
+            n_test_obs=n_test_obs,
+            flow_expected_rsv=flow_expected_rsv,
+            num_folds=num_folds,
+            num_iterations=num_iterations,
+            metric=metric,
+            metric_name=metric_name,
+            task_type=task_type,
+            sentinel=sentinel,
+        )
+
+    def _run_and_upload_regression(self, clf, task_id, n_missing_vals,
+                                   n_test_obs, flow_expected_rsv,
+                                   sentinel=None):
+        num_folds = 1  # because of holdout
+        num_iterations = 5  # for base search algorithms
+        metric = sklearn.metrics.mean_absolute_error  # metric class
+        metric_name = 'mean_absolute_error'  # openml metric name
+        task_type = TaskTypeEnum.SUPERVISED_REGRESSION  # task type
+
+        return self._run_and_upload(
+            clf=clf,
+            task_id=task_id,
+            n_missing_vals=n_missing_vals,
+            n_test_obs=n_test_obs,
+            flow_expected_rsv=flow_expected_rsv,
+            num_folds=num_folds,
+            num_iterations=num_iterations,
+            metric=metric,
+            metric_name=metric_name,
+            task_type=task_type,
+            sentinel=sentinel,
+        )
 
     def test_run_and_upload_logistic_regression(self):
-        lr = LogisticRegression()
+        lr = LogisticRegression(solver='lbfgs')
         task_id = self.TEST_SERVER_TASK_SIMPLE[0]
         n_missing_vals = self.TEST_SERVER_TASK_SIMPLE[1]
         n_test_obs = self.TEST_SERVER_TASK_SIMPLE[2]
-        self._run_and_upload(lr, task_id, n_missing_vals, n_test_obs, '62501')
+        self._run_and_upload_classification(lr, task_id, n_missing_vals,
+                                            n_test_obs, '62501')
+
+    def test_run_and_upload_linear_regression(self):
+        lr = LinearRegression()
+        task_id = self.TEST_SERVER_TASK_REGRESSION[0]
+        n_missing_vals = self.TEST_SERVER_TASK_REGRESSION[1]
+        n_test_obs = self.TEST_SERVER_TASK_REGRESSION[2]
+        self._run_and_upload_regression(lr, task_id, n_missing_vals,
+                                        n_test_obs, '62501')
 
     def test_run_and_upload_pipeline_dummy_pipeline(self):
 
-        pipeline1 = Pipeline(steps=[('scaler', StandardScaler(with_mean=False)),
-                                    ('dummy', DummyClassifier(strategy='prior'))])
+        pipeline1 = Pipeline(steps=[('scaler',
+                                     StandardScaler(with_mean=False)),
+                                    ('dummy',
+                                     DummyClassifier(strategy='prior'))])
         task_id = self.TEST_SERVER_TASK_SIMPLE[0]
         n_missing_vals = self.TEST_SERVER_TASK_SIMPLE[1]
         n_test_obs = self.TEST_SERVER_TASK_SIMPLE[2]
-        self._run_and_upload(pipeline1, task_id, n_missing_vals, n_test_obs,
-                             '62501')
+        self._run_and_upload_classification(pipeline1, task_id, n_missing_vals,
+                                            n_test_obs, '62501')
 
     @unittest.skipIf(LooseVersion(sklearn.__version__) < "0.20",
                      reason="columntransformer introduction in 0.20.0")
     def test_run_and_upload_column_transformer_pipeline(self):
         import sklearn.compose
         import sklearn.impute
 
@@ -463,54 +526,60 @@
                         strategy='constant', fill_value=-1)),
                     ('transformer', inner),
                     ('classifier', sklearn.tree.DecisionTreeClassifier())
                 ]
             )
 
         sentinel = self._get_sentinel()
-        self._run_and_upload(get_ct_cf(self.TEST_SERVER_TASK_SIMPLE[3],
-                                       self.TEST_SERVER_TASK_SIMPLE[4]),
-                             self.TEST_SERVER_TASK_SIMPLE[0],
-                             self.TEST_SERVER_TASK_SIMPLE[1],
-                             self.TEST_SERVER_TASK_SIMPLE[2],
-                             '62501',
-                             sentinel)
+        self._run_and_upload_classification(
+            get_ct_cf(self.TEST_SERVER_TASK_SIMPLE[3],
+                      self.TEST_SERVER_TASK_SIMPLE[4]),
+            self.TEST_SERVER_TASK_SIMPLE[0], self.TEST_SERVER_TASK_SIMPLE[1],
+            self.TEST_SERVER_TASK_SIMPLE[2], '62501', sentinel=sentinel)
         # Due to #602, it is important to test this model on two tasks
         # with different column specifications
-        self._run_and_upload(get_ct_cf(self.TEST_SERVER_TASK_MISSING_VALS[3],
-                                       self.TEST_SERVER_TASK_MISSING_VALS[4]),
-                             self.TEST_SERVER_TASK_MISSING_VALS[0],
-                             self.TEST_SERVER_TASK_MISSING_VALS[1],
-                             self.TEST_SERVER_TASK_MISSING_VALS[2],
-                             '62501',
-                             sentinel)
+        self._run_and_upload_classification(
+            get_ct_cf(self.TEST_SERVER_TASK_MISSING_VALS[3],
+                      self.TEST_SERVER_TASK_MISSING_VALS[4]),
+            self.TEST_SERVER_TASK_MISSING_VALS[0],
+            self.TEST_SERVER_TASK_MISSING_VALS[1],
+            self.TEST_SERVER_TASK_MISSING_VALS[2],
+            '62501', sentinel=sentinel)
 
     def test_run_and_upload_decision_tree_pipeline(self):
         pipeline2 = Pipeline(steps=[('Imputer', Imputer(strategy='median')),
                                     ('VarianceThreshold', VarianceThreshold()),
                                     ('Estimator', RandomizedSearchCV(
                                         DecisionTreeClassifier(),
-                                        {'min_samples_split': [2 ** x for x in range(1, 7 + 1)],
-                                         'min_samples_leaf': [2 ** x for x in range(0, 6 + 1)]},
+                                        {'min_samples_split':
+                                         [2 ** x for x in range(1, 8)],
+                                         'min_samples_leaf':
+                                         [2 ** x for x in range(0, 7)]},
                                         cv=3, n_iter=10))])
         task_id = self.TEST_SERVER_TASK_MISSING_VALS[0]
         n_missing_vals = self.TEST_SERVER_TASK_MISSING_VALS[1]
         n_test_obs = self.TEST_SERVER_TASK_MISSING_VALS[2]
-        self._run_and_upload(pipeline2, task_id, n_missing_vals, n_test_obs,
-                             '62501')
+        self._run_and_upload_classification(pipeline2, task_id, n_missing_vals,
+                                            n_test_obs, '62501')
 
     def test_run_and_upload_gridsearch(self):
         gridsearch = GridSearchCV(BaggingClassifier(base_estimator=SVC()),
                                   {"base_estimator__C": [0.01, 0.1, 10],
                                    "base_estimator__gamma": [0.01, 0.1, 10]})
         task_id = self.TEST_SERVER_TASK_SIMPLE[0]
         n_missing_vals = self.TEST_SERVER_TASK_SIMPLE[1]
         n_test_obs = self.TEST_SERVER_TASK_SIMPLE[2]
-        self._run_and_upload(gridsearch, task_id, n_missing_vals, n_test_obs,
-                             '62501')
+        run = self._run_and_upload_classification(
+            clf=gridsearch,
+            task_id=task_id,
+            n_missing_vals=n_missing_vals,
+            n_test_obs=n_test_obs,
+            flow_expected_rsv='62501',
+        )
+        self.assertEqual(len(run.trace.trace_iterations), 9)
 
     def test_run_and_upload_randomsearch(self):
         randomsearch = RandomizedSearchCV(
             RandomForestClassifier(n_estimators=5),
             {"max_depth": [3, None],
              "max_features": [1, 2, 3, 4],
              "min_samples_split": [2, 3, 4, 5, 6, 7, 8, 9, 10],
@@ -521,20 +590,27 @@
             n_iter=5)
         # The random states for the RandomizedSearchCV is set after the
         # random state of the RandomForestClassifier is set, therefore,
         # it has a different value than the other examples before
         task_id = self.TEST_SERVER_TASK_SIMPLE[0]
         n_missing_vals = self.TEST_SERVER_TASK_SIMPLE[1]
         n_test_obs = self.TEST_SERVER_TASK_SIMPLE[2]
-        self._run_and_upload(randomsearch, task_id, n_missing_vals,
-                             n_test_obs, '12172')
+        run = self._run_and_upload_classification(
+            clf=randomsearch,
+            task_id=task_id,
+            n_missing_vals=n_missing_vals,
+            n_test_obs=n_test_obs,
+            flow_expected_rsv='12172',
+        )
+        self.assertEqual(len(run.trace.trace_iterations), 5)
 
     def test_run_and_upload_maskedarrays(self):
         # This testcase is important for 2 reasons:
-        # 1) it verifies the correct handling of masked arrays (not all parameters are active)
+        # 1) it verifies the correct handling of masked arrays (not all
+        # parameters are active)
         # 2) it verifies the correct handling of a 2-layered grid search
         gridsearch = GridSearchCV(
             RandomForestClassifier(n_estimators=5),
             [
                 {'max_features': [2, 4]},
                 {'min_samples_leaf': [1, 10]}
             ],
@@ -542,29 +618,32 @@
         )
         # The random states for the GridSearchCV is set after the
         # random state of the RandomForestClassifier is set, therefore,
         # it has a different value than the other examples before
         task_id = self.TEST_SERVER_TASK_SIMPLE[0]
         n_missing_vals = self.TEST_SERVER_TASK_SIMPLE[1]
         n_test_obs = self.TEST_SERVER_TASK_SIMPLE[2]
-        self._run_and_upload(gridsearch, task_id, n_missing_vals, n_test_obs,
-                             '12172')
+        self._run_and_upload_classification(gridsearch, task_id,
+                                            n_missing_vals, n_test_obs,
+                                            '12172')
 
-    ############################################################################
+    ##########################################################################
 
     def test_learning_curve_task_1(self):
         task_id = 801  # diabates dataset
         num_test_instances = 6144  # for learning curve
         num_missing_vals = 0
         num_repeats = 1
         num_folds = 10
         num_samples = 8
 
-        pipeline1 = Pipeline(steps=[('scaler', StandardScaler(with_mean=False)),
-                                    ('dummy', DummyClassifier(strategy='prior'))])
+        pipeline1 = Pipeline(steps=[('scaler',
+                                     StandardScaler(with_mean=False)),
+                                    ('dummy',
+                                     DummyClassifier(strategy='prior'))])
         run = self._perform_run(task_id, num_test_instances, num_missing_vals,
                                 pipeline1, flow_expected_rsv='62501')
         self._check_sample_evaluations(run.sample_evaluations, num_repeats,
                                        num_folds, num_samples)
 
     def test_learning_curve_task_2(self):
         task_id = 801  # diabates dataset
@@ -574,16 +653,18 @@
         num_folds = 10
         num_samples = 8
 
         pipeline2 = Pipeline(steps=[('Imputer', Imputer(strategy='median')),
                                     ('VarianceThreshold', VarianceThreshold()),
                                     ('Estimator', RandomizedSearchCV(
                                         DecisionTreeClassifier(),
-                                        {'min_samples_split': [2 ** x for x in range(1, 7 + 1)],
-                                         'min_samples_leaf': [2 ** x for x in range(0, 6 + 1)]},
+                                        {'min_samples_split':
+                                         [2 ** x for x in range(1, 8)],
+                                         'min_samples_leaf':
+                                         [2 ** x for x in range(0, 7)]},
                                         cv=3, n_iter=10))])
         run = self._perform_run(task_id, num_test_instances, num_missing_vals,
                                 pipeline2, flow_expected_rsv='62501')
         self._check_sample_evaluations(run.sample_evaluations, num_repeats,
                                        num_folds, num_samples)
 
     def test_initialize_cv_from_run(self):
@@ -595,164 +676,194 @@
              "min_samples_leaf": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
              "bootstrap": [True, False],
              "criterion": ["gini", "entropy"]},
             cv=StratifiedKFold(n_splits=2, shuffle=True),
             n_iter=2)
 
         task = openml.tasks.get_task(11)
-        run = openml.runs.run_model_on_task(task, randomsearch,
-                                            avoid_duplicate_runs=False, seed=1)
+        run = openml.runs.run_model_on_task(
+            model=randomsearch,
+            task=task,
+            avoid_duplicate_runs=False,
+            seed=1,
+        )
         run_ = run.publish()
         run = openml.runs.get_run(run_.run_id)
 
-        modelR = openml.runs.initialize_model_from_run(run.run_id)
-        modelS = openml.setups.initialize_model(run.setup_id)
+        modelR = openml.runs.initialize_model_from_run(run_id=run.run_id)
+        modelS = openml.setups.initialize_model(setup_id=run.setup_id)
 
         self.assertEqual(modelS.cv.random_state, 62501)
         self.assertEqual(modelR.cv.random_state, 62501)
 
     def _test_local_evaluations(self, run):
 
         # compare with the scores in user defined measures
         accuracy_scores_provided = []
         for rep in run.fold_evaluations['predictive_accuracy'].keys():
-            for fold in run.fold_evaluations['predictive_accuracy'][rep].keys():
-                accuracy_scores_provided.append(run.fold_evaluations['predictive_accuracy'][rep][fold])
+            for fold in run.fold_evaluations['predictive_accuracy'][rep].\
+                    keys():
+                accuracy_scores_provided.append(
+                    run.fold_evaluations['predictive_accuracy'][rep][fold])
         accuracy_scores = run.get_metric_fn(sklearn.metrics.accuracy_score)
-        np.testing.assert_array_almost_equal(accuracy_scores_provided, accuracy_scores)
+        np.testing.assert_array_almost_equal(accuracy_scores_provided,
+                                             accuracy_scores)
 
         # also check if we can obtain some other scores: # TODO: how to do AUC?
         tests = [(sklearn.metrics.cohen_kappa_score, {'weights': None}),
                  (sklearn.metrics.auc, {'reorder': True}),
                  (sklearn.metrics.average_precision_score, {}),
                  (sklearn.metrics.jaccard_similarity_score, {}),
                  (sklearn.metrics.precision_score, {'average': 'macro'}),
                  (sklearn.metrics.brier_score_loss, {})]
         for test_idx, test in enumerate(tests):
-            alt_scores = run.get_metric_fn(test[0], test[1])
+            alt_scores = run.get_metric_fn(
+                sklearn_fn=test[0],
+                kwargs=test[1],
+            )
             self.assertEqual(len(alt_scores), 10)
             for idx in range(len(alt_scores)):
                 self.assertGreaterEqual(alt_scores[idx], 0)
                 self.assertLessEqual(alt_scores[idx], 1)
 
     def test_local_run_metric_score_swapped_parameter_order_model(self):
 
         # construct sci-kit learn classifier
-        clf = Pipeline(steps=[('imputer', Imputer(strategy='median')), ('estimator', RandomForestClassifier())])
+        clf = Pipeline(steps=[('imputer', Imputer(strategy='median')),
+                              ('estimator', RandomForestClassifier())])
 
         # download task
         task = openml.tasks.get_task(7)
 
         # invoke OpenML run
-        run = openml.runs.run_model_on_task(clf, task)
+        run = openml.runs.run_model_on_task(
+            model=clf,
+            task=task,
+            avoid_duplicate_runs=False,
+            upload_flow=False,
+        )
 
         self._test_local_evaluations(run)
 
     def test_local_run_metric_score_swapped_parameter_order_flow(self):
 
         # construct sci-kit learn classifier
-        clf = Pipeline(steps=[('imputer', Imputer(strategy='median')), ('estimator', RandomForestClassifier())])
+        clf = Pipeline(steps=[('imputer', Imputer(strategy='median')),
+                              ('estimator', RandomForestClassifier())])
 
-        flow = sklearn_to_flow(clf)
+        flow = self.extension.model_to_flow(clf)
         # download task
         task = openml.tasks.get_task(7)
 
         # invoke OpenML run
-        run = openml.runs.run_flow_on_task(flow, task)
+        run = openml.runs.run_flow_on_task(
+            flow=flow,
+            task=task,
+            avoid_duplicate_runs=False,
+            upload_flow=False,
+        )
 
         self._test_local_evaluations(run)
 
     def test_local_run_metric_score(self):
 
         # construct sci-kit learn classifier
-        clf = Pipeline(steps=[('imputer', Imputer(strategy='median')), ('estimator', RandomForestClassifier())])
+        clf = Pipeline(steps=[('imputer', Imputer(strategy='median')),
+                              ('estimator', RandomForestClassifier())])
 
         # download task
         task = openml.tasks.get_task(7)
 
         # invoke OpenML run
-        run = openml.runs.run_model_on_task(task, clf)
+        run = openml.runs.run_model_on_task(
+            model=clf,
+            task=task,
+            avoid_duplicate_runs=False,
+            upload_flow=False,
+        )
 
         self._test_local_evaluations(run)
 
     def test_online_run_metric_score(self):
         openml.config.server = self.production_server
+
         # important to use binary classification task,
         # due to assertions
         run = openml.runs.get_run(9864498)
+
         self._test_local_evaluations(run)
 
     def test_initialize_model_from_run(self):
-        clf = sklearn.pipeline.Pipeline(steps=[('Imputer', Imputer(strategy='median')),
-                                               ('VarianceThreshold', VarianceThreshold(threshold=0.05)),
-                                               ('Estimator', GaussianNB())])
+        clf = sklearn.pipeline.Pipeline(steps=[
+            ('Imputer', Imputer(strategy='median')),
+            ('VarianceThreshold', VarianceThreshold(threshold=0.05)),
+            ('Estimator', GaussianNB())])
         task = openml.tasks.get_task(11)
-        run = openml.runs.run_model_on_task(task, clf, avoid_duplicate_runs=False)
+        run = openml.runs.run_model_on_task(
+            model=clf,
+            task=task,
+            avoid_duplicate_runs=False,
+        )
         run_ = run.publish()
         run = openml.runs.get_run(run_.run_id)
 
-        modelR = openml.runs.initialize_model_from_run(run.run_id)
-        modelS = openml.setups.initialize_model(run.setup_id)
+        modelR = openml.runs.initialize_model_from_run(run_id=run.run_id)
+        modelS = openml.setups.initialize_model(setup_id=run.setup_id)
 
-        flowR = openml.flows.sklearn_to_flow(modelR)
-        flowS = openml.flows.sklearn_to_flow(modelS)
-        flowL = openml.flows.sklearn_to_flow(clf)
+        flowR = self.extension.model_to_flow(modelR)
+        flowS = self.extension.model_to_flow(modelS)
+        flowL = self.extension.model_to_flow(clf)
         openml.flows.assert_flows_equal(flowR, flowL)
         openml.flows.assert_flows_equal(flowS, flowL)
 
-        self.assertEqual(flowS.components['Imputer'].parameters['strategy'], '"median"')
-        self.assertEqual(flowS.components['VarianceThreshold'].parameters['threshold'], '0.05')
+        self.assertEqual(flowS.components['Imputer'].
+                         parameters['strategy'], '"median"')
+        self.assertEqual(flowS.components['VarianceThreshold'].
+                         parameters['threshold'], '0.05')
 
     def test_get_run_trace(self):
         # get_run_trace is already tested implicitly in test_run_and_publish
         # this test is a bit additional.
         num_iterations = 10
         num_folds = 1
         task_id = 119
 
         task = openml.tasks.get_task(task_id)
-        # IMPORTANT! Do not sentinel this flow. is faster if we don't wait on openml server
+
+        # IMPORTANT! Do not sentinel this flow. is faster if we don't wait
+        # on openml server
         clf = RandomizedSearchCV(RandomForestClassifier(random_state=42,
                                                         n_estimators=5),
+
                                  {"max_depth": [3, None],
                                   "max_features": [1, 2, 3, 4],
                                   "bootstrap": [True, False],
                                   "criterion": ["gini", "entropy"]},
                                  num_iterations, random_state=42, cv=3)
 
-        # [SPEED] make unit test faster by exploiting run information from the past
+        # [SPEED] make unit test faster by exploiting run information
+        # from the past
         try:
             # in case the run did not exists yet
-            run = openml.runs.run_model_on_task(clf, task,
-                                                avoid_duplicate_runs=True)
+            run = openml.runs.run_model_on_task(
+                model=clf,
+                task=task,
+                avoid_duplicate_runs=True,
+            )
+
             self.assertEqual(
                 len(run.trace.trace_iterations),
                 num_iterations * num_folds,
             )
             run = run.publish()
             self._wait_for_processed_run(run.run_id, 200)
             run_id = run.run_id
-        except openml.exceptions.PyOpenMLError as e:
-            if 'Run already exists in server' not in e.message:
-                # in this case the error was not the one we expected
-                raise e
-            # run was already performed
-            message = e.message
-            if sys.version_info[0] == 2:
-                # Parse a string like:
-                # 'Run already exists in server. Run id(s): set([37501])'
-                run_ids = (
-                    message.split('[')[1].replace(']', '').
-                    replace(')', '').split(',')
-                )
-            else:
-                # Parse a string like:
-                # "Run already exists in server. Run id(s): {36980}"
-                run_ids = message.split('{')[1].replace('}', '').split(',')
-            run_ids = [int(run_id) for run_id in run_ids]
+        except openml.exceptions.OpenMLRunsExistError as e:
+            # The only error we expect, should fail otherwise.
+            run_ids = [int(run_id) for run_id in e.run_ids]
             self.assertGreater(len(run_ids), 0)
             run_id = random.choice(list(run_ids))
 
         # now the actual unit test ...
         run_trace = openml.runs.get_run_trace(run_id)
         self.assertEqual(len(run_trace.trace_iterations), num_iterations * num_folds)
 
@@ -776,308 +887,172 @@
 
         task = openml.tasks.get_task(115)
 
         for clf in clfs:
             try:
                 # first populate the server with this run.
                 # skip run if it was already performed.
-                run = openml.runs.run_model_on_task(task, clf, seed=rs,
-                                                    avoid_duplicate_runs=True)
+                run = openml.runs.run_model_on_task(
+                    model=clf,
+                    task=task,
+                    seed=rs,
+                    avoid_duplicate_runs=True,
+                    upload_flow=True
+                )
                 run.publish()
-            except openml.exceptions.PyOpenMLError as e:
+            except openml.exceptions.PyOpenMLError:
                 # run already existed. Great.
                 pass
 
-            flow = openml.flows.sklearn_to_flow(clf)
+            flow = self.extension.model_to_flow(clf)
             flow_exists = openml.flows.flow_exists(flow.name, flow.external_version)
             self.assertGreater(flow_exists, 0)
             # Do NOT use get_flow reinitialization, this potentially sets
             # hyperparameter values wrong. Rather use the local model.
             downloaded_flow = openml.flows.get_flow(flow_exists)
             downloaded_flow.model = clf
             setup_exists = openml.setups.setup_exists(downloaded_flow)
             self.assertGreater(setup_exists, 0)
-            run_ids = _run_exists(task.task_id, setup_exists)
+            run_ids = run_exists(task.task_id, setup_exists)
             self.assertTrue(run_ids, msg=(run_ids, clf))
 
-    def test__get_seeded_model(self):
-        # randomized models that are initialized without seeds, can be seeded
-        randomized_clfs = [
-            BaggingClassifier(),
-            RandomizedSearchCV(RandomForestClassifier(),
-                               {"max_depth": [3, None],
-                                "max_features": [1, 2, 3, 4],
-                                "bootstrap": [True, False],
-                                "criterion": ["gini", "entropy"],
-                                "random_state" : [-1, 0, 1, 2]},
-                               cv=StratifiedKFold(n_splits=2, shuffle=True)),
-            DummyClassifier()
-        ]
-
-        for idx, clf in enumerate(randomized_clfs):
-            const_probe = 42
-            all_params = clf.get_params()
-            params = [key for key in all_params if key.endswith('random_state')]
-            self.assertGreater(len(params), 0)
-
-            # before param value is None
-            for param in params:
-                self.assertIsNone(all_params[param])
-
-            # now seed the params
-            clf_seeded = _get_seeded_model(clf, const_probe)
-            new_params = clf_seeded.get_params()
-
-            randstate_params = [key for key in new_params if key.endswith('random_state')]
-
-            # afterwards, param value is set
-            for param in randstate_params:
-                self.assertIsInstance(new_params[param], int)
-                self.assertIsNotNone(new_params[param])
-
-            if idx == 1:
-                self.assertEqual(clf.cv.random_state, 56422)
-
-    def test__get_seeded_model_raises(self):
-        # the _get_seeded_model should raise exception if random_state is anything else than an int
-        randomized_clfs = [
-            BaggingClassifier(random_state=np.random.RandomState(42)),
-            DummyClassifier(random_state="OpenMLIsGreat")
-        ]
-
-        for clf in randomized_clfs:
-            self.assertRaises(ValueError, _get_seeded_model, model=clf, seed=42)
-
-    def test__extract_arfftrace(self):
-        param_grid = {"hidden_layer_sizes": [[5, 5], [10, 10], [20, 20]],
-                      "activation" : ['identity', 'logistic', 'tanh', 'relu'],
-                      "learning_rate_init": [0.1, 0.01, 0.001, 0.0001],
-                      "max_iter": [10, 20, 40, 80]}
-        num_iters = 10
-        task = openml.tasks.get_task(20)
-        clf = RandomizedSearchCV(MLPClassifier(), param_grid, num_iters)
-        # just run the task
-        train, _ = task.get_train_test_split_indices(0, 0)
-        X, y = task.get_X_and_y()
-        clf.fit(X[train], y[train])
-
-        # check num layers of MLP
-        self.assertIn(clf.best_estimator_.hidden_layer_sizes, param_grid['hidden_layer_sizes'])
-
-        trace_attribute_list = _extract_arfftrace_attributes(clf)
-        trace_list = _extract_arfftrace(clf, 0, 0)
-        self.assertIsInstance(trace_attribute_list, list)
-        self.assertEqual(len(trace_attribute_list), 5 + len(param_grid))
-        self.assertIsInstance(trace_list, list)
-        self.assertEqual(len(trace_list), num_iters)
-
-        # found parameters
-        optimized_params = set()
-
-        for att_idx in range(len(trace_attribute_list)):
-            att_type = trace_attribute_list[att_idx][1]
-            att_name = trace_attribute_list[att_idx][0]
-            # They no longer start with parameter_ if they come from
-            # extract_arff_trace!
-            if att_name.startswith("parameter_"):
-                # add this to the found parameters
-                param_name = att_name[len("parameter_"):]
-                optimized_params.add(param_name)
-
-                for line_idx in range(len(trace_list)):
-                    val = json.loads(trace_list[line_idx][att_idx])
-                    legal_values = param_grid[param_name]
-                    self.assertIn(val, legal_values)
-            else:
-                # repeat, fold, itt, bool
-                for line_idx in range(len(trace_list)):
-                    val = trace_list[line_idx][att_idx]
-                    if isinstance(att_type, list):
-                        self.assertIn(val, att_type)
-                    elif att_name in [
-                        'hidden_layer_sizes',
-                        'activation',
-                        'learning_rate_init',
-                        'max_iter',
-                    ]:
-                        self.assertIsInstance(
-                            trace_list[line_idx][att_idx],
-                            str,
-                            msg=att_name
-                        )
-                        optimized_params.add(att_name)
-                    elif att_name in ['repeat', 'fold', 'iteration']:
-                        self.assertIsInstance(
-                            trace_list[line_idx][att_idx],
-                            int,
-                            msg=att_name
-                        )
-                    else: # att_type = real
-                        self.assertIsInstance(
-                            trace_list[line_idx][att_idx],
-                            float,
-                            msg=att_name
-                        )
-
-        self.assertEqual(set(param_grid.keys()), optimized_params)
-
-    def test__prediction_to_row(self):
-        repeat_nr = 0
-        fold_nr = 0
-        clf = sklearn.pipeline.Pipeline(steps=[('Imputer', Imputer(strategy='mean')),
-                                               ('VarianceThreshold', VarianceThreshold(threshold=0.05)),
-                                               ('Estimator', GaussianNB())])
-        task = openml.tasks.get_task(20)
-        train, test = task.get_train_test_split_indices(repeat_nr, fold_nr)
-        X, y = task.get_X_and_y()
-        clf.fit(X[train], y[train])
-
-        test_X = X[test]
-        test_y = y[test]
-
-        probaY = clf.predict_proba(test_X)
-        predY = clf.predict(test_X)
-        sample_nr = 0 # default for this task
-        for idx in range(0, len(test_X)):
-            arff_line = _prediction_to_row(repeat_nr, fold_nr, sample_nr, idx,
-                                           task.class_labels[test_y[idx]],
-                                           predY[idx], probaY[idx], task.class_labels, clf.classes_)
-
-            self.assertIsInstance(arff_line, list)
-            self.assertEqual(len(arff_line), 6 + len(task.class_labels))
-            self.assertEqual(arff_line[0], repeat_nr)
-            self.assertEqual(arff_line[1], fold_nr)
-            self.assertEqual(arff_line[2], sample_nr)
-            self.assertEqual(arff_line[3], idx)
-            sum = 0.0
-            for att_idx in range(4, 4 + len(task.class_labels)):
-                self.assertIsInstance(arff_line[att_idx], float)
-                self.assertGreaterEqual(arff_line[att_idx], 0.0)
-                self.assertLessEqual(arff_line[att_idx], 1.0)
-                sum += arff_line[att_idx]
-            self.assertAlmostEqual(sum, 1.0)
-
-            self.assertIn(arff_line[-1], task.class_labels)
-            self.assertIn(arff_line[-2], task.class_labels)
-        pass
-
-    def test_run_with_classifiers_in_param_grid(self):
+    def test_run_with_illegal_flow_id(self):
+        # check the case where the user adds an illegal flow id to a
+        # non-existing flow
         task = openml.tasks.get_task(115)
+        clf = DecisionTreeClassifier()
+        flow = self.extension.model_to_flow(clf)
+        flow, _ = self._add_sentinel_to_flow_name(flow, None)
+        flow.flow_id = -1
+        expected_message_regex = ("Flow does not exist on the server, "
+                                  "but 'flow.flow_id' is not None.")
+        with self.assertRaisesRegex(openml.exceptions.PyOpenMLError, expected_message_regex):
+            openml.runs.run_flow_on_task(
+                task=task,
+                flow=flow,
+                avoid_duplicate_runs=True,
+            )
 
-        param_grid = {
-            "base_estimator": [DecisionTreeClassifier(), ExtraTreeClassifier()]
-        }
-
-        clf = GridSearchCV(BaggingClassifier(), param_grid=param_grid)
-        self.assertRaises(TypeError, openml.runs.run_model_on_task,
-                          task=task, model=clf, avoid_duplicate_runs=False)
-
-    def test_run_with_illegal_flow_id(self):
-        # check the case where the user adds an illegal flow id to a non-existing flow
+    def test_run_with_illegal_flow_id_after_load(self):
+        # Same as `test_run_with_illegal_flow_id`, but test this error is also
+        # caught if the run is stored to and loaded from disk first.
         task = openml.tasks.get_task(115)
         clf = DecisionTreeClassifier()
-        flow = sklearn_to_flow(clf)
+        flow = self.extension.model_to_flow(clf)
         flow, _ = self._add_sentinel_to_flow_name(flow, None)
         flow.flow_id = -1
-        expected_message_regex = 'flow.flow_id is not None, but the flow does not' \
-                                 'exist on the server according to flow_exists'
-        self.assertRaisesRegexp(ValueError, expected_message_regex,
-                                openml.runs.run_flow_on_task,
-                                task=task, flow=flow, avoid_duplicate_runs=False)
+        run = openml.runs.run_flow_on_task(
+            task=task,
+            flow=flow,
+            avoid_duplicate_runs=False,
+            upload_flow=False
+        )
+
+        cache_path = os.path.join(
+            self.workdir,
+            'runs',
+            str(random.getrandbits(128)),
+        )
+        run.to_filesystem(cache_path)
+        loaded_run = openml.runs.OpenMLRun.from_filesystem(cache_path)
+
+        expected_message_regex = ("Flow does not exist on the server, "
+                                  "but 'flow.flow_id' is not None.")
+        with self.assertRaisesRegex(openml.exceptions.PyOpenMLError, expected_message_regex):
+            loaded_run.publish()
 
     def test_run_with_illegal_flow_id_1(self):
-        # check the case where the user adds an illegal flow id to an existing flow
-        # comes to a different value error than the previous test
+        # Check the case where the user adds an illegal flow id to an existing
+        # flow. Comes to a different value error than the previous test
         task = openml.tasks.get_task(115)
         clf = DecisionTreeClassifier()
-        flow_orig = sklearn_to_flow(clf)
+        flow_orig = self.extension.model_to_flow(clf)
         try:
             flow_orig.publish()  # ensures flow exist on server
         except openml.exceptions.OpenMLServerException:
             # flow already exists
             pass
-        flow_new = sklearn_to_flow(clf)
+        flow_new = self.extension.model_to_flow(clf)
 
         flow_new.flow_id = -1
         expected_message_regex = (
-            "Result from API call flow_exists and flow.flow_id are not same: "
+            "Local flow_id does not match server flow_id: "
             "'-1' vs '[0-9]+'"
         )
-        self.assertRaisesRegexp(
-            ValueError,
-            expected_message_regex,
-            openml.runs.run_flow_on_task,
+        with self.assertRaisesRegex(openml.exceptions.PyOpenMLError, expected_message_regex):
+            openml.runs.run_flow_on_task(
+                task=task,
+                flow=flow_new,
+                avoid_duplicate_runs=True,
+            )
+
+    def test_run_with_illegal_flow_id_1_after_load(self):
+        # Same as `test_run_with_illegal_flow_id_1`, but test this error is
+        # also caught if the run is stored to and loaded from disk first.
+        task = openml.tasks.get_task(115)
+        clf = DecisionTreeClassifier()
+        flow_orig = self.extension.model_to_flow(clf)
+        try:
+            flow_orig.publish()  # ensures flow exist on server
+        except openml.exceptions.OpenMLServerException:
+            # flow already exists
+            pass
+        flow_new = self.extension.model_to_flow(clf)
+        flow_new.flow_id = -1
+
+        run = openml.runs.run_flow_on_task(
             task=task,
             flow=flow_new,
             avoid_duplicate_runs=False,
+            upload_flow=False
+        )
+
+        cache_path = os.path.join(
+            self.workdir,
+            'runs',
+            str(random.getrandbits(128)),
+        )
+        run.to_filesystem(cache_path)
+        loaded_run = openml.runs.OpenMLRun.from_filesystem(cache_path)
+
+        expected_message_regex = (
+            "Local flow_id does not match server flow_id: "
+            "'-1' vs '[0-9]+'"
+        )
+        self.assertRaisesRegex(
+            openml.exceptions.PyOpenMLError,
+            expected_message_regex,
+            loaded_run.publish
         )
 
     def test__run_task_get_arffcontent(self):
         task = openml.tasks.get_task(7)
         num_instances = 3196
         num_folds = 10
         num_repeats = 1
 
+        flow = unittest.mock.Mock()
+        flow.name = 'dummy'
         clf = SGDClassifier(loss='log', random_state=1)
         res = openml.runs.functions._run_task_get_arffcontent(
-            clf,
-            task,
+            flow=flow,
+            extension=self.extension,
+            model=clf,
+            task=task,
             add_local_measures=True,
         )
         arff_datacontent, trace, fold_evaluations, _ = res
         # predictions
         self.assertIsInstance(arff_datacontent, list)
         # trace. SGD does not produce any
         self.assertIsInstance(trace, type(None))
 
-        self._check_fold_evaluations(fold_evaluations, num_repeats, num_folds)
-
-        # 10 times 10 fold CV of 150 samples
-        self.assertEqual(len(arff_datacontent), num_instances * num_repeats)
-        for arff_line in arff_datacontent:
-            # check number columns
-            self.assertEqual(len(arff_line), 8)
-            # check repeat
-            self.assertGreaterEqual(arff_line[0], 0)
-            self.assertLessEqual(arff_line[0], num_repeats - 1)
-            # check fold
-            self.assertGreaterEqual(arff_line[1], 0)
-            self.assertLessEqual(arff_line[1], num_folds - 1)
-            # check row id
-            self.assertGreaterEqual(arff_line[2], 0)
-            self.assertLessEqual(arff_line[2], num_instances - 1)
-            # check confidences
-            self.assertAlmostEqual(sum(arff_line[4:6]), 1.0)
-            self.assertIn(arff_line[6], ['won', 'nowin'])
-            self.assertIn(arff_line[7], ['won', 'nowin'])
-
-    def test__run_model_on_fold(self):
-        task = openml.tasks.get_task(7)
-        num_instances = 320
-        num_folds = 1
-        num_repeats = 1
-
-        clf = SGDClassifier(loss='log', random_state=1)
-        can_measure_runtime = sys.version_info[:2] >= (3, 3)
-        res = openml.runs.functions._run_model_on_fold(clf, task, 0, 0, 0,
-                                                       can_measure_runtime=can_measure_runtime,
-                                                       add_local_measures=True)
-
-        arff_datacontent, arff_tracecontent, user_defined_measures, model = res
-        # predictions
-        self.assertIsInstance(arff_datacontent, list)
-        # trace. SGD does not produce any
-        self.assertIsInstance(arff_tracecontent, list)
-        self.assertEqual(len(arff_tracecontent), 0)
-
-        fold_evaluations = collections.defaultdict(lambda: collections.defaultdict(dict))
-        for measure in user_defined_measures:
-            fold_evaluations[measure][0][0] = user_defined_measures[measure]
-
-        self._check_fold_evaluations(fold_evaluations, num_repeats, num_folds)
+        task_type = TaskTypeEnum.SUPERVISED_CLASSIFICATION
+        self._check_fold_timing_evaluations(fold_evaluations, num_repeats, num_folds,
+                                            task_type=task_type)
 
         # 10 times 10 fold CV of 150 samples
         self.assertEqual(len(arff_datacontent), num_instances * num_repeats)
         for arff_line in arff_datacontent:
             # check number columns
             self.assertEqual(len(arff_line), 8)
             # check repeat
@@ -1091,15 +1066,16 @@
             self.assertLessEqual(arff_line[2], num_instances - 1)
             # check confidences
             self.assertAlmostEqual(sum(arff_line[4:6]), 1.0)
             self.assertIn(arff_line[6], ['won', 'nowin'])
             self.assertIn(arff_line[7], ['won', 'nowin'])
 
     def test__create_trace_from_arff(self):
-        with open(self.static_cache_dir + '/misc/trace.arff', 'r') as arff_file:
+        with open(self.static_cache_dir + '/misc/trace.arff',
+                  'r') as arff_file:
             trace_arff = arff.load(arff_file)
         OpenMLRunTrace.trace_from_arff(trace_arff)
 
     def test_get_run(self):
         # this run is not available on test
         openml.config.server = self.production_server
         run = openml.runs.get_run(473351)
@@ -1112,20 +1088,20 @@
                          (4, 0.839567),
                          (5, 0.840922),
                          (6, 0.840985),
                          (7, 0.847129),
                          (8, 0.84218),
                          (9, 0.844014)]:
             self.assertEqual(run.fold_evaluations['f_measure'][0][i], value)
-        assert('weka' in run.tags)
-        assert('weka_3.7.12' in run.tags)
+        assert ('weka' in run.tags)
+        assert ('weka_3.7.12' in run.tags)
 
     def _check_run(self, run):
         self.assertIsInstance(run, dict)
-        self.assertEqual(len(run), 5)
+        self.assertEqual(len(run), 7)
 
     def test_get_runs_list(self):
         # TODO: comes from live, no such lists on test
         openml.config.server = self.production_server
         runs = openml.runs.list_runs(id=[2], show_errors=True)
         self.assertEqual(len(runs), 1)
         for rid in runs:
@@ -1134,14 +1110,18 @@
     def test_list_runs_empty(self):
         runs = openml.runs.list_runs(task=[0])
         if len(runs) > 0:
             raise ValueError('UnitTest Outdated, got somehow results')
 
         self.assertIsInstance(runs, dict)
 
+    def test_list_runs_output_format(self):
+        runs = openml.runs.list_runs(size=1000, output_format='dataframe')
+        self.assertIsInstance(runs, pd.DataFrame)
+
     def test_get_runs_list_by_task(self):
         # TODO: comes from live, no such lists on test
         openml.config.server = self.production_server
         task_ids = [20]
         runs = openml.runs.list_runs(task=task_ids)
         self.assertGreaterEqual(len(runs), 590)
         for rid in runs:
@@ -1155,15 +1135,15 @@
         for rid in runs:
             self.assertIn(runs[rid]['task_id'], task_ids)
             self._check_run(runs[rid])
 
     def test_get_runs_list_by_uploader(self):
         # TODO: comes from live, no such lists on test
         openml.config.server = self.production_server
-        # 29 is Dominik Kirchhoff - Joaquin and Jan have too many runs right now
+        # 29 is Dominik Kirchhoff
         uploader_ids = [29]
 
         runs = openml.runs.list_runs(uploader=uploader_ids)
         self.assertGreaterEqual(len(runs), 2)
         for rid in runs:
             self.assertIn(runs[rid]['uploader'], uploader_ids)
             self._check_run(runs[rid])
@@ -1198,33 +1178,36 @@
     def test_get_runs_pagination(self):
         # TODO: comes from live, no such lists on test
         openml.config.server = self.production_server
         uploader_ids = [1]
         size = 10
         max = 100
         for i in range(0, max, size):
-            runs = openml.runs.list_runs(offset=i, size=size, uploader=uploader_ids)
+            runs = openml.runs.list_runs(offset=i, size=size,
+                                         uploader=uploader_ids)
             self.assertGreaterEqual(size, len(runs))
             for rid in runs:
                 self.assertIn(runs[rid]["uploader"], uploader_ids)
 
     def test_get_runs_list_by_filters(self):
         # TODO: comes from live, no such lists on test
         openml.config.server = self.production_server
         ids = [505212, 6100]
         tasks = [2974, 339]
         uploaders_1 = [1, 2]
         uploaders_2 = [29, 274]
         flows = [74, 1718]
 
         '''
-        Since the results are taken by batch size, the function does not throw an OpenMLServerError anymore. 
-        Instead it throws a TimeOutException. For the moment commented out.
+        Since the results are taken by batch size, the function does not
+        throw an OpenMLServerError anymore. Instead it throws a
+        TimeOutException. For the moment commented out.
         '''
-        #self.assertRaises(openml.exceptions.OpenMLServerError, openml.runs.list_runs)
+        # self.assertRaises(openml.exceptions.OpenMLServerError,
+        # openml.runs.list_runs)
 
         runs = openml.runs.list_runs(id=ids)
         self.assertEqual(len(runs), 2)
 
         runs = openml.runs.list_runs(task=tasks)
         self.assertGreaterEqual(len(runs), 2)
 
@@ -1232,75 +1215,64 @@
         self.assertGreaterEqual(len(runs), 10)
 
         runs = openml.runs.list_runs(flow=flows)
         self.assertGreaterEqual(len(runs), 100)
 
         runs = openml.runs.list_runs(id=ids, task=tasks, uploader=uploaders_1)
 
+    @unittest.skip("API currently broken: https://github.com/openml/OpenML/issues/948")
     def test_get_runs_list_by_tag(self):
         # TODO: comes from live, no such lists on test
         openml.config.server = self.production_server
         runs = openml.runs.list_runs(tag='curves')
         self.assertGreaterEqual(len(runs), 1)
 
     def test_run_on_dataset_with_missing_labels(self):
         # Check that _run_task_get_arffcontent works when one of the class
         # labels only declared in the arff file, but is not present in the
         # actual data
 
+        flow = unittest.mock.Mock()
+        flow.name = 'dummy'
         task = openml.tasks.get_task(2)
-        class_labels = task.class_labels
 
         model = Pipeline(steps=[('Imputer', Imputer(strategy='median')),
                                 ('Estimator', DecisionTreeClassifier())])
 
-        data_content,  _, _, _ = _run_task_get_arffcontent(
-            model,
-            task,
+        data_content, _, _, _ = _run_task_get_arffcontent(
+            flow=flow,
+            model=model,
+            task=task,
+            extension=self.extension,
             add_local_measures=True,
         )
         # 2 folds, 5 repeats; keep in mind that this task comes from the test
         # server, the task on the live server is different
         self.assertEqual(len(data_content), 4490)
         for row in data_content:
             # repeat, fold, row_id, 6 confidences, prediction and correct label
             self.assertEqual(len(row), 12)
 
-    def test_predict_proba_hardclassifier(self):
-        # task 1 (test server) is important, as it is a task with an unused class
-        tasks = [1, 3, 115]
-
-        for task_id in tasks:
-            task = openml.tasks.get_task(task_id)
-            clf1 = sklearn.pipeline.Pipeline(steps=[
-                ('imputer', sklearn.preprocessing.Imputer()), ('estimator', GaussianNB())
-            ])
-            clf2 = sklearn.pipeline.Pipeline(steps=[
-                ('imputer', sklearn.preprocessing.Imputer()), ('estimator', HardNaiveBayes())
-            ])
-
-            arff_content1, _, _, _ = _run_task_get_arffcontent(
-                clf1,
-                task,
-                add_local_measures=True,
-            )
-            arff_content2, _, _, _ = _run_task_get_arffcontent(
-                clf2,
-                task,
-                add_local_measures=True,
-            )
-
-            # verifies last two arff indices (predict and correct)
-            # TODO: programmatically check wether these are indeed features (predict, correct)
-            predictionsA = np.array(arff_content1)[:, -2:]
-            predictionsB = np.array(arff_content2)[:, -2:]
-
-            np.testing.assert_array_equal(predictionsA, predictionsB)
-
     def test_get_cached_run(self):
         openml.config.cache_directory = self.static_cache_dir
         openml.runs.functions._get_cached_run(1)
 
     def test_get_uncached_run(self):
         openml.config.cache_directory = self.static_cache_dir
         with self.assertRaises(openml.exceptions.OpenMLCacheException):
             openml.runs.functions._get_cached_run(10)
+
+    def test_run_model_on_task_downloaded_flow(self):
+        model = sklearn.ensemble.RandomForestClassifier(n_estimators=33)
+        flow = self.extension.model_to_flow(model)
+        flow.publish(raise_error_if_exists=False)
+
+        downloaded_flow = openml.flows.get_flow(flow.flow_id, reinstantiate=True)
+        task = openml.tasks.get_task(119)  # diabetes
+        run = openml.runs.run_flow_on_task(
+            flow=downloaded_flow,
+            task=task,
+            avoid_duplicate_runs=False,
+            upload_flow=False,
+        )
+
+        run.publish()
```

### Comparing `openml-0.8.0/tests/test_runs/test_trace.py` & `openml-0.9.0/tests/test_runs/test_trace.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,46 +11,46 @@
                     t = OpenMLTraceIteration(
                         repeat=i,
                         fold=j,
                         iteration=5,
                         setup_string='parameter_%d%d%d' % (i, j, k),
                         evaluation=1.0 * i + 0.1 * j + 0.01 * k,
                         selected=(i == j and i == k and i == 2),
-                        paramaters=None,
+                        parameters=None,
                     )
                     trace_iterations[(i, j, k)] = t
 
         trace = OpenMLRunTrace(-1, trace_iterations=trace_iterations)
         # This next one should simply not fail
         self.assertEqual(trace.get_selected_iteration(2, 2), 2)
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
                 'Could not find the selected iteration for rep/fold 3/3',
         ):
 
             trace.get_selected_iteration(3, 3)
 
     def test_initialization(self):
         """Check all different ways to fail the initialization """
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
             'Trace content not available.',
         ):
             OpenMLRunTrace.generate(attributes='foo', content=None)
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
             'Trace attributes not available.',
         ):
             OpenMLRunTrace.generate(attributes=None, content='foo')
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
             'Trace content is empty.'
         ):
             OpenMLRunTrace.generate(attributes='foo', content=[])
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
             'Trace_attributes and trace_content not compatible:'
         ):
             OpenMLRunTrace.generate(attributes=['abc'], content=[[1, 2]])
 
     def test_duplicate_name(self):
         # Test that the user does not pass a parameter which has the same name
@@ -60,28 +60,28 @@
             ('fold', 'NUMERICAL'),
             ('iteration', 'NUMERICAL'),
             ('evaluation', 'NUMERICAL'),
             ('selected', ['true', 'false']),
             ('repeat', 'NUMERICAL'),
         ]
         trace_content = [[0, 0, 0, 0.5, 'true', 1], [0, 0, 0, 0.9, 'false', 2]]
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
             'Either setup_string or parameters needs to be passed as argument.'
         ):
             OpenMLRunTrace.generate(trace_attributes, trace_content)
 
         trace_attributes = [
             ('repeat', 'NUMERICAL'),
             ('fold', 'NUMERICAL'),
             ('iteration', 'NUMERICAL'),
             ('evaluation', 'NUMERICAL'),
             ('selected', ['true', 'false']),
             ('sunshine', 'NUMERICAL'),
         ]
         trace_content = [[0, 0, 0, 0.5, 'true', 1], [0, 0, 0, 0.9, 'false', 2]]
-        with self.assertRaisesRegexp(
+        with self.assertRaisesRegex(
             ValueError,
             'Encountered unknown attribute sunshine that does not start with '
             'prefix parameter_'
         ):
             OpenMLRunTrace.generate(trace_attributes, trace_content)
```

### Comparing `openml-0.8.0/tests/test_setups/test_setup_functions.py` & `openml-0.9.0/tests/test_setups/test_setup_functions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,109 @@
-import sys
 import hashlib
 import time
+import unittest.mock
 
 import openml
 import openml.exceptions
+import openml.extensions.sklearn
 from openml.testing import TestBase
+from typing import Dict
+import pandas as pd
 
-from sklearn.ensemble import BaggingClassifier
-from sklearn.tree import DecisionTreeClassifier
-from sklearn.linear_model import LogisticRegression
-from sklearn.naive_bayes import GaussianNB
-from sklearn.base import BaseEstimator, ClassifierMixin
+import sklearn.tree
+import sklearn.naive_bayes
+import sklearn.base
 
 
 def get_sentinel():
     # Create a unique prefix for the flow. Necessary because the flow is
     # identified by its name and external version online. Having a unique
     #  name allows us to publish the same flow in each test run
     md5 = hashlib.md5()
     md5.update(str(time.time()).encode('utf-8'))
     sentinel = md5.hexdigest()[:10]
     sentinel = 'TEST%s' % sentinel
     return sentinel
 
 
-class ParameterFreeClassifier(BaseEstimator, ClassifierMixin):
-    def __init__(self):
-        self.estimator = None
-
-    def fit(self, X, y):
-        self.estimator = DecisionTreeClassifier()
-        self.estimator.fit(X, y)
-        self.classes_ = self.estimator.classes_
-        return self
-
-    def predict(self, X):
-        return self.estimator.predict(X)
-
-    def predict_proba(self, X):
-        return self.estimator.predict_proba(X)
-
-    def set_params(self, **params):
-        pass
-
-    def get_params(self, deep=True):
-        return {}
-
-
 class TestSetupFunctions(TestBase):
     _multiprocess_can_split_ = True
 
+    def setUp(self):
+        self.extension = openml.extensions.sklearn.SklearnExtension()
+        super().setUp()
+
     def test_nonexisting_setup_exists(self):
         # first publish a non-existing flow
         sentinel = get_sentinel()
         # because of the sentinel, we can not use flows that contain subflows
-        dectree = DecisionTreeClassifier()
-        flow = openml.flows.sklearn_to_flow(dectree)
+        dectree = sklearn.tree.DecisionTreeClassifier()
+        flow = self.extension.model_to_flow(dectree)
         flow.name = 'TEST%s%s' % (sentinel, flow.name)
         flow.publish()
 
         # although the flow exists (created as of previous statement),
         # we can be sure there are no setups (yet) as it was just created
         # and hasn't been ran
         setup_id = openml.setups.setup_exists(flow)
         self.assertFalse(setup_id)
 
     def _existing_setup_exists(self, classif):
-        flow = openml.flows.sklearn_to_flow(classif)
+
+        flow = self.extension.model_to_flow(classif)
         flow.name = 'TEST%s%s' % (get_sentinel(), flow.name)
         flow.publish()
 
         # although the flow exists, we can be sure there are no
         # setups (yet) as it hasn't been ran
         setup_id = openml.setups.setup_exists(flow)
         self.assertFalse(setup_id)
         setup_id = openml.setups.setup_exists(flow)
         self.assertFalse(setup_id)
 
         # now run the flow on an easy task:
         task = openml.tasks.get_task(115)  # diabetes
-        run = openml.runs.run_flow_on_task(task, flow)
+        run = openml.runs.run_flow_on_task(flow, task)
         # spoof flow id, otherwise the sentinel is ignored
         run.flow_id = flow.flow_id
         run.publish()
         # download the run, as it contains the right setup id
         run = openml.runs.get_run(run.run_id)
 
         # execute the function we are interested in
         setup_id = openml.setups.setup_exists(flow)
-        self.assertEquals(setup_id, run.setup_id)
+        self.assertEqual(setup_id, run.setup_id)
 
     def test_existing_setup_exists_1(self):
-        # Check a flow with zero hyperparameters
-        self._existing_setup_exists(ParameterFreeClassifier())
+        def side_effect(self):
+            self.var_smoothing = 1e-9
+            self.priors = None
+        with unittest.mock.patch.object(
+                sklearn.naive_bayes.GaussianNB,
+                '__init__',
+                side_effect,
+        ):
+            # Check a flow with zero hyperparameters
+            nb = sklearn.naive_bayes.GaussianNB()
+            self._existing_setup_exists(nb)
 
     def test_exisiting_setup_exists_2(self):
         # Check a flow with one hyperparameter
-        self._existing_setup_exists(GaussianNB())
+        self._existing_setup_exists(sklearn.naive_bayes.GaussianNB())
 
     def test_existing_setup_exists_3(self):
         # Check a flow with many hyperparameters
         self._existing_setup_exists(
-            DecisionTreeClassifier(max_depth=5,  # many hyperparameters
-                                   min_samples_split=3,
-                                   # Not setting the random state will
-                                   # make this flow fail as running it
-                                   # will add a random random_state.
-                                   random_state=1)
+            sklearn.tree.DecisionTreeClassifier(
+                max_depth=5,
+                min_samples_split=3,
+                # Not setting the random state will make this flow fail as running it
+                # will add a random random_state.
+                random_state=1,
+            )
         )
 
     def test_get_setup(self):
         # no setups in default test server
         openml.config.server = 'https://www.openml.org/api/v1/xml/'
 
         # contains all special cases, 0 params, 1 param, n params.
@@ -120,43 +113,61 @@
 
         for idx in range(len(setups)):
             current = openml.setups.get_setup(setups[idx])
             assert current.flow_id > 0
             if num_params[idx] == 0:
                 self.assertIsNone(current.parameters)
             else:
-                self.assertEquals(len(current.parameters), num_params[idx])
+                self.assertEqual(len(current.parameters), num_params[idx])
 
     def test_setup_list_filter_flow(self):
         openml.config.server = self.production_server
 
         flow_id = 5873
 
         setups = openml.setups.list_setups(flow=flow_id)
 
-        self.assertGreater(len(setups), 0) # TODO: please adjust 0
+        self.assertGreater(len(setups), 0)  # TODO: please adjust 0
         for setup_id in setups.keys():
-            self.assertEquals(setups[setup_id].flow_id, flow_id)
+            self.assertEqual(setups[setup_id].flow_id, flow_id)
 
     def test_list_setups_empty(self):
         setups = openml.setups.list_setups(setup=[0])
         if len(setups) > 0:
             raise ValueError('UnitTest Outdated, got somehow results')
 
         self.assertIsInstance(setups, dict)
 
+    def test_list_setups_output_format(self):
+        openml.config.server = self.production_server
+        flow_id = 6794
+        setups = openml.setups.list_setups(flow=flow_id, output_format='object', size=10)
+        self.assertIsInstance(setups, Dict)
+        self.assertIsInstance(setups[list(setups.keys())[0]],
+                              openml.setups.setup.OpenMLSetup)
+        self.assertEqual(len(setups), 10)
+
+        setups = openml.setups.list_setups(flow=flow_id, output_format='dataframe', size=10)
+        self.assertIsInstance(setups, pd.DataFrame)
+        self.assertEqual(len(setups), 10)
+
+        setups = openml.setups.list_setups(flow=flow_id, output_format='dict', size=10)
+        self.assertIsInstance(setups, Dict)
+        self.assertIsInstance(setups[list(setups.keys())[0]], Dict)
+        self.assertEqual(len(setups), 10)
+
     def test_setuplist_offset(self):
         # TODO: remove after pull on live for better testing
         # openml.config.server = self.production_server
 
         size = 10
         setups = openml.setups.list_setups(offset=0, size=size)
-        self.assertEquals(len(setups), size)
+        self.assertEqual(len(setups), size)
         setups2 = openml.setups.list_setups(offset=size, size=size)
-        self.assertEquals(len(setups2), size)
+        self.assertEqual(len(setups2), size)
 
         all = set(setups.keys()).union(setups2.keys())
 
         self.assertEqual(len(all), size * 2)
 
     def test_get_cached_setup(self):
         openml.config.cache_directory = self.static_cache_dir
```

### Comparing `openml-0.8.0/tests/test_tasks/test_split.py` & `openml-0.9.0/tests/test_tasks/test_split.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import inspect
 import os
-import unittest
 
 import numpy as np
 
 from openml import OpenMLSplit
 from openml.testing import TestBase
 
 
@@ -22,15 +21,16 @@
         )
         # TODO Needs to be adapted regarding the python version
         self.pd_filename = self.arff_filename.replace(".arff", ".pkl")
 
     def tearDown(self):
         try:
             os.remove(self.pd_filename)
-        except:
+        except (OSError, FileNotFoundError):
+            #  Replaced bare except. Not sure why these exceptions are acceptable.
             pass
 
     def test_eq(self):
         split = OpenMLSplit._from_arff_file(self.arff_filename)
         self.assertEqual(split, split)
 
         split2 = OpenMLSplit._from_arff_file(self.arff_filename)
@@ -60,19 +60,28 @@
         self.assertIsInstance(split.split[0][0][0][1], np.ndarray)
         self.assertIsInstance(split.split[0][0][0].test, np.ndarray)
         self.assertIsInstance(split.split[0][0][0].test, np.ndarray)
         for i in range(10):
             for j in range(10):
                 self.assertGreaterEqual(split.split[i][j][0].train.shape[0], 808)
                 self.assertGreaterEqual(split.split[i][j][0].test.shape[0], 89)
-                self.assertEqual(split.split[i][j][0].train.shape[0] +
-                                 split.split[i][j][0].test.shape[0], 898)
+                self.assertEqual(split.split[i][j][0].train.shape[0]
+                                 + split.split[i][j][0].test.shape[0],
+                                 898)
 
     def test_get_split(self):
         split = OpenMLSplit._from_arff_file(self.arff_filename)
         train_split, test_split = split.get(fold=5, repeat=2)
         self.assertEqual(train_split.shape[0], 808)
         self.assertEqual(test_split.shape[0], 90)
-        self.assertRaisesRegexp(ValueError, "Repeat 10 not known",
-                                split.get, 10, 2)
-        self.assertRaisesRegexp(ValueError, "Fold 10 not known",
-                                split.get, 2, 10)
+        self.assertRaisesRegex(
+            ValueError,
+            "Repeat 10 not known",
+            split.get,
+            10, 2,
+        )
+        self.assertRaisesRegex(
+            ValueError,
+            "Fold 10 not known",
+            split.get,
+            2, 10,
+        )
```

### Comparing `openml-0.8.0/tests/test_tasks/test_task_functions.py` & `openml-0.9.0/tests/test_tasks/test_task_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 import os
-import sys
-
-import six
-
-if sys.version_info[0] >= 3:
-    from unittest import mock
-else:
-    import mock
+from unittest import mock
 
 from openml.testing import TestBase
 from openml import OpenMLSplit, OpenMLTask
 from openml.exceptions import OpenMLCacheException
 import openml
 import unittest
+import pandas as pd
 
 
 class TestTask(TestBase):
     _multiprocess_can_split_ = True
 
     def test__get_cached_tasks(self):
         openml.config.cache_directory = self.static_cache_dir
@@ -28,17 +22,20 @@
     def test__get_cached_task(self):
         openml.config.cache_directory = self.static_cache_dir
         task = openml.tasks.functions._get_cached_task(1)
         self.assertIsInstance(task, OpenMLTask)
 
     def test__get_cached_task_not_cached(self):
         openml.config.cache_directory = self.static_cache_dir
-        self.assertRaisesRegexp(OpenMLCacheException,
-                                'Task file for tid 2 not cached',
-                                openml.tasks.functions._get_cached_task, 2)
+        self.assertRaisesRegex(
+            OpenMLCacheException,
+            'Task file for tid 2 not cached',
+            openml.tasks.functions._get_cached_task,
+            2,
+        )
 
     def test__get_estimation_procedure_list(self):
         estimation_procedures = openml.tasks.functions.\
             _get_estimation_procedure_list()
         self.assertIsInstance(estimation_procedures, list)
         self.assertIsInstance(estimation_procedures[0], dict)
         self.assertEqual(estimation_procedures[0]['task_type_id'], 1)
@@ -51,37 +48,43 @@
 
     def _check_task(self, task):
         self.assertEqual(type(task), dict)
         self.assertGreaterEqual(len(task), 2)
         self.assertIn('did', task)
         self.assertIsInstance(task['did'], int)
         self.assertIn('status', task)
-        self.assertIsInstance(task['status'], six.string_types)
+        self.assertIsInstance(task['status'], str)
         self.assertIn(task['status'],
                       ['in_preparation', 'active', 'deactivated'])
 
     def test_list_tasks_by_type(self):
-        num_curves_tasks = 200 # number is flexible, check server if fails
-        ttid=3
+        num_curves_tasks = 200  # number is flexible, check server if fails
+        ttid = 3
         tasks = openml.tasks.list_tasks(task_type_id=ttid)
         self.assertGreaterEqual(len(tasks), num_curves_tasks)
         for tid in tasks:
-            self.assertEquals(ttid, tasks[tid]["ttid"])
+            self.assertEqual(ttid, tasks[tid]["ttid"])
             self._check_task(tasks[tid])
 
+    def test_list_tasks_output_format(self):
+        ttid = 3
+        tasks = openml.tasks.list_tasks(task_type_id=ttid, output_format='dataframe')
+        self.assertIsInstance(tasks, pd.DataFrame)
+        self.assertGreater(len(tasks), 100)
+
     def test_list_tasks_empty(self):
         tasks = openml.tasks.list_tasks(tag='NoOneWillEverUseThisTag')
         if len(tasks) > 0:
             raise ValueError('UnitTest Outdated, got somehow results (tag is used, please adapt)')
 
         self.assertIsInstance(tasks, dict)
 
     def test_list_tasks_by_tag(self):
-        num_basic_tasks = 100 # number is flexible, check server if fails
-        tasks = openml.tasks.list_tasks(tag='study_14')
+        num_basic_tasks = 100  # number is flexible, check server if fails
+        tasks = openml.tasks.list_tasks(tag='OpenML100')
         self.assertGreaterEqual(len(tasks), num_basic_tasks)
         for tid in tasks:
             self._check_task(tasks[tid])
 
     def test_list_tasks(self):
         tasks = openml.tasks.list_tasks()
         self.assertGreaterEqual(len(tasks), 900)
@@ -97,27 +100,27 @@
             for tid in tasks:
                 self._check_task(tasks[tid])
 
     def test_list_tasks_per_type_paginate(self):
         size = 10
         max = 100
         task_types = 4
-        for j in range(1,task_types):
+        for j in range(1, task_types):
             for i in range(0, max, size):
                 tasks = openml.tasks.list_tasks(task_type_id=j, offset=i, size=size)
                 self.assertGreaterEqual(size, len(tasks))
                 for tid in tasks:
-                    self.assertEquals(j, tasks[tid]["ttid"])
+                    self.assertEqual(j, tasks[tid]["ttid"])
                     self._check_task(tasks[tid])
 
     def test__get_task(self):
         openml.config.cache_directory = self.static_cache_dir
         openml.tasks.get_task(1882)
 
-    @unittest.skip("Please await outcome of discussion: https://github.com/openml/OpenML/issues/776")
+    @unittest.skip("Please await outcome of discussion: https://github.com/openml/OpenML/issues/776")  # noqa: E501
     def test__get_task_live(self):
         # Test the following task as it used to throw an Unicode Error.
         # https://github.com/openml/openml-python/issues/378
         openml.config.server = self.production_server
         openml.tasks.get_task(34536)
 
     def test_get_task(self):
@@ -129,22 +132,45 @@
         self.assertTrue(os.path.exists(os.path.join(
             self.workdir, 'org', 'openml', 'test', "tasks", "1", "datasplits.arff"
         )))
         self.assertTrue(os.path.exists(os.path.join(
             self.workdir, 'org', 'openml', 'test', "datasets", "1", "dataset.arff"
         )))
 
+    def test_get_task_lazy(self):
+        task = openml.tasks.get_task(2, download_data=False)
+        self.assertIsInstance(task, OpenMLTask)
+        self.assertTrue(os.path.exists(os.path.join(
+            self.workdir, 'org', 'openml', 'test', "tasks", "2", "task.xml",
+        )))
+        self.assertEqual(task.class_labels, ['1', '2', '3', '4', '5', 'U'])
+
+        self.assertFalse(os.path.exists(os.path.join(
+            self.workdir, 'org', 'openml', 'test', "tasks", "2", "datasplits.arff"
+        )))
+        # Since the download_data=False is propagated to get_dataset
+        self.assertFalse(os.path.exists(os.path.join(
+            self.workdir, 'org', 'openml', 'test', "datasets", "2", "dataset.arff"
+        )))
+
+        task.download_split()
+        self.assertTrue(os.path.exists(os.path.join(
+            self.workdir, 'org', 'openml', 'test', "tasks", "2", "datasplits.arff"
+        )))
+
     @mock.patch('openml.tasks.functions.get_dataset')
     def test_removal_upon_download_failure(self, get_dataset):
         class WeirdException(Exception):
             pass
+
         def assert_and_raise(*args, **kwargs):
             # Make sure that the file was created!
             assert os.path.join(os.getcwd(), "tasks", "1", "tasks.xml")
             raise WeirdException()
+
         get_dataset.side_effect = assert_and_raise
         try:
             openml.tasks.get_task(1)
         except WeirdException:
             pass
         # Now the file should no longer exist
         self.assertFalse(os.path.exists(
```

### Comparing `openml-0.8.0/tests/test_utils/test_utils.py` & `openml-0.9.0/tests/test_utils/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     import mock
 
 
 class OpenMLTaskTest(TestBase):
     _multiprocess_can_split_ = True
     _batch_size = 25
 
-    def mocked_perform_api_call(call):
+    def mocked_perform_api_call(call, request_method):
         # TODO: JvR: Why is this not a staticmethod?
         url = openml.config.server + '/' + call
-        return openml._api_calls._read_url(url)
+        return openml._api_calls._read_url(url, request_method=request_method)
 
     def test_list_all(self):
-        openml.utils._list_all(openml.tasks.functions._list_tasks)
+        openml.utils._list_all(listing_call=openml.tasks.functions._list_tasks)
 
-    @mock.patch('openml._api_calls._perform_api_call', 
+    @mock.patch('openml._api_calls._perform_api_call',
                 side_effect=mocked_perform_api_call)
     def test_list_all_few_results_available(self, _perform_api_call):
         # we want to make sure that the number of api calls is only 1.
         # Although we have multiple versions of the iris dataset, there is only
         # one with this name/version combination
 
         datasets = openml.datasets.list_datasets(size=1000,
@@ -42,15 +42,17 @@
         for did in datasets:
             self._check_dataset(datasets[did])
 
     def test_list_datasets_with_high_size_parameter(self):
         datasets_a = openml.datasets.list_datasets()
         datasets_b = openml.datasets.list_datasets(size=np.inf)
 
-        self.assertEqual(len(datasets_a), len(datasets_b))
+        # note that in the meantime the number of datasets could have increased
+        # due to tests that run in parallel.
+        self.assertGreaterEqual(len(datasets_b), len(datasets_a))
 
     def test_list_all_for_tasks(self):
         required_size = 1068  # default test server reset value
         tasks = openml.tasks.list_tasks(batch_size=self._batch_size, size=required_size)
 
         self.assertEqual(len(tasks), required_size)
```

