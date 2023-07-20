# Comparing `tmp/pyracer-1.0.3.tar.gz` & `tmp/pyracer-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracer-1.0.3.tar", last modified: Thu Jul 20 01:48:32 2023, max compression
+gzip compressed data, was "pyracer-1.1.0.tar", last modified: Thu Jul 20 19:23:29 2023, max compression
```

## Comparing `pyracer-1.0.3.tar` & `pyracer-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:48:32.810479 pyracer-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 01:48:21.000000 pyracer-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 01:48:32.810479 pyracer-1.0.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:48:32.810479 pyracer-1.0.3/RACER/
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-07-20 01:48:21.000000 pyracer-1.0.3/RACER/RACER.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 01:48:21.000000 pyracer-1.0.3/RACER/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-20 01:48:21.000000 pyracer-1.0.3/RACER/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 01:48:21.000000 pyracer-1.0.3/RACER/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-20 01:48:21.000000 pyracer-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 01:48:32.810479 pyracer-1.0.3/pyracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 01:48:32.000000 pyracer-1.0.3/pyracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 01:48:32.000000 pyracer-1.0.3/pyracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 01:48:32.000000 pyracer-1.0.3/pyracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 01:48:32.000000 pyracer-1.0.3/pyracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 01:48:32.000000 pyracer-1.0.3/pyracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 01:48:32.810479 pyracer-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-20 01:48:21.000000 pyracer-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:23:29.132282 pyracer-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-20 19:23:20.000000 pyracer-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 19:23:29.132282 pyracer-1.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:23:29.132282 pyracer-1.1.0/RACER/
+-rw-r--r--   0 runner    (1001) docker     (123)    14422 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/RACER.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 19:23:20.000000 pyracer-1.1.0/RACER/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-20 19:23:20.000000 pyracer-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 19:23:29.132282 pyracer-1.1.0/pyracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 19:23:29.000000 pyracer-1.1.0/pyracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 19:23:29.132282 pyracer-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-20 19:23:20.000000 pyracer-1.1.0/setup.py
```

### Comparing `pyracer-1.0.3/LICENSE` & `pyracer-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracer-1.0.3/PKG-INFO` & `pyracer-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.0.3
+Version: 1.1.0
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.0.3/RACER/RACER.py` & `pyracer-1.1.0/RACER/RACER.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,22 +374,24 @@
         self._extants_if = new_extants_if
 
     def _finalize_rules(self) -> None:
         """Removes redundant rules to form the final ruleset"""
         temp_rules_if = self._final_rules_if
         temp_rules_then = self._final_rules_then
         temp_rules_fitnesses = self._fitnesses
-        for i in range(len(temp_rules_if) - 2):
+        i = 0
+        while i < len(temp_rules_if) - 1:
             mask = np.ones(len(temp_rules_if), dtype=bool)
             covered = self._covered(temp_rules_if[i + 1 :], temp_rules_if[i])
             mask[i + 1 :][covered] = False
             temp_rules_if, temp_rules_then, temp_rules_fitnesses = (
                 temp_rules_if[mask],
                 temp_rules_then[mask],
                 temp_rules_fitnesses[mask],
             )
+            i += 1
 
         self._final_rules_if, self._final_rules_then, self._fitnesses = (
             temp_rules_if,
             temp_rules_then,
             temp_rules_fitnesses,
         )
```

### Comparing `pyracer-1.0.3/RACER/preprocessing.py` & `pyracer-1.1.0/RACER/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 from typing import Tuple, Union
 
 import numpy as np
 import pandas as pd
 
-from optbinning import MDLP
+from optbinning import MulticlassOptimalBinning as MOB, MDLP
 
 
 class RACERPreprocessor:
-    def __init__(self, max_num_splits=32):
+    def __init__(self, target: str="multiclass", max_n_bins=32, max_num_splits=32):
         """RACER preprocessing step that quantizes numerical columns and dummy encodes the categorical ones.
-        Quantization is based on the entropy-based  Minimum Description Length Principle algorithm (MDLP).
+        Quantization is based on the optimal binning algorithm for "multiclass" tasks and the entropy-based MDLP
+        algorithm for "binary" tasks.
 
         Args:
+            target (str, optional): Whether the task if "multiclass" or "binary" classification. Defaults to "multiclass".
+            max_n_bins (int, optional): Maximum number of bins to quantize in. Defaults to 32.
             max_num_splits (int, optional): Maximum number of splits to consider at each partition for MDLP. Defaults to 32.
         """
-        self._max_num_splits = max_num_splits
+        assert target in ["multiclass", "binary"], "`target` must either be 'multiclass' or 'binary'"
+        if target == "multiclass":
+            self._quantizer = MOB(max_n_bins=max_n_bins)
+        elif target == "binary":
+            self._quantizer = MDLP(max_candidates=max_num_splits)
 
     def fit_transform(
         self, X: Union[pd.DataFrame, np.ndarray], y: Union[pd.DataFrame, np.ndarray]
     ) -> Tuple[Union[pd.DataFrame, np.ndarray], Union[pd.DataFrame, np.ndarray]]:
         """Preprocesses the dataset by replacing nominal vaues with dummy variables.
         Converts to numpy boolean arrays and returns the dataset. All numerical values are discretized
         using an optimal binning strategy that employs a decision tree as a preprocessing step.
@@ -30,17 +37,17 @@
         Returns:
             Tuple[Union[pd.DataFrame, np.ndarray], Union[pd.DataFrame, np.ndarray]]: Transformed features and targets vectors.
         """
         X, y = pd.DataFrame(X), pd.DataFrame(y)
         numerics_X = X.select_dtypes(include=[np.number]).columns.tolist()
         if numerics_X:
             for col in numerics_X:
-                optb = MDLP(max_candidates=self._max_num_splits)
-                optb.fit(X[col].values, np.squeeze(y.values))
-                X[col] = pd.cut(X[col], bins=optb.splits, duplicates="drop")
+                self._quantizer.fit(X[col].values, np.squeeze(y.values))
+                bins = [X[col].min()] + self._quantizer.splits.tolist() + [X[col].max()]
+                X[col] = pd.cut(X[col], bins=bins, include_lowest=True, labels=False)
         X, y = X.astype("category"), y.astype("category")
         X = pd.get_dummies(X).to_numpy()
         y = pd.get_dummies(y).to_numpy()
         return X, y
 
     def fit(
         self, X: Union[pd.DataFrame, np.ndarray], y: Union[pd.DataFrame, np.ndarray]
```

### Comparing `pyracer-1.0.3/README.md` & `pyracer-1.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 $ pip install pyracer
 ```
 
 ## Usage
 RACER is designed to be consistent with Scikit-learn estimator API which makes it very easy to use.
 
 
-The following example demonstrates the use of RACER on the Zoo dataset.
+The following example demonstrates the use of RACER on the Zoo dataset. Take a look at [examples](https://github.com/Adversarian/RACER/tree/main/examples) for more use cases.
 ### Data Obtention and Cleaning
 ```python
 from RACER import RACER, RACERPreprocessor
 from sklearn.model_selection import train_test_split
 import pandas as pd
 
 # dataset from https://archive.ics.uci.edu/ml/machine-learning-databases/zoo/
```

### Comparing `pyracer-1.0.3/pyracer.egg-info/PKG-INFO` & `pyracer-1.1.0/pyracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracer
-Version: 1.0.3
+Version: 1.1.0
 Summary: Unofficial Python implementation of the RACER classification algorithm.
 Home-page: https://github.com/Adversarian/RACER
 Author: Arian Tashakkor, Mohammad Safaiyan
 Author-email: a77physics@gmail.com
 License: MIT
 Keywords: machine learning,classification,RACER
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyracer-1.0.3/setup.py` & `pyracer-1.1.0/setup.py`

 * *Files identical despite different names*

