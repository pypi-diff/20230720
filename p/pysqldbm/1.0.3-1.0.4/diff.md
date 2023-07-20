# Comparing `tmp/pysqldbm-1.0.3.tar.gz` & `tmp/pysqldbm-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqldbm-1.0.3.tar", last modified: Thu Jul 20 08:29:23 2023, max compression
+gzip compressed data, was "pysqldbm-1.0.4.tar", last modified: Thu Jul 20 08:57:54 2023, max compression
```

## Comparing `pysqldbm-1.0.3.tar` & `pysqldbm-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.237094 pysqldbm-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:29:23.237094 pysqldbm-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 08:29:15.000000 pysqldbm-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.229094 pysqldbm-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/src/pysqldbm/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/src/pysqldbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/src/pysqldbm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 08:57:47.000000 pysqldbm-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.487440 pysqldbm-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/src/pysqldbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/src/pysqldbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 08:57:54.000000 pysqldbm-1.0.4/src/pysqldbm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:54.491440 pysqldbm-1.0.4/src/pysqldbm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 08:57:45.000000 pysqldbm-1.0.4/src/pysqldbm_cli/run.py
```

### Comparing `pysqldbm-1.0.3/PKG-INFO` & `pysqldbm-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.3
+Version: 1.0.4
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
 
 # pysqldm
 
+[![PyPI Version](https://img.shields.io/pypi/v/pysqldbm.svg)](https://pypi.python.org/pypi/pysqldbm)
+
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
 ### Installation
 
 ```bash
 pip install pysqldbm[cli]
 ```
 
 ### Usage
 
 ```bash
-sqldb --help
+sqldbm --help
 
 export SQLDB_API_KEY="your_api_key"
 sqldbm list-projects # or `sqldbm --api-key="your_api_key" list-projects`
 ```
 
 ## `pysqldbm` library
```

### Comparing `pysqldbm-1.0.3/README.md` & `pysqldbm-1.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # pysqldm
 
+[![PyPI Version](https://img.shields.io/pypi/v/pysqldbm.svg)](https://pypi.python.org/pypi/pysqldbm)
+
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
 ### Installation
 
 ```bash
 pip install pysqldbm[cli]
 ```
 
 ### Usage
 
 ```bash
-sqldb --help
+sqldbm --help
 
 export SQLDB_API_KEY="your_api_key"
 sqldbm list-projects # or `sqldbm --api-key="your_api_key" list-projects`
 ```
 
 ## `pysqldbm` library
```

### Comparing `pysqldbm-1.0.3/setup.py` & `pysqldbm-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 with (Path(__file__).parent / "README.md").open(encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="pysqldbm",
-    version="1.0.3",
+    version="1.0.4",
     url="https://github.com/drewsonne/pysqldbm",
     license="Apache",
     author="Drew J. Sonne",
     author_email="drew.sonne@gmail.com",
     description="A library to wrap SQLdbm API",
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `pysqldbm-1.0.3/src/pysqldbm/client.py` & `pysqldbm-1.0.4/src/pysqldbm/client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.3/src/pysqldbm/rest_client.py` & `pysqldbm-1.0.4/src/pysqldbm/rest_client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.3/src/pysqldbm.egg-info/PKG-INFO` & `pysqldbm-1.0.4/src/pysqldbm.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.3
+Version: 1.0.4
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
 
 # pysqldm
 
+[![PyPI Version](https://img.shields.io/pypi/v/pysqldbm.svg)](https://pypi.python.org/pypi/pysqldbm)
+
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
 ### Installation
 
 ```bash
 pip install pysqldbm[cli]
 ```
 
 ### Usage
 
 ```bash
-sqldb --help
+sqldbm --help
 
 export SQLDB_API_KEY="your_api_key"
 sqldbm list-projects # or `sqldbm --api-key="your_api_key" list-projects`
 ```
 
 ## `pysqldbm` library
```

### Comparing `pysqldbm-1.0.3/src/pysqldbm_cli/run.py` & `pysqldbm-1.0.4/src/pysqldbm_cli/run.py`

 * *Files identical despite different names*

