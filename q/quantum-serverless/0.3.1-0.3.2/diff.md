# Comparing `tmp/quantum_serverless-0.3.1.tar.gz` & `tmp/quantum_serverless-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantum_serverless-0.3.1.tar", last modified: Fri Jul 14 11:35:00 2023, max compression
+gzip compressed data, was "quantum_serverless-0.3.2.tar", last modified: Thu Jul 20 15:36:39 2023, max compression
```

## Comparing `quantum_serverless-0.3.1.tar` & `quantum_serverless-0.3.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.636289 quantum_serverless-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-14 11:35:00.636289 quantum_serverless-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/program.py
--rw-r--r--   0 runner    (1001) docker     (123)    19102 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/core/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless/library/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/library/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/quantum_serverless.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/serializers/program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/serializers/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/utils/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless/visualizaiton/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/visualizaiton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/quantum_serverless/visualizaiton/widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/quantum_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-14 11:35:00.000000 quantum_serverless-0.3.1/quantum_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-14 11:35:00.000000 quantum_serverless-0.3.1/quantum_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 11:35:00.000000 quantum_serverless-0.3.1/quantum_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-14 11:35:00.000000 quantum_serverless-0.3.1/quantum_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 11:35:00.000000 quantum_serverless-0.3.1/quantum_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-14 11:35:00.636289 quantum_serverless-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/core/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/core/test_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/core/test_program_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/core/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.632289 quantum_serverless-0.3.1/tests/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/library/test_transpiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 11:35:00.636289 quantum_serverless-0.3.1/tests/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/serializers/test_program_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/serializers/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/test_quantum_serverless.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-14 11:34:52.000000 quantum_serverless-0.3.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.375639 quantum_serverless-0.3.2/quantum_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.375639 quantum_serverless-0.3.2/quantum_serverless/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12729 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12264 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/core/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.375639 quantum_serverless-0.3.2/quantum_serverless/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/library/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/quantum_serverless.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.375639 quantum_serverless-0.3.2/quantum_serverless/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/serializers/program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/serializers/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.375639 quantum_serverless-0.3.2/quantum_serverless/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/utils/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/quantum_serverless/visualizaiton/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/visualizaiton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/quantum_serverless/visualizaiton/widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.375639 quantum_serverless-0.3.2/quantum_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-20 15:36:39.000000 quantum_serverless-0.3.2/quantum_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 15:36:39.000000 quantum_serverless-0.3.2/quantum_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:36:39.000000 quantum_serverless-0.3.2/quantum_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-20 15:36:39.000000 quantum_serverless-0.3.2/quantum_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 15:36:39.000000 quantum_serverless-0.3.2/quantum_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/core/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/core/test_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/core/test_program_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/core/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/tests/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/library/test_transpiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:39.379639 quantum_serverless-0.3.2/tests/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/serializers/test_program_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/serializers/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/test_quantum_serverless.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 15:36:29.000000 quantum_serverless-0.3.2/tests/utils.py
```

### Comparing `quantum_serverless-0.3.1/PKG-INFO` & `quantum_serverless-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum_serverless
-Version: 0.3.1
+Version: 0.3.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.3.1/README.md` & `quantum_serverless-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/__init__.py` & `quantum_serverless-0.3.2/quantum_serverless/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from .core import (
     BaseProvider,
     distribute_task,
     get,
     put,
     get_refs_by_status,
-    KuberayProvider,
     Provider,
     save_result,
 )
 from .quantum_serverless import (
     QuantumServerless,
     get_auto_discovered_provider,
     QuantumServerlessException,
```

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/__init__.py` & `quantum_serverless-0.3.2/quantum_serverless/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 -----------------
 
 .. autosummary::
     :toctree: ../stubs/
 
     Provider
     BaseProvider
-    KuberayProvider
     ComputeResource
     Job
     GatewayJobClient
     BaseJobClient
     RayJobClient
     save_result
     Program
@@ -64,15 +63,15 @@
 .. autosummary::
     :toctree: ../stubs/
 
     StateHandler
     RedisStateHandler
 """
 
-from .provider import BaseProvider, ComputeResource, KuberayProvider, Provider
+from .provider import BaseProvider, ComputeResource, Provider
 from .job import BaseJobClient, RayJobClient, GatewayJobClient, Job, save_result
 from .program import (
     Program,
     ProgramStorage,
     ProgramRepository,
     download_and_unpack_artifact,
 )
```

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/constants.py` & `quantum_serverless-0.3.2/quantum_serverless/core/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,14 @@
 
 
 # repository
 REPO_HOST_KEY = "REPO_HOST_KEY"
 REPO_PORT_KEY = "REPO_PORT_KEY"
 
 
-# container image
-RAY_IMAGE = "icr.io/quantum-public/quantum-serverless-ray-node:latest-py39"
-
 # keycloak
 ENV_KEYCLOAK_REALM = "ENV_KEYCLOAK_REALM"
 ENV_KEYCLOAK_CLIENT_ID = "ENV_KEYCLOAK_CLIENT_ID"
 
 # request timeout
 REQUESTS_TIMEOUT: int = 30
```

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/decorators.py` & `quantum_serverless-0.3.2/quantum_serverless/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/events.py` & `quantum_serverless-0.3.2/quantum_serverless/core/events.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/job.py` & `quantum_serverless-0.3.2/quantum_serverless/core/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,18 @@
     ENV_JOB_ID_GATEWAY,
     ENV_GATEWAY_PROVIDER_VERSION,
     GATEWAY_PROVIDER_VERSION_DEFAULT,
     MAX_ARTIFACT_FILE_SIZE_MB,
 )
 from quantum_serverless.core.program import Program
 from quantum_serverless.exception import QuantumServerlessException
-from quantum_serverless.serializers.program_serializers import QiskitObjectsEncoder
+from quantum_serverless.serializers.program_serializers import (
+    QiskitObjectsEncoder,
+    QiskitObjectsDecoder,
+)
 from quantum_serverless.utils.json import is_jsonable, safe_json_request
 
 RuntimeEnv = ray.runtime_env.RuntimeEnv
 
 
 class BaseJobClient:
     """Base class for Job clients."""
@@ -258,15 +261,17 @@
         response_data = safe_json_request(
             request=lambda: requests.get(
                 f"{self.host}/api/{self.version}/jobs/{job_id}/",
                 headers={"Authorization": f"Bearer {self._token}"},
                 timeout=REQUESTS_TIMEOUT,
             )
         )
-        return json.loads(response_data.get("result", "{}") or "{}")
+        return json.loads(
+            response_data.get("result", "{}") or "{}", cls=QiskitObjectsDecoder
+        )
 
     def get(self, job_id) -> Optional["Job"]:
         url = f"{self.host}/api/{self.version}/jobs/{job_id}/"
         response_data = safe_json_request(
             request=lambda: requests.get(
                 url,
                 headers={"Authorization": f"Bearer {self._token}"},
@@ -381,15 +386,15 @@
 
     url = (
         f"{os.environ.get(ENV_JOB_GATEWAY_HOST)}/"
         f"api/{version}/jobs/{os.environ.get(ENV_JOB_ID_GATEWAY)}/result/"
     )
     response = requests.post(
         url,
-        json={"result": result},
+        data={"result": json.dumps(result or {}, cls=QiskitObjectsEncoder)},
         headers={"Authorization": f"Bearer {token}"},
         timeout=REQUESTS_TIMEOUT,
     )
     if not response.ok:
         logging.warning("Something went wrong: %s", response.text)
 
     return response.ok
```

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/program.py` & `quantum_serverless-0.3.2/quantum_serverless/core/program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/provider.py` & `quantum_serverless-0.3.2/quantum_serverless/core/provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,22 +26,20 @@
     ComputeResource
     Provider
 """
 import logging
 import os.path
 from dataclasses import dataclass
 from typing import Optional, List, Dict, Any
-import warnings
 
 import ray
 import requests
 from ray.dashboard.modules.job.sdk import JobSubmissionClient
 
 from quantum_serverless.core.constants import (
-    RAY_IMAGE,
     REQUESTS_TIMEOUT,
     ENV_GATEWAY_PROVIDER_HOST,
     ENV_GATEWAY_PROVIDER_VERSION,
     GATEWAY_PROVIDER_VERSION_DEFAULT,
 )
 from quantum_serverless.core.job import (
     Job,
@@ -281,208 +279,14 @@
                 f"Selected provider: {self}"
             )
             return None
 
         return job_client.run(program, arguments)
 
 
-class KuberayProvider(BaseProvider):
-    """(Deprecated) Implements CRUD for Kuberay API server."""
-
-    def __init__(
-        self,
-        name: str,
-        host: Optional[str] = None,
-        namespace: Optional[str] = "default",
-        img: Optional[str] = RAY_IMAGE,
-        token: Optional[str] = None,
-        compute_resource: Optional[ComputeResource] = None,
-        available_compute_resources: Optional[List[ComputeResource]] = None,
-    ):
-        """(Deprecated) Kuberay provider for serverless computation.
-
-        Example:
-            >>> provider = Provider(
-            >>>    name="<NAME>",
-            >>>    host="<HOST>",
-            >>>    namespace="<NAMESPACE>",
-            >>>    token="<TOKEN>",
-            >>>    compute_resource=ComputeResource(
-            >>>        name="<COMPUTE_RESOURCE_NAME>",
-            >>>        host="<COMPUTE_RESOURCE_HOST>"
-            >>>    ),
-            >>> )
-
-        Args:
-            name: name of provider
-            host: host of provider a.k.a managers host
-            namespace: namespace to deploy provider in
-            image: container image to use for ray cluster
-            token: authentication token for manager
-            compute_resource: selected compute_resource from provider
-            available_compute_resources: available clusters in provider
-        """
-        super().__init__(name)
-        warnings.warn(
-            "`KuberayProvider` is deprecated "
-            "and will be removed in v0.3. "
-            "Please, consider using `Provider`.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
-
-        self.name = name
-        self.host = host
-        self.token = token
-        self.namespace = namespace
-        self.image = img
-        self.compute_resource = compute_resource
-        if available_compute_resources is None:
-            if compute_resource is not None:
-                available_compute_resources = [compute_resource]
-            else:
-                available_compute_resources = []
-        self.available_compute_resources = available_compute_resources
-        self.api_root = f"{self.host}/apis/v1alpha2/namespaces/{self.namespace}"
-
-    def get_compute_resources(self) -> List[ComputeResource]:
-        """Return compute resources for provider."""
-        req = requests.get(self.api_root + "/clusters", timeout=TIMEOUT)
-        if req.status_code != 200 or not req.json():
-            return []
-
-        clusters = req.json()["clusters"]
-
-        resources = []
-        # for each cluster, create a ComputeResource and append it
-        for cluster in clusters:
-            resource = ComputeResource(name=cluster["name"])
-            resources.append(resource)
-
-        return resources
-
-    def create_compute_resource(self, resource) -> int:
-        """
-        Create compute resource for provider.
-
-        First, create a compute_template based on the defined ComputeResource.
-        If the compute_template already exists (which shouldn't be the case,
-        exit silently. Otherwise, create the template. This template is
-        ephemeral and will be deleted when no longer needed (either the cluster
-        was created or we failed to create it and thus need to start over).
-
-        Then use that template to create a KubeRay Cluster. If the cluster
-        already exists, we exit silently. Users are only able to configure the
-        amount of cpu/memory and the number of worker replicas. The full spec
-        can be found in the KubeRay API spec under the "protoCluster"
-        definition:
-        https://github.com/ray-project/kuberay/blob/master/proto/swagger/cluster.swagger.json
-        """
-        template_name = self.name + "-template"
-
-        # Create template from resource
-        req = requests.get(
-            self.api_root + f"/compute_templates/{template_name}",
-            timeout=TIMEOUT,
-        )
-        if req.ok:
-            print(f"template name {template_name} already exists")
-            return 1
-
-        data = {
-            "name": template_name,
-            "namespace": self.namespace,
-            "cpu": resource.resources["cpu"],
-            "memory": resource.resources["memory"],
-        }
-        req = requests.post(
-            self.api_root + "/compute_templates", json=data, timeout=TIMEOUT
-        )
-        if not req.ok:
-            req.raise_for_status()
-            return 1
-
-        # Create cluster from template
-        req = requests.get(
-            self.api_root + f"/clusters/{self.name}",
-            timeout=TIMEOUT,
-        )
-        if req.ok:
-            print(f"cluster {self.name} already exists")
-            self.delete_kuberay_template(template_name)
-            return 1
-
-        data = {
-            "name": self.name,
-            "namespace": self.namespace,
-            "user": "default",
-            "clusterSpec": {
-                "headGroupSpec": {
-                    "computeTemplate": template_name,
-                    "image": self.image,
-                    "rayStartParams": {
-                        "dashboard-host": "127.0.0.1",
-                        "metrics-export-port": "8080",
-                    },
-                    "volumes": [],
-                },
-            },
-            "workerGroupSpec": [
-                {
-                    "groupName": "default-group",
-                    "computeTemplate": template_name,
-                    "image": self.image,
-                    "replicas": resource.resources["worker_replicas"],
-                    "rayStartParams": {
-                        "node-ip-address": "$MY_POD_IP",
-                    },
-                },
-            ],
-        }
-        req = requests.post(
-            self.api_root + "/clusters",
-            json=data,
-            timeout=TIMEOUT,
-        )
-        if req.status_code != 200:
-            self.delete_kuberay_template(template_name)
-            req.raise_for_status()
-            return 1
-
-        # Delete template
-        req = self.delete_kuberay_template(template_name)
-        if req.status_code != 200:
-            req.raise_for_status()
-            return 1
-
-        return 0
-
-    def delete_compute_resource(self, resource) -> int:
-        """Delete compute resource for provider."""
-        req = requests.delete(
-            self.api_root + f"/clusters/{resource}",
-            timeout=TIMEOUT,
-        )
-        if req.status_code != 200:
-            req.raise_for_status()
-            return 1
-
-        return 0
-
-    def delete_kuberay_template(self, resource):
-        """Delete a KubeRay compute template (helper function."""
-        return requests.delete(
-            self.api_root + f"/compute_templates/{resource}",
-            timeout=TIMEOUT,
-        )
-
-    def get_jobs(self, **kwargs) -> List[Job]:
-        raise NotImplementedError
-
-
 class Provider(BaseProvider):
     """Provider."""
 
     def __init__(
         self,
         name: Optional[str] = None,
         host: Optional[str] = None,
```

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/state.py` & `quantum_serverless-0.3.2/quantum_serverless/core/state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/core/tracing.py` & `quantum_serverless-0.3.2/quantum_serverless/core/tracing.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/exception.py` & `quantum_serverless-0.3.2/quantum_serverless/exception.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/library/__init__.py` & `quantum_serverless-0.3.2/quantum_serverless/library/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/library/transpiler.py` & `quantum_serverless-0.3.2/quantum_serverless/library/transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/quantum_serverless.py` & `quantum_serverless-0.3.2/quantum_serverless/quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/serializers/__init__.py` & `quantum_serverless-0.3.2/quantum_serverless/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/serializers/program_serializers.py` & `quantum_serverless-0.3.2/quantum_serverless/serializers/program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/serializers/serializers.py` & `quantum_serverless-0.3.2/quantum_serverless/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/utils/__init__.py` & `quantum_serverless-0.3.2/quantum_serverless/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/utils/errors.py` & `quantum_serverless-0.3.2/quantum_serverless/utils/errors.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/utils/json.py` & `quantum_serverless-0.3.2/quantum_serverless/utils/json.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/utils/storage.py` & `quantum_serverless-0.3.2/quantum_serverless/utils/storage.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/visualizaiton/__init__.py` & `quantum_serverless-0.3.2/quantum_serverless/visualizaiton/__init__.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless/visualizaiton/widget.py` & `quantum_serverless-0.3.2/quantum_serverless/visualizaiton/widget.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/quantum_serverless.egg-info/PKG-INFO` & `quantum_serverless-0.3.2/quantum_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantum-serverless
-Version: 0.3.1
+Version: 0.3.2
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: quantum serverless qiskit
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `quantum_serverless-0.3.1/quantum_serverless.egg-info/SOURCES.txt` & `quantum_serverless-0.3.2/quantum_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/setup.py` & `quantum_serverless-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/core/test_decorator.py` & `quantum_serverless-0.3.2/tests/core/test_decorator.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/core/test_program.py` & `quantum_serverless-0.3.2/tests/core/test_program.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/core/test_program_repository.py` & `quantum_serverless-0.3.2/tests/core/test_program_repository.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/core/test_state.py` & `quantum_serverless-0.3.2/tests/core/test_state.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/library/test_transpiler.py` & `quantum_serverless-0.3.2/tests/library/test_transpiler.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/serializers/test_program_serializers.py` & `quantum_serverless-0.3.2/tests/serializers/test_program_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/serializers/test_serializers.py` & `quantum_serverless-0.3.2/tests/serializers/test_serializers.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/test_quantum_serverless.py` & `quantum_serverless-0.3.2/tests/test_quantum_serverless.py`

 * *Files identical despite different names*

### Comparing `quantum_serverless-0.3.1/tests/utils.py` & `quantum_serverless-0.3.2/tests/utils.py`

 * *Files identical despite different names*

