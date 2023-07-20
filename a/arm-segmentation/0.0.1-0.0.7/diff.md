# Comparing `tmp/arm_segmentation-0.0.1.tar.gz` & `tmp/arm_segmentation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arm_segmentation-0.0.1.tar", last modified: Wed Jul 12 02:53:09 2023, max compression
+gzip compressed data, was "arm_segmentation-0.0.7.tar", last modified: Thu Jul 20 17:31:40 2023, max compression
```

## Comparing `arm_segmentation-0.0.1.tar` & `arm_segmentation-0.0.7.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:53:09.293555 arm_segmentation-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-12 02:53:09.293555 arm_segmentation-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 02:53:09.293555 arm_segmentation-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:53:09.289555 arm_segmentation-0.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:53:09.289555 arm_segmentation-0.0.1/src/arm_segmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/arm_segmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/arm_segmentation/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/arm_segmentation/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:53:09.293555 arm_segmentation-0.0.1/src/arm_segmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-07-12 02:53:09.000000 arm_segmentation-0.0.1/src/arm_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-12 02:53:09.000000 arm_segmentation-0.0.1/src/arm_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 02:53:09.000000 arm_segmentation-0.0.1/src/arm_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-12 02:53:09.000000 arm_segmentation-0.0.1/src/arm_segmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-12 02:53:09.000000 arm_segmentation-0.0.1/src/arm_segmentation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:53:09.293555 arm_segmentation-0.0.1/src/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/detection/coco_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/detection/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/detection/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/src/detection/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 02:53:09.293555 arm_segmentation-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-12 02:50:21.000000 arm_segmentation-0.0.1/tests/test_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:31:40.317357 arm_segmentation-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-20 17:31:40.317357 arm_segmentation-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 17:31:40.317357 arm_segmentation-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:31:40.313356 arm_segmentation-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:31:40.313356 arm_segmentation-0.0.7/src/arm_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/arm_segmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/arm_segmentation/predictor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/arm_segmentation/train.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/arm_segmentation/visualize_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/arm_segmentation/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:31:40.313356 arm_segmentation-0.0.7/src/arm_segmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-20 17:31:40.000000 arm_segmentation-0.0.7/src/arm_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-20 17:31:40.000000 arm_segmentation-0.0.7/src/arm_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 17:31:40.000000 arm_segmentation-0.0.7/src/arm_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-20 17:31:40.000000 arm_segmentation-0.0.7/src/arm_segmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-20 17:31:40.000000 arm_segmentation-0.0.7/src/arm_segmentation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:31:40.313356 arm_segmentation-0.0.7/src/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/detection/coco_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/detection/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/detection/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/src/detection/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 17:31:40.313356 arm_segmentation-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 17:29:19.000000 arm_segmentation-0.0.7/tests/test_predictor.py
```

### Comparing `arm_segmentation-0.0.1/PKG-INFO` & `arm_segmentation-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm_segmentation
-Version: 0.0.1
+Version: 0.0.7
 Summary: Training and inference of instance segmentation
 Author-email: Peter Mitrano <pmitrano@umich.edu>
 Maintainer-email: Peter Mitrano <pmitrano@umich.edu>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
@@ -18,14 +18,21 @@
 # Data
 
 This repository assumes you have used RoboFlow to annotate your dataset.
 You should export your dataset as a COCO style dataset, which stores annotations in JSON.
 
 # Installation & Setup
 
+You can install via pip
+```
+pip install arm_segmentation
+```
+
+Or you can clone the source code and install it that way.
+
 1. Clone this repository
    ```
    git clone git@github.com:UM-ARM-Lab/arm_segmentation.git
    ```
 2. In an existing or new python virtual environment, install the dependencies
     ```
     pip install -r requirements.txt
```

### Comparing `arm_segmentation-0.0.1/README.md` & `arm_segmentation-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 # Data
 
 This repository assumes you have used RoboFlow to annotate your dataset.
 You should export your dataset as a COCO style dataset, which stores annotations in JSON.
 
 # Installation & Setup
 
+You can install via pip
+```
+pip install arm_segmentation
+```
+
+Or you can clone the source code and install it that way.
+
 1. Clone this repository
    ```
    git clone git@github.com:UM-ARM-Lab/arm_segmentation.git
    ```
 2. In an existing or new python virtual environment, install the dependencies
     ```
     pip install -r requirements.txt
```

### Comparing `arm_segmentation-0.0.1/pyproject.toml` & `arm_segmentation-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'arm_segmentation'
-version="0.0.1"
+version="0.0.7"
 description="Training and inference of instance segmentation"
 readme = "README.md"
 
 requires-python = ">=3.6"
 
 license = { file = "LICENSE.txt" }
```

### Comparing `arm_segmentation-0.0.1/src/arm_segmentation/predictor.py` & `arm_segmentation-0.0.7/src/arm_segmentation/predictor.py`

 * *Files identical despite different names*

### Comparing `arm_segmentation-0.0.1/src/arm_segmentation/viz.py` & `arm_segmentation-0.0.7/src/arm_segmentation/viz.py`

 * *Files identical despite different names*

### Comparing `arm_segmentation-0.0.1/src/arm_segmentation.egg-info/PKG-INFO` & `arm_segmentation-0.0.7/src/arm_segmentation.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-segmentation
-Version: 0.0.1
+Version: 0.0.7
 Summary: Training and inference of instance segmentation
 Author-email: Peter Mitrano <pmitrano@umich.edu>
 Maintainer-email: Peter Mitrano <pmitrano@umich.edu>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
@@ -18,14 +18,21 @@
 # Data
 
 This repository assumes you have used RoboFlow to annotate your dataset.
 You should export your dataset as a COCO style dataset, which stores annotations in JSON.
 
 # Installation & Setup
 
+You can install via pip
+```
+pip install arm_segmentation
+```
+
+Or you can clone the source code and install it that way.
+
 1. Clone this repository
    ```
    git clone git@github.com:UM-ARM-Lab/arm_segmentation.git
    ```
 2. In an existing or new python virtual environment, install the dependencies
     ```
     pip install -r requirements.txt
```

### Comparing `arm_segmentation-0.0.1/src/detection/coco_utils.py` & `arm_segmentation-0.0.7/src/detection/coco_utils.py`

 * *Files identical despite different names*

### Comparing `arm_segmentation-0.0.1/src/detection/engine.py` & `arm_segmentation-0.0.7/src/detection/engine.py`

 * *Files identical despite different names*

### Comparing `arm_segmentation-0.0.1/src/detection/transforms.py` & `arm_segmentation-0.0.7/src/detection/transforms.py`

 * *Files identical despite different names*

### Comparing `arm_segmentation-0.0.1/src/detection/utils.py` & `arm_segmentation-0.0.7/src/detection/utils.py`

 * *Files identical despite different names*

### Comparing `arm_segmentation-0.0.1/tests/test_predictor.py` & `arm_segmentation-0.0.7/tests/test_predictor.py`

 * *Files identical despite different names*

