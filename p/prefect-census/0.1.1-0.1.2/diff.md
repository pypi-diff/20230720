# Comparing `tmp/prefect-census-0.1.1.tar.gz` & `tmp/prefect-census-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-census/prefect-census/dist/.tmp-cxtg8u1r/prefect-census-0.1.1.tar", last modified: Thu Feb  2 21:43:04 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-census/prefect-census/dist/.tmp-nk559lmp/prefect-census-0.1.2.tar", last modified: Thu Jul 20 18:48:18 2023, max compression
```

## Comparing `prefect-census-0.1.1.tar` & `prefect-census-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:43:04.000000 prefect-census-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-02-02 21:41:28.000000 prefect-census-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-02 21:41:28.000000 prefect-census-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-02-02 21:43:04.000000 prefect-census-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-02-02 21:41:28.000000 prefect-census-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/flows.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/runs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/syncs.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-02-02 21:41:28.000000 prefect-census-0.1.1/prefect_census/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-02 21:43:04.000000 prefect-census-0.1.1/prefect_census.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-02-02 21:41:28.000000 prefect-census-0.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-02 21:41:28.000000 prefect-census-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-02-02 21:43:04.000000 prefect-census-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-02-02 21:41:28.000000 prefect-census-0.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-02-02 21:41:28.000000 prefect-census-0.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:48:18.000000 prefect-census-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-20 18:47:25.000000 prefect-census-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 18:47:25.000000 prefect-census-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-20 18:48:18.000000 prefect-census-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-20 18:47:25.000000 prefect-census-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/syncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-20 18:47:25.000000 prefect-census-0.1.2/prefect_census/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 18:48:18.000000 prefect-census-0.1.2/prefect_census.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 18:47:25.000000 prefect-census-0.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 18:47:25.000000 prefect-census-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-20 18:48:18.000000 prefect-census-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-07-20 18:47:25.000000 prefect-census-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:48:18.000000 prefect-census-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-20 18:47:25.000000 prefect-census-0.1.2/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-20 18:47:25.000000 prefect-census-0.1.2/tests/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-07-20 18:47:25.000000 prefect-census-0.1.2/tests/test_syncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-07-20 18:47:25.000000 prefect-census-0.1.2/versioneer.py
```

### Comparing `prefect-census-0.1.1/LICENSE` & `prefect-census-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/PKG-INFO` & `prefect-census-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-census
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prefect integrations for working with Census syncs
 Home-page: https://github.com/PrefectHQ/prefect-census
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-census-0.1.1/README.md` & `prefect-census-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/prefect_census/client.py` & `prefect-census-0.1.2/prefect_census/client.py`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/prefect_census/credentials.py` & `prefect-census-0.1.2/prefect_census/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/prefect_census/flows.py` & `prefect-census-0.1.2/prefect_census/flows.py`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/prefect_census/runs.py` & `prefect-census-0.1.2/prefect_census/runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     """Census sync statuses."""
 
     CANCELLED = "cancelled"
     WORKING = "working"
     FAILED = "failed"
     COMPLETED = "completed"
     SKIPPED = "skipped"
+    QUEUED = "queued"
 
     @classmethod
     def is_terminal_status_code(cls, status_code: str) -> bool:
         """
         Returns True if a status code is terminal for a sync run.
         Returns False otherwise.
         """
```

### Comparing `prefect-census-0.1.1/prefect_census/syncs.py` & `prefect-census-0.1.2/prefect_census/syncs.py`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/prefect_census/utils.py` & `prefect-census-0.1.2/prefect_census/utils.py`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/prefect_census.egg-info/PKG-INFO` & `prefect-census-0.1.2/prefect_census.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-census
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prefect integrations for working with Census syncs
 Home-page: https://github.com/PrefectHQ/prefect-census
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-census-0.1.1/prefect_census.egg-info/SOURCES.txt` & `prefect-census-0.1.2/prefect_census.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -15,8 +15,11 @@
 prefect_census/syncs.py
 prefect_census/utils.py
 prefect_census.egg-info/PKG-INFO
 prefect_census.egg-info/SOURCES.txt
 prefect_census.egg-info/dependency_links.txt
 prefect_census.egg-info/entry_points.txt
 prefect_census.egg-info/requires.txt
-prefect_census.egg-info/top_level.txt
+prefect_census.egg-info/top_level.txt
+tests/test_block_standards.py
+tests/test_runs.py
+tests/test_syncs.py
```

### Comparing `prefect-census-0.1.1/setup.cfg` & `prefect-census-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/setup.py` & `prefect-census-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-census-0.1.1/versioneer.py` & `prefect-census-0.1.2/versioneer.py`

 * *Files identical despite different names*

