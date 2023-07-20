# Comparing `tmp/qiskit-ibm-experiment-0.3.3.tar.gz` & `tmp/qiskit-ibm-experiment-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-experiment-0.3.3.tar", last modified: Tue May 30 10:55:27 2023, max compression
+gzip compressed data, was "qiskit-ibm-experiment-0.3.4.tar", last modified: Thu Jul 20 17:29:23 2023, max compression
```

## Comparing `qiskit-ibm-experiment-0.3.3.tar` & `qiskit-ibm-experiment-0.3.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.313119 qiskit-ibm-experiment-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-30 10:55:27.313119 qiskit-ibm-experiment-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.301118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.305118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.305118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment_rest_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/device_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/experiment_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    69048 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/ibm_experiment_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.305118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:55:27.313119 qiskit-ibm-experiment-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/test/service/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/ibm_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_experiment_data_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_experiment_server_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_local_experiment_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.653028 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.653028 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.653028 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/experiment_rest_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28234 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/experiment_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69823 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/ibm_experiment_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.653028 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-07-20 17:29:23.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 17:29:23.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:29:23.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:29:23.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-20 17:29:23.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 17:29:23.000000 qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/test/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/service/ibm_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/service/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22554 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/service/test_experiment_data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67326 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/service/test_experiment_server_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18855 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/service/test_local_experiment_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:23.657028 qiskit-ibm-experiment-0.3.4/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/utils/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-20 17:29:07.000000 qiskit-ibm-experiment-0.3.4/test/utils/utils.py
```

### Comparing `qiskit-ibm-experiment-0.3.3/LICENSE.txt` & `qiskit-ibm-experiment-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/PKG-INFO` & `qiskit-ibm-experiment-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3.3
+Version: 0.3.4
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-experiment-0.3.3/README.md` & `qiskit-ibm-experiment-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/__init__.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/__init__.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/account.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/configuration.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/exceptions.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/management.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/storage.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/__init__.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Client for accessing IBM Quantum experiment services."""
 
 import logging
-from typing import List, Dict, Optional, Union
+import json
+from typing import List, Dict, Optional, Union, Type
 from qiskit_ibm_experiment.client.session import RetrySession
 from .experiment_rest_adapter import ExperimentRestAdapter
 
 logger = logging.getLogger(__name__)
 
 
 class ExperimentClient:
@@ -325,25 +326,28 @@
         Args:
             experiment_id: Experiment ID.
             file_name: The intended name of the data file
             file_data: The contents of the data file
         """
         self.api.file_upload(experiment_id, file_name, file_data)
 
-    def experiment_file_download(self, experiment_id: str, file_name: str) -> Dict:
+    def experiment_file_download(
+        self, experiment_id: str, file_name: str, json_decoder: Type[json.JSONDecoder]
+    ) -> Dict:
         """Downloads a data file from the DB
 
         Args:
             experiment_id: Experiment ID.
             file_name: The name of the data file
+            json_decoder: Custom decoder to use to decode the retrieved experiment.
 
         Returns:
             The Dictionary of contents of the file
         """
-        return self.api.file_download(experiment_id, file_name)
+        return self.api.file_download(experiment_id, file_name, json_decoder)
 
     def device_components(self, backend_name: Optional[str]) -> List[Dict]:
         """Return device components for the backend.
 
         Args:
             backend_name: Name of the backend.
```

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment_rest_adapter.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/experiment_rest_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 # Any modifications or derivative works of this code must retain this
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Experiment REST adapter."""
 
 import logging
-from typing import Dict, List, Any, Union, Optional
+import json
+from typing import Dict, List, Any, Union, Optional, Type
+import yaml
 from qiskit_ibm_experiment.client.session import RetrySession
 
 logger = logging.getLogger(__name__)
 
 
 class ExperimentRestAdapter:
     """REST adapter for experiment result DB"""
@@ -431,25 +433,30 @@
             uuid=experiment_id, path=file_pathname
         )
         upload_url = self.session.get(upload_request_url).json()["url"]
         self.session.put(
             upload_url, data=file_data, headers=self._HEADER_JSON_CONTENT, bare=True
         )
 
-    def file_download(self, experiment_id: str, file_name: str) -> Dict:
+    def file_download(
+        self, experiment_id: str, file_name: str, json_decoder: Type[json.JSONDecoder]
+    ) -> Dict:
         """Downloads a data file from the DB
 
         Args:
             experiment_id: Experiment ID.
             file_name: The name of the data file
+            json_decoder: Custom decoder to use to decode the retrieved experiment.
 
         Returns:
             The Dictionary of contents of the file
         """
         download_request_url = self.get_url("files_download")
         download_request_url = download_request_url.format(
             uuid=experiment_id, path=file_name
         )
         result = self.session.get(download_request_url)
         if result.status_code == 200:
-            return result.json()
+            if file_name.endswith(".yaml"):
+                return yaml.safe_load(result.content)
+            return result.json(cls=json_decoder)
         return result
```

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/local_client.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/local_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,18 @@
 # pylint: disable=no-member
 
 import logging
 import os
 import uuid
 import json
 from datetime import datetime
-from typing import List, Dict, Optional, Union, Any
+from typing import List, Dict, Optional, Union, Any, Type
 import pandas as pd
 import numpy as np
+import yaml
 
 from qiskit_ibm_experiment.exceptions import (
     IBMExperimentEntryNotFound,
     IBMExperimentEntryExists,
     IBMApiError,
     RequestsApiError,
 )
@@ -771,25 +772,30 @@
             "Size": len(file_data),
             "LastModified": str(datetime.now()),
         }
         self._files_list[experiment_id].append(new_file_element)
         self._files[experiment_id][file_name] = file_data
         self.save()
 
-    def experiment_file_download(self, experiment_id: str, file_name: str) -> Dict:
+    def experiment_file_download(
+        self, experiment_id: str, file_name: str, json_decoder: Type[json.JSONDecoder]
+    ) -> Dict:
         """Downloads a data file from the DB
 
         Args:
             experiment_id: Experiment ID.
             file_name: The name of the data file
+            json_decoder: Custom decoder to use to decode the retrieved experiment.
 
         Returns:
             The Dictionary of contents of the file
 
         Raises:
             IBMExperimentEntryNotFound: if experiment or file not found
         """
         if experiment_id not in self._files:
             raise IBMExperimentEntryNotFound
         if file_name not in self._files[experiment_id]:
             raise IBMExperimentEntryNotFound
-        return json.loads(self._files[experiment_id][file_name])
+        if file_name.endswith(".yaml"):
+            return yaml.safe_load(self._files[experiment_id][file_name])
+        return json.loads(self._files[experiment_id][file_name], cls=json_decoder)
```

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/session.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/client/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/exceptions.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/__init__.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/constants.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/device_component.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/device_component.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/experiment_dataclasses.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/experiment_dataclasses.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/ibm_experiment_service.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/ibm_experiment_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from typing import Optional, List, Dict, Union, Tuple, Any, Type
 from datetime import datetime
 from collections import defaultdict
 import requests
 import numpy as np
 from pandas import DataFrame
 import pandas as pd
+import yaml
 from .constants import (
     ExperimentShareLevel,
     ResultQuality,
     RESULT_QUALITY_FROM_API,
     RESULT_QUALITY_TO_API,
     RESULT_QUALITY_FROM_DATAFRAME,
     RESULT_QUALITY_TO_DATAFRAME,
@@ -1679,49 +1680,68 @@
             IBMApiError: If the request to the server failed.
         """
         with map_api_error(f"Experiment {experiment_id} file list not received."):
             data = self._api_client.experiment_files_get(experiment_id)
         return data
 
     def file_upload(
-        self, experiment_id: str, file_name: str, file_data: Union[Dict, str]
+        self,
+        experiment_id: str,
+        file_name: str,
+        file_data: Union[Dict, str],
+        json_encoder: Type[json.JSONEncoder] = json.JSONEncoder,
     ):
         """Uploads a data file to the DB
 
         Args:
             experiment_id: The experiment the data file belongs to
             file_name: The expected filename of the data file
             file_data: The dictionary of data to save, or JSON serialization of it
+            json_encoder: Custom encoder to use to encode the experiment.
 
         Additional info:
             The filename is expected to end with ".json" (otherwise it will be added)
             and the data itself should be either a dictionary or a JSON serialization
             with the default encoder.
         """
         # currently the resultdb enforces files to end with .json or .yaml
-        if not file_name.endswith(".json"):
+        # without suffix, we assume json formatting
+        if not (file_name.endswith(".json") or file_name.endswith(".yaml")):
             file_name += ".json"
         if isinstance(file_data, dict):
-            file_data = json.dumps(file_data)
+            # for now we avoid using custom encoder with yaml files
+            if file_name.endswith(".yaml"):
+                file_data = yaml.dump(file_data)
+            else:
+                file_data = json.dumps(file_data, cls=json_encoder)
         self._api_client.experiment_file_upload(experiment_id, file_name, file_data)
 
-    def file_download(self, experiment_id: str, file_name: str) -> Dict:
+    def file_download(
+        self,
+        experiment_id: str,
+        file_name: str,
+        json_decoder: Type[json.JSONDecoder] = json.JSONDecoder,
+    ) -> Dict:
         """Downloads a data file from the DB and returns its deserialization
         Args:
             experiment_id: The experiment the data file belongs to
             file_name: The filename of the data file
+            json_decoder: Custom decoder to use to decode the retrieved experiment.
         Returns:
             The JSON deserialization of the data file
         Additional info:
             The filename is expected to end with ".json", otherwise
             it will be added.
         """
-        if not file_name.endswith(".json"):
+        if not (file_name.endswith(".json") or file_name.endswith(".yaml")):
             file_name += ".json"
-        file_data = self._api_client.experiment_file_download(experiment_id, file_name)
+        # for now we avoid using custom decoder with yaml files
+        file_data = self._api_client.experiment_file_download(
+            experiment_id, file_name, json_decoder
+        )
         return file_data
 
     def experiment_has_file(self, experiment_id: str, file_name: str) -> bool:
         """Checks whether a specific expriment has a specific file
         Args:
             experiment_id: The experiment the data file belongs to
             file_name: The filename of the data file
```

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/utils.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/service/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/version.py` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/PKG-INFO` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3.3
+Version: 0.3.4
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/SOURCES.txt` & `qiskit-ibm-experiment-0.3.4/qiskit_ibm_experiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/setup.py` & `qiskit-ibm-experiment-0.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/test/__init__.py` & `qiskit-ibm-experiment-0.3.4/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/test/service/ibm_test_case.py` & `qiskit-ibm-experiment-0.3.4/test/service/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/test/service/test_experiment.py` & `qiskit-ibm-experiment-0.3.4/test/service/test_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/test/service/test_experiment_data_integration.py` & `qiskit-ibm-experiment-0.3.4/test/service/test_experiment_data_integration.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 # copyright notice, and modified files need to carry a notice indicating
 # that they have been altered from the originals.
 
 """Experiment integration tests."""
 
 import os
 import unittest
-from unittest import mock, SkipTest, skipIf
+from unittest import mock, skipIf
 import contextlib
 from test.service.ibm_test_case import IBMTestCase
 import numpy as np
-from qiskit import transpile
+from qiskit import transpile, QuantumCircuit
 from qiskit.providers import JobStatus
 from qiskit.test.reference_circuits import ReferenceCircuits
-from qiskit_experiments.framework import ExperimentData
+from qiskit_experiments.framework import (
+    ExperimentData,
+    ExperimentDecoder,
+    ExperimentEncoder,
+)
 from qiskit_experiments.framework.experiment_data import ExperimentStatus
 from qiskit_experiments.framework import AnalysisResult
 from qiskit_experiments.database_service.exceptions import ExperimentEntryNotFound
 from qiskit_ibm_provider import IBMProvider
 
 from qiskit_ibm_experiment import IBMExperimentService
 from qiskit_ibm_experiment.exceptions import IBMExperimentEntryNotFound
@@ -43,15 +47,16 @@
         """Initial class level setup."""
         super().setUpClass()
         try:
             cls._setup_service()
             cls._setup_provider()
             cls.circuit = transpile(ReferenceCircuits.bell(), cls.backend)
         except Exception as err:
-            raise SkipTest("Not authorized to use experiment service.") from err
+            cls.log.info("Error while setting the service/provider: %s", err)
+            raise
 
     @classmethod
     def _setup_service(cls):
         """Get the service for the class."""
         cls.service = IBMExperimentService(
             token=os.getenv("QISKIT_IBM_STAGING_API_TOKEN"),
             url=os.getenv("QISKIT_IBM_STAGING_API_URL"),
@@ -136,15 +141,15 @@
 
         job_ids = []
         for _ in range(2):
             job = self._run_circuit()
             exp_data.add_jobs(job)
             job_ids.append(job.job_id())
 
-        exp_data.block_for_results().save()
+        exp_data.block_for_results().save(suppress_errors=False)
         self.experiments_to_delete.append(exp_data.experiment_id)
 
         hub, group, project = list(self.backend.provider._hgps)[0].split("/")
 
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         self._verify_experiment_data(exp_data, rexp)
         self.assertEqual(hub, rexp.hub)  # pylint: disable=no-member
@@ -157,15 +162,15 @@
 
         for _ in range(2):
             job = self._run_circuit()
             exp_data.add_jobs(job)
         exp_data.tags = ["foo", "bar"]
         exp_data.share_level = "hub"
         exp_data.notes = "some notes"
-        exp_data.block_for_results().save()
+        exp_data.block_for_results().save(suppress_errors=False)
 
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         self._verify_experiment_data(exp_data, rexp)
 
     def _verify_experiment_data(self, expected, actual):
         """Verify the input experiment data."""
         self.assertEqual(expected.experiment_id, actual.experiment_id)
@@ -190,30 +195,30 @@
             experiment_id=exp_data.experiment_id,
             quality="good",
             verified=True,
             tags=["foo", "bar"],
             service=self.service,
         )
         exp_data.add_analysis_results(aresult)
-        exp_data.save()
+        exp_data.save(suppress_errors=False)
 
         rresult = AnalysisResult.load(aresult.result_id, self.service)
         self.assertEqual(exp_data.experiment_id, rresult.experiment_id)
         self._verify_analysis_result(aresult, rresult)
 
     def test_update_analysis_result(self):
         """Test updating an analysis result."""
         aresult, exp_data = self._create_analysis_result()
 
         rdata = {"complex": 2 + 3j, "numpy": np.zeros(2)}
         aresult.value = rdata
         aresult.quality = "good"
         aresult.verified = True
         aresult.tags = ["foo", "bar"]
-        aresult.save()
+        aresult.save(suppress_errors=False)
 
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         rresult = rexp.analysis_results(0)
         self._verify_analysis_result(aresult, rresult)
 
     def _verify_analysis_result(self, expected, actual):
         """Verify the input analysis result."""
@@ -230,15 +235,15 @@
         self.assertEqual(expected.value["numpy"].all(), actual.value["numpy"].all())
 
     def test_delete_analysis_result(self):
         """Test deleting an analysis result."""
         aresult, exp_data = self._create_analysis_result()
         with mock.patch("builtins.input", lambda _: "y"):
             exp_data.delete_analysis_result(0)
-            exp_data.save()
+            exp_data.save(suppress_errors=False)
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         self.assertRaises(
             ExperimentEntryNotFound, rexp.analysis_results, aresult.result_id
         )
         self.assertRaises(
             IBMExperimentEntryNotFound, self.service.analysis_result, aresult.result_id
         )
@@ -313,15 +318,15 @@
         figure_name = "hello.svg"
 
         exp_data.add_figures(
             figures=hello_bytes, figure_names=figure_name, save_figure=True
         )
         with mock.patch("builtins.input", lambda _: "y"):
             exp_data.delete_figure(0)
-            exp_data.save()
+            exp_data.save(suppress_errors=False)
 
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         self.assertRaises(IBMExperimentEntryNotFound, rexp.figure, figure_name)
         self.assertRaises(
             IBMExperimentEntryNotFound,
             self.service.figure,
             exp_data.experiment_id,
@@ -337,40 +342,40 @@
             name="qiskit_test",
             device_components=self.device_components,
             experiment_id=exp_data.experiment_id,
         )
         exp_data.add_analysis_results(aresult)
         hello_bytes = str.encode("hello world")
         exp_data.add_figures(hello_bytes, figure_names="hello.svg")
-        exp_data.save()
+        exp_data.save(suppress_errors=False)
 
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         # Experiment tag order is not necessarily preserved
         # so compare tags with a predictable sort order.
         self.assertEqual(["bar", "foo"], sorted(rexp.tags))
         self.assertEqual(aresult.result_id, rexp.analysis_results(0).result_id)
         self.assertEqual(hello_bytes, rexp.figure(0).figure)
 
         exp_data.delete_analysis_result(0)
         exp_data.delete_figure(0)
         with mock.patch("builtins.input", lambda _: "y"):
-            exp_data.save()
+            exp_data.save(suppress_errors=False)
 
         rexp = ExperimentData.load(exp_data.experiment_id, self.service)
         self.assertRaises(IBMExperimentEntryNotFound, rexp.figure, "hello.svg")
         self.assertRaises(
             ExperimentEntryNotFound, rexp.analysis_results, aresult.result_id
         )
 
     def test_set_service_job(self):
         """Test setting service with a job."""
         exp_data = ExperimentData(experiment_type="qiskit_test", service=self.service)
         job = self._run_circuit()
         exp_data.add_jobs(job)
-        exp_data.save()
+        exp_data.save(suppress_errors=False)
         self.experiments_to_delete.append(exp_data.experiment_id)
 
         rexp = self.service.experiment(exp_data.experiment_id)
         self.assertEqual([job.job_id()], rexp.job_ids)
 
     def test_auto_save_experiment(self):
         """Test auto save."""
@@ -516,37 +521,54 @@
             job = self._run_circuit()
             exp_data.add_jobs(job)
             jobs.append(job)
         exp_data.block_for_results()
         self.assertTrue(all(job.status() == JobStatus.DONE for job in jobs))
         self.assertEqual(ExperimentStatus.DONE, exp_data.status())
 
+    def test_file_upload_download(self):
+        """test upload and download of actual experiment data"""
+        exp_id = self._create_experiment_data().experiment_id
+        qc = QuantumCircuit(2)
+        qc.h(0)
+        qc.measure_all()
+        data = {"string": "b-string", "int": 10, "float": 0.333, "circuit": qc}
+        json_filename = "data.json"
+
+        self.service.file_upload(
+            exp_id, json_filename, data, json_encoder=ExperimentEncoder
+        )
+        rjson_data = self.service.file_download(
+            exp_id, json_filename, json_decoder=ExperimentDecoder
+        )
+        self.assertEqual(data, rjson_data)
+
     def _create_experiment_data(self):
         """Create an experiment data."""
         exp_data = ExperimentData(
             backend=self.backend,
             experiment_type="qiskit_test",
             verbose=False,
             service=self.service,
         )
-        exp_data.save()
+        exp_data.save(suppress_errors=False)
         self.experiments_to_delete.append(exp_data.experiment_id)
         return exp_data
 
     def _create_analysis_result(self):
         """Create a simple analysis result."""
         exp_data = self._create_experiment_data()
         aresult = AnalysisResult(
             value={},
             name="qiskit_test",
             device_components=self.device_components,
             experiment_id=exp_data.experiment_id,
         )
         exp_data.add_analysis_results(aresult)
-        exp_data.save()
+        exp_data.save(suppress_errors=False)
         self.results_to_delete.append(aresult.result_id)
         return aresult, exp_data
 
     def _run_circuit(self, circuit=None):
         """Run a circuit."""
         circuit = circuit or self.circuit
         job = self.backend.run(circuit, shots=1)
```

### Comparing `qiskit-ibm-experiment-0.3.3/test/service/test_experiment_server_integration.py` & `qiskit-ibm-experiment-0.3.4/test/service/test_experiment_server_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 """Experiment integration test with server."""
 
 import os
 import uuid
 import unittest
 import json
 import re
-from unittest import mock, SkipTest, skipIf
+from unittest import mock, skipIf
 from datetime import datetime, timedelta
 from typing import Optional, Dict, Any
 from test.service.ibm_test_case import IBMTestCase
 from test.utils.utils import ExperimentEncoder, ExperimentDecoder
 import numpy as np
 from dateutil import tz
+import yaml
 from qiskit_ibm_provider import IBMProvider
 from qiskit_ibm_experiment.service import ResultQuality, ExperimentShareLevel
 from qiskit_ibm_experiment import IBMExperimentEntryNotFound, IBMApiError
 from qiskit_ibm_experiment import IBMExperimentService
 from qiskit_ibm_experiment import ExperimentData, AnalysisResultData
 
 
@@ -43,15 +44,15 @@
         super().setUpClass()
         cls.default_exp_type = "qiskit_test"
         try:
             cls._setup_service()
             cls._setup_provider()
         except Exception as err:
             cls.log.info("Error while setting the service/provider: %s", err)
-            raise SkipTest("Not authorized to use experiment service.") from err
+            raise
 
     @classmethod
     def _setup_service(cls):
         """Get the service for the class."""
         cls.service = IBMExperimentService(
             token=os.getenv("QISKIT_IBM_STAGING_API_TOKEN"),
             url=os.getenv("QISKIT_IBM_STAGING_API_URL"),
@@ -558,15 +559,15 @@
                 job_ids=["job1", "job2"],
                 tags=["qiskit_test"],
                 notes="some notes",
                 share_level=ExperimentShareLevel.PROJECT,
                 start_datetime=datetime.now(),
             ),
             provider=self.provider,
-        )
+        )["uuid"]
         self.experiments_to_delete.append(new_exp_id)
         self.assertEqual(exp_id, new_exp_id)
         new_exp = self.service.experiment(new_exp_id)
 
         hub, group, project = list(self.provider._hgps)[0].split("/")
         self.assertEqual(hub, new_exp.hub)  # pylint: disable=no-member
         self.assertEqual(group, new_exp.group)  # pylint: disable=no-member
@@ -1500,14 +1501,33 @@
         filename = "another_data_file"
         self.service.file_upload(exp_id, filename, data)
         rdata = self.service.file_download(exp_id, filename)
         self.assertEqual(data, rdata)
         file_list = self.service.files(exp_id)["files"]
         self.assertEqual(len(file_list), 2)
 
+    def test_file_upload_formats(self):
+        """Test file upload/download for JSON and YAML formats"""
+        exp_id = self._create_experiment()
+        data = {"string": "b-string", "int": 10, "float": 0.333}
+        yaml_data = yaml.dump(data)
+        json_data = json.dumps(data)
+        yaml_filename = "data.yaml"
+        json_filename = "data.json"
+
+        self.service.file_upload(exp_id, json_filename, json_data)
+        rjson_data = self.service.file_download(exp_id, json_filename)
+        self.assertEqual(data, rjson_data)
+
+        self.service.file_upload(exp_id, yaml_filename, yaml_data)
+        ryaml_data = self.service.file_download(exp_id, yaml_filename)
+        self.assertEqual(data, ryaml_data)
+        file_list = self.service.files(exp_id)["files"]
+        self.assertEqual(len(file_list), 2)
+
     def _create_experiment(
         self,
         experiment_type: Optional[str] = None,
         backend_name: Optional[str] = None,
         json_encoder: Optional[json.JSONEncoder] = None,
         **kwargs,
     ) -> str:
@@ -1517,15 +1537,15 @@
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type=experiment_type,
                 backend=backend_name,
                 **kwargs,
             ),
             json_encoder=json_encoder,
-        )
+        )["uuid"]
         self.experiments_to_delete.append(exp_id)
         return exp_id
 
     def _create_analysis_result(
         self,
         exp_id: Optional[str] = None,
         result_type: Optional[str] = None,
```

### Comparing `qiskit-ibm-experiment-0.3.3/test/service/test_local_experiment_client.py` & `qiskit-ibm-experiment-0.3.4/test/service/test_local_experiment_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import unittest
 import uuid
 import json
 from typing import Optional, Dict, Any
 from datetime import datetime, timedelta
 from test.service.ibm_test_case import IBMTestCase
 from dateutil import tz
+import yaml
 from qiskit_ibm_experiment import IBMExperimentService
 from qiskit_ibm_experiment import ExperimentData, AnalysisResultData
 from qiskit_ibm_experiment.service import ResultQuality
 from qiskit_ibm_experiment.exceptions import (
     IBMExperimentEntryNotFound,
     IBMExperimentEntryExists,
 )
@@ -402,14 +403,33 @@
                     tags=tags,
                     sort_by=sort_by,
                     experiment_type_operator="like",
                     experiment_type="qiskit_test",
                 )
                 self.assertEqual(expected, [exp.experiment_id for exp in experiments])
 
+    def test_file_upload_formats(self):
+        """Test file upload/download for JSON and YAML formats"""
+        exp_id = self._create_experiment()
+        data = {"string": "b-string", "int": 10, "float": 0.333}
+        yaml_data = yaml.dump(data)
+        json_data = json.dumps(data)
+        yaml_filename = "data.yaml"
+        json_filename = "data.json"
+
+        self.service.file_upload(exp_id, json_filename, json_data)
+        rjson_data = self.service.file_download(exp_id, json_filename)
+        self.assertEqual(data, rjson_data)
+
+        self.service.file_upload(exp_id, yaml_filename, yaml_data)
+        ryaml_data = self.service.file_download(exp_id, yaml_filename)
+        self.assertEqual(data, ryaml_data)
+        file_list = self.service.files(exp_id)["files"]
+        self.assertEqual(len(file_list), 2)
+
     def _create_experiment(
         self,
         experiment_type: Optional[str] = None,
         json_encoder: Optional[json.JSONEncoder] = None,
         **kwargs,
     ) -> str:
         """Create a new experiment."""
```

### Comparing `qiskit-ibm-experiment-0.3.3/test/utils/program.py` & `qiskit-ibm-experiment-0.3.4/test/utils/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/test/utils/templates.py` & `qiskit-ibm-experiment-0.3.4/test/utils/templates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.3/test/utils/utils.py` & `qiskit-ibm-experiment-0.3.4/test/utils/utils.py`

 * *Files identical despite different names*

