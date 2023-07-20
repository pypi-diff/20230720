# Comparing `tmp/torchanalyse-0.0.1.tar.gz` & `tmp/torchanalyse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchanalyse-0.0.1.tar", last modified: Thu Jul 20 13:23:32 2023, max compression
+gzip compressed data, was "torchanalyse-0.0.2.tar", last modified: Thu Jul 20 13:43:30 2023, max compression
```

## Comparing `torchanalyse-0.0.1.tar` & `torchanalyse-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,32 @@
-drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:23:32.296587 torchanalyse-0.0.1/
--rw-r--r--   0 catbeta    (501) staff       (20)      113 2023-07-20 13:23:32.296422 torchanalyse-0.0.1/PKG-INFO
--rw-r--r--   0 catbeta    (501) staff       (20)     1686 2023-07-19 19:22:54.000000 torchanalyse-0.0.1/README.md
--rw-r--r--   0 catbeta    (501) staff       (20)       38 2023-07-20 13:23:32.296635 torchanalyse-0.0.1/setup.cfg
--rw-r--r--   0 catbeta    (501) staff       (20)      398 2023-07-20 13:19:12.000000 torchanalyse-0.0.1/setup.py
-drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:23:32.294265 torchanalyse-0.0.1/torchanalyse/
--rw-r--r--   0 catbeta    (501) staff       (20)      113 2023-07-20 13:15:23.000000 torchanalyse-0.0.1/torchanalyse/__init__.py
--rw-r--r--   0 catbeta    (501) staff       (20)     6106 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/handlers.py
--rw-r--r--   0 catbeta    (501) staff       (20)     1276 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/profile.py
--rw-r--r--   0 catbeta    (501) staff       (20)     6791 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/system.py
--rw-r--r--   0 catbeta    (501) staff       (20)     1764 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/unit.py
-drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:23:32.295611 torchanalyse-0.0.1/torchanalyse/utils/
--rw-r--r--   0 catbeta    (501) staff       (20)        0 2023-07-18 14:32:14.000000 torchanalyse-0.0.1/torchanalyse/utils/__init__.py
--rw-r--r--   0 catbeta    (501) staff       (20)      676 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/utils/flatten.py
-drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:23:32.296227 torchanalyse-0.0.1/torchanalyse/utils/ir/
--rw-r--r--   0 catbeta    (501) staff       (20)       79 2023-07-18 14:30:16.000000 torchanalyse-0.0.1/torchanalyse/utils/ir/__init__.py
--rw-r--r--   0 catbeta    (501) staff       (20)     1324 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/utils/ir/graph.py
--rw-r--r--   0 catbeta    (501) staff       (20)     1479 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/utils/ir/node.py
--rw-r--r--   0 catbeta    (501) staff       (20)      945 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/utils/ir/variable.py
--rw-r--r--   0 catbeta    (501) staff       (20)     1739 2023-07-19 19:09:01.000000 torchanalyse-0.0.1/torchanalyse/utils/trace.py
--rw-r--r--   0 catbeta    (501) staff       (20)       22 2023-07-20 13:15:07.000000 torchanalyse-0.0.1/torchanalyse/version.py
-drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:23:32.294996 torchanalyse-0.0.1/torchanalyse.egg-info/
--rw-r--r--   0 catbeta    (501) staff       (20)      113 2023-07-20 13:23:32.000000 torchanalyse-0.0.1/torchanalyse.egg-info/PKG-INFO
--rw-r--r--   0 catbeta    (501) staff       (20)      557 2023-07-20 13:23:32.000000 torchanalyse-0.0.1/torchanalyse.egg-info/SOURCES.txt
--rw-r--r--   0 catbeta    (501) staff       (20)        1 2023-07-20 13:23:32.000000 torchanalyse-0.0.1/torchanalyse.egg-info/dependency_links.txt
--rw-r--r--   0 catbeta    (501) staff       (20)       54 2023-07-20 13:23:32.000000 torchanalyse-0.0.1/torchanalyse.egg-info/requires.txt
--rw-r--r--   0 catbeta    (501) staff       (20)       13 2023-07-20 13:23:32.000000 torchanalyse-0.0.1/torchanalyse.egg-info/top_level.txt
+drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:43:30.128005 torchanalyse-0.0.2/
+-rw-r--r--   0 catbeta    (501) staff       (20)      113 2023-07-20 13:43:30.127783 torchanalyse-0.0.2/PKG-INFO
+-rw-r--r--   0 catbeta    (501) staff       (20)     1573 2023-07-20 13:25:49.000000 torchanalyse-0.0.2/README.md
+-rw-r--r--   0 catbeta    (501) staff       (20)       38 2023-07-20 13:43:30.128060 torchanalyse-0.0.2/setup.cfg
+-rw-r--r--   0 catbeta    (501) staff       (20)      359 2023-07-20 13:36:04.000000 torchanalyse-0.0.2/setup.py
+drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:43:30.125057 torchanalyse-0.0.2/torchanalyse/
+-rw-r--r--   0 catbeta    (501) staff       (20)      113 2023-07-20 13:15:23.000000 torchanalyse-0.0.2/torchanalyse/__init__.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     1243 2023-07-20 13:34:34.000000 torchanalyse-0.0.2/torchanalyse/profile.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     6791 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/system.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     1764 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/unit.py
+drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:43:30.126127 torchanalyse-0.0.2/torchanalyse/utils/
+-rw-r--r--   0 catbeta    (501) staff       (20)       65 2023-07-20 13:36:04.000000 torchanalyse-0.0.2/torchanalyse/utils/__init__.py
+-rw-r--r--   0 catbeta    (501) staff       (20)      676 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/flatten.py
+drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:43:30.126701 torchanalyse-0.0.2/torchanalyse/utils/ir/
+-rw-r--r--   0 catbeta    (501) staff       (20)       79 2023-07-18 14:30:16.000000 torchanalyse-0.0.2/torchanalyse/utils/ir/__init__.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     1324 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/ir/graph.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     1479 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/ir/node.py
+-rw-r--r--   0 catbeta    (501) staff       (20)      945 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/ir/variable.py
+drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:43:30.127551 torchanalyse-0.0.2/torchanalyse/utils/operatorlist/
+-rw-r--r--   0 catbeta    (501) staff       (20)       41 2023-07-20 13:36:04.000000 torchanalyse-0.0.2/torchanalyse/utils/operatorlist/__init__.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     7976 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/operatorlist/energy_cost.py
+-rw-r--r--   0 catbeta    (501) staff       (20)      132 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/operatorlist/math.py
+-rw-r--r--   0 catbeta    (501) staff       (20)    19991 2023-07-20 12:28:05.000000 torchanalyse-0.0.2/torchanalyse/utils/operatorlist/operator_base.py
+-rw-r--r--   0 catbeta    (501) staff       (20)    11200 2023-07-20 13:36:04.000000 torchanalyse-0.0.2/torchanalyse/utils/operatorlist/operator_list.py
+-rw-r--r--   0 catbeta    (501) staff       (20)     1739 2023-07-19 19:09:01.000000 torchanalyse-0.0.2/torchanalyse/utils/trace.py
+-rw-r--r--   0 catbeta    (501) staff       (20)       22 2023-07-20 13:39:48.000000 torchanalyse-0.0.2/torchanalyse/version.py
+drwxr-xr-x   0 catbeta    (501) staff       (20)        0 2023-07-20 13:43:30.125743 torchanalyse-0.0.2/torchanalyse.egg-info/
+-rw-r--r--   0 catbeta    (501) staff       (20)      113 2023-07-20 13:43:30.000000 torchanalyse-0.0.2/torchanalyse.egg-info/PKG-INFO
+-rw-r--r--   0 catbeta    (501) staff       (20)      761 2023-07-20 13:43:30.000000 torchanalyse-0.0.2/torchanalyse.egg-info/SOURCES.txt
+-rw-r--r--   0 catbeta    (501) staff       (20)        1 2023-07-20 13:43:30.000000 torchanalyse-0.0.2/torchanalyse.egg-info/dependency_links.txt
+-rw-r--r--   0 catbeta    (501) staff       (20)       54 2023-07-20 13:43:30.000000 torchanalyse-0.0.2/torchanalyse.egg-info/requires.txt
+-rw-r--r--   0 catbeta    (501) staff       (20)       13 2023-07-20 13:43:30.000000 torchanalyse-0.0.2/torchanalyse.egg-info/top_level.txt
```

### Comparing `torchanalyse-0.0.1/README.md` & `torchanalyse-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 
 # torchanalyse
 A pytorch model profiler with information about flops, energy, and e.t.c
 # How to use
-Please see `test_linear.py` and `test_transformer.py` for more information.
+Please see the files at `/examples ` like `test_linear.py` and `test_transformer.py` for more information.
 
-Basically, we use the `profiler` function in torch analyse.
+Basically, we use the `profiler` function in torch analyze.
 
 # What will the result be like
 
 ## Result of linear layer
 
 |   | Op Type      | Dimension                      | Bound | C/M ratio            | Op Intensity       | Latency (msec)         | Cycles             | C Effcy | Flops (MFLOP) | Input_a (MB) | Input_w (MB) | Output (MB) | Total Data (MB) | Throughput (Tflops) | Roofline Throughput offchip (Tflops) | Roofline Throughput onchip (Tflops) | Compute Cycles      | Memory Cycles      | Sparsity | Total energy (mJ)  |
 |---|--------------|--------------------------------|-------|----------------------|--------------------|------------------------|--------------------|---------|---------------|--------------|--------------|-------------|-----------------|---------------------|--------------------------------------|-------------------------------------|---------------------|--------------------|----------|--------------------|
 | 0 | aten::linear | "([1, 16], [32, 16], [1, 32])" | M     | 0.006689895470383274 | 0.9142857142857143 | 1.2444444444444445e-06 | 1.1697777777777778 | 1.0     | 0.001024      | 1.6e-05      | 0.000512     | 3.2e-05     | 0.00056         | 0.8228571428571428  | 0.8228571428571428                   | 0.8228571428571428                  | 0.00782569105691057 | 1.1697777777777778 | 0.0      | 154980.04707236143 |
 
-## Result of Transformer
-
-![image-20230720032249955](/Users/catbeta/Library/Application Support/typora-user-images/image-20230720032249955.png)
```

### Comparing `torchanalyse-0.0.1/torchanalyse/profile.py` & `torchanalyse-0.0.2/torchanalyse/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import warnings
 
-from .utils.operatorlist.operator_list import operator_list
-from .utils.trace import trace
+from .utils import operator_list
+from .utils import trace
 import pandas as pd
 import numpy as np
 
 __all__ = ["profiler"]
 
 
 def profiler(
```

### Comparing `torchanalyse-0.0.1/torchanalyse/system.py` & `torchanalyse-0.0.2/torchanalyse/system.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse/unit.py` & `torchanalyse-0.0.2/torchanalyse/unit.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse/utils/flatten.py` & `torchanalyse-0.0.2/torchanalyse/utils/flatten.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse/utils/ir/graph.py` & `torchanalyse-0.0.2/torchanalyse/utils/ir/graph.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse/utils/ir/node.py` & `torchanalyse-0.0.2/torchanalyse/utils/ir/node.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse/utils/ir/variable.py` & `torchanalyse-0.0.2/torchanalyse/utils/ir/variable.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse/utils/trace.py` & `torchanalyse-0.0.2/torchanalyse/utils/trace.py`

 * *Files identical despite different names*

### Comparing `torchanalyse-0.0.1/torchanalyse.egg-info/SOURCES.txt` & `torchanalyse-0.0.2/torchanalyse.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.py
 torchanalyse/__init__.py
-torchanalyse/handlers.py
 torchanalyse/profile.py
 torchanalyse/system.py
 torchanalyse/unit.py
 torchanalyse/version.py
 torchanalyse.egg-info/PKG-INFO
 torchanalyse.egg-info/SOURCES.txt
 torchanalyse.egg-info/dependency_links.txt
@@ -13,8 +12,13 @@
 torchanalyse.egg-info/top_level.txt
 torchanalyse/utils/__init__.py
 torchanalyse/utils/flatten.py
 torchanalyse/utils/trace.py
 torchanalyse/utils/ir/__init__.py
 torchanalyse/utils/ir/graph.py
 torchanalyse/utils/ir/node.py
-torchanalyse/utils/ir/variable.py
+torchanalyse/utils/ir/variable.py
+torchanalyse/utils/operatorlist/__init__.py
+torchanalyse/utils/operatorlist/energy_cost.py
+torchanalyse/utils/operatorlist/math.py
+torchanalyse/utils/operatorlist/operator_base.py
+torchanalyse/utils/operatorlist/operator_list.py
```

