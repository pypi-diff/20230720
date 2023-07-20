# Comparing `tmp/piqp-0.1.2.tar.gz` & `tmp/piqp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piqp-0.1.2.tar", last modified: Fri Jul 14 13:27:59 2023, max compression
+gzip compressed data, was "piqp-0.1.3.tar", last modified: Thu Jul 20 13:26:13 2023, max compression
```

## Comparing `piqp-0.1.2.tar` & `piqp-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:27:59.868991 piqp-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-14 13:27:45.000000 piqp-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-14 13:27:59.868991 piqp-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-14 13:27:45.000000 piqp-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:27:59.868991 piqp-0.1.2/interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:27:59.868991 piqp-0.1.2/interfaces/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:27:59.868991 piqp-0.1.2/interfaces/python/piqp/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-14 13:27:45.000000 piqp-0.1.2/interfaces/python/piqp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:27:59.868991 piqp-0.1.2/piqp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-14 13:27:59.000000 piqp-0.1.2/piqp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 13:27:59.000000 piqp-0.1.2/piqp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:27:59.000000 piqp-0.1.2/piqp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 13:27:59.000000 piqp-0.1.2/piqp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-14 13:27:59.000000 piqp-0.1.2/piqp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-14 13:27:59.000000 piqp-0.1.2/piqp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-14 13:27:45.000000 piqp-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 13:27:59.868991 piqp-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-14 13:27:45.000000 piqp-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.672752 piqp-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-20 13:25:57.000000 piqp-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 13:26:13.672752 piqp-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-20 13:25:57.000000 piqp-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.668752 piqp-0.1.3/interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.668752 piqp-0.1.3/interfaces/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.668752 piqp-0.1.3/interfaces/python/piqp/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-20 13:25:57.000000 piqp-0.1.3/interfaces/python/piqp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:26:13.672752 piqp-0.1.3/piqp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-20 13:26:13.000000 piqp-0.1.3/piqp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-20 13:25:57.000000 piqp-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:26:13.672752 piqp-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-20 13:25:57.000000 piqp-0.1.3/setup.py
```

### Comparing `piqp-0.1.2/LICENSE` & `piqp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `piqp-0.1.2/PKG-INFO` & `piqp-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.1.2
+Version: 0.1.3
 Summary: An embedded Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `piqp-0.1.2/README.md` & `piqp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `piqp-0.1.2/interfaces/python/piqp/__init__.py` & `piqp-0.1.3/interfaces/python/piqp/__init__.py`

 * *Files identical despite different names*

### Comparing `piqp-0.1.2/piqp.egg-info/PKG-INFO` & `piqp-0.1.3/piqp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piqp
-Version: 0.1.2
+Version: 0.1.3
 Summary: An embedded Proximal Interior Point Quadratic Programming solver
 Home-page: https://github.com/PREDICT-EPFL/piqp
 Author: Roland Schwan
 Author-email: roland.schwan@epfl.ch
 License: BSD-2-Clause
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `piqp-0.1.2/pyproject.toml` & `piqp-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piqp-0.1.2/setup.py` & `piqp-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="piqp",
-    version="0.1.2",
+    version="0.1.3",
     url='https://github.com/PREDICT-EPFL/piqp',
     author="Roland Schwan",
     author_email="roland.schwan@epfl.ch",
     license='BSD-2-Clause',
     description="An embedded Proximal Interior Point Quadratic Programming solver",
     long_description=long_description,
     long_description_content_type='text/markdown',
```

