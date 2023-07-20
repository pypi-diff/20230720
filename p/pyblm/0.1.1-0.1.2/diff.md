# Comparing `tmp/pyblm-0.1.1.tar.gz` & `tmp/pyblm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblm-0.1.1.tar", last modified: Thu Jul 20 17:42:07 2023, max compression
+gzip compressed data, was "pyblm-0.1.2.tar", last modified: Thu Jul 20 17:59:40 2023, max compression
```

## Comparing `pyblm-0.1.1.tar` & `pyblm-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.433488 pyblm-0.1.1/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:42:07.428694 pyblm-0.1.1/PKG-INFO
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10239 2023-07-20 17:40:09.000000 pyblm-0.1.1/README.md
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.198409 pyblm-0.1.1/blm/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:15:34.000000 pyblm-0.1.1/blm/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     8935 2023-07-20 17:02:41.000000 pyblm-0.1.1/blm/blm_cluster.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.313847 pyblm-0.1.1/blm/lib/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:15:34.000000 pyblm-0.1.1/blm/lib/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17844 2023-07-20 15:15:34.000000 pyblm-0.1.1/blm/lib/blm_batch.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17562 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/blm_concat.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    41023 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/blm_results.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     6703 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/blm_setup.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    24399 2023-07-20 15:15:35.000000 pyblm-0.1.1/blm/lib/fileio.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.339059 pyblm-0.1.1/pyblm.egg-info/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/PKG-INFO
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      439 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/SOURCES.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        1 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/dependency_links.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)       47 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/entry_points.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      154 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/requires.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        9 2023-07-20 17:42:06.000000 pyblm-0.1.1/pyblm.egg-info/top_level.txt
--rw-rw-r--   0 inf852   (30112) nichols  (30016)       38 2023-07-20 17:42:07.434017 pyblm-0.1.1/setup.cfg
--rw-rw-r--   0 inf852   (30112) nichols  (30016)      918 2023-07-20 17:40:45.000000 pyblm-0.1.1/setup.py
-drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:42:07.425153 pyblm-0.1.1/test/
--rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 15:14:57.000000 pyblm-0.1.1/test/__init__.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)     8699 2023-07-20 15:15:35.000000 pyblm-0.1.1/test/blm_cluster_test.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    11040 2023-07-20 15:15:35.000000 pyblm-0.1.1/test/cleanup.py
--rw-rw-r--   0 inf852   (30112) nichols  (30016)    17906 2023-07-20 15:15:35.000000 pyblm-0.1.1/test/generate_test_data.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.163139 pyblm-0.1.2/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:59:40.161011 pyblm-0.1.2/PKG-INFO
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10239 2023-07-20 17:58:15.000000 pyblm-0.1.2/README.md
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.103329 pyblm-0.1.2/blm/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     8935 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/blm_cluster.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.132415 pyblm-0.1.2/blm/lib/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17844 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_batch.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17562 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_concat.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    41023 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_results.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     6703 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/blm_setup.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    24399 2023-07-20 17:58:15.000000 pyblm-0.1.2/blm/lib/fileio.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.146939 pyblm-0.1.2/pyblm.egg-info/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    10674 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/PKG-INFO
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      439 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/SOURCES.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        1 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/dependency_links.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)       47 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/entry_points.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      154 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/requires.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        9 2023-07-20 17:59:39.000000 pyblm-0.1.2/pyblm.egg-info/top_level.txt
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)       38 2023-07-20 17:59:40.163414 pyblm-0.1.2/setup.cfg
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)      918 2023-07-20 17:59:26.000000 pyblm-0.1.2/setup.py
+drwxrwsr-x   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:59:40.158242 pyblm-0.1.2/test/
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)        0 2023-07-20 17:58:01.000000 pyblm-0.1.2/test/__init__.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)     8699 2023-07-20 17:58:15.000000 pyblm-0.1.2/test/blm_cluster_test.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    11040 2023-07-20 17:58:15.000000 pyblm-0.1.2/test/cleanup.py
+-rw-rw-r--   0 inf852   (30112) nichols  (30016)    17906 2023-07-20 17:58:15.000000 pyblm-0.1.2/test/generate_test_data.py
```

### Comparing `pyblm-0.1.1/PKG-INFO` & `pyblm-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblm
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Big Linear Models Toolbox
 Home-page: https://github.com/tommaullin/blm
 Author: Tom Maullin
 Author-email: TomMaullin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyblm-0.1.1/README.md` & `pyblm-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/blm/blm_cluster.py` & `pyblm-0.1.2/blm/blm_cluster.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/blm/lib/blm_batch.py` & `pyblm-0.1.2/blm/lib/blm_batch.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/blm/lib/blm_concat.py` & `pyblm-0.1.2/blm/lib/blm_concat.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/blm/lib/blm_results.py` & `pyblm-0.1.2/blm/lib/blm_results.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/blm/lib/blm_setup.py` & `pyblm-0.1.2/blm/lib/blm_setup.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/blm/lib/fileio.py` & `pyblm-0.1.2/blm/lib/fileio.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/pyblm.egg-info/PKG-INFO` & `pyblm-0.1.2/pyblm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblm
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Big Linear Models Toolbox
 Home-page: https://github.com/tommaullin/blm
 Author: Tom Maullin
 Author-email: TomMaullin@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyblm-0.1.1/setup.py` & `pyblm-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requirements = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pyblm",
-    version="0.1.1",
+    version="0.1.2",
     author="Tom Maullin",
     author_email="TomMaullin@gmail.com",
     description="The Big Linear Models Toolbox",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tommaullin/blm",
     packages=find_packages(),
```

### Comparing `pyblm-0.1.1/test/blm_cluster_test.py` & `pyblm-0.1.2/test/blm_cluster_test.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/test/cleanup.py` & `pyblm-0.1.2/test/cleanup.py`

 * *Files identical despite different names*

### Comparing `pyblm-0.1.1/test/generate_test_data.py` & `pyblm-0.1.2/test/generate_test_data.py`

 * *Files identical despite different names*

