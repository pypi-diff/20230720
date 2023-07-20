# Comparing `tmp/pysqldbm-1.0.2.tar.gz` & `tmp/pysqldbm-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqldbm-1.0.2.tar", last modified: Thu Jul 20 08:15:05 2023, max compression
+gzip compressed data, was "pysqldbm-1.0.3.tar", last modified: Thu Jul 20 08:29:23 2023, max compression
```

## Comparing `pysqldbm-1.0.2.tar` & `pysqldbm-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.928705 pysqldbm-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 08:15:05.928705 pysqldbm-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:15:05.928705 pysqldbm-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-20 08:14:58.000000 pysqldbm-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/pysqldbm/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm/rest_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/pysqldbm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 08:15:05.000000 pysqldbm-1.0.2/src/pysqldbm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:15:05.924704 pysqldbm-1.0.2/src/pysqldbm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 08:14:54.000000 pysqldbm-1.0.2/src/pysqldbm_cli/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.237094 pysqldbm-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:29:23.237094 pysqldbm-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 08:29:15.000000 pysqldbm-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.229094 pysqldbm-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/src/pysqldbm/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm/rest_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/src/pysqldbm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 08:29:23.000000 pysqldbm-1.0.3/src/pysqldbm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:23.233094 pysqldbm-1.0.3/src/pysqldbm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-20 08:29:11.000000 pysqldbm-1.0.3/src/pysqldbm_cli/run.py
```

### Comparing `pysqldbm-1.0.2/PKG-INFO` & `pysqldbm-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library to wrap SQLdbm API
 Home-page: https://github.com/drewsonne/pysqldbm
 Author: Drew J. Sonne
 Author-email: drew.sonne@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -17,17 +17,15 @@
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
 ### Installation
 
 ```bash
-git clone git@github.com:drewsonne/pysqldbm.git
-cd pysqldbm
-pip install -e .[cli]
+pip install pysqldbm[cli]
 ```
 
 ### Usage
 
 ```bash
 sqldb --help
 
@@ -36,17 +34,21 @@
 ```
 
 ## `pysqldbm` library
 
 ### Installation
 
 ```bash
-git clone git@github.com:drewsonne/pysqldbm.git
-cd pysqldbm
-pip install -e .
+pip install pysqldbm
+```
+
+If you would like to use the latest overnight builds, you can install from test pypi
+
+```bash
+pip install -i https://test.pypi.org/simple/ pysqldbm
 ```
 
 ### Sample Usage with Client
 
 ```python
 import pysqldbm
```

### Comparing `pysqldbm-1.0.2/README.md` & `pysqldbm-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
 ### Installation
 
 ```bash
-git clone git@github.com:drewsonne/pysqldbm.git
-cd pysqldbm
-pip install -e .[cli]
+pip install pysqldbm[cli]
 ```
 
 ### Usage
 
 ```bash
 sqldb --help
 
@@ -22,17 +20,21 @@
 ```
 
 ## `pysqldbm` library
 
 ### Installation
 
 ```bash
-git clone git@github.com:drewsonne/pysqldbm.git
-cd pysqldbm
-pip install -e .
+pip install pysqldbm
+```
+
+If you would like to use the latest overnight builds, you can install from test pypi
+
+```bash
+pip install -i https://test.pypi.org/simple/ pysqldbm
 ```
 
 ### Sample Usage with Client
 
 ```python
 import pysqldbm
```

### Comparing `pysqldbm-1.0.2/setup.py` & `pysqldbm-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # The text of the README file
 with (Path(__file__).parent / "README.md").open(encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="pysqldbm",
-    version = "1.0.2",
+    version="1.0.3",
     url="https://github.com/drewsonne/pysqldbm",
     license="Apache",
     author="Drew J. Sonne",
     author_email="drew.sonne@gmail.com",
     description="A library to wrap SQLdbm API",
     long_description=README,
     long_description_content_type="text/markdown",
```

### Comparing `pysqldbm-1.0.2/src/pysqldbm/client.py` & `pysqldbm-1.0.3/src/pysqldbm/client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.2/src/pysqldbm/rest_client.py` & `pysqldbm-1.0.3/src/pysqldbm/rest_client.py`

 * *Files identical despite different names*

### Comparing `pysqldbm-1.0.2/src/pysqldbm.egg-info/PKG-INFO` & `pysqldbm-1.0.3/src/pysqldbm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqldbm
-Version: 1.0.2
+Version: 1.0.3
 Summary: A library to wrap SQLdbm API
 Home-page: https://github.com/drewsonne/pysqldbm
 Author: Drew J. Sonne
 Author-email: drew.sonne@gmail.com
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -17,17 +17,15 @@
 A python API to wrap https://developers.sqldbm.com/.
 
 ## `sqldbm` CLI tool
 
 ### Installation
 
 ```bash
-git clone git@github.com:drewsonne/pysqldbm.git
-cd pysqldbm
-pip install -e .[cli]
+pip install pysqldbm[cli]
 ```
 
 ### Usage
 
 ```bash
 sqldb --help
 
@@ -36,17 +34,21 @@
 ```
 
 ## `pysqldbm` library
 
 ### Installation
 
 ```bash
-git clone git@github.com:drewsonne/pysqldbm.git
-cd pysqldbm
-pip install -e .
+pip install pysqldbm
+```
+
+If you would like to use the latest overnight builds, you can install from test pypi
+
+```bash
+pip install -i https://test.pypi.org/simple/ pysqldbm
 ```
 
 ### Sample Usage with Client
 
 ```python
 import pysqldbm
```

### Comparing `pysqldbm-1.0.2/src/pysqldbm_cli/run.py` & `pysqldbm-1.0.3/src/pysqldbm_cli/run.py`

 * *Files identical despite different names*

