# Comparing `tmp/deepcellpredictor-0.1.tar.gz` & `tmp/deepcellpredictor-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepcellpredictor-0.1.tar", last modified: Thu Jul 20 21:02:13 2023, max compression
+gzip compressed data, was "deepcellpredictor-0.2.tar", last modified: Thu Jul 20 21:44:37 2023, max compression
```

## Comparing `deepcellpredictor-0.1.tar` & `deepcellpredictor-0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 21:02:13.593500 deepcellpredictor-0.1/
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 21:02:13.593500 deepcellpredictor-0.1/DCP/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.1/DCP/ModelPlanner.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8286 2023-07-20 15:52:22.000000 deepcellpredictor-0.1/DCP/VAEtorch.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.1/DCP/__init__.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11581 2023-07-20 15:52:22.000000 deepcellpredictor-0.1/DCP/deep_predictor.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.1/DCP/flow.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.1/DCP/utils.py
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.1/LICENSE
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      296 2023-07-20 21:02:13.593500 deepcellpredictor-0.1/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.1/README.md
-drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 21:02:13.593500 deepcellpredictor-0.1/deepcellpredictor.egg-info/
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      296 2023-07-20 21:02:13.000000 deepcellpredictor-0.1/deepcellpredictor.egg-info/PKG-INFO
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 21:02:13.000000 deepcellpredictor-0.1/deepcellpredictor.egg-info/SOURCES.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 21:02:13.000000 deepcellpredictor-0.1/deepcellpredictor.egg-info/dependency_links.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       81 2023-07-20 21:02:13.000000 deepcellpredictor-0.1/deepcellpredictor.egg-info/requires.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 21:02:13.000000 deepcellpredictor-0.1/deepcellpredictor.egg-info/top_level.txt
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 21:02:13.593500 deepcellpredictor-0.1/setup.cfg
--rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      750 2023-07-20 21:01:53.000000 deepcellpredictor-0.1/setup.py
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 21:44:37.163933 deepcellpredictor-0.2/
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 21:44:37.163933 deepcellpredictor-0.2/DCP/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1245 2023-07-20 15:52:22.000000 deepcellpredictor-0.2/DCP/ModelPlanner.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     8286 2023-07-20 15:52:22.000000 deepcellpredictor-0.2/DCP/VAEtorch.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      474 2023-07-20 20:33:00.000000 deepcellpredictor-0.2/DCP/__init__.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)    11581 2023-07-20 15:52:22.000000 deepcellpredictor-0.2/DCP/deep_predictor.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     4056 2023-07-20 15:52:22.000000 deepcellpredictor-0.2/DCP/flow.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      679 2023-07-20 15:52:22.000000 deepcellpredictor-0.2/DCP/utils.py
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)     1063 2023-07-20 20:33:00.000000 deepcellpredictor-0.2/LICENSE
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      442 2023-07-20 21:44:37.163933 deepcellpredictor-0.2/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      182 2023-07-20 15:52:22.000000 deepcellpredictor-0.2/README.md
+drwxrwxr-x   0 gaurav    (1001) gaurav    (1001)        0 2023-07-20 21:44:37.163933 deepcellpredictor-0.2/deepcellpredictor.egg-info/
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      442 2023-07-20 21:44:36.000000 deepcellpredictor-0.2/deepcellpredictor.egg-info/PKG-INFO
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      329 2023-07-20 21:44:37.000000 deepcellpredictor-0.2/deepcellpredictor.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        1 2023-07-20 21:44:36.000000 deepcellpredictor-0.2/deepcellpredictor.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      140 2023-07-20 21:44:37.000000 deepcellpredictor-0.2/deepcellpredictor.egg-info/requires.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)        4 2023-07-20 21:44:37.000000 deepcellpredictor-0.2/deepcellpredictor.egg-info/top_level.txt
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)       38 2023-07-20 21:44:37.163933 deepcellpredictor-0.2/setup.cfg
+-rw-rw-r--   0 gaurav    (1001) gaurav    (1001)      879 2023-07-20 21:44:28.000000 deepcellpredictor-0.2/setup.py
```

### Comparing `deepcellpredictor-0.1/DCP/ModelPlanner.py` & `deepcellpredictor-0.2/DCP/ModelPlanner.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.1/DCP/VAEtorch.py` & `deepcellpredictor-0.2/DCP/VAEtorch.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.1/DCP/deep_predictor.py` & `deepcellpredictor-0.2/DCP/deep_predictor.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.1/DCP/flow.py` & `deepcellpredictor-0.2/DCP/flow.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.1/DCP/utils.py` & `deepcellpredictor-0.2/DCP/utils.py`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.1/LICENSE` & `deepcellpredictor-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepcellpredictor-0.1/setup.py` & `deepcellpredictor-0.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.1'
+VERSION = '0.2'
 DESCRIPTION = "a transfer learning approach that explicitly models changes in transcriptional variance using a combination of variational autoencoders and normalizing flows"
 
 setup(
     name='deepcellpredictor',
     version=VERSION,
     description='transfer learning approach',
-    long_description='DESCRIPTION',
+    long_description=DESCRIPTION,
     packages=find_packages(),
     install_requires=[
-        'numpy','pandas','matplotlib','torch','anndata','pytorch_lightning','typing','scanpy','scipy','scvi'
+        'numpy==1.21.0',
+        'pandas==1.4.2',
+        'matplotlib==3.5.2',
+        'torch==1.11.0',
+        'anndata==0.8.0',
+        'pytorch_lightning==1.7.7',
+        'scanpy==1.9.1',
+        'scipy==1.8.1',
+        'scvi==0.19.0'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
     ],
-  python_requires=">=3.6",
+    python_requires=">=3.6",
 )
```

