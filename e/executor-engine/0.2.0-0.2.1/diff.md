# Comparing `tmp/executor-engine-0.2.0.tar.gz` & `tmp/executor-engine-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "executor-engine-0.2.0.tar", last modified: Thu May 11 14:31:48 2023, max compression
+gzip compressed data, was "executor-engine-0.2.1.tar", last modified: Thu Jul 20 13:52:18 2023, max compression
```

## Comparing `executor-engine-0.2.0.tar` & `executor-engine-0.2.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.739999 executor-engine-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-11 14:31:31.000000 executor-engine-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 14:31:48.739999 executor-engine-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-05-11 14:31:31.000000 executor-engine-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.731999 executor-engine-0.2.0/executor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.735999 executor-engine-0.2.0/executor/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.735999 executor-engine-0.2.0/executor/engine/job/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.735999 executor-engine-0.2.0/executor/engine/job/extend/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/extend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/extend/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/extend/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.739999 executor-engine-0.2.0/executor/engine/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/launcher/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.739999 executor-engine-0.2.0/executor/engine/middle/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/middle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/middle/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/middle/dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-11 14:31:31.000000 executor-engine-0.2.0/executor/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:31:48.739999 executor-engine-0.2.0/executor_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-11 14:31:48.000000 executor-engine-0.2.0/executor_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-05-11 14:31:48.000000 executor-engine-0.2.0/executor_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:31:48.000000 executor-engine-0.2.0/executor_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:31:48.000000 executor-engine-0.2.0/executor_engine.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-11 14:31:48.000000 executor-engine-0.2.0/executor_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-11 14:31:48.000000 executor-engine-0.2.0/executor_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:31:48.739999 executor-engine-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-05-11 14:31:31.000000 executor-engine-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.421561 executor-engine-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-20 13:52:05.000000 executor-engine-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 13:52:18.421561 executor-engine-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-20 13:52:05.000000 executor-engine-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.413563 executor-engine-0.2.1/executor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.417562 executor-engine-0.2.1/executor/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.417562 executor-engine-0.2.1/executor/engine/job/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.417562 executor-engine-0.2.1/executor/engine/job/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/extend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/extend/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/extend/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.417562 executor-engine-0.2.1/executor/engine/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/launcher/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.417562 executor-engine-0.2.1/executor/engine/middle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/middle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/middle/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/middle/dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-07-20 13:52:05.000000 executor-engine-0.2.1/executor/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:52:18.421561 executor-engine-0.2.1/executor_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 13:52:18.000000 executor-engine-0.2.1/executor_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-20 13:52:18.000000 executor-engine-0.2.1/executor_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:52:18.000000 executor-engine-0.2.1/executor_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:52:18.000000 executor-engine-0.2.1/executor_engine.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 13:52:18.000000 executor-engine-0.2.1/executor_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 13:52:18.000000 executor-engine-0.2.1/executor_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:52:18.421561 executor-engine-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-20 13:52:05.000000 executor-engine-0.2.1/setup.py
```

### Comparing `executor-engine-0.2.0/LICENSE` & `executor-engine-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/PKG-INFO` & `executor-engine-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: executor-engine
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for manage job executions.
 Home-page: https://github.com/Nanguage/executor-engine
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT
 Keywords: Job Management
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `executor-engine-0.2.0/README.md` & `executor-engine-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/core.py` & `executor-engine-0.2.1/executor/engine/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,21 +273,29 @@
             if n_wait_jobs == 0:
                 break
             if total_time <= 0:
                 break
             await asyncio.sleep(time_delta)
             total_time -= time_delta
 
-    async def join(self, timeout: T.Optional[float] = None):
+    async def join(
+            self,
+            jobs: T.Optional[T.List[Job]] = None,
+            timeout: T.Optional[float] = None):
         """Join all running and pending jobs."""
-        running = self.jobs.running.values()
-        pending = self.jobs.pending.values()
+        if jobs is None:
+            jobs_for_join = (
+                self.jobs.running.values() +
+                self.jobs.pending.values()
+            )
+        else:
+            jobs_for_join = jobs
         tasks = [
             asyncio.create_task(job.join())
-            for job in (running + pending)
+            for job in jobs_for_join
         ]
         if len(tasks) > 0:
             await asyncio.wait(tasks, timeout=timeout)
 
     def get_cache_dir(self) -> Path:
         """Get cache directory for engine."""
         cache_path = self.setting.cache_path
```

### Comparing `executor-engine-0.2.0/executor/engine/job/base.py` & `executor-engine-0.2.1/executor/engine/job/base.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/condition.py` & `executor-engine-0.2.1/executor/engine/job/condition.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/dask.py` & `executor-engine-0.2.1/executor/engine/job/dask.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/extend/subprocess.py` & `executor-engine-0.2.1/executor/engine/job/extend/subprocess.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/extend/webapp.py` & `executor-engine-0.2.1/executor/engine/job/extend/webapp.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/process.py` & `executor-engine-0.2.1/executor/engine/job/process.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/thread.py` & `executor-engine-0.2.1/executor/engine/job/thread.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/job/utils.py` & `executor-engine-0.2.1/executor/engine/job/utils.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/launcher/core.py` & `executor-engine-0.2.1/executor/engine/launcher/core.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/manager.py` & `executor-engine-0.2.1/executor/engine/manager.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/middle/capture.py` & `executor-engine-0.2.1/executor/engine/middle/capture.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor/engine/utils.py` & `executor-engine-0.2.1/executor/engine/utils.py`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/executor_engine.egg-info/PKG-INFO` & `executor-engine-0.2.1/executor_engine.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: executor-engine
-Version: 0.2.0
+Version: 0.2.1
 Summary: Package for manage job executions.
 Home-page: https://github.com/Nanguage/executor-engine
 Author: Weize Xu
 Author-email: vet.xwz@gmail.com
 License: MIT
 Keywords: Job Management
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `executor-engine-0.2.0/executor_engine.egg-info/SOURCES.txt` & `executor-engine-0.2.1/executor_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `executor-engine-0.2.0/setup.py` & `executor-engine-0.2.1/setup.py`

 * *Files identical despite different names*

