# Comparing `tmp/morch-1.0.1.tar.gz` & `tmp/morch-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morch-1.0.1.tar", last modified: Thu Jul 20 07:01:36 2023, max compression
+gzip compressed data, was "morch-1.0.2.tar", last modified: Thu Jul 20 12:47:13 2023, max compression
```

## Comparing `morch-1.0.1.tar` & `morch-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 morch-1.0.1/LICENSE
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1418 2023-07-20 07:01:36.978978 morch-1.0.1/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      788 2023-07-20 06:58:40.000000 morch-1.0.1/README.md
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/morch/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 12:33:56.000000 morch-1.0.1/morch/__init__.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/morch/helpers/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      142 2023-06-22 12:33:56.000000 morch-1.0.1/morch/helpers/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 12:33:56.000000 morch-1.0.1/morch/helpers/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-22 12:33:56.000000 morch-1.0.1/morch/helpers/celery_utils.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 12:33:56.000000 morch-1.0.1/morch/helpers/handlers.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2320 2023-07-20 06:59:56.000000 morch-1.0.1/morch/helpers/repository.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 12:33:56.000000 morch-1.0.1/morch/helpers/status.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-22 12:33:56.000000 morch-1.0.1/morch/helpers/utils.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/morch/saga/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 12:33:56.000000 morch-1.0.1/morch/saga/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 12:33:56.000000 morch-1.0.1/morch/saga/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 12:33:56.000000 morch-1.0.1/morch/saga/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5578 2023-07-20 06:58:40.000000 morch-1.0.1/morch/saga/stateful.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/morch/steps/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-22 12:33:56.000000 morch-1.0.1/morch/steps/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 12:33:56.000000 morch-1.0.1/morch/steps/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 12:33:56.000000 morch-1.0.1/morch/steps/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-22 12:33:56.000000 morch-1.0.1/morch/steps/sync.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/morch.egg-info/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1418 2023-07-20 07:01:36.000000 morch-1.0.1/morch.egg-info/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      618 2023-07-20 07:01:36.000000 morch-1.0.1/morch.egg-info/SOURCES.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-07-20 07:01:36.000000 morch-1.0.1/morch.egg-info/dependency_links.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      105 2023-07-20 07:01:36.000000 morch-1.0.1/morch.egg-info/requires.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       12 2023-07-20 07:01:36.000000 morch-1.0.1/morch.egg-info/top_level.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      656 2023-07-20 07:01:36.978978 morch-1.0.1/setup.cfg
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1325 2023-07-20 07:01:30.000000 morch-1.0.1/setup.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 07:01:36.978978 morch-1.0.1/tests/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 morch-1.0.1/tests/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     6615 2023-06-22 12:33:56.000000 morch-1.0.1/tests/test_async_saga.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2086 2023-06-22 12:33:56.000000 morch-1.0.1/tests/test_sync_saga.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 morch-1.0.2/LICENSE
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1430 2023-07-20 12:47:13.340273 morch-1.0.2/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      800 2023-07-20 12:45:57.000000 morch-1.0.2/README.md
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 12:33:56.000000 morch-1.0.2/morch/__init__.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/helpers/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      142 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/celery_utils.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/handlers.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2388 2023-07-20 12:45:57.000000 morch-1.0.2/morch/helpers/repository.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/status.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-22 12:33:56.000000 morch-1.0.2/morch/helpers/utils.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/saga/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 12:33:56.000000 morch-1.0.2/morch/saga/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 12:33:56.000000 morch-1.0.2/morch/saga/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 12:33:56.000000 morch-1.0.2/morch/saga/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5578 2023-07-20 06:58:40.000000 morch-1.0.2/morch/saga/stateful.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch/steps/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-22 12:33:56.000000 morch-1.0.2/morch/steps/sync.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/morch.egg-info/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1430 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      618 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/SOURCES.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/dependency_links.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      107 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/requires.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       12 2023-07-20 12:47:13.000000 morch-1.0.2/morch.egg-info/top_level.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      656 2023-07-20 12:47:13.340273 morch-1.0.2/setup.cfg
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1327 2023-07-20 12:46:33.000000 morch-1.0.2/setup.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-07-20 12:47:13.340273 morch-1.0.2/tests/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 morch-1.0.2/tests/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     6615 2023-06-22 12:33:56.000000 morch-1.0.2/tests/test_async_saga.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2086 2023-06-22 12:33:56.000000 morch-1.0.2/tests/test_sync_saga.py
```

### Comparing `morch-1.0.1/LICENSE` & `morch-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/PKG-INFO` & `morch-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morch
-Version: 1.0.1
+Version: 1.0.2
 Summary: SAGA Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/morch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/morch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
@@ -15,20 +15,24 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Microservice Orchestration (morch)
 
 ### Installation:
-> pip install morch
+
+```bash
+pip install morch
+```
 
 ### Usage:
     coming soon...
 
 ### Description:
 Microservice orchestration architecture provides a robust framework for building and managing complex applications. By leveraging independent services and a centralized orchestrator, you can achieve scalability, fault tolerance, and maintainability. Refer to Chris Richardson's book [Microservices Patterns](https://microservices.io/index.html) for more in-depth guidance on this architecture.
 
 ---
 
 ### Credit:
 This project has been inspired by [saga framework](https://github.com/absent1706/saga-framework) and the book [Microservices Patterns](https://www.amazon.com/Microservices-Patterns-examples-Chris-Richardson/dp/1617294543) written by Chris Richardson.
 
+
```

### Comparing `morch-1.0.1/README.md` & `morch-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 ## Microservice Orchestration (morch)
 
 ### Installation:
-> pip install morch
+
+```bash
+pip install morch
+```
 
 ### Usage:
     coming soon...
 
 ### Description:
 Microservice orchestration architecture provides a robust framework for building and managing complex applications. By leveraging independent services and a centralized orchestrator, you can achieve scalability, fault tolerance, and maintainability. Refer to Chris Richardson's book [Microservices Patterns](https://microservices.io/index.html) for more in-depth guidance on this architecture.
 
 ---
 
 ### Credit:
-This project has been inspired by [saga framework](https://github.com/absent1706/saga-framework) and the book [Microservices Patterns](https://www.amazon.com/Microservices-Patterns-examples-Chris-Richardson/dp/1617294543) written by Chris Richardson.
+This project has been inspired by [saga framework](https://github.com/absent1706/saga-framework) and the book [Microservices Patterns](https://www.amazon.com/Microservices-Patterns-examples-Chris-Richardson/dp/1617294543) written by Chris Richardson.
```

### Comparing `morch-1.0.1/morch/helpers/asynch.py` & `morch-1.0.2/morch/helpers/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/helpers/celery_utils.py` & `morch-1.0.2/morch/helpers/celery_utils.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/helpers/handlers.py` & `morch-1.0.2/morch/helpers/handlers.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/helpers/repository.py` & `morch-1.0.2/morch/helpers/repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,17 +35,18 @@
         return self.get_saga_state_filter(saga_state_id).update(failed_step=failed_step.name,
                                                                 failed_at=datetime.datetime.utcnow(),
                                                                 failure_details=initial_failure_payload
                                                                 )
 
     def get_saga_payload(self, saga_state) -> dict:
         return saga_state.payload
-
+        
     def get_last_saga_state_payload(self, saga_id: int) -> dict:
-        last_saga_state = self.state.objects.filter(saga_id=saga_id).last()
+        saga = self.state.objects.filter(pk=saga_id).first().saga
+        last_saga_state = self.state.objects.filter(saga=saga).last()
         return last_saga_state.payload if last_saga_state else dict()
 
 
 def _get_saga_status(status):
     status_ = status.split('.')[-1]
     map_ = {'running': SagaStatus.PENDING.value,
             'succeeded': SagaStatus.APPROVED.value,
```

### Comparing `morch-1.0.1/morch/helpers/utils.py` & `morch-1.0.2/morch/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/saga/asynch.py` & `morch-1.0.2/morch/saga/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/saga/base.py` & `morch-1.0.2/morch/saga/base.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/saga/stateful.py` & `morch-1.0.2/morch/saga/stateful.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch/steps/asynch.py` & `morch-1.0.2/morch/steps/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/morch.egg-info/PKG-INFO` & `morch-1.0.2/morch.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morch
-Version: 1.0.1
+Version: 1.0.2
 Summary: SAGA Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/morch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/morch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
@@ -15,20 +15,24 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Microservice Orchestration (morch)
 
 ### Installation:
-> pip install morch
+
+```bash
+pip install morch
+```
 
 ### Usage:
     coming soon...
 
 ### Description:
 Microservice orchestration architecture provides a robust framework for building and managing complex applications. By leveraging independent services and a centralized orchestrator, you can achieve scalability, fault tolerance, and maintainability. Refer to Chris Richardson's book [Microservices Patterns](https://microservices.io/index.html) for more in-depth guidance on this architecture.
 
 ---
 
 ### Credit:
 This project has been inspired by [saga framework](https://github.com/absent1706/saga-framework) and the book [Microservices Patterns](https://www.amazon.com/Microservices-Patterns-examples-Chris-Richardson/dp/1617294543) written by Chris Richardson.
 
+
```

### Comparing `morch-1.0.1/morch.egg-info/SOURCES.txt` & `morch-1.0.2/morch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/setup.cfg` & `morch-1.0.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = morch
-version = 1.0.1
+version = 1.0.2
 author = Saeed Hasani Borzadaran
 author_email = hassanisaeed19@gmail.com
 description = Python Microservice Orchestrator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hasanisaeed/morch
 project_urls =
```

### Comparing `morch-1.0.1/setup.py` & `morch-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 setuptools.setup(name="morch",
-                 version="1.0.1",
+                 version="1.0.2",
                  author="Saeed Hasani Borzadaran",
                  author_email="hassanisaeed19@gmail.com",
                  description="SAGA Python Microservice Orchestrator",
                  long_description_content_type="text/markdown",
                  url="https://github.com/hasanisaeed/morch",
                  keywords='microservice, saga, patterns, microservice patterns, saga pattern',
                  python_requires='>=3.9',
                  install_requires=["asyncapi==0.14.1",
-                                   "uvicorn==0.22.0",
+                                   "uvicorn==0.23.1",
                                    "typer==0.9.0",
-                                   "PyYAML==6.0",
+                                   "PyYAML==6.0.1",
                                    "Jinja2==3.1.2",
                                    "apidaora==0.28.0",
                                    "markdown==3.4.3"
                                    ],
                  project_urls={"Bug Tracker": "https://github.com/hasanisaeed/morch/issues/new",
                                },
                  classifiers=["Programming Language :: Python :: 3",
```

### Comparing `morch-1.0.1/tests/test_async_saga.py` & `morch-1.0.2/tests/test_async_saga.py`

 * *Files identical despite different names*

### Comparing `morch-1.0.1/tests/test_sync_saga.py` & `morch-1.0.2/tests/test_sync_saga.py`

 * *Files identical despite different names*

