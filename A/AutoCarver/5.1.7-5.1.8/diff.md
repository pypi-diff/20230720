# Comparing `tmp/AutoCarver-5.1.7.tar.gz` & `tmp/AutoCarver-5.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoCarver-5.1.7.tar", last modified: Mon Jul 17 21:00:50 2023, max compression
+gzip compressed data, was "AutoCarver-5.1.8.tar", last modified: Thu Jul 20 10:59:00 2023, max compression
```

## Comparing `AutoCarver-5.1.7.tar` & `AutoCarver-5.1.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.353508 AutoCarver-5.1.7/AutoCarver/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35190 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/auto_carver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.357508 AutoCarver-5.1.7/AutoCarver/converters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/converters/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.357508 AutoCarver-5.1.7/AutoCarver/discretizers/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24512 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.361508 AutoCarver-5.1.7/AutoCarver/discretizers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36173 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/base_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/grouped_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    31789 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/qualitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/quantitative_discretizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/discretizers/utils/type_discretizers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.361508 AutoCarver-5.1.7/AutoCarver/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/feature_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.361508 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/base_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/qualitative_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/filters/quantitative_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/base_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/qualitative_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/AutoCarver/feature_selection/measures/quantitative_measures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.353508 AutoCarver-5.1.7/AutoCarver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 21:00:50.000000 AutoCarver-5.1.7/AutoCarver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:00:50.365508 AutoCarver-5.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10638 2023-07-17 21:00:36.000000 AutoCarver-5.1.7/tests/test_auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35655 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/auto_carver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10629 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/converters/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/discretizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25459 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/discretizers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35455 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/base_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10581 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/grouped_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32441 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/qualitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7342 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/quantitative_discretizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/discretizers/utils/type_discretizers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16385 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/feature_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/base_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/qualitative_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/filters/quantitative_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/base_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/qualitative_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/AutoCarver/feature_selection/measures/quantitative_measures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/AutoCarver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 10:59:00.000000 AutoCarver-5.1.8/AutoCarver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-20 10:59:00.380810 AutoCarver-5.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:59:00.376810 AutoCarver-5.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-07-20 10:58:48.000000 AutoCarver-5.1.8/tests/test_auto_carver.py
```

### Comparing `AutoCarver-5.1.7/AutoCarver/auto_carver.py` & `AutoCarver-5.1.8/AutoCarver/auto_carver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 """Tool to build optimized buckets out of Quantitative and Qualitative features
 for a binary classification model.
 """
 
 from typing import Any
 
-from IPython.display import display_html
 from numpy import add, array, searchsorted, sqrt, unique, zeros
 from pandas import DataFrame, Series, crosstab
 from scipy.stats import chi2_contingency
 from tqdm import tqdm
 
 from .discretizers import GroupedList
 from .discretizers.discretizers import Discretizer
 from .discretizers.utils.base_discretizers import (
     BaseDiscretizer,
     convert_to_labels,
     convert_to_values,
 )
 from .discretizers.utils.serialization import json_deserialize_values_orders
 
+# trying to import extra dependencies
+try:
+    from IPython.display import display_html
+except ImportError:
+    _has_idisplay = False
+else:
+    _has_idisplay = True
+
 
 class AutoCarver(BaseDiscretizer):
     """Automatic carving of continuous, discrete, categorical and ordinal
     features that maximizes association with a binary target.
 
     First fits a :ref:`Discretizer`. Raw data should be provided as input (not a result of ``Discretizer.transform()``).
     """
@@ -167,15 +174,23 @@
         ), " - [AutoCarver] A feature of qualitative_features or ordinal_features also is in quantitative_features. Please, be carreful with your inputs!"
 
         # class specific attributes
         self.min_freq = min_freq  # minimum frequency per base bucket
         self.max_n_mod = max_n_mod  # maximum number of modality per feature
         # self.min_carved_freq = min_carved_freq  # TODO
         self.min_group_size = 1
-        self.pretty_print = pretty_print
+        if pretty_print:
+            if _has_idisplay:  # checking for installed dependencies
+                self.pretty_print = pretty_print
+            else:
+                self.verbose = True
+                print(
+                    "Package not found: ipython. Defaulting to verbose=True. Install extra dependencies with pip install autocarver[jupyter]"
+                )
+
         measures = ["tschuprowt", "cramerv"]  # association measure used to find the best groups
         assert (
             sort_by in measures
         ), f""" - [AutoCarver] Measure '{sort_by}' not yet implemented. Choose from: {str(measures)}."""
         self.sort_by = sort_by
 
         assert unknown_handling in [
```

### Comparing `AutoCarver-5.1.7/AutoCarver/converters/converters.py` & `AutoCarver-5.1.8/AutoCarver/converters/converters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/discretizers.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/discretizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,14 +370,22 @@
                 verbose=self.verbose,
             )
             x_copy = string_discretizer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(string_discretizer.values_orders)
 
+        # adding known nans at training
+        for feature in self.features:
+            if feature in self.values_orders:
+                order = self.values_orders[feature]
+                if any(x_copy[feature].isna()) and (self.str_nan not in order):
+                    order.append(self.str_nan)
+                    self.values_orders.update({feature: order})
+
         # checking that all unique values in X are in values_orders
         self._check_new_values(x_copy, features=self.ordinal_features)
 
         return x_copy
 
     def _remove_feature(self, feature: str) -> None:
         """Removes a feature from all `feature` attributes
@@ -404,19 +412,34 @@
 
         y : Series
             Binary target feature.
         """
         # checking data before bucketization
         x_copy = self._prepare_data(X, y)
 
+        # Base discretization (useful if already discretized)
+        base_discretizer = BaseDiscretizer(
+            features=[feature for feature in self.features if feature in self.values_orders],
+            values_orders=self.values_orders,
+            input_dtypes="str",
+            output_dtype="str",
+            dropna=False,
+            copy=True,
+            verbose=self.verbose,
+            str_nan="__NAN__",
+            str_default="__OTHER__",
+        )
+        x_copy = base_discretizer.fit_transform(x_copy, y)
+
         # [Qualitative ordinal features] Grouping rare values into closest common one
         if len(self.ordinal_features) > 0:
             ordinal_discretizer = OrdinalDiscretizer(
                 ordinal_features=self.ordinal_features,
                 values_orders=self.values_orders,
+                input_dtypes=self.input_dtypes,
                 min_freq=self.min_freq,
                 verbose=self.verbose,
                 str_nan=self.str_nan,
                 copy=False,
             )
             ordinal_discretizer.fit(x_copy, y)
```

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/utils/base_discretizers.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/utils/base_discretizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -247,20 +247,14 @@
 
         # checking for unexpected values for each feature
         for feature in features:
             unexpected = [
                 val for val in uniques[feature] if val not in self.values_orders[feature].values()
             ]
             assert (
-                self.str_nan not in unexpected
-            ), " - [BaseDiscretizer] It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_nan`. "
-            assert (
-                self.str_default not in unexpected
-            ), " - [BaseDiscretizer] It seems that your dataset has already been Discretized. AutoCarver only takes raw data as input (Discretizer included since v5.0.0). Be careful with `copy=False` not to rerun the same code twice. Ohterwise pass orders to `values_orders` or change the value of `str_default`. "
-            assert (
                 len(unexpected) == 0
             ), f" - [BaseDiscretizer] Unexpected value! The ordering for values: {str(list(unexpected))} of feature '{feature}' was not provided. There might be new values in your test/dev set. Consider taking a bigger test/dev set or dropping the column {feature}."
 
     def fit(self, X: DataFrame = None, y: Series = None) -> None:
         """Learns the labels associated to each value for each feature
 
         Parameters
@@ -419,15 +413,15 @@
             Model target, by default None
 
         Returns
         -------
         DataFrame
             Discretized X.
         """
-        # filling up nans with specified value
+        # filling up nans from features that have some
         if self.str_nan:
             X[self.qualitative_features] = X[self.qualitative_features].fillna(self.str_nan)
 
         # checking that all unique values in X are in values_orders
         self._check_new_values(X, features=self.qualitative_features)
 
         # replacing values for there corresponding label
@@ -463,14 +457,15 @@
             "copy": self.copy,
         }
 
         # dumping as json
         return json_serialized_groupedlistdiscretizer
 
     # TODO: add crosstabs per feature for a provided X?
+    # TODO: change str_nan for str(nan)
     def summary(self) -> DataFrame:
         """Summarizes the data discretization process.
 
         Returns
         -------
         DataFrame
             A summary of features' values per modalities.
```

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/utils/grouped_list.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/utils/grouped_list.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/utils/qualitative_discretizers.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/utils/qualitative_discretizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,24 +110,24 @@
             # initiating features missing from values_orders
             if feature not in self.values_orders:
                 self.values_orders.update({feature: GroupedList(nan_unique(x_copy[feature]))})
 
         # checking that all unique values in X are in values_orders
         self._check_new_values(x_copy, features=self.qualitative_features)
 
-        # checking that all unique values in values_orders are in X
-        # check_missing_values(x_copy, self.qualitative_features, self.values_orders)
-
         # adding NANS
         for feature in self.qualitative_features:
+            order = self.values_orders[feature]
             if any(x_copy[feature].isna()):
-                self.values_orders[feature].append(self.str_nan)
+                if self.str_nan not in order.values():
+                    order.append(self.str_nan)
+                    self.values_orders.update({feature: order})
 
         # filling up NaNs
-        x_copy = x_copy[self.qualitative_features].fillna(self.str_nan)
+        x_copy[self.qualitative_features] = x_copy[self.qualitative_features].fillna(self.str_nan)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series) -> None:
         """Finds simple buckets of modalities of X.
 
         Parameters
@@ -179,14 +179,19 @@
         # sorting orders based on target rates
         for feature in self.qualitative_features:
             order = self.values_orders[feature]
 
             # new ordering according to target rate
             new_order = list(target_rates[feature])
 
+            # checking for default but no value observed, enable to group this modality, raising error
+            assert (self.str_default in order and self.str_default in new_order) or (
+                self.str_default not in order and self.str_default not in new_order
+            ), f"Some values from values_orders['{feature}'] are never observed. Can not fit a distribution without any observation. Please remove following values {str([value for value in order.content[self.str_default] if value != self.str_default])} from values_orders['{feature}']."
+
             # leaving NaNs at the end of the list
             if self.str_nan in new_order:
                 new_order.remove(self.str_nan)
                 new_order += [self.str_nan]
 
             # sorting order updating values_orders
             self.values_orders.update({feature: order.sort_by(new_order)})
@@ -415,17 +420,14 @@
             If ``True``, feature processing at transform is applied to a copy of the provided DataFrame, by default ``False``
 
         verbose : bool, optional
             If ``True``, prints raw Discretizers Fit and Transform steps, by default ``False``
 
         str_nan : str, optional
             String representation to input ``numpy.nan``. If ``dropna=False``, ``numpy.nan`` will be left unchanged, by default ``"__NAN__"``
-
-        str_default : str, optional
-            String representation for default qualitative values, i.e. values less frequent than ``min_freq``, by default ``"__OTHER__"``
         """
         # Initiating BaseDiscretizer
         super().__init__(
             features=qualitative_features,
             values_orders=values_orders,
             input_dtypes="str",
             output_dtype="str",
@@ -565,23 +567,19 @@
             )
             x_copy = stringer.fit_transform(x_copy)
 
             # updating values_orders accordingly
             self.values_orders.update(stringer.values_orders)
 
         # filling nans
-        x_copy = x_copy.fillna(self.str_nan)
+        x_copy[self.features] = x_copy[self.features].fillna(self.str_nan)
 
         # adding nans and unknown values
         for feature in self.features:
-            # adding NaNs to the order if any
             order = self.values_orders[feature]
-            if any(x_copy[feature] == self.str_nan):
-                order.append(self.str_nan)
-
             # checking for unknown values (missing from known_values)
             unknown_values = [
                 value
                 for value in x_copy[feature].unique()
                 if value not in self.known_values and value != self.str_nan
             ]
 
@@ -596,28 +594,33 @@
                 # dropping unknown value
                 else:  # unknown_handling='drop'
                     # alerting user
                     print(
                         f" - [ChainedDiscretizer] Order for feature '{feature}' was not provided for values:  {str(unknown_values)}, these values will be converted to '{self.str_nan}' (policy unknown_handling='drop')"
                     )
 
-                    # adding nan to the order if not already present
-                    if self.str_nan not in order:
-                        order.append(self.str_nan)
-
                     # adding unknown to the order
                     for unknown_value in unknown_values:
                         order.append(unknown_value)
+                        order.append(self.str_nan)
                         # grouping unknown value with str_nan
                         order.group(unknown_value, self.str_nan)
-                        x_copy[feature] = x_copy[feature].replace(unknown_value, self.str_nan)
 
             # updating values_orders accordingly
             self.values_orders.update({feature: order})
 
+        # adding up NAN for all features of values_orders for seamless integration
+        # when GroupedList._tranform_qualitative is called nans are replaced by str_nan
+        for feature, order in self.values_orders.items():
+            # adding NaNs to the order if any
+            if any(x_copy[feature].isna()) or any(x_copy[feature] == self.str_nan):
+                if self.str_nan not in order:
+                    order.append(self.str_nan)
+                    self.values_orders.update({feature: order})
+
         # checking that all unique values in X are in values_orders
         self._check_new_values(x_copy, features=self.features)
 
         return x_copy
 
     def fit(self, X: DataFrame, y: Series = None) -> None:
         """Finds simple buckets of modalities of X.
@@ -642,15 +645,17 @@
             frequencies = x_copy[feature].value_counts(normalize=True)
 
             # iterating over each specified orders
             for level_order in self.chained_orders:
                 values, frequencies = frequencies.index, frequencies.values
 
                 # values that are frequent enough
-                to_keep = list(values[frequencies >= self.min_freq])
+                to_keep = list(values[frequencies >= self.min_freq]) + [
+                    self.str_nan,
+                ]
 
                 # values from the order to group (not frequent enough or absent)
                 values_to_group = [value for value in level_order.values() if value not in to_keep]
 
                 # values to group into discarded values
                 groups_value = [level_order.get_group(value) for value in values_to_group]
```

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/utils/quantitative_discretizers.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/utils/quantitative_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/utils/serialization.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/discretizers/utils/type_discretizers.py` & `AutoCarver-5.1.8/AutoCarver/discretizers/utils/type_discretizers.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/feature_selector.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """Tools to select the best Quantitative and Qualitative features."""
 
 from random import shuffle
 from typing import Any, Callable
 
-from IPython.display import display_html
 from pandas import DataFrame, Series
 
 from .filters import cramerv_filter, spearman_filter, thresh_filter
 from .measures import cramerv_measure, dtype_measure, kruskal_measure, mode_measure, nans_measure
 
+# trying to import extra dependencies
+try:
+    from IPython.display import display_html
+except ImportError:
+    _has_idisplay = False
+else:
+    _has_idisplay = True
+
 
 class FeatureSelector:
     """A pipeline of measures to perform a feature pre-selection that maximizes association
     with a binary target.
 
     * Best features are the n_best of each measure
     * Get your best features with ``FeatureSelector.select()``!
@@ -134,15 +141,22 @@
         self.filters = [thresh_filter] + filters[:]
 
         # names of measures to sort by
         self.measure_names = [measure.__name__ for measure in measures[::-1]]
 
         # wether or not to print tables
         self.verbose = bool(max(verbose, pretty_print))
-        self.pretty_print = pretty_print
+        if pretty_print:
+            if _has_idisplay:  # checking for installed dependencies
+                self.pretty_print = pretty_print
+            else:
+                self.verbose = True
+                print(
+                    "Package not found: ipython. Defaulting to verbose=True. Install extra dependencies with pip install autocarver[jupyter]"
+                )
 
         # keyword arguments
         self.params = params
 
     def _select_features(
         self, X: DataFrame, y: Series, features: list[str], n_best: int
     ) -> list[str]:
```

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/filters/base_filters.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/filters/base_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/filters/qualitative_filters.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/filters/qualitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/filters/quantitative_filters.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/filters/quantitative_filters.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/measures/base_measures.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/measures/base_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/measures/qualitative_measures.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/measures/qualitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver/feature_selection/measures/quantitative_measures.py` & `AutoCarver-5.1.8/AutoCarver/feature_selection/measures/quantitative_measures.py`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/AutoCarver.egg-info/PKG-INFO` & `AutoCarver-5.1.8/AutoCarver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.7
+Version: 5.1.8
 Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: jupyter
 License-File: LICENSE
 
 \n</p>
 <p align="left">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
```

### Comparing `AutoCarver-5.1.7/AutoCarver.egg-info/SOURCES.txt` & `AutoCarver-5.1.8/AutoCarver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/LICENSE` & `AutoCarver-5.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/PKG-INFO` & `AutoCarver-5.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoCarver
-Version: 5.1.7
+Version: 5.1.8
 Summary: Automatic Discretization of Features with Optimal Target Association
 Home-page: https://github.com/mdefrance/AutoCarver
 Author: Mario DEFRANCE
 Author-email: defrancemario@gmail.com
 License: MIT
 Project-URL: Documentation, https://autocarver.readthedocs.io/en/latest/index.html
 Project-URL: Bug Tracker, https://github.com/mdefrance/AutoCarver/issues
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: jupyter
 License-File: LICENSE
 
 \n</p>
 <p align="left">
     <img alt="PyPI" src="https://img.shields.io/pypi/v/autocarver">
     <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/autocarver">
     <img alt="GitHub" src="https://img.shields.io/github/license/mdefrance/autocarver">
```

### Comparing `AutoCarver-5.1.7/README.md` & `AutoCarver-5.1.8/README.md`

 * *Files identical despite different names*

### Comparing `AutoCarver-5.1.7/setup.py` & `AutoCarver-5.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="AutoCarver",
-    version="5.1.7",
+    version="5.1.8",
     author="Mario DEFRANCE",
     author_email="defrancemario@gmail.com",
     description="Automatic Discretization of Features with Optimal Target Association",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mdefrance/AutoCarver",
     project_urls={
@@ -25,16 +25,20 @@
     install_requires=[
         "pandas",
         "numpy",
         "scipy",
         "scikit-learn",
         "statsmodels",
         "tqdm",
-        "ipython",
     ],
+    extras_require={
+        "jupyter": [
+            "ipython",
+        ]
+    },
     packages=find_packages(),
     classifiers=[
         # ou 4 - Beta ou 5 - Production/Stable
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `AutoCarver-5.1.7/tests/test_auto_carver.py` & `AutoCarver-5.1.8/tests/test_auto_carver.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,16 +163,16 @@
         sort_by=sort_by,
         output_dtype=output_dtype,
         dropna=dropna,
         copy=copy,
         verbose=False,
     )
     x_discretized = auto_carver.fit_transform(
-        x_discretized,
-        x_discretized["quali_ordinal_target"],
+        x_train,
+        x_train["quali_ordinal_target"],
         X_dev=x_dev_1,
         y_dev=x_dev_1["quali_ordinal_target"],
     )
     x_dev_discretized = auto_carver.transform(x_dev_1)
 
     assert all(
         x_discretized[auto_carver.features].nunique() <= max_n_mod
@@ -292,15 +292,17 @@
         max_n_mod=max_n_mod,
         sort_by=sort_by,
         output_dtype=output_dtype,
         dropna=dropna,
         copy=copy,
         verbose=False,
     )
-    x_discretized = auto_carver.fit_transform(x_discretized, x_discretized["quali_ordinal_target"])
+    x_discretized = auto_carver.fit_transform(
+        x_train_wrong_2, x_train_wrong_2["quali_ordinal_target"]
+    )
 
     if not dropna and sort_by == "cramerv":
         expected = {
             "Mediums": [
                 "Low+",
                 "Low",
                 "Low-",
@@ -310,18 +312,18 @@
                 "Medium",
                 "Medium-",
                 "Mediums",
             ],
             "High+": ["High", "High-", "Highs", "Best", "ALONE", "BEST", "High+"],
             "__NAN__": ["unknown", "__NAN__"],
         }
-        print(auto_carver.values_orders["Qualitative_Ordinal_lownan"].content)
         assert (
             auto_carver.values_orders["Qualitative_Ordinal_lownan"].content == expected
         ), "Unknown modalities should be kept in the order"
+
     elif dropna and sort_by == "tschuprowt":
         expected = {
             "Mediums": [
                 "Low+",
                 "Low",
                 "Low-",
                 "Lows",
@@ -330,11 +332,10 @@
                 "Medium",
                 "Medium-",
                 "Mediums",
             ],
             "High+": ["High", "High-", "Highs", "Best", "ALONE", "BEST", "High+"],
             "__NAN__": ["unknown", "__NAN__"],
         }
-        print(auto_carver.values_orders["Qualitative_Ordinal_lownan"].content)
         assert (
             auto_carver.values_orders["Qualitative_Ordinal_lownan"].content == expected
         ), "Unknown modalities should be kept in the order"
```

