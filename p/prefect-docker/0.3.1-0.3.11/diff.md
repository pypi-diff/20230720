# Comparing `tmp/prefect-docker-0.3.1.tar.gz` & `tmp/prefect-docker-0.3.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-0nw3a3ow/prefect-docker-0.3.1.tar", last modified: Mon Jun 26 14:27:49 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-docker/prefect-docker/dist/.tmp-7qfk5eav/prefect-docker-0.3.11.tar", last modified: Thu Jul 20 14:29:07 2023, max compression
```

## Comparing `prefect-docker-0.3.1.tar` & `prefect-docker-0.3.11.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    29217 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 14:27:49.000000 prefect-docker-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/tests/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-26 14:26:05.000000 prefect-docker-0.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-20 14:28:20.000000 prefect-docker-0.3.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 14:28:20.000000 prefect-docker-0.3.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-20 14:28:20.000000 prefect-docker-0.3.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29082 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5653 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:29:07.000000 prefect-docker-0.3.11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/tests/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-20 14:28:21.000000 prefect-docker-0.3.11/versioneer.py
```

### Comparing `prefect-docker-0.3.1/LICENSE` & `prefect-docker-0.3.11/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/PKG-INFO` & `prefect-docker-0.3.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.3.1
+Version: 0.3.11
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.3.1/README.md` & `prefect-docker-0.3.11/README.md`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/prefect_docker/containers.py` & `prefect-docker-0.3.11/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/prefect_docker/credentials.py` & `prefect-docker-0.3.11/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/prefect_docker/deployments/steps.py` & `prefect-docker-0.3.11/prefect_docker/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/prefect_docker/host.py` & `prefect-docker-0.3.11/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/prefect_docker/images.py` & `prefect-docker-0.3.11/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/prefect_docker/worker.py` & `prefect-docker-0.3.11/prefect_docker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 """
-<span class="badge-api beta"/>
-
 Module containing the Docker worker used for executing flow runs as Docker containers.
 
-Note this module is in **beta**. The interfaces within may change without notice.
-
 To start a Docker worker, run the following command:
 
 ```bash
 prefect worker start --pool 'my-work-pool' --type docker
 ```
 
 Replace `my-work-pool` with the name of the work pool you want the worker
@@ -367,15 +363,14 @@
     _description = (
         "Execute flow runs within Docker containers. Works well for managing flow "
         "execution environments via Docker images. Requires access to a running "
         "Docker daemon."
     )
     _display_name = "Docker"
     _documentation_url = "https://prefecthq.github.io/prefect-docker/worker/"
-    _is_beta = True
     _logo_url = "https://images.ctfassets.net/gm98wzqotmnx/2IfXXfMq66mrzJBDFFCHTp/6d8f320d9e4fc4393f045673d61ab612/Moby-logo.png?h=250"  # noqa
 
     def __init__(self, *args: Any, test_mode: bool = None, **kwargs: Any) -> None:
         if test_mode is None:
             self.test_mode = bool(os.getenv("PREFECT_DOCKER_TEST_MODE", False))
         else:
             self.test_mode = test_mode
```

### Comparing `prefect-docker-0.3.1/prefect_docker.egg-info/PKG-INFO` & `prefect-docker-0.3.11/prefect_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.3.1
+Version: 0.3.11
 Summary: Prefect integrations for working with Docker
 Home-page: https://github.com/PrefectHQ/prefect-docker
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-docker-0.3.1/prefect_docker.egg-info/SOURCES.txt` & `prefect-docker-0.3.11/prefect_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/setup.cfg` & `prefect-docker-0.3.11/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/setup.py` & `prefect-docker-0.3.11/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/tests/test_containers.py` & `prefect-docker-0.3.11/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/tests/test_host.py` & `prefect-docker-0.3.11/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/tests/test_images.py` & `prefect-docker-0.3.11/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/tests/test_worker.py` & `prefect-docker-0.3.11/tests/test_worker.py`

 * *Files identical despite different names*

### Comparing `prefect-docker-0.3.1/versioneer.py` & `prefect-docker-0.3.11/versioneer.py`

 * *Files identical despite different names*

