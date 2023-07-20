# Comparing `tmp/gwdg_idm_api-2.2.0.tar.gz` & `tmp/gwdg_idm_api-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdg_idm_api-2.2.0.tar", last modified: Thu Jul 20 16:33:34 2023, max compression
+gzip compressed data, was "gwdg_idm_api-2.2.1.tar", last modified: Thu Jul 20 16:45:03 2023, max compression
```

## Comparing `gwdg_idm_api-2.2.0.tar` & `gwdg_idm_api-2.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      279 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      916 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.093876 gwdg_idm_api-2.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.097876 gwdg_idm_api-2.2.0/src/gwdg_idm_api/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     5096 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/benutzerverwaltung.py
--rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6878 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/string_cleaner.py
--rw-rw-rw-   0 root         (0) root         (0)     1399 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      566 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 16:33:34.000000 gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:33:34.101876 gwdg_idm_api-2.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/tests/examples.py
--rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/tests/predict_username.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      279 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      169 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      196 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.387746 gwdg_idm_api-2.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/src/gwdg_idm_api/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     5096 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/benutzerverwaltung.py
+-rw-rw-rw-   0 root         (0) root         (0)     6803 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6878 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/string_cleaner.py
+-rw-rw-rw-   0 root         (0) root         (0)     1399 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      685 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      566 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       50 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-07-20 16:45:03.000000 gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 16:45:03.391746 gwdg_idm_api-2.2.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3302 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/tests/examples.py
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/tests/predict_username.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-07-20 16:33:16.000000 gwdg_idm_api-2.2.1/tox.ini
```

### Comparing `gwdg_idm_api-2.2.0/.pre-commit-config.yaml` & `gwdg_idm_api-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/LICENSE` & `gwdg_idm_api-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/PKG-INFO` & `gwdg_idm_api-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg_idm_api
-Version: 2.2.0
+Version: 2.2.1
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.2.0/setup.cfg` & `gwdg_idm_api-2.2.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
 packages = find:
 install_requires = 
-	pydantic==1
+	pydantic<2
 	requests
 python_requires = >=3.10
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
```

### Comparing `gwdg_idm_api-2.2.0/src/gwdg_idm_api/benutzerverwaltung.py` & `gwdg_idm_api-2.2.1/src/gwdg_idm_api/benutzerverwaltung.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/src/gwdg_idm_api/models.py` & `gwdg_idm_api-2.2.1/src/gwdg_idm_api/models.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/src/gwdg_idm_api/string_cleaner.py` & `gwdg_idm_api-2.2.1/src/gwdg_idm_api/string_cleaner.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/src/gwdg_idm_api/util.py` & `gwdg_idm_api-2.2.1/src/gwdg_idm_api/util.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/PKG-INFO` & `gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdg-idm-api
-Version: 2.2.0
+Version: 2.2.1
 Summary: Interface to the GWDG IDM api
 Home-page: https://gitlab.gwdg.de/mpi-dortmund/ze-edv-public/gwdg_idm_api
 Author: Markus Stabrin
 Author-email: markus.stabrin@mpi-dortmund.mpg.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gwdg_idm_api-2.2.0/src/gwdg_idm_api.egg-info/SOURCES.txt` & `gwdg_idm_api-2.2.1/src/gwdg_idm_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/tests/examples.py` & `gwdg_idm_api-2.2.1/tests/examples.py`

 * *Files identical despite different names*

### Comparing `gwdg_idm_api-2.2.0/tests/predict_username.py` & `gwdg_idm_api-2.2.1/tests/predict_username.py`

 * *Files identical despite different names*

