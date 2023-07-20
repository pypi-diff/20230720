# Comparing `tmp/PCCanalyser-0.5.1.tar.gz` & `tmp/PCCanalyser-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PCCanalyser-0.5.1.tar", last modified: Thu Jun 29 20:44:55 2023, max compression
+gzip compressed data, was "PCCanalyser-0.5.2.tar", last modified: Thu Jul 20 14:38:39 2023, max compression
```

## Comparing `PCCanalyser-0.5.1.tar` & `PCCanalyser-0.5.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.663468 PCCanalyser-0.5.1/
--rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.5.1/LICENSE
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.637054 PCCanalyser-0.5.1/PCCanalyser.egg-info/
--rw-r--r--   0 v94623eb2   (504) staff       (20)    16282 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)      482 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/SOURCES.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/dependency_links.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/entry_points.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       76 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/requires.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-06-29 20:44:55.000000 PCCanalyser-0.5.1/PCCanalyser.egg-info/top_level.txt
--rw-r--r--   0 v94623eb2   (504) staff       (20)    16282 2023-06-29 20:44:55.662856 PCCanalyser-0.5.1/PKG-INFO
--rw-r--r--   0 v94623eb2   (504) staff       (20)    16117 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/README.md
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.646735 PCCanalyser-0.5.1/matgen/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.1/matgen/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    65850 2023-06-29 20:36:38.000000 PCCanalyser-0.5.1/matgen/base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     1648 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/characterise.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     5922 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/entropic.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    19059 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/matutils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/ndisangles.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/ndisorientquat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)    12153 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/sparsemat.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/matgen/utils.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      940 2023-06-29 20:43:04.000000 PCCanalyser-0.5.1/pyproject.toml
--rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-06-29 20:44:55.663558 PCCanalyser-0.5.1/setup.cfg
-drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-06-29 20:44:55.649227 PCCanalyser-0.5.1/tests/
--rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.1/tests/__init__.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.5.1/tests/test_base.py
--rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-06-06 19:55:50.000000 PCCanalyser-0.5.1/tests/test_sparsemat.py
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-07-20 14:38:39.246471 PCCanalyser-0.5.2/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    35149 2022-09-08 11:03:35.000000 PCCanalyser-0.5.2/LICENSE
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-07-20 14:38:39.230148 PCCanalyser-0.5.2/PCCanalyser.egg-info/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16282 2023-07-20 14:38:39.000000 PCCanalyser-0.5.2/PCCanalyser.egg-info/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      482 2023-07-20 14:38:39.000000 PCCanalyser-0.5.2/PCCanalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        1 2023-07-20 14:38:39.000000 PCCanalyser-0.5.2/PCCanalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      172 2023-07-20 14:38:39.000000 PCCanalyser-0.5.2/PCCanalyser.egg-info/entry_points.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       90 2023-07-20 14:38:39.000000 PCCanalyser-0.5.2/PCCanalyser.egg-info/requires.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       13 2023-07-20 14:38:39.000000 PCCanalyser-0.5.2/PCCanalyser.egg-info/top_level.txt
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16282 2023-07-20 14:38:39.246106 PCCanalyser-0.5.2/PKG-INFO
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    16117 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/README.md
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-07-20 14:38:39.241614 PCCanalyser-0.5.2/matgen/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.2/matgen/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    65850 2023-06-29 20:36:38.000000 PCCanalyser-0.5.2/matgen/base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1638 2023-07-20 14:34:24.000000 PCCanalyser-0.5.2/matgen/characterise.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     5902 2023-07-20 14:34:02.000000 PCCanalyser-0.5.2/matgen/entropic.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    19059 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/matgen/matutils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     1567 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/matgen/ndisangles.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     3034 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/matgen/ndisorientquat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)    12153 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/matgen/sparsemat.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)     2145 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/matgen/utils.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      958 2023-07-20 14:37:48.000000 PCCanalyser-0.5.2/pyproject.toml
+-rw-r--r--   0 v94623eb2   (504) staff       (20)       38 2023-07-20 14:38:39.246536 PCCanalyser-0.5.2/setup.cfg
+drwxr-xr-x   0 v94623eb2   (504) staff       (20)        0 2023-07-20 14:38:39.245669 PCCanalyser-0.5.2/tests/
+-rw-r--r--   0 v94623eb2   (504) staff       (20)        0 2022-09-08 11:03:35.000000 PCCanalyser-0.5.2/tests/__init__.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      298 2023-02-27 16:00:35.000000 PCCanalyser-0.5.2/tests/test_base.py
+-rw-r--r--   0 v94623eb2   (504) staff       (20)      466 2023-06-06 19:55:50.000000 PCCanalyser-0.5.2/tests/test_sparsemat.py
```

### Comparing `PCCanalyser-0.5.1/LICENSE` & `PCCanalyser-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/PCCanalyser.egg-info/PKG-INFO` & `PCCanalyser-0.5.2/PCCanalyser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCCanalyser
-Version: 0.5.1
+Version: 0.5.2
 Summary: Polyhedral Cell Complex (PCC) Analysis tools
 Author: Oleg Bushuev
 Project-URL: documentation, https://github.com/PRISBteam/Voronoi_PCC_Analyser
 Project-URL: repository, https://github.com/PRISBteam/Voronoi_PCC_Analyser.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.1 Summary: Polyhedral Cell
+Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.2 Summary: Polyhedral Cell
 Complex (PCC) Analysis tools Author: Oleg Bushuev Project-URL: documentation,
 https://github.com/PRISBteam/Voronoi_PCC_Analyser Project-URL: repository,
 https://github.com/PRISBteam/Voronoi_PCC_Analyser.git Description-Content-Type:
 text/markdown License-File: LICENSE # Polyhedral Cell Complex (PCC) Analyser ##
 Quick start Installation: ``` pip install PCCanalyser ``` Using of classes: ```
 from matgen.base import CellComplex from matgen.entropic import
 TripleJunctionSet ``` Command-line interface (CLI) tools: ``` # generate sparse
```

### Comparing `PCCanalyser-0.5.1/PKG-INFO` & `PCCanalyser-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PCCanalyser
-Version: 0.5.1
+Version: 0.5.2
 Summary: Polyhedral Cell Complex (PCC) Analysis tools
 Author: Oleg Bushuev
 Project-URL: documentation, https://github.com/PRISBteam/Voronoi_PCC_Analyser
 Project-URL: repository, https://github.com/PRISBteam/Voronoi_PCC_Analyser.git
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.1 Summary: Polyhedral Cell
+Metadata-Version: 2.1 Name: PCCanalyser Version: 0.5.2 Summary: Polyhedral Cell
 Complex (PCC) Analysis tools Author: Oleg Bushuev Project-URL: documentation,
 https://github.com/PRISBteam/Voronoi_PCC_Analyser Project-URL: repository,
 https://github.com/PRISBteam/Voronoi_PCC_Analyser.git Description-Content-Type:
 text/markdown License-File: LICENSE # Polyhedral Cell Complex (PCC) Analyser ##
 Quick start Installation: ``` pip install PCCanalyser ``` Using of classes: ```
 from matgen.base import CellComplex from matgen.entropic import
 TripleJunctionSet ``` Command-line interface (CLI) tools: ``` # generate sparse
```

### Comparing `PCCanalyser-0.5.1/README.md` & `PCCanalyser-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/matgen/base.py` & `PCCanalyser-0.5.2/matgen/base.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/matgen/characterise.py` & `PCCanalyser-0.5.2/matgen/characterise.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Module for cell complex characterisation.
 """
 
 import argparse
-import os
 import time
 import glob
 import logging
 import pandas as pd
 
 from matgen.entropic import TripleJunctionSet
```

### Comparing `PCCanalyser-0.5.1/matgen/entropic.py` & `PCCanalyser-0.5.2/matgen/entropic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 Software module for the Entropic analysis paper
 """
 import math
 from typing import Iterable
 import logging
 import numpy as np
-import pandas as pd
 
 class TripleJunctionSet:
     """
     structure representation
     """
     def __init__(self, p, j_tuple) -> None:
         """
```

### Comparing `PCCanalyser-0.5.1/matgen/matutils.py` & `PCCanalyser-0.5.2/matgen/matutils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/matgen/ndisangles.py` & `PCCanalyser-0.5.2/matgen/ndisangles.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/matgen/ndisorientquat.py` & `PCCanalyser-0.5.2/matgen/ndisorientquat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/matgen/sparsemat.py` & `PCCanalyser-0.5.2/matgen/sparsemat.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/matgen/utils.py` & `PCCanalyser-0.5.2/matgen/utils.py`

 * *Files identical despite different names*

### Comparing `PCCanalyser-0.5.1/pyproject.toml` & `PCCanalyser-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PCCanalyser"
-version = "0.5.1"
+version = "0.5.2"
 dependencies = [
     "numpy >= 1.21.5", "scipy >= 1.7.3", "tqdm >= 4.64.1",
-    "jupyterlab >= 3.4.4", "matplotlib >= 3.5.2",
+    "jupyterlab >= 3.4.4", "matplotlib >= 3.5.2", "pandas >= 1.3.4"
 ]
 description = "Polyhedral Cell Complex (PCC) Analysis tools"
 readme = "README.md"
 authors = [{ name = "Oleg Bushuev" },]
 
 [project.urls]
 documentation = "https://github.com/PRISBteam/Voronoi_PCC_Analyser"
```

