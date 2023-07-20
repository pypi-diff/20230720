# Comparing `tmp/uframe-0.0.2.tar.gz` & `tmp/uframe-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uframe-0.0.2.tar", last modified: Thu Jul 20 07:47:21 2023, max compression
+gzip compressed data, was "uframe-0.0.3.tar", last modified: Thu Jul 20 08:08:26 2023, max compression
```

## Comparing `uframe-0.0.2.tar` & `uframe-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 07:47:21.467515 uframe-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5081 2023-07-20 07:47:21.467515 uframe-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.2/README.md
--rw-rw-rw-   0        0        0     1053 2023-07-20 07:41:54.000000 uframe-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      462 2023-07-20 07:47:21.467515 uframe-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-07-11 11:16:34.000000 uframe-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:47:21.427358 uframe-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-20 07:47:21.451830 uframe-0.0.2/src/uframe/
--rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.2/src/uframe/__init__.py
--rw-rw-rw-   0        0        0    62423 2023-07-19 09:03:01.000000 uframe-0.0.2/src/uframe/uframe.py
--rw-rw-rw-   0        0        0     7066 2023-07-11 11:16:34.000000 uframe-0.0.2/src/uframe/uframe_from_mice.py
--rw-rw-rw-   0        0        0    12408 2023-07-11 11:16:34.000000 uframe-0.0.2/src/uframe/uframe_instance.py
-drwxrwxrwx   0        0        0        0 2023-07-20 07:47:21.467515 uframe-0.0.2/src/uframe.egg-info/
--rw-rw-rw-   0        0        0     5081 2023-07-20 07:47:21.000000 uframe-0.0.2/src/uframe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      409 2023-07-20 07:47:21.000000 uframe-0.0.2/src/uframe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 07:47:21.000000 uframe-0.0.2/src/uframe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.2/src/uframe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       85 2023-07-20 07:47:21.000000 uframe-0.0.2/src/uframe.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-20 07:47:21.000000 uframe-0.0.2/src/uframe.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-20 07:47:21.467515 uframe-0.0.2/tests/
--rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.2/tests/test_uframe.py
--rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.2/tests/test_uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.903653 uframe-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-07-11 11:16:34.000000 uframe-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5081 2023-07-20 08:08:26.903653 uframe-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4479 2023-07-11 11:16:34.000000 uframe-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1053 2023-07-20 08:05:14.000000 uframe-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      462 2023-07-20 08:08:26.903653 uframe-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-07-11 11:16:34.000000 uframe-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.855255 uframe-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.871376 uframe-0.0.3/src/uframe/
+-rw-rw-rw-   0        0        0      534 2023-07-11 11:16:34.000000 uframe-0.0.3/src/uframe/__init__.py
+-rw-rw-rw-   0        0        0    61128 2023-07-20 08:07:55.000000 uframe-0.0.3/src/uframe/uframe.py
+-rw-rw-rw-   0        0        0     7066 2023-07-11 11:16:34.000000 uframe-0.0.3/src/uframe/uframe_from_mice.py
+-rw-rw-rw-   0        0        0    12408 2023-07-11 11:16:34.000000 uframe-0.0.3/src/uframe/uframe_instance.py
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.890588 uframe-0.0.3/src/uframe.egg-info/
+-rw-rw-rw-   0        0        0     5081 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-20 07:40:14.000000 uframe-0.0.3/src/uframe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       85 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-20 08:08:26.000000 uframe-0.0.3/src/uframe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 08:08:26.903653 uframe-0.0.3/tests/
+-rw-rw-rw-   0        0        0      224 2023-07-11 11:16:34.000000 uframe-0.0.3/tests/test_uframe.py
+-rw-rw-rw-   0        0        0     2703 2023-07-11 11:16:34.000000 uframe-0.0.3/tests/test_uframe_instance.py
```

### Comparing `uframe-0.0.2/LICENSE` & `uframe-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uframe-0.0.2/PKG-INFO` & `uframe-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.2/README.md` & `uframe-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `uframe-0.0.2/pyproject.toml` & `uframe-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
 
 [project]
 name = "uframe"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Christian Amesoder", email="christian.amesoeder@informatik.uni-regensburg.de" },
   { name="Michael Hagn", email="michael.hagn@stud.uni-regensburg.de" }
 ]
 description = "Package for handling uncertain data"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `uframe-0.0.2/src/uframe/__init__.py` & `uframe-0.0.3/src/uframe/__init__.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.2/src/uframe/uframe.py` & `uframe-0.0.3/src/uframe/uframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import numpy as np
 #from src.uframe import uframe_instance
-from uframe_instance import uframe_instance
 import scipy
 from scipy import stats
 from sklearn.neighbors import KernelDensity
 import sklearn.neighbors
-from sklearn.preprocessing import LabelEncoder, OneHotEncoder, MinMaxScaler
+from sklearn.preprocessing import OneHotEncoder, MinMaxScaler
 import miceforest as mf
 import math
-from copy import deepcopy
 import pickle 
-from sklearn.mixture import GaussianMixture 
-import torch 
 import matplotlib.pyplot as plt 
 from matplotlib.backends.backend_pdf import PdfPages
 
 #SOLANGE DAS NICHT FUNKTIONIERT; MÜSSEN WERTE IN KATEGORIELLEN SPALTEN GANZZAHLIG SEIN
 #nur Integer als Keys für kategorielle Verteilung zugelassen, muss append Funktion entsprechend anpassen 
 #checke jeweils, ob schon cat value dict vorhanden, falls ja, ob es ergänzt werden muss
 #falls kein cat value dict vorhanden, suche eine cat value Liste, die geeignet ist 
@@ -1107,42 +1103,15 @@
     return [["Var",str(round(np.var(residues),2))],
             ["MAE", str(round(np.mean(np.abs(residues)),2))],
             ["RMSE", str(round(np.sqrt(np.mean(residues**2)),2))],
             ["Diff Quantile", str(round(np.mean(np.abs(true_q - new_q)),2))]]
             
        
 
-#makes sense for continuous uncertain variables only 
-def prepare_for_adf(frame, n_samples=10):
-    
-    means = frame.array_rep()
-    variances = np.zeros(means.shape)
-    
-    #iterate over instances and use sample function of uframe_instance, if necessary
-    for i, inst in enumerate(frame.data):
-        
-        if np.any(np.isnan(means[i,:])):
-            nan_indices = np.argwhere(np.isnan(means[i,:]))
-            nan_indices.reshape(nan_indices.shape[0])
-            print("nan indices", nan_indices)
-            samples = inst.sample(n=n_samples)[:, nan_indices].squeeze(axis=2)
-            print("Samples", samples)
-            print(samples.shape)
-            gm = GaussianMixture(n_components=1, covariance_type='diag').fit(samples)
-        
-        distr_index = 0
-        for j in range(means.shape[1]):
-            if np.isnan(means[i,j]):
-                means[i,j] = gm.means_[0, distr_index]
-                variances[i,j] = gm.covariances_[0, distr_index]
-                distr_index +=1
-    
-    means = torch.from_numpy(means)
-    variances = torch.from_numpy(variances)
-    return means, variances
+
         
 # takes np array, randomly picks percentage of values p and introduces uncertainty there
 # allow different kernels for the values given by mice, then use the mixed distr append function
 # allow scipy or sklearn kernels
 # one multidimensional kernel is fitted for each row with missing values
 def uframe_from_array_mice(a: np.ndarray, p=0.1, mice_iterations=5, kernel="stats.gaussian_kde",
                            scaler= "min_max"):
```

### Comparing `uframe-0.0.2/src/uframe/uframe_from_mice.py` & `uframe-0.0.3/src/uframe/uframe_from_mice.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.2/src/uframe/uframe_instance.py` & `uframe-0.0.3/src/uframe/uframe_instance.py`

 * *Files identical despite different names*

### Comparing `uframe-0.0.2/src/uframe.egg-info/PKG-INFO` & `uframe-0.0.3/src/uframe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uframe
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for handling uncertain data
 Author: Christian Amesoeder and Michael Hagn
 Author-email: Christian Amesoder <christian.amesoeder@informatik.uni-regensburg.de>, Michael Hagn <michael.hagn@stud.uni-regensburg.de>
 Project-URL: Homepage, https://github.com/URWI2/uframe
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `uframe-0.0.2/tests/test_uframe_instance.py` & `uframe-0.0.3/tests/test_uframe_instance.py`

 * *Files identical despite different names*

