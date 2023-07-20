# Comparing `tmp/pysqldbm-1.0.4.tar.gz` & `tmp/pysqldbm-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqldbm-1.0.4.tar", last modified: Thu Jul 20 08:57:54 2023, max compression
+gzip compressed data, was "pysqldbm-1.0.5.tar", last modified: Thu Jul 20 14:23:40 2023, max compression
```

## Comparing `pysqldbm-1.0.4.tar` & `pysqldbm-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 08:57:47.000000 pysqldbm-1.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.487440 pysqldbm-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/src/pysqldbm/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/src/pysqldbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/src/pysqldbm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-20 14:23:28.000000 pysqldbm-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 14:23:31.000000 pysqldbm-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/src/pysqldbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 14:23:28.000000 pysqldbm-1.0.5/src/pysqldbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 14:23:28.000000 pysqldbm-1.0.5/src/pysqldbm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-20 14:23:28.000000 pysqldbm-1.0.5/src/pysqldbm/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/src/pysqldbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-07-20 14:23:40.000000 pysqldbm-1.0.5/src/pysqldbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 14:23:40.000000 pysqldbm-1.0.5/src/pysqldbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:23:40.000000 pysqldbm-1.0.5/src/pysqldbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 14:23:40.000000 pysqldbm-1.0.5/src/pysqldbm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 14:23:40.000000 pysqldbm-1.0.5/src/pysqldbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 14:23:40.000000 pysqldbm-1.0.5/src/pysqldbm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:40.474731 pysqldbm-1.0.5/src/pysqldbm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:23:28.000000 pysqldbm-1.0.5/src/pysqldbm_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 14:23:28.000000 pysqldbm-1.0.5/src/pysqldbm_cli/run.py
```

### Comparing `pysqldbm-1.0.4/PKG-INFO` & `pysqldbm-1.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.4
+Version: 1.0.5
 Summary: A library to wrap SQLdbm API
 Home-page: https://github.com/drewsonne/pysqldbm
 Author: Drew J. Sonne
 Author-email: drew.sonne@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 
-# pysqldm
+# pysqldbm
 
 [![PyPI Version](https://img.shields.io/pypi/v/pysqldbm.svg)](https://pypi.python.org/pypi/pysqldbm)
 
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
@@ -59,7 +59,11 @@
 sqldbm = pysqldbm.client(API_KEY)
 
 for project in sqldbm.list_projects():
     print(f"Show revisions for project '{project['name']}'...")
     for revision in sqldbm.list_revisions(project['id']):
         print(revision)
 ```
+
+## Architecture
+
+See [ARCHITECTURE.md](ARCHITECTURE.md).
```

### Comparing `pysqldbm-1.0.4/README.md` & `pysqldbm-1.0.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pysqldm
+# pysqldbm
 
 [![PyPI Version](https://img.shields.io/pypi/v/pysqldbm.svg)](https://pypi.python.org/pypi/pysqldbm)
 
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
@@ -45,7 +45,11 @@
 sqldbm = pysqldbm.client(API_KEY)
 
 for project in sqldbm.list_projects():
     print(f"Show revisions for project '{project['name']}'...")
     for revision in sqldbm.list_revisions(project['id']):
         print(revision)
 ```
+
+## Architecture
+
+See [ARCHITECTURE.md](ARCHITECTURE.md).
```

### Comparing `pysqldbm-1.0.4/setup.py` & `pysqldbm-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 with (Path(__file__).parent / "README.md").open(encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="pysqldbm",
-    version="1.0.4",
+    version="1.0.5",
     url="https://github.com/drewsonne/pysqldbm",
     license="Apache",
     author="Drew J. Sonne",
     author_email="drew.sonne@gmail.com",
     description="A library to wrap SQLdbm API",
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `pysqldbm-1.0.4/src/pysqldbm/client.py` & `pysqldbm-1.0.5/src/pysqldbm/client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.4/src/pysqldbm/rest_client.py` & `pysqldbm-1.0.5/src/pysqldbm/rest_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, Generator, Optional
+from typing import Dict, Generator, Optional, Union
 from urllib.parse import urljoin
 
 import backoff
 import click
 from requests import Session
 
 
@@ -37,15 +37,15 @@
 
     @backoff.on_exception(
         backoff.expo,
         (RateLimited,),
         on_backoff=backoff_hdlr,
         jitter=backoff.full_jitter,
     )
-    def get(self, resource: str, query: Optional[Dict] = None) -> Dict:
+    def get(self, resource: str, query: Optional[Dict] = None) -> Union[Dict, str]:
         """Get a resource from the SQLDBM API."""
         response = self._session.get(resource, params=query)
         if response.status_code == 429:
             raise RateLimited(response.content)
         response.raise_for_status()
 
         return response.json()["data"]
```

### Comparing `pysqldbm-1.0.4/src/pysqldbm.egg-info/PKG-INFO` & `pysqldbm-1.0.5/src/pysqldbm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.4
+Version: 1.0.5
 Summary: A library to wrap SQLdbm API
 Home-page: https://github.com/drewsonne/pysqldbm
 Author: Drew J. Sonne
 Author-email: drew.sonne@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: cli
 
-# pysqldm
+# pysqldbm
 
 [![PyPI Version](https://img.shields.io/pypi/v/pysqldbm.svg)](https://pypi.python.org/pypi/pysqldbm)
 
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
@@ -59,7 +59,11 @@
 sqldbm = pysqldbm.client(API_KEY)
 
 for project in sqldbm.list_projects():
     print(f"Show revisions for project '{project['name']}'...")
     for revision in sqldbm.list_revisions(project['id']):
         print(revision)
 ```
+
+## Architecture
+
+See [ARCHITECTURE.md](ARCHITECTURE.md).
```

### Comparing `pysqldbm-1.0.4/src/pysqldbm_cli/run.py` & `pysqldbm-1.0.5/src/pysqldbm_cli/run.py`

 * *Files identical despite different names*

