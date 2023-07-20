# Comparing `tmp/eugene_tools-0.1.0.tar.gz` & `tmp/eugene_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eugene_tools-0.1.0.tar", max compression
+gzip compressed data, was "eugene_tools-0.1.1.tar", max compression
```

## Comparing `eugene_tools-0.1.0.tar` & `eugene_tools-0.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1066 2023-01-26 02:27:24.000000 eugene_tools-0.1.0/LICENSE
--rw-r--r--   0        0        0     1840 2023-03-21 15:05:35.000000 eugene_tools-0.1.0/README.md
--rw-r--r--   0        0        0      578 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/__init__.py
--rw-r--r--   0        0        0     6279 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/_settings.py
--rw-r--r--   0        0        0     1455 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/conftest.py
--rw-r--r--   0        0        0       45 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/dataload/__init__.py
--rw-r--r--   0        0        0    15141 2023-06-21 23:18:28.000000 eugene_tools-0.1.0/eugene/dataload/_augment.py
--rw-r--r--   0        0        0     1244 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/dataload/_utils.py
--rw-r--r--   0        0        0      258 2023-06-04 23:20:15.000000 eugene_tools-0.1.0/eugene/evaluate/__init__.py
--rw-r--r--   0        0        0     1259 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/evaluate/_evaluate.py
--rw-r--r--   0        0        0     8522 2023-06-19 16:37:09.000000 eugene_tools-0.1.0/eugene/evaluate/_predict.py
--rw-r--r--   0        0        0      991 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/_utils.py
--rw-r--r--   0        0        0        0 2023-06-04 23:18:14.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0     2741 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_binary_classification.py
--rw-r--r--   0        0        0      541 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_multiclass_classification.py
--rw-r--r--   0        0        0    13629 2023-06-22 01:19:28.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_profile_prediction.py
--rw-r--r--   0        0        0      745 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/evaluate/metrics/_regression.py
--rw-r--r--   0        0        0     3049 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_AdverserialModule.py
--rw-r--r--   0        0        0     8244 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_AugmentModule.py
--rw-r--r--   0        0        0     7013 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_GenerativeModule.py
--rw-r--r--   0        0        0        0 2023-06-02 01:31:03.000000 eugene_tools-0.1.0/eugene/experimental/_LanguageModule.py
--rw-r--r--   0        0        0     1204 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_hyperopt_wandb.py
--rw-r--r--   0        0        0     7154 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_language_models.py
--rw-r--r--   0        0        0     1905 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/experimental/_preprocess.py
--rw-r--r--   0        0        0      218 2023-06-22 19:12:07.000000 eugene_tools-0.1.0/eugene/interpret/__init__.py
--rw-r--r--   0        0        0     1981 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/interpret/_attribute.py
--rw-r--r--   0        0        0     5085 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/interpret/_filters.py
--rw-r--r--   0        0        0     2804 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/interpret/_generative.py
--rw-r--r--   0        0        0     4390 2023-06-22 19:11:28.000000 eugene_tools-0.1.0/eugene/interpret/_gia.py
--rw-r--r--   0        0        0     8268 2023-06-22 01:39:46.000000 eugene_tools-0.1.0/eugene/models/_ProfileModule.py
--rw-r--r--   0        0        0    11056 2023-06-21 19:34:53.000000 eugene_tools-0.1.0/eugene/models/_SequenceModule.py
--rw-r--r--   0        0        0      255 2023-06-22 22:48:25.000000 eugene_tools-0.1.0/eugene/models/__init__.py
--rw-r--r--   0        0        0     1778 2023-06-22 23:12:56.000000 eugene_tools-0.1.0/eugene/models/_utils.py
--rw-r--r--   0        0        0        0 2023-06-02 01:31:03.000000 eugene_tools-0.1.0/eugene/models/base/__init__.py
--rw-r--r--   0        0        0     8986 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_blocks.py
--rw-r--r--   0        0        0     4566 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_initializers.py
--rw-r--r--   0        0        0    11661 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_layers.py
--rw-r--r--   0        0        0     3654 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_losses.py
--rw-r--r--   0        0        0     1642 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_metrics.py
--rw-r--r--   0        0        0    10447 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_module.py
--rw-r--r--   0        0        0      625 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_optimizers.py
--rw-r--r--   0        0        0     3311 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_regularizers.py
--rw-r--r--   0        0        0      121 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_schedulers.py
--rw-r--r--   0        0        0    12485 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_towers.py
--rw-r--r--   0        0        0     1731 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/base/_utils.py
--rw-r--r--   0        0        0      347 2023-06-22 22:46:51.000000 eugene_tools-0.1.0/eugene/models/zoo/__init__.py
--rw-r--r--   0        0        0    21129 2023-06-19 16:39:57.000000 eugene_tools-0.1.0/eugene/models/zoo/_basic_models.py
--rw-r--r--   0        0        0     4964 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_cre_activity_predictors.py
--rw-r--r--   0        0        0     6353 2023-06-21 19:28:04.000000 eugene_tools-0.1.0/eugene/models/zoo/_profile_predictors.py
--rw-r--r--   0        0        0    13340 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_regulatory_classifiers.py
--rw-r--r--   0        0        0     3291 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_single_cell_predictors.py
--rw-r--r--   0        0        0    10772 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/models/zoo/_tf_binding_predictors.py
--rw-r--r--   0        0        0      578 2023-06-22 19:12:32.000000 eugene_tools-0.1.0/eugene/plot/__init__.py
--rw-r--r--   0        0        0     7390 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_catplot.py
--rw-r--r--   0        0        0     7922 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_classification.py
--rw-r--r--   0        0        0     3601 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_dim_reduce.py
--rw-r--r--   0        0        0     3450 2023-06-22 19:07:58.000000 eugene_tools-0.1.0/eugene/plot/_gia.py
--rw-r--r--   0        0        0     6217 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_regression.py
--rw-r--r--   0        0        0    20681 2023-06-23 20:45:02.000000 eugene_tools-0.1.0/eugene/plot/_seq.py
--rw-r--r--   0        0        0    11115 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_summary.py
--rw-r--r--   0        0        0     3868 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/plot/_training.py
--rw-r--r--   0        0        0     9721 2023-06-23 20:43:47.000000 eugene_tools-0.1.0/eugene/plot/_utils.py
--rw-r--r--   0        0        0      281 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/preprocess/__init__.py
--rw-r--r--   0        0        0     8699 2023-06-23 20:21:46.000000 eugene_tools-0.1.0/eugene/preprocess/_seqdata.py
--rw-r--r--   0        0        0     1084 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/preprocess/_utils.py
--rw-r--r--   0        0        0       78 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/train/__init__.py
--rw-r--r--   0        0        0     8499 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/train/_fit.py
--rw-r--r--   0        0        0     7183 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/train/_hyperopt.py
--rw-r--r--   0        0        0       30 2023-06-04 01:53:27.000000 eugene_tools-0.1.0/eugene/utils/__init__.py
--rw-r--r--   0        0        0      412 2023-06-19 16:37:10.000000 eugene_tools-0.1.0/eugene/utils/_utils.py
--rw-r--r--   0        0        0      679 2023-06-23 20:48:37.000000 eugene_tools-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2804 1970-01-01 00:00:00.000000 eugene_tools-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-26 02:27:24.000000 eugene_tools-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1061 2023-07-20 18:47:35.000000 eugene_tools-0.1.1/README.md
+-rw-r--r--   0        0        0      584 2023-07-17 22:54:02.000000 eugene_tools-0.1.1/eugene/__init__.py
+-rw-r--r--   0        0        0     6279 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/_settings.py
+-rw-r--r--   0        0        0     1455 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/conftest.py
+-rw-r--r--   0        0        0       73 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/dataload/__init__.py
+-rw-r--r--   0        0        0     2709 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/dataload/_augment.py
+-rw-r--r--   0        0        0     2263 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/dataload/_utils.py
+-rw-r--r--   0        0        0      258 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/_evaluate.py
+-rw-r--r--   0        0        0    13118 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/_predict.py
+-rw-r--r--   0        0        0      991 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0     2741 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_binary_classification.py
+-rw-r--r--   0        0        0      541 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_multiclass_classification.py
+-rw-r--r--   0        0        0    13629 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_profile_prediction.py
+-rw-r--r--   0        0        0      745 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_regression.py
+-rw-r--r--   0        0        0     3049 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_AdverserialModule.py
+-rw-r--r--   0        0        0     8244 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_AugmentModule.py
+-rw-r--r--   0        0        0     7013 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_GenerativeModule.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_LanguageModule.py
+-rw-r--r--   0        0        0     1204 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_hyperopt_wandb.py
+-rw-r--r--   0        0        0     7154 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_language_models.py
+-rw-r--r--   0        0        0     1905 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_preprocess.py
+-rw-r--r--   0        0        0      218 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/__init__.py
+-rw-r--r--   0        0        0     4089 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/_attribute.py
+-rw-r--r--   0        0        0     8720 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/_filters.py
+-rw-r--r--   0        0        0     3703 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/_generative.py
+-rw-r--r--   0        0        0     6549 2023-07-20 03:46:53.000000 eugene_tools-0.1.1/eugene/interpret/_gia.py
+-rw-r--r--   0        0        0    10508 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/_ProfileModule.py
+-rw-r--r--   0        0        0    14478 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/_SequenceModule.py
+-rw-r--r--   0        0        0      346 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/__init__.py
+-rw-r--r--   0        0        0     2043 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/__init__.py
+-rw-r--r--   0        0        0     8986 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_blocks.py
+-rw-r--r--   0        0        0     5621 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_initializers.py
+-rw-r--r--   0        0        0    11661 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_layers.py
+-rw-r--r--   0        0        0     3654 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_losses.py
+-rw-r--r--   0        0        0     1827 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_metrics.py
+-rw-r--r--   0        0        0    10447 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_module.py
+-rw-r--r--   0        0        0       83 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_optimizers.py
+-rw-r--r--   0        0        0     3311 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_regularizers.py
+-rw-r--r--   0        0        0      121 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_schedulers.py
+-rw-r--r--   0        0        0    12485 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_towers.py
+-rw-r--r--   0        0        0     1731 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_utils.py
+-rw-r--r--   0        0        0      347 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/zoo/__init__.py
+-rw-r--r--   0        0        0    27146 2023-07-18 15:50:10.000000 eugene_tools-0.1.1/eugene/models/zoo/_basic_models.py
+-rw-r--r--   0        0        0     5615 2023-07-18 15:51:03.000000 eugene_tools-0.1.1/eugene/models/zoo/_cre_activity_predictors.py
+-rw-r--r--   0        0        0     6596 2023-07-18 15:51:35.000000 eugene_tools-0.1.1/eugene/models/zoo/_profile_predictors.py
+-rw-r--r--   0        0        0    18311 2023-07-18 15:54:07.000000 eugene_tools-0.1.1/eugene/models/zoo/_regulatory_classifiers.py
+-rw-r--r--   0        0        0     3291 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/zoo/_single_cell_predictors.py
+-rw-r--r--   0        0        0    13955 2023-07-18 15:56:56.000000 eugene_tools-0.1.1/eugene/models/zoo/_tf_binding_predictors.py
+-rw-r--r--   0        0        0      483 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/__init__.py
+-rw-r--r--   0        0        0     7410 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_catplot.py
+-rw-r--r--   0        0        0     8227 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_classification.py
+-rw-r--r--   0        0        0     3545 2023-07-20 03:47:25.000000 eugene_tools-0.1.1/eugene/plot/_experimental.py
+-rw-r--r--   0        0        0     4458 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_gia.py
+-rw-r--r--   0        0        0     6317 2023-07-20 03:47:32.000000 eugene_tools-0.1.1/eugene/plot/_regression.py
+-rw-r--r--   0        0        0    21089 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_seq.py
+-rw-r--r--   0        0        0    11244 2023-07-20 03:55:05.000000 eugene_tools-0.1.1/eugene/plot/_summary.py
+-rw-r--r--   0        0        0     4835 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_training.py
+-rw-r--r--   0        0        0     9721 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_utils.py
+-rw-r--r--   0        0        0      231 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/preprocess/__init__.py
+-rw-r--r--   0        0        0    12762 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/preprocess/_seqdata.py
+-rw-r--r--   0        0        0      850 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/preprocess/_utils.py
+-rw-r--r--   0        0        0      322 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/train/__init__.py
+-rw-r--r--   0        0        0    10310 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/train/_fit.py
+-rw-r--r--   0        0        0    13397 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/train/_hyperopt.py
+-rw-r--r--   0        0        0       30 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/utils/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/utils/_utils.py
+-rw-r--r--   0        0        0     1301 2023-07-20 19:30:12.000000 eugene_tools-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 eugene_tools-0.1.1/PKG-INFO
```

### Comparing `eugene_tools-0.1.0/LICENSE` & `eugene_tools-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/__init__.py` & `eugene_tools-0.1.1/eugene/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from ._settings import settings
 
 try:
     import importlib.metadata as importlib_metadata
 except ModuleNotFoundError:
     import importlib_metadata
 
-package_name = "eugene"
+package_name = "eugene-tools"
 __version__ = importlib_metadata.version(package_name)
 
 # This prevents double output.
 eugene_logger = logging.getLogger("eugene")
 eugene_logger.propagate = False
 
 __all__ = [
```

### Comparing `eugene_tools-0.1.0/eugene/_settings.py` & `eugene_tools-0.1.1/eugene/_settings.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/conftest.py` & `eugene_tools-0.1.1/eugene/conftest.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/evaluate/_evaluate.py` & `eugene_tools-0.1.1/eugene/evaluate/_evaluate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import numpy as np
 from .metrics._multiclass_classification import calculate_auroc, calculate_aupr
 from .metrics._regression import calculate_mse, calculate_pearsonr, calculate_spearmanr
 
 
 def evaluate_model(y_test, pred, task, verbose=True):
-    if (
-        task == "regression"
-    ):  # isinstance(pl_model.criterion, torch.nn.modules.loss.MSELoss):
+    if (task == "regression"):
         mse = calculate_mse(y_test, pred)
         pearsonr = calculate_pearsonr(y_test, pred)
         spearmanr = calculate_spearmanr(y_test, pred)
         if verbose:
             print("Test MSE       : %.4f +/- %.4f" % (np.nanmean(mse), np.nanstd(mse)))
             print(
                 "Test Pearson r : %.4f +/- %.4f"
```

### Comparing `eugene_tools-0.1.0/eugene/evaluate/_utils.py` & `eugene_tools-0.1.1/eugene/evaluate/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/evaluate/metrics/_binary_classification.py` & `eugene_tools-0.1.1/eugene/evaluate/metrics/_binary_classification.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/evaluate/metrics/_multiclass_classification.py` & `eugene_tools-0.1.1/eugene/evaluate/metrics/_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/evaluate/metrics/_profile_prediction.py` & `eugene_tools-0.1.1/eugene/evaluate/metrics/_profile_prediction.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/evaluate/metrics/_regression.py` & `eugene_tools-0.1.1/eugene/evaluate/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/experimental/_AdverserialModule.py` & `eugene_tools-0.1.1/eugene/experimental/_AdverserialModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/experimental/_AugmentModule.py` & `eugene_tools-0.1.1/eugene/experimental/_AugmentModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/experimental/_GenerativeModule.py` & `eugene_tools-0.1.1/eugene/experimental/_GenerativeModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/experimental/_hyperopt_wandb.py` & `eugene_tools-0.1.1/eugene/experimental/_hyperopt_wandb.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/experimental/_language_models.py` & `eugene_tools-0.1.1/eugene/experimental/_language_models.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/experimental/_preprocess.py` & `eugene_tools-0.1.1/eugene/experimental/_preprocess.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/interpret/_generative.py` & `eugene_tools-0.1.1/eugene/interpret/_generative.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,73 @@
 import torch
 from tqdm.auto import tqdm
 from seqexplainer import evolution
 from .._settings import settings
 import xarray as xr
 import numpy as np
 
+from typing import Optional, List, Dict, Any
+
 
 def evolve_seqs_sdata(
     model: torch.nn.Module,
-    sdata,
+    sdata: xr.Dataset,
     rounds: int,
-    seq_key: str = "ohe_seq",
+    seq_var: str = "ohe_seq",
     axis_order=("_sequence", "_ohe", "length"),
     add_seqs=True,
     return_seqs: bool = False,
     device: str = "cpu",
     batch_size: int = 128,
     copy: bool = False,
-    **kwargs,
-):
-    """
-    In silico evolve a set of sequences that are stored in a SeqData object.
+) -> Optional[xr.Dataset]:
+    """In silico evolve a set of sequences that are stored in a SeqData object.
+
+    This function is a wrapper around the `evolution` function from the `seqexplainer`
+    package. It takes a SeqData object containing sequences and evolves them in silico
+    using the specified model. The evolved sequences are stored in the SeqData object
+    as a new variable. The function returns the evolved sequences if `return_seqs` is
+    set to True.
 
     Parameters
     ----------
-    model: torch.nn.Module
+    model : torch.nn.Module
         The model to score the sequences with
-    sdata: SeqData
+    sdata : xr.Dataset
         The SeqData object containing the sequences to evolve
-    rounds: int
+    rounds : int
         The number of rounds of evolution to perform
-    return_seqs: bool, optional
-        Whether to return the evolved sequences
-    device: str, optional
-        Whether to use a 'cpu' or 'cuda'.
-    copy: bool, optional
-        Whether to copy the SeqData object before mutating it
-    kwargs: dict, optional
-        Additional arguments to pass to the evolution function
+    seq_var : str, optional
+        The name of the sequence variable in the SeqData object, by default "ohe_seq"
+    axis_order : tuple, optional
+        The axis order of the sequence variable in the SeqData object, by default ("_sequence", "_ohe", "length")
+    add_seqs : bool, optional
+        Whether to add the evolved sequences to the SeqData object, by default True
+    return_seqs : bool, optional
+        Whether to return the evolved sequences, by default False
+    device : str, optional
+        The device to use for scoring the sequences, by default "cpu"
+    batch_size : int, optional
+        The batch size to use for scoring the sequences, by default 128
+    copy : bool, optional
+        Whether to copy the SeqData object before adding the evolved sequences, by default False
 
     Returns
     -------
-    sdata: SeqData
-        The SeqData object containing the evolved sequences
+    sdata   
+        The SeqData object with the evolved sequences added
     """
 
     sdata = sdata.copy() if copy else sdata
 
     # Set device
     device = "cuda" if settings.gpus > 0 else "cpu" if device is None else device
 
     # Grab seqs
-    ohe_seqs = sdata[seq_key].transpose(*axis_order).to_numpy()
+    ohe_seqs = sdata[seq_var].transpose(*axis_order).to_numpy()
     evolved_seqs = np.zeros(ohe_seqs.shape)
     deltas = np.zeros((sdata.dims["_sequence"], rounds))
 
     # Evolve seqs
     for i, ohe_seq in tqdm(
         enumerate(ohe_seqs), total=len(ohe_seqs), desc="Evolving seqs"
     ):
```

### Comparing `eugene_tools-0.1.0/eugene/models/_SequenceModule.py` & `eugene_tools-0.1.1/eugene/models/base/_module.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,49 @@
-from typing import Callable, Optional, Tuple, Union
-
-import numpy as np
 import torch
-import torch.nn as nn
+import numpy as np
+from tqdm.auto import tqdm
+from typing import Union, Callable, Optional, Tuple
 from pytorch_lightning import seed_everything
 from pytorch_lightning.core import LightningModule
 from pytorch_lightning.utilities.model_summary import ModelSummary
-from tqdm.auto import tqdm
+from base._losses import LOSS_REGISTRY
+from base._optimizers import OPTIMIZER_REGISTRY
+from base._schedulers import SCHEDULER_REGISTRY
+from base._metrics import METRIC_REGISTRY, DEFAULT_TASK_METRICS, DEFAULT_METRIC_KWARGS
 
-from .base._losses import LOSS_REGISTRY
-from .base._metrics import (
-    DEFAULT_METRIC_KWARGS,
-    DEFAULT_TASK_METRICS,
-    METRIC_REGISTRY,
-    calculate_metric,
-)
-from .base._optimizers import OPTIMIZER_REGISTRY
-from .base._schedulers import SCHEDULER_REGISTRY
 
-
-class SequenceModule(LightningModule):
+class BaseModule(LightningModule):
     """
-    Base sequence model class to be inherited by all models in EUGENe
-
-    Parameters:
-    ----------
-    input_len (int):
-        length of input sequence
-    output_dim (int):
-        number of output dimensions
-    task (str):
-        task of the model
-    loss_fxn (str):
-        loss function to use
-    hp_metric (str):
-        metric to use for hyperparameter tuning
-    kwargs (dict):
-        additional arguments to pass to the model
+    TODO: Make this a protocol with expectations for multiple child class modules
     """
 
     def __init__(
         self,
-        arch: torch.nn.Module,
+        model: torch.nn.Module,
         task: str = "regression",
         loss_fxn: Union[str, Callable] = "mse",
         optimizer: str = "adam",
         optimizer_lr: float = 1e-3,
         optimizer_kwargs: dict = {},
         scheduler: str = None,
         scheduler_monitor: str = "val_loss_epoch",
         scheduler_kwargs: dict = {},
         metric: str = None,
         metric_kwargs: dict = None,
         seed: int = None,
         save_hyperparams: bool = True,
-        arch_name: str = None,  # TODO: this should be a class attribute
-        model_name: str = None
+        arch: str = None,  # TODO: this should be a class attribute
+        name: str = None,
     ):
         super().__init__()
 
         # Set the base attributes of a Sequence model
-        self.arch = arch
-        self.input_len = arch.input_len
-        self.output_dim = arch.output_dim
-
-        # Set the task
+        self.input_len = model.input_len
+        self.output_dim = model.output_dim
         self.task = task
-        self.arch_name = (
-            arch_name if arch_name is not None else self.arch.__class__.__name__
-        )
 
         # Set the loss function
         self.loss_fxn = (
             LOSS_REGISTRY[loss_fxn] if isinstance(loss_fxn, str) else loss_fxn
         )
 
         # Set the optimizer
@@ -101,49 +72,50 @@
             self.seed = seed
             seed_everything(self.seed)
         else:
             self.seed = None
 
         # Set the hyperparameters if passed in
         if save_hyperparams:
-            self.save_hyperparameters(ignore=["arch"])
+            self.save_hyperparameters()
+
+        # Set the architecture
+        self.arch = arch if arch is not None else self.model.__class__.__name__
 
-        # Set the model name, if none given make up a fun one
-        self.model_name = model_name if model_name is not None else "model"
+        # Set the model name
+        self.name = name if name is not None else "model"
 
     def forward(self, x) -> torch.Tensor:
         """
-        Forward pass of the arch.
+        Forward pass of the model. This method must be implemented by the child class.
 
         Parameters:
         ----------
         x (torch.Tensor):
             input sequence
         """
-        return self.arch(x)
+        self.model(x)
 
-    def predict(self, x, batch_size=128, verbose=True):
+    def predict(self, x, batch_size=128):
         """
-        Predict the output of the model in batches.
+        Predict the output of the model in batches
         """
         with torch.no_grad():
-            device = self.device
-            self.eval()
+            device = self.model.device
+            self.model.eval()
             if isinstance(x, np.ndarray):
                 x = torch.from_numpy(x.astype(np.float32))
             outs = []
             for _, i in tqdm(
                 enumerate(range(0, len(x), batch_size)),
                 desc="Predicting on batches",
                 total=len(x) // batch_size,
-                disable=not verbose,
             ):
                 batch = x[i : i + batch_size].to(device)
-                out = self(batch).detach().cpu()
-                outs.append(out)
+                outs.append(self.model(batch))
             return torch.cat(outs)
 
     def _common_step(self, batch, batch_idx, stage: str):
         """Common step for training, validation and test
 
         Parameters:
         ----------
@@ -156,70 +128,54 @@
 
         Returns:
         ----------
         dict:
             dictionary of metrics
         """
         # Get and log loss
-        X, y = batch["ohe_seq"], batch["target"]
-        outs = self(X).squeeze()
-        loss = self.loss_fxn(outs, y)  # train
+        X, y = batch["seq"], batch["target"]
+        outs = self.model(X).squeeze(dim=1)
+        loss = self.loss_fxn(outs, y.float())  # train
         return {"loss": loss, "outs": outs.detach(), "y": y.detach()}
 
     def training_step(self, batch, batch_idx):
         """Training step"""
         step_dict = self._common_step(batch, batch_idx, "train")
-        self.log(
-            "train_loss", step_dict["loss"], on_step=True, on_epoch=False, prog_bar=True
-        )
+        self.log("train_loss", step_dict["loss"], on_step=True, on_epoch=False)
         self.log("train_loss_epoch", step_dict["loss"], on_step=False, on_epoch=True)
-        calculate_metric(
-            self.train_metric, self.metric_name, step_dict["outs"], step_dict["y"]
-        )
+        self.train_metric(step_dict["outs"], step_dict["y"])
         self.log(
             f"train_{self.metric_name}_epoch",
             self.train_metric,
             on_step=False,
             on_epoch=True,
         )
         return step_dict
 
     def validation_step(self, batch, batch_idx):
         """Validation step"""
         step_dict = self._common_step(batch, batch_idx, "val")
         self.log("val_loss_epoch", step_dict["loss"], on_step=False, on_epoch=True)
-        calculate_metric(
-            self.val_metric, self.metric_name, step_dict["outs"], step_dict["y"]
-        )
+        self.val_metric(step_dict["outs"], step_dict["y"])
         self.log(
             f"val_{self.metric_name}_epoch",
             self.val_metric,
             on_step=False,
             on_epoch=True,
-            prog_bar=True,
         )
 
     def test_step(self, batch, batch_idx):
         """Test step"""
         step_dict = self._common_step(batch, batch_idx, "test")
         self.log("test_loss", step_dict["loss"], on_step=False, on_epoch=True)
-        calculate_metric(
-            self.test_metric, self.metric_name, step_dict["outs"], step_dict["y"]
-        )
+        self.test_metric(step_dict["outs"], step_dict["y"])
         self.log(
             f"test_{self.metric_name}", self.test_metric, on_step=False, on_epoch=True
         )
 
-    def predict_step(self, batch, batch_idx, dataloader_idx=None):
-        """Predict step"""
-        X, y = batch["ohe_seq"], batch["target"]
-        y = y.detach().cpu().numpy()
-        outs = self(X).squeeze().detach().cpu().numpy()
-        return np.column_stack([outs, y])
-
     def configure_metrics(self, metric, metric_kwargs):
         """Configure metrics
         Keeping this a function allows for the metric to be reconfigured
         in inherited classes
         TODO: add support for multiple metrics
         Returns:
         ----------
@@ -258,15 +214,15 @@
                 "optimizer": optimizer,
                 "lr_scheduler": scheduler,
                 "monitor": self.scheduler_monitor,
             }
 
     def summary(self):
         """Print a summary of the model"""
-        print(f"Model: {self.arch.__class__.__name__}")
+        print(f"Model: {self.model.__class__.__name__}")
         print(f"Sequence length: {self.input_len}")
         print(f"Output dimension: {self.output_dim}")
         print(f"Task: {self.task}")
         print(f"Loss function: {self.loss_fxn.__name__}")
         print(f"Optimizer: {self.optimizer.__name__}")
         print(f"\tOptimizer parameters: {self.optimizer_kwargs}")
         print(f"\tOptimizer starting learning rate: {self.optimizer_lr}")
@@ -274,25 +230,45 @@
             f"Scheduler: {self.scheduler.__name__}"
         ) if self.scheduler is not None else print("Scheduler: None")
         print(f"\tScheduler parameters: {self.scheduler_kwargs}")
         print(f"Metric: {self.metric_name}")
         print(f"\tMetric parameters: {self.metric_kwargs}")
         print(f"Seed: {self.seed}")
         print(f"Parameters summary:")
-        return ModelSummary(self)
+        return ModelSummary(self.model)
 
     @property
-    def arch(self) -> nn.Module:
+    def model(self) -> nn.Module:
         """Model"""
-        return self._arch
+        return self._model
 
-    @arch.setter
-    def arch(self, value: nn.Module):
+    @model.setter
+    def model(self, value: nn.Module):
         """Set model"""
-        self._arch = value
+        self._model = value
+
+    @property
+    def input_len(self) -> int:
+        """Input length"""
+        return self._input_len
+
+    @input_len.setter
+    def input_len(self, value: int):
+        """Set input length"""
+        self._input_len = value
+
+    @property
+    def output_dim(self) -> int:
+        """Output dimension"""
+        return self._output_dim
+
+    @output_dim.setter
+    def output_dim(self, value: int):
+        """Set output dimension"""
+        self._output_dim = value
 
     @property
     def task(self) -> str:
         """Task"""
         return self._task
 
     @task.setter
```

### Comparing `eugene_tools-0.1.0/eugene/models/base/_blocks.py` & `eugene_tools-0.1.1/eugene/models/base/_blocks.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/base/_initializers.py` & `eugene_tools-0.1.1/eugene/models/base/_initializers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import torch
 import torch.nn as nn
 from typing import Dict
 import torch.nn.init as init
 from .._utils import get_layer
 from motifdata import to_kernel
 from motifdata import MotifSet
+from typing import Union, Callable, Optional, Any, Tuple, List, Literal
 
 
 INITIALIZERS_REGISTRY = {
     "uniform": init.uniform_,
     "normal": init.normal_,
     "constant": init.constant_,
     "eye": init.eye_,
@@ -20,15 +21,19 @@
     "orthogonal": init.orthogonal_,
     "sparse": init.sparse_,
     "ones": init.ones_,
     "zeros": init.zeros_,
 }
 
 
-def _init_weights(module, initializer):
+def _init_weights(
+    module: nn.Module,
+    initializer: str = "xavier_uniform",
+    **kwargs,
+) -> None:
     """Initialize the weights of a module.
 
     Parameters
     ----------
     module : torch.nn.Module
         The module to initialize.
     initializer : str, optional
@@ -48,15 +53,19 @@
         init_func(module.weight)
     elif isinstance(module, nn.ParameterList):
         for param in module:
             if param.dim() > 1:
                 init_func(param)
 
 
-def init_weights(model, initializer="kaiming_normal", **kwargs):
+def init_weights(
+    model: nn.Module,
+    initializer: str = "kaiming_normal",
+    **kwargs,
+) -> None:
     """Initialize the weights of a model.
 
     Parameters
     ----------
     model : LightningModule
         The model to initialize.
     initializer : str, optional
@@ -64,41 +73,53 @@
     **kwargs
         Additional arguments to pass to the initializer.
     """
     model.apply(lambda m: _init_weights(m, initializer, **kwargs))
 
 
 def init_motif_weights(
-    model,
-    layer_name,
-    motifs,
-    list_index=None,
-    initializer="kaiming_normal",
-    convert_to_pwm=True,
-    divide_by_bg=False,
-    motif_align="center",
-    kernel_align="center",
+    model: nn.Module,
+    layer_name: str,
+    motifs: MotifSet,
+    list_index: Optional[int] = None,
+    initializer: str = "kaiming_normal",
+    convert_to_pwm: bool = True,
+    divide_by_bg: bool = True,
+    motif_align: Literal["center", "left", "right"] = "center",
+    kernel_align: Literal["center", "left", "right"] = "center",
 ):
     """Initialize the convolutional kernel of choice using a set of motifs
 
     This function is designed to initialize the convolutional kernels of a given layer of a model with a set of motifs.
     It has only been tested on nn.Conv1d layers and ParameterList layers that have a shape of (num_kernels, 4, kernel_size).
     Simply use the named module of the layer you want to initialize and pass it to this function. If the layer is a ParameterList,
     you must also pass the index of the kernel you want to initialize. If the layer is a Conv1d layer, you can pass None as the index.
 
+    This function modifies the model in place.
+
     Parameters
     ----------
     model :
         The model to initialize.
     layer_name : str
         The name of the layer to initialize. You can use the list_available_layers function to get a list of available layers.
     motifs : MotifSet
-        A MotifSet object containing the motifs to initialize the kernel with.
+        A MotifSet object containing the motifs to initialize the kernel with. MotifSets are from the package motifdata.
     list_index : int, optional
         The index of the kernel to initialize. Only required if the layer is a ParameterList layer, by default None
+    initializer : str, optional
+        The name of the initializer to use, by default "kaiming_normal"
+    convert_to_pwm : bool, optional
+        Whether to convert the kernel to a PWM after initializing, by default True
+    divide_by_bg : bool, optional
+        Whether to divide the kernel by the background frequencies after initializing, by default True
+    motif_align : Literal["center", "left", "right"], optional
+        How to align the motifs when converting to a PWM, by default "center"
+    kernel_align : Literal["center", "left", "right"], optional
+        How to align the kernel when converting to a PWM, by default "center"
 
     Returns
     -------
     None
 
     Examples
     --------
```

### Comparing `eugene_tools-0.1.0/eugene/models/base/_layers.py` & `eugene_tools-0.1.1/eugene/models/base/_layers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/base/_losses.py` & `eugene_tools-0.1.1/eugene/models/base/_losses.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/base/_metrics.py` & `eugene_tools-0.1.1/eugene/models/base/_metrics.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,25 +25,29 @@
     "regression": {},
     "binary_classification": {"task": "binary"},
     "multiclass_classification": {"task": "multiclass"},
     "multilabel_classification": {"task": "multilabel"},
 }
 
 
-def calculate_metric(metric, metric_name, outs, y):
+def calculate_metric(metric, metric_name, metric_kwargs, outs, y):
     """Calculate a metric from a metric name and the model outputs and targets.
 
     Args:
         metric (torchmetrics.Metric): The metric to calculate.
         metric_name (str): The name of the metric.
         y (torch.Tensor): The targets.
         outs (torch.Tensor): The model outputs.
 
     Returns:
         float: The calculated metric.
     """
     if metric_name in ["accuracy", "auroc", "f1score", "precision", "recall"]:
         if len(y.shape) > 1:
-            y = torch.argmax(y.squeeze(), dim=1)
+            if "task" in metric_kwargs:
+                if "multilabel" in metric_kwargs["task"]:
+                    y = y.squeeze().long()
+                else:
+                    y = torch.argmax(y.squeeze(), dim=1)
     else:
         outs = outs.squeeze()
-    metric(outs, y)
+    metric(outs, y)
```

### Comparing `eugene_tools-0.1.0/eugene/models/base/_regularizers.py` & `eugene_tools-0.1.1/eugene/models/base/_regularizers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/base/_towers.py` & `eugene_tools-0.1.1/eugene/models/base/_towers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/base/_utils.py` & `eugene_tools-0.1.1/eugene/models/base/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/zoo/_basic_models.py` & `eugene_tools-0.1.1/eugene/models/zoo/_basic_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from ..base import _layers as layers
 from ..base import _blocks as blocks
 from ..base import _towers as towers
+from typing import Union, Callable, Optional, Any, Tuple, List
 
 
 class FCN(nn.Module):
-    """
+    """Basic fully connected network
+
     Instantiate a fully connected neural network with the specified layers and parameters.
 
     By default, this architecture flattens the one-hot encoded sequence and passes
-    it through a set of layers that are fully connected. The task defines how the output is
-    treated (e.g. sigmoid activation for binary classification). The loss function is
-    should be matched to the task (e.g. binary cross entropy ("bce") for binary classification).
+    it through a set of layers that are fully connected.
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    input_dims:
+        The number of input dimensions. This is equivalent to the alphabet length.
     dense_kwargs:
-        The keyword arguments for the fully connected layer.
+        The keyword arguments for the fully connected layer. These come from
+        the models.DenseBlock class. See the documentation for that class for
+        more information on what arguments are available.
     """
 
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         input_dims: int = 4,
@@ -41,45 +43,50 @@
         self.input_dims = input_dims
         self.output_dim = output_dim
         self.dense_kwargs = dense_kwargs
         self.flattened_input_dims = input_len * input_dims
 
         # Create the blocks
         self.dense_block = blocks.DenseBlock(
-            input_dim=self.flattened_input_dims, output_dim=output_dim, **dense_kwargs
+            input_dim=self.flattened_input_dims, 
+            output_dim=output_dim, 
+            **dense_kwargs
         )
 
     def forward(self, x):
         x = x.flatten(start_dim=1)
         x = self.dense_block(x)
         return x
 
 
 class CNN(nn.Module):
-    """
+    """Basic convolutional network
+
     Instantiate a CNN model with a set of convolutional layers and a set of fully
     connected layers.
 
     By default, this architecture passes the one-hot encoded sequence through a set
-    1D convolutions with 4 channels. The task defines how the output is treated (e.g.
-    sigmoid activation for binary classification). The loss function is should be matched
-    to the task (e.g. binary cross entropy ("bce") for binary classification).
+    1D convolutions with 4 channels followed by a set of fully connected layers.
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    conv_kwargs:
+        The keyword arguments for the convolutional layers. These come from the
+        models.Conv1DTower class. See the documentation for that class for more
+        information on what arguments are available.
     dense_kwargs:
         The keyword arguments for the fully connected layer. If not provided, the
         default passes the flattened output of the convolutional layers directly to
-        the output layer.
+        the output layer. These come from the models.DenseBlock class. See the
+        documentation for that class for more information on what arguments are
+        available.
     """
 
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         conv_kwargs: dict,
@@ -89,49 +96,59 @@
 
         # Set the attributes
         self.input_len = input_len
         self.output_dim = output_dim
         self.conv_kwargs = conv_kwargs
 
         # Create the blocks
-        self.conv1d_tower = towers.Conv1DTower(input_len=input_len, **conv_kwargs)
+        self.conv1d_tower = towers.Conv1DTower(
+            input_len=input_len, 
+            **conv_kwargs
+        )
         self.dense_block = blocks.DenseBlock(
             input_dim=self.conv1d_tower.flatten_dim,
             output_dim=output_dim,
             **dense_kwargs
         )
 
     def forward(self, x):
         x = self.conv1d_tower(x)
         x = x.view(x.size(0), self.conv1d_tower.flatten_dim)
         x = self.dense_block(x)
         return x
 
 
 class RNN(nn.Module):
-    """
+    """Basic recurrent network
+
     Instantiate an RNN model with a set of recurrent layers and a set of fully
     connected layers.
 
     By default, this model passes the one-hot encoded sequence through recurrent layers
     and then through a set of fully connected layers. The output of the fully connected
     layers is passed to the output layer.
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    recurrent_kwargs:
+        The keyword arguments for the recurrent layers. These come from the
+        models.RecurrentBlock class. See the documentation for that class for more
+        information on what arguments are available.
+    input_dims:
+        The number of input dimensions. This is equivalent to the alphabet length.
     dense_kwargs:
         The keyword arguments for the fully connected layer. If not provided, the
         default passes the recurrent output of the recurrent layers directly to the
-        output layer.
+        output layer. These come from the models.DenseBlock class. See the
+        documentation for that class for more information on what arguments are
+        available.
     """
 
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         recurrent_kwargs: dict,
@@ -161,32 +178,41 @@
         x, _ = self.recurrent_block(x)
         x = x[:, -1, :]
         x = self.dense_block(x)
         return x
 
 
 class Hybrid(nn.Module):
-    """
+    """Basic hybrid network
+
     A hybrid model that uses both a CNN and an RNN to extract features then passes the
     features through a set of fully connected layers.
 
     By default, the CNN is used to extract features from the input sequence, and the RNN is used to
     to combine those features. The output of the RNN is passed to a set of fully connected
     layers to make the final prediction.
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    conv_kwargs:
+        The keyword arguments for the convolutional layers. These come from the
+        models.Conv1DTower class. See the documentation for that class for more
+        information on what arguments are available.
+    recurrent_kwargs:
+        The keyword arguments for the recurrent layers. These come from the
+        models.RecurrentBlock class. See the documentation for that class for more
+        information on what arguments are available.
     dense_kwargs:
-        The keyword arguments for the fully connected layer.
+        The keyword arguments for the fully connected layer. These come from
+        the models.DenseBlock class. See the documentation for that class for
+        more information on what arguments are available.
     """
 
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         conv_kwargs: dict,
@@ -199,15 +225,18 @@
         self.input_len = input_len
         self.output_dim = output_dim
         self.conv_kwargs = conv_kwargs
         self.recurrent_kwargs = recurrent_kwargs
         self.dense_kwargs = dense_kwargs
 
         # Create the blocks
-        self.conv1d_tower = towers.Conv1DTower(input_len=input_len, **conv_kwargs)
+        self.conv1d_tower = towers.Conv1DTower(
+            input_len=input_len,
+            **conv_kwargs
+        )
         self.recurrent_block = blocks.RecurrentBlock(
             input_dim=self.conv1d_tower.out_channels, **recurrent_kwargs
         )
         self.dense_block = blocks.DenseBlock(
             input_dim=self.recurrent_block.out_channels,
             output_dim=output_dim,
             **dense_kwargs
@@ -220,29 +249,24 @@
         out = self.dense_block(out[:, -1, :])
         return out
 
 
 class TutorialCNN(nn.Module):
     """Tutorial CNN model
 
-    This is a very simple one layer convolutional model for testing purposes. It is featured in testing and tutorial
-    notebooks.
+    This is a very simple one layer convolutional model for testing purposes. It has 4 input channels,
+    a single convolutional layer of width 21 and with 30 output channels, and a single dense layer with
+    30 hidden units. This model is featured in testing and tutorial notebooks.
 
     Parameters
     ----------
     input_len : int
         Length of the input sequence.
     output_dim : int
         Dimension of the output.
-    task : str, optional
-        Task of the model. Either "regression" or "classification".
-    loss_fxn : str, optional
-        Loss function.
-    **kwargs
-        Keyword arguments to pass to the nn.Module class.
     """
 
     def __init__(
         self,
         input_len: int,
         output_dim: int,
     ):
@@ -260,19 +284,46 @@
         x = F.relu(self.conv1(x))
         x = F.max_pool1d(x, x.size()[-1]).flatten(1, -1)
         x = self.dense(x)
         return x
 
 
 class Inception(nn.Module):
+    """Inecption1DConv network
+
+    Instantiate a CNN model with a set of convolutional layers and a set of fully connected layers in
+    the same way as CNN, but the convolutional layers are replaced with InceptionConv1D layers. These layers
+    follow from the 2D inception layers in the original Inception architecture, but have been modified for 1D
+
+    Parameters
+    ----------
+    input_len:
+        The length of the input sequence.
+    output_dim:
+        The dimension of the output.
+    channels:
+        The number of channels in each layer of the InceptionConv1D tower.
+    kernel_size2:
+        The kernel for the first non 1 unit convolution in each layer
+    kernel_size3:
+        The kernel for the second non 1 unit convolution in each layer
+    conv_maxpool_kernel_size:
+        The kernel size for the maxpooling layer in each layer
+    dense_kwargs:
+        The keyword arguments for the fully connected layer. If not provided, the
+        default passes the flattened output of the convolutional layers directly to
+        the output layer. These come from the models.DenseBlock class. See the
+        documentation for that class for more information on what arguments are
+        available.
+    """
     def __init__(
         self,
         input_len: int,
         output_dim: int,
-        channels=[4, 64, 128, 256],
+        channels: List[int] = [4, 32, 64, 128],
         kernel_size2: int = 4,
         kernel_size3: int = 8,
         conv_maxpool_kernel_size: int = 3,
         dense_kwargs: dict = {},
     ):
         super(Inception, self).__init__()
 
@@ -307,32 +358,41 @@
     def forward(self, x):
         x = self.conv_tower(x)
         x = x.view(x.shape[0], -1)
         x = self.dense_block(x)
         return x
 
 class dsFCN(nn.Module):
-    """
+    """Basic FCN model with reverse complement
+
     Instantiate a fully connected neural network with the specified layers and parameters.
     
     By default, this architecture flattens the one-hot encoded sequence and passes 
     it through a set of layers that are fully connected. The task defines how the output is
     treated (e.g. sigmoid activation for binary classification). The loss function is
     should be matched to the task (e.g. binary cross entropy ("bce") for binary classification).
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    input_dims:
+        The number of input dimensions. This is equivalent to the alphabet length.
+    aggr:
+        The method for aggregating the output of the forward pass of the reverse complement.
+        If "concat", the output of the forward pass and the reverse complement pass are
+        concatenated and passed to the dense block. If "max" or "avg", the output of the
+        forward pass and the reverse complement pass are passed to the dense block and
+        the max or average of the two outputs is returned.
     dense_kwargs:
-        The keyword arguments for the fully connected layer.
+        The keyword arguments for the fully connected layer. These come from
+        the models.DenseBlock class. See the documentation for that class for
+        more information on what arguments are available.
     """
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         input_dims: int = 4,
         aggr: str = "concat",
@@ -381,35 +441,46 @@
                 x = torch.max(x, x_rev_comp)
             elif self.aggr == "avg":
                 x = (x + x_rev_comp) / 2
         return x
     
 
 class dsCNN(nn.Module):
-    """
+    """Basic CNN model with reverse complement
+
     Instantiate a CNN model with a set of convolutional layers and a set of fully
     connected layers.
 
     By default, this architecture passes the one-hot encoded sequence through a set
     1D convolutions with 4 channels. The task defines how the output is treated (e.g.
     sigmoid activation for binary classification). The loss function is should be matched
     to the task (e.g. binary cross entropy ("bce") for binary classification).
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    conv_kwargs:
+        The keyword arguments for the convolutional layers. These come from the
+        models.Conv1DTower class. See the documentation for that class for more
+        information on what arguments are available.
+    aggr:
+        The method for aggregating the output of the forward pass of the reverse complement.
+        If "concat", the output of the forward pass and the reverse complement pass are
+        concatenated and passed to the dense block. If "max" or "avg", the output of the
+        forward pass and the reverse complement pass are passed to the dense block and
+        the max or average of the two outputs is returned.
     dense_kwargs:
         The keyword arguments for the fully connected layer. If not provided, the
         default passes the flattened output of the convolutional layers directly to 
-        the output layer.
+        the output layer. These come from the models.DenseBlock class. See the
+        documentation for that class for more information on what arguments are
+        available.
     """
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         conv_kwargs: dict,
         aggr: str = "concat",
@@ -466,30 +537,42 @@
                 x = torch.max(x, x_rev_comp)
             elif self.aggr == "avg":
                 x = (x + x_rev_comp) / 2
         return x
     
 
 class dsRNN(nn.Module):
-    """
+    """Basic RNN model with reverse complement
+
     Instantiate an RNN model with a set of recurrent layers and a set of fully
     connected layers.
 
     By default, this model passes the one-hot encoded sequence through recurrent layers
     and then through a set of fully connected layers. The output of the fully connected
     layers is passed to the output layer.
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    recurrent_kwargs:
+        The keyword arguments for the recurrent layers. These come from the
+        models.RecurrentBlock class. See the documentation for that class for more
+        information on what arguments are available.
+    input_dims:
+        The number of input dimensions. This is equivalent to the alphabet length. You
+        do not need to specify this argument in the recurrent_kwargs dictionary.
+    aggr:
+        The method for aggregating the output of the forward pass of the reverse complement.
+        If "concat", the output of the forward pass and the reverse complement pass are
+        concatenated and passed to the dense block. If "max" or "avg", the output of the
+        forward pass and the reverse complement pass are passed to the dense block and
+        the max or average of the two outputs is returned.
     dense_kwargs:
         The keyword arguments for the fully connected layer. If not provided, the
         default passes the recurrent output of the recurrent layers directly to the
         output layer.
     """
     def __init__(
         self,
@@ -548,30 +631,45 @@
                 x = torch.max(x, x_rev_comp)
             elif self.aggr == "avg":
                 x = (x + x_rev_comp) / 2
         return x
 
 
 class dsHybrid(nn.Module):
-    """
+    """Basic hybrid network with reverse complement
+    
     A hybrid model that uses both a CNN and an RNN to extract features then passes the
     features through a set of fully connected layers.
     
     By default, the CNN is used to extract features from the input sequence, and the RNN is used to 
     to combine those features. The output of the RNN is passed to a set of fully connected
     layers to make the final prediction.
 
     Parameters
     ----------
     input_len:
         The length of the input sequence.
     output_dim:
         The dimension of the output.
-    task:
-        The task of the model.
+    conv_kwargs:
+        The keyword arguments for the convolutional layers. These come from the
+        models.Conv1DTower class. See the documentation for that class for more\
+        information on what arguments are available.
+    recurrent_kwargs:
+        The keyword arguments for the recurrent layers. These come from the
+        models.RecurrentBlock class. See the documentation for that class for more
+        information on what arguments are available.
+    aggr:
+        The method for aggregating the output of the forward pass of the reverse complement.
+        If "concat_cnn", the output of the forward pass and the reverse complement pass are
+        concatenated and passed to the recurrent block. If "concat_rnn", the output of the
+        recurrent block is concatenated with the output of the reverse complement recurrent
+        block and passed to the dense block. If "max" or "avg", the output of the forward
+        pass and the reverse complement pass are passed to the dense block and the max
+        or average of the two outputs is returned.
     dense_kwargs:
         The keyword arguments for the fully connected layer.
     """
     def __init__(
         self,
         input_len: int,
         output_dim: int,
```

### Comparing `eugene_tools-0.1.0/eugene/models/zoo/_cre_activity_predictors.py` & `eugene_tools-0.1.1/eugene/models/zoo/_cre_activity_predictors.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,20 +18,14 @@
 
     Parameters
     ----------
     input_len : int
         Length of the input sequence.
     output_dim : int
         Dimension of the output.
-    strand : str, optional
-        Strand of the input. Only ss is supported for this model
-    task : str, optional
-        Task of the model. Either "regression" or "classification".
-    aggr : str, optional
-        Aggregation method. Does not apply to this model and will be ignored
     filters : int, optional
         Number of filters in the convolutional layers.
     kernel_size : int, optional
         Kernel size of the convolutional layers.
     layers : int, optional
         Number of convolutional layers.
     stride : int, optional
@@ -93,17 +87,36 @@
         x = self.batchnorm(x)
         x = F.relu(x)
         x = self.fc2(x)
         return x
 
 
 class DeepSTARR(nn.Module):
-    """DeepSTARR model from de Almeida et al., 2022; see <https://www.nature.com/articles/s41588-022-01048-5>
+    """DeepSTARR model from de Almeida et al 2022
+
+    This is a flexible implementation of the original DeepSTARR model.
+    If parameters for the CNN and FCN are not passed in, the model
+    will be instantiated with the parameters described in Quang and Xie 2016.
 
     Parameters
+    ----------
+    input_len : int
+        Length of the input sequence.
+    output_dim : int
+        Dimension of the output.
+    conv_kwargs : dict, optional
+        Keyword arguments for the convolutional tower. These come from the
+        models.Conv1DTower class. See the documentation for that class for more
+        information on what arguments are available. If not specified,
+        the default parameters from de Almeida et al 2022 will be used.
+    dense_kwargs : dict, optional
+        Keyword arguments for the dense block. These come from the
+        models.DenseBlock class. See the documentation for that class for more
+        information on what arguments are available. If not specified,
+        the default parameters from de Almeida et al 2022 will be used.
     """
 
     def __init__(
         self, input_len: int, output_dim: int, conv_kwargs={}, dense_kwargs={}
     ):
         super(DeepSTARR, self).__init__()
```

### Comparing `eugene_tools-0.1.0/eugene/models/zoo/_profile_predictors.py` & `eugene_tools-0.1.1/eugene/models/zoo/_profile_predictors.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 from ..base import _layers as layers
 from ..base import _blocks as blocks
 from ..base import _towers as towers
 
 
 class BPNet(nn.Module):
     """
-    This nn.Module was 
+    This nn.Module was taken without permission from a Mr. Schreiber.
+    Just kidding, he made it open source so, ipso facto, I do have permission.
+    Anyway the documentation below is from him, so yell at him if it doesn't
+    work.
 
     A basic BPNet model with stranded profile and total count prediction.
     This is a reference implementation for BPNet. The model takes in
     one-hot encoded sequence, runs it through:
     (1) a single wide convolution operation
     THEN
     (2) a user-defined number of dilated residual convolutions
@@ -34,14 +37,15 @@
     (3) A single log softmax is applied across both strands such that
     the logsumexp of both strands together is 0. Put another way, the
     two strands are concatenated together, a log softmax is applied,
     and the MNLL loss is calculated on the concatenation.
     (4) The count prediction task is predicting the total counts across
     both strands. The counts are then distributed across strands according
     to the single log softmax from 3.
+    
     Parameters
     ----------
     n_filters: int, optional
             The number of filters to use per convolution. Default is 64.
     n_layers: int, optional
             The number of dilated residual layers to include in the model.
             Default is 8.
@@ -117,27 +121,30 @@
         n_count_control = 1 if n_control_tracks > 0 else 0
         self.linear = torch.nn.Linear(
             n_filters + n_count_control, 1, bias=count_output_bias
         )
 
     def forward(self, X, X_ctl=None):
         """A forward pass of the model.
+        
         This method takes in a nucleotide sequence X, a corresponding
         per-position value from a control track, and a per-locus value
         from the control track and makes predictions for the profile
         and for the counts. This per-locus value is usually the
         log(sum(X_ctl_profile)+1) when the control is an experimental
         read track but can also be the output from another model.
+        
         Parameters
         ----------
         X: torch.tensor, shape=(batch_size, 4, sequence_length)
                 The one-hot encoded batch of sequences.
         X_ctl: torch.tensor, shape=(batch_size, n_strands, sequence_length)
                 A value representing the signal of the control at each position in
                 the sequence.
+       
         Returns
         -------
         y_profile: torch.tensor, shape=(batch_size, n_strands, out_length)
                 The output predictions for each strand.
         """
         start, end = self.trimming, X.shape[2] - self.trimming
```

### Comparing `eugene_tools-0.1.0/eugene/models/zoo/_single_cell_predictors.py` & `eugene_tools-0.1.1/eugene/models/zoo/_single_cell_predictors.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/models/zoo/_tf_binding_predictors.py` & `eugene_tools-0.1.1/eugene/models/zoo/_tf_binding_predictors.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,19 +3,16 @@
 import torch.nn.functional as F
 from ..base import _layers as layers
 from ..base import _blocks as blocks
 from ..base import _towers as towers
 
 
 class DeepBind(nn.Module):
-    """
-    DeepBind model implemented from Alipanahi et al 2015 in PyTorch
+    """DeepBind architecture implemented from Alipanahi et al 2015 in PyTorch
 
-    DeepBind is a model that takes in a DNA or RNA sequence and outputs a probability of
-    binding for a given DNA transcription factor or RNA binding protein respectively.
     This is a flexible implementation of the original DeepBind architecture that allows users
     to modify the number of convolutional layers, the number of fully connected layers, and
     many more hyperparameters. If parameters for the CNN and FCN are not passed in, the model
     will be instantiated with the parameters described in Alipanahi et al 2015.
 
     Like the original DeepBind models, this model can be used for both DNA and RNA binding. For DNA,
     we implemented the "dna" mode which only uses the max pooling of the representation generated by
@@ -24,38 +21,27 @@
 
     Parameters
     ----------
     input_len : int
         Length of input sequence
     output_dim : int
         Number of output classes
-    mode : str
-        Mode of model, either "dna" or "rbp"
-    strand : str
-        Strand of model, either "ss", "ds", or "ts"
-    task : str
-        Task of model, either "regression" or "classification"
-    aggr : str
-        Aggregation method of model, either "max" or "avg"
-    loss_fxn : str
-        Loss function of model, either "mse" or "cross_entropy"
-    optimizer : str
-        Optimizer of model, either "adam" or "sgd"
-    lr : float
-        Learning rate of model
-    scheduler : str
-        Scheduler of model, either "lr_scheduler" or "plateau"
-    scheduler_patience : int
-        Scheduler patience of model
-    mp_kwargs : dict
-        Keyword arguments for multiprocessing
     conv_kwargs : dict
-        Keyword arguments for convolutional layers
+        Keyword arguments for convolutional layers. These come from the
+        models.Conv1DTower class. See the documentation for that class for more
+        information on what arguments are available. If not specified,
+        the default parameters from Alipanahi et al 2015 will be used.
     dense_kwargs : dict
-        Keyword arguments for fully connected layers
+        Keyword arguments for fully connected layers. These come from the
+        models.DenseBlock class. See the documentation for that class for more
+        information on what arguments are available. If not specified,
+    mode : str
+        Mode of model, either "dna" or "rbp". Controls the pooling layers.
+        if "dna", only max pooling is used. If "rbp", both max and average
+        pooling are used.
     """
 
     def __init__(
         self,
         input_len: int,
         output_dim: int,
         conv_kwargs: dict = {},
@@ -108,15 +94,86 @@
         dense_kwargs.setdefault("hidden_dims", [32])
         dense_kwargs.setdefault("dropout_rates", 0.25)
         dense_kwargs.setdefault("batchnorm", False)
         return conv_kwargs, dense_kwargs
 
 
 class ResidualBind(nn.Module):
-    # TODO: clean this up
+    """ResidualBind architecture implemented from Koo et al 2021 in PyTorch
+
+    This is a flexible reimplementation of the original ResidualBind architecture
+    that allows users to tweak  hyperparameters. If parameters for the CNN and FCN 
+    are not passed in, the model will be instantiated with the parameters described 
+    in Koo et al 2021.
+
+    Parameters
+    ----------
+    input_len : int
+        Length of input sequence
+    output_dim : int
+        Number of output neurons
+    input_chanels : int, optional
+        Number of input channels, by default 4
+    conv_channels : list, optional
+        Number of channels in the first convolutional layer, by default [96]
+    conv_kernel_size : list, optional
+        Kernel size of the first convolutional layer, by default [11]
+    conv_stride_size : list, optional
+        Stride size of the first convolutional layer, by default [1]
+    conv_dilation_rate : list, optional
+        Dilation rate of the first convolutional layer, by default [1]
+    conv_padding : str, optional
+        Padding of the first convolutional layer, by default "valid"
+    conv_activation : str, optional
+        Activation function of the first convolutional layer, by default "relu"
+    conv_batchnorm : bool, optional
+        Whether to use batchnorm in the first convolutional layer, by default True
+    conv_batchnorm_first : bool, optional
+        Whether to use batchnorm before or after the activation in the first convolutional layer, by default True
+    conv_dropout_rates : float, optional
+        Dropout rate of the first convolutional layer, by default 0.1
+    conv_biases : bool, optional
+        Whether to use biases in the first convolutional layer, by default False
+    residual_channels : list, optional
+        Number of channels in the residual blocks, by default [96, 96, 96]
+    residual_kernel_size : list, optional
+        Kernel size of the residual blocks, by default [3, 3, 3]
+    residual_stride_size : list, optional
+        Stride size of the residual blocks, by default [1, 1, 1]
+    residual_dilation_rate : list, optional
+        Dilation rate of the residual blocks, by default [1, 2, 4]
+    residual_padding : str, optional
+        Padding of the residual blocks, by default "same"
+    residual_activation : str, optional
+        Activation function of the residual blocks, by default "relu"
+    residual_batchnorm : bool, optional
+        Whether to use batchnorm in the residual blocks, by default True
+    residual_batchnorm_first : bool, optional
+        Whether to use batchnorm before or after the activation in the residual blocks, by default True
+    residual_dropout_rates : float, optional
+        Dropout rate of the residual blocks, by default 0.1
+    residual_biases : bool, optional
+        Whether to use biases in the residual blocks, by default False
+    pool_kernel_size : int, optional
+        Kernel size of the average pooling layer, by default 10
+    pool_dropout_rate : float, optional
+        Dropout rate of the average pooling layer, by default 0.2
+    dense_hidden_dims : list, optional
+        Number of neurons in the fully connected layers, by default [256]
+    dense_activation : str, optional
+        Activation function of the fully connected layers, by default "relu"
+    dense_batchnorm : bool, optional
+        Whether to use batchnorm in the fully connected layers, by default True
+    dense_batchnorm_first : bool, optional
+        Whether to use batchnorm before or after the activation in the fully connected layers, by default True
+    dense_dropout_rates : float, optional
+        Dropout rate of the fully connected layers, by default 0.5
+    dense_biases : bool, optional
+        Whether to use biases in the fully connected layers, by default False
+    """
     def __init__(
         self,
         input_len,
         output_dim,
         input_chanels=4,
         conv_channels=[96],
         conv_kernel_size=[11],
@@ -213,31 +270,25 @@
         x = self.dropout(x)
         x = self.flatten(x)
         x = self.dense_block(x)
         return x
 
 
 class Kopp21CNN(nn.Module):
-    """
-    Custom convolutional model used in Kopp et al. 2021 paper
+    """Custom convolutional model used in Kopp et al. 2021 paper
 
     PyTorch implementation of the TensorFlow model described here:
     https://github.com/wkopp/janggu_usecases/tree/master/01_jund_prediction
 
-    This model can only be run in "ds" mode. The reverse complement must be included in the Dataloader
     Parameters
     ----------
     input_len : int
         Length of the input sequence.
     output_dim : int
         Dimension of the output.
-    strand : str, optional
-        Strand of the input. This model is only implemented for "ds"
-    task : str, optional
-        Task for this model. By default "binary_classification" for this mode
     aggr : str, optional
         Aggregation method. Either "concat", "max", or "avg". By default "max" for this model.
     filters : list, optional
         Number of filters in the convolutional layers.
     conv_kernel_size : list, optional
         Kernel size of the convolutional layers.
     maxpool_kernel_size : int, optional
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_catplot.py` & `eugene_tools-0.1.1/eugene/plot/_catplot.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,193 +1,181 @@
 import seaborn as sns
 from .. import settings
 import matplotlib.pyplot as plt
-from typing import Union, Mapping
-from typing import Sequence, Iterable
+from typing import Union, Mapping, Sequence, Iterable, Optional
 from ._utils import _plot_seaborn, _violin_long
+import xarray as xr
 
 
 def countplot(
-    sdata,
-    keys: Union[str, Sequence[str]],
-    groupby: str = None,
+    sdata: xr.Dataset,
+    vars: Union[str, Sequence[str]],
+    groupby: Optional[str] = None,
     orient: str = "h",
     rc_context: Mapping[str, str] = settings.rc_context,
     return_axes: bool = False,
     **kwargs
-) -> None:
+) -> Optional[plt.Axes]:
     """
-    Plots a countplot of a column(s) in seqs_annot using Seaborn.
+    Plots a countplot of a vars in a SeqData using Seaborn.
 
     This function can be used to show the counts of observations in a single
     or multiple columns of seqs_annot within a SeqData. If a groupby is
     provided then the counts are grouped by the groupby column.
 
     Parameters
     ----------
     sdata : SeqData
-        SeqData object that contains keys in seqs_annot.
-    keys : str or list of str
-        Keys to plot. Will be plotted in separate adjacent subplots.
+        SeqData object that contains vars in seqs_annot.
+    vars : str or list of str
+        vars to plot. Will be plotted in separate adjacent subplots.
     groupby : str
         Key to group by. If None, will plot counts of each key.
     orient : str
         Orientation of plot. Either "h" (horizontal) or "v" (vertical).
     rc_context : Mapping[str, str]
         Matplotlib rc context. Default is eugene.settings.rc_context.
     return_axes : bool
         Return axes.
     **kwargs
         Additional keyword arguments to pass to seaborn.
-
-    Returns
-    -------
-        None
     """
-    keys = [keys] if isinstance(keys, str) else keys
+    vars = [vars] if isinstance(vars, str) else vars
     if groupby is None:
-        sdata_df = sdata[keys].to_dataframe()
+        sdata_df = sdata[vars].to_dataframe().reset_index()
     else:
-        sdata_df = sdata[keys + [groupby]].to_dataframe()
+        sdata_df = sdata[vars + [groupby]].to_dataframe()
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
-            sdata_df, keys, func=sns.countplot, groupby=groupby, orient=orient, **kwargs
+            sdata_df, vars, func=sns.countplot, groupby=groupby, orient=orient, **kwargs
         )
     if return_axes:
         return ax
 
 
 def histplot(
-    sdata,
-    keys: Union[str, Sequence[str]],
+    sdata: xr.Dataset,
+    vars: Union[str, Sequence[str]],
     orient: str = "v",
     rc_context: Mapping[str, str] = settings.rc_context,
     return_axes: bool = False,
     **kwargs
-) -> None:
+) -> Optional[plt.Axes]:
     """
-    Plots a histogram of a column(s) in seqs_annot using seaborn.
+    Plots a histogram of a vars in a SeqData using seaborn.
 
     This function can be used to show the distribution of a single or multiple
     columns of seqs_annot within a SeqData. If a groupby is provided then the
     distribution is grouped by the groupby column.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    keys : str or list of str
-        Keys to plot.
+    vars : str or list of str
+        vars to plot.
     groupby : str
         Key to group by.
     orient : str
         Orientation of plot.
     rc_context : Mapping[str, str]
         Matplotlib rc context.
     return_axes : bool
         Return axes.
     **kwargs
         Additional keyword arguments to pass to seaborn.
-
-    Returns
-    -------
-        None
     """
-    sdata_df = sdata[keys].to_dataframe()
+    sdata_df = sdata[vars].to_dataframe()
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
-            sdata_df, keys, func=sns.histplot, orient=orient, ylab="Frequency", **kwargs
+            sdata_df, vars, func=sns.histplot, orient=orient, ylab="Frequency", **kwargs
         )
     if return_axes:
         return ax
 
 
 def boxplot(
-    sdata,
-    keys: Union[str, Sequence[str]],
-    groupby: str = None,
+    sdata: xr.Dataset,
+    vars: Union[str, Sequence[str]],
+    groupby: Optional[str] = None,
     orient: str = "v",
     jitter=False,
     rc_context: Mapping[str, str] = settings.rc_context,
     return_axes: bool = False,
     **kwargs
-) -> None:
+) -> Optional[plt.Axes]:
     """
-    Plots a boxplot of a column(s) in seqs_annot using Seaborn.
+    Plots a boxplot of a vars in a SeqData using Seaborn.
 
     This function can be used to show the distribution of a single or multiple
     columns of seqs_annot within a SeqData. If a groupby is provided then the
     distribution is grouped by the groupby column.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    keys : str or list of str
-        Keys to plot.
+    vars : str or list of str
+        vars to plot.
     groupby : str
         Key to group by.
     orient : str
         Orientation of plot.
     rc_context : Mapping[str, str]
         Matplotlib rc context.
     return_axes : bool
         Return axes.
     **kwargs
         Additional keyword arguments to pass to seaborn.
-
-    Returns
-    -------
-        None
     """
-    keys = [keys] if isinstance(keys, str) else keys
+    vars = [vars] if isinstance(vars, str) else vars
     if groupby is None:
-        sdata_df = sdata[keys].to_dataframe()
+        sdata_df = sdata[vars].to_dataframe()
     else:
-        sdata_df = sdata[keys + [groupby]].to_dataframe()
+        sdata_df = sdata[vars + [groupby]].to_dataframe()
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
-            sdata_df, keys, func=sns.boxplot, groupby=groupby, orient=orient, **kwargs
+            sdata_df, vars, func=sns.boxplot, groupby=groupby, orient=orient, **kwargs
         )
-        if jitter == True:
+        if jitter is True:
             _plot_seaborn(
                 sdata_df,
-                keys,
+                vars,
                 func=sns.stripplot,
                 groupby=groupby,
                 orient=orient,
                 ax=ax,
                 **kwargs
             )
     if return_axes:
         return ax
 
 
 def violinplot(
-    sdata,
-    keys: Union[str, Sequence[str]] = None,
-    groupby: str = None,
+    sdata: xr.Dataset,
+    vars: Optional[Union[str, Sequence[str]]] = None,
+    groupby: Optional[str] = None,
     orient: str = "v",
     rc_context: Mapping[str, str] = settings.rc_context,
     return_axes: bool = False,
     **kwargs
-) -> None:
+) -> Optional[plt.Axes]:
     """
-    Plots a violinplot of a column(s) in seqs_annot using Seaborn.
+    Plots a violinplot of a vars in a SeqData using Seaborn.
 
     This function can be used to show the distribution of a single or multiple
     columns of seqs_annot within a SeqData as a violin plot. If a groupby is provided
     then the distribution is grouped by the groupby column.
 
     Parameters
-     ----------
+    ----------
      sdata : SeqData
          SeqData object.
-     keys : str or list of str
-         Keys to plot.
+     vars : str or list of str
+         vars to plot.
      groupby : str
          Key to group by.
      orient : str
          Orientation of plot.
      rc_context : Mapping[str, str]
          Matplotlib rc context. Uses settings by default.
      return_axes : bool
@@ -195,45 +183,45 @@
      **kwargs
          Additional keyword arguments to pass to seaborn.
 
      Returns
      -------
          None
     """
-    keys = [keys] if isinstance(keys, str) else keys
+    vars = [vars] if isinstance(vars, str) else vars
     if groupby is None:
-        sdata_df = sdata[keys].to_dataframe()
-    elif groupby is not None and isinstance(groupby, Iterable) and keys is None:
+        sdata_df = sdata[vars].to_dataframe()
+    elif groupby is not None and isinstance(groupby, Iterable) and vars is None:
         sdata_df = sdata[groupby].to_dataframe()
     else:
-        sdata_df = sdata[keys + [groupby]].to_dataframe()
+        sdata_df = sdata[vars + [groupby]].to_dataframe()
     with plt.rc_context(rc_context):
-        if groupby is not None and isinstance(groupby, Iterable) and keys is None:
+        if groupby is not None and isinstance(groupby, Iterable) and vars is None:
             ax = _violin_long(sdata_df, groupby, **kwargs)
         else:
             ax = _plot_seaborn(
                 sdata_df,
-                keys,
+                vars,
                 func=sns.violinplot,
                 groupby=groupby,
                 orient=orient,
                 **kwargs
             )
     if return_axes:
         return ax
 
 
 def scatterplot(
     sdata,
     x: str,
     y: str,
-    seq_idx: Sequence[int] = None,
+    seq_idx: Optional[Sequence[int]] = None,
     return_axes: bool = False,
     **kwargs
-) -> None:
+) -> Optional[plt.Axes]:
     """
     Plots a scatterplot of two columns in seqs_annot using Seaborn.
 
     This function can be used to show the relationship between two columns of
     seqs_annot within a SeqData. If seq_idx is provided then only the sequences
     with the given indices are plotted.
 
@@ -251,14 +239,14 @@
         Additional keyword arguments to pass to _plot_seaborn.
     Returns
     -------
     None
     """
     if seq_idx is not None:
         sdata = sdata[seq_idx]
-    keys = [keys] if isinstance(keys, str) else keys
-    sdata_df = sdata[keys].to_dataframe()
+    vars = [x, y]
+    sdata_df = sdata[vars].to_dataframe()
     ax = _plot_seaborn(
-        sdata_df, keys=x, func=sns.scatterplot, groupby=y, xlab=x, ylab=y, **kwargs
+        sdata_df, vars=x, func=sns.scatterplot, groupby=y, xlab=x, ylab=y, **kwargs
     )
     if return_axes:
         return ax
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_classification.py` & `eugene_tools-0.1.1/eugene/plot/_classification.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,27 +9,28 @@
     auc,
     precision_recall_curve,
     average_precision_score,
 )
 from typing import Union, Sequence
 from sklearn.preprocessing import binarize
 from ._utils import _check_input, _label_plot, _save_fig
-
+from typing import Optional
+import xarray as xr
 
 def _plot_binary_confusion_mtx(
-    sdata,
-    target_key: str,
-    prediction_key: str,
+    sdata: xr.Dataset,
+    target_var: str,
+    prediction_var: str,
     threshold: float,
-    title: str = None,
-    xlab: str = None,
-    ylab: str = None,
+    title: Optional[str] = None,
+    xlab: Optional[str] = None,
+    ylab: Optional[str] = None,
     figsize: tuple = (6, 6),
-    save: PathLike = None,
-    ax=None,
+    save: Optional[PathLike] = None,
+    ax: Optional[plt.Axes] = None,
     **kwargs,
 ) -> None:
     """
     Plot a confusion matrix for binary classification.
 
     This function plots a binary confusion matrix as a seaborn heatmap.
     Pulls a target and prediction key from seqs_annot and uses the passed in
@@ -54,16 +55,16 @@
     Returns
     -------
     None
     """
     if ax is None:
         _, ax = plt.subplots(1, 1, figsize=figsize)
     cf_names = ["True Neg", "False Pos", "False Neg", "True Pos"]
-    ts = sdata[target_key].values.reshape(-1, 1)
-    ps = binarize(sdata[prediction_key].values.reshape(-1, 1), threshold=threshold)
+    ts = sdata[target_var].values.reshape(-1, 1)
+    ps = binarize(sdata[prediction_var].values.reshape(-1, 1), threshold=threshold)
     cf_mtx = confusion_matrix(ts, ps)
     cf_pcts = [
         "{0:.2%}".format(value)
         for value in (cf_mtx / cf_mtx.sum(axis=1)[:, None]).flatten()
     ]
     labels = [
         f"{v1}\n{v2}\n{v3}" for v1, v2, v3 in zip(cf_mtx.flatten(), cf_pcts, cf_names)
@@ -81,17 +82,17 @@
     plt.tight_layout()
     if save:
         _save_fig(save)
     return ax
 
 
 def confusion_mtx(
-    sdata,
-    target_key: str,
-    prediction_key: str,
+    sdata: xr.Dataset,
+    target_var: str,
+    prediction_var: str,
     kind: str = "binary",
     threshold: float = 0.5,
     rc_context: dict = settings.rc_context,
     return_axes: bool = False,
     **kwargs,
 ) -> None:
     """
@@ -100,17 +101,17 @@
     Creates a confusion matrix from the given target and prediction keys held
     in the seqs_annot of the passed in SeqData. The
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    target_key : str
+    target_var : str
         Key to use as target.
-    prediction_key : str
+    prediction_var : str
         Key to use as prediction.
     kind : str
         Kind of confusion matrix to plot. Currently only allow for binary
     threshold : float
         Threshold to use to generate a binary confusion matrix.
     rc_context : Mapping[str, str]
         Matplotlib rc context. Defaults to eugene.settings.rc_context.
@@ -120,33 +121,37 @@
     Returns
     -------
         None
     """
     with plt.rc_context(rc_context):
         if kind == "binary":
             ax = _plot_binary_confusion_mtx(
-                sdata, target_key, prediction_key, threshold, **kwargs
+                sdata=sdata,
+                target_var=target_var,
+                prediction_var=prediction_var,
+                threshold=threshold,
+                **kwargs
             )
         else:
             raise ValueError(
                 f"Confusion matrix for '{kind}' classification not currently supported."
             )
     if return_axes:
         return ax
 
 
 def auroc(
-    sdata,
-    target_keys: Union[Sequence[str], str],
-    prediction_keys: Union[Sequence[str], str],
+    sdata: xr.Dataset,
+    target_vars: Union[Sequence[str], str],
+    prediction_vars: Union[Sequence[str], str],
     labels: Union[Sequence[str], str] = "",
     xlab: str = "False Positive Rate",
     ylab: str = "True Positive Rate",
     figsize: tuple = (8, 8),
-    save: str = None,
+    save: Optional[str] = None,
     ax=None,
     **kwargs,
 ) -> None:
     """
     Plot the area under the receiver operating characteristic curve for one or more predictions against
     a one or more targets.
 
@@ -154,39 +159,39 @@
     You must pass in the same number of target keys as prediction keys. If you want to compare the same target
     against multiple predictions, pass in the same target key for each predictions key.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    target_keys : Union[Sequence[str], str]
+    target_vars : Union[Sequence[str], str]
         Target keys to use for plotting.
-    prediction_keys : Union[Sequence[str], str]
+    prediction_vars : Union[Sequence[str], str]
         Prediction keys to use for plotting.
     labels : Union[Sequence[str], str]
         Labels to use for each prediction. If not passed in, the labels_{i} will be used.
     xlab : str
         Label for the x-axis.
     ylab : str
         Label for the y-axis.
     figsize : tuple
         Size of the figure.
     save : str
         Path to save the figure. If none, figure will not be saved.
     **kwargs
         Additional keyword arguments to pass to matplotlib plot function
     """
-    target_keys, prediction_keys, labels = _check_input(
-        sdata, target_keys, prediction_keys, labels
+    target_vars, prediction_vars, labels = _check_input(
+        sdata, target_vars, prediction_vars, labels
     )
     if ax is None:
         _, ax = plt.subplots(1, 1, figsize=figsize)
-    for label, target_key, prediction_key in zip(labels, target_keys, prediction_keys):
-        ts = sdata[target_key].values.reshape(-1, 1)
-        ps = sdata[prediction_key].values.reshape(-1, 1)
+    for label, target_var, prediction_var in zip(labels, target_vars, prediction_vars):
+        ts = sdata[target_var].values.reshape(-1, 1)
+        ps = sdata[prediction_var].values.reshape(-1, 1)
         fpr, tpr, _ = roc_curve(ts, ps)
         roc_auc = auc(fpr, tpr)
         print(roc_auc, label)
         ax.plot(fpr, tpr, label=f"{label} (AUC = {roc_auc:.3f})", **kwargs)
         ax.plot([0, 1], [0, 1], "k--")
         ax.set_xlabel(xlab, fontsize=20)
         ax.set_ylabel(ylab, fontsize=20)
@@ -194,61 +199,61 @@
         plt.tight_layout()
     if save:
         _save_fig(save)
     return ax
 
 
 def auprc(
-    sdata,
-    target_keys: Union[Sequence[str], str],
-    prediction_keys: Union[Sequence[str], str],
+    sdata: xr.Dataset,
+    target_vars: Union[Sequence[str], str],
+    prediction_vars: Union[Sequence[str], str],
     labels: Union[Sequence[str], str] = "",
     xlab: str = "Recall",
     ylab: str = "Precision",
     figsize: tuple = (8, 8),
-    save: str = None,
-    ax=None,
+    save: Optional[str] = None,
+    ax: Optional[plt.Axes] = None,
     **kwargs,
 ) -> None:
     """
     Plot the area under the precision recall curve for one or more predictions against
     a one or more targets.
 
 
     You must pass in the same number of target keys as prediction keys. If you want to compare the same target
     against multiple predictions, pass in the same target key for each predictions key.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    target_keys : Union[Sequence[str], str]
+    target_vars : Union[Sequence[str], str]
         Target keys to use for plotting.
-    prediction_keys : Union[Sequence[str], str]
+    prediction_vars : Union[Sequence[str], str]
         Prediction keys to use for plotting.
     labels : Union[Sequence[str], str]
         Labels to use for each prediction. If not passed in, the labels_{i} will be used.
     xlab : str
         Label for the x-axis.
     ylab : str
         Label for the y-axis.
     figsize : tuple
         Size of the figure.
     save : str
         Path to save the figure. If none, figure will not be saved.
     **kwargs
         Additional keyword arguments to pass to matplotlib plot function
     """
-    target_keys, prediction_keys, labels = _check_input(
-        sdata, target_keys, prediction_keys, labels
+    target_vars, prediction_vars, labels = _check_input(
+        sdata, target_vars, prediction_vars, labels
     )
     _, ax = plt.subplots(1, 1, figsize=figsize)
-    for label, target_key, prediction_key in zip(labels, target_keys, prediction_keys):
-        ts = sdata[target_key].values.reshape(-1, 1)
-        ps = sdata[prediction_key].values.reshape(-1, 1)
+    for label, target_var, prediction_var in zip(labels, target_vars, prediction_vars):
+        ts = sdata[target_var].values.reshape(-1, 1)
+        ps = sdata[prediction_var].values.reshape(-1, 1)
         precision, recall, _ = precision_recall_curve(ts, ps)
         average_precision = average_precision_score(ts, ps)
         ax.plot(
             recall, precision, label=f"{label} (AP = {average_precision:.3f})", **kwargs
         )
         ax.set_xlabel(xlab, fontsize=20)
         ax.set_ylabel(ylab, fontsize=20)
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_dim_reduce.py` & `eugene_tools-0.1.1/eugene/plot/_experimental.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 
 
 def pca(
     sdata,
-    seqsm_key,
+    var,
     pc1=0,
     pc2=1,
     loadings=None,
     labels=None,
     n=5,
     return_axes=False,
     **kwargs
@@ -15,15 +15,15 @@
     """
     Plot the PCA of the data.
 
     Parameters
     ----------
     sdata :
         SeqData The SeqData object.
-    seqsm_key :
+    var :
     str The key of the SeqSM object to use.
     pc1 : int
         The first PC to plot.
     pc2 : int
         The second PC to plot.
     color : str
         The color of the points.
@@ -34,15 +34,15 @@
     n :
         int The number of points to plot.
 
     Returns
     -------
     None
     """
-    pc_data = sdata.seqsm[seqsm_key]
+    pc_data = sdata.seqsm[var]
     xs = pc_data[:, pc1]
     ys = pc_data[:, pc2]
     scalex = 1.0 / (xs.max() - xs.min())
     scaley = 1.0 / (ys.max() - ys.min())
     ax = plt.scatter(xs * scalex, ys * scaley, **kwargs)
     if loadings is not None:
         if n > loadings.shape[0]:
@@ -81,65 +81,65 @@
     plt.ylim(-1, 1)
     plt.xlabel("PC{}".format(1))
     plt.ylabel("PC{}".format(2))
     if return_axes:
         return ax
 
 
-def skree(sdata, uns_key, n_comp=30, return_variance=False):
-    """
-    Function to generate and output a Skree plot using matplotlib barplot
+def skree(sdata, var, n_comp=30, return_variance=False):
+    """Function to generate and output a Skree plot using matplotlib barplot
+    
     Parameters
     ----------
     pca_obj : scikit-learn pca object
     n_comp : number of components to show in the plot
 
     Returns
     -------
 
     """
     variance = {}
-    for i, val in enumerate(sdata.uns[uns_key].explained_variance_ratio_.tolist()):
+    for i, val in enumerate(sdata[var].explained_variance_ratio_.tolist()):
         key = "PC" + str(i + 1)
         variance[key] = val * 100
     plt.bar(
         ["PC" + str(i) for i in range(1, n_comp + 1)],
-        sdata.uns[uns_key].explained_variance_ratio_ * 100,
+        sdata[var].explained_variance_ratio_ * 100,
     )
     plt.xticks(rotation=90)
     plt.ylabel("Variance Explained")
     plt.xlabel("Principal Component")
     if return_variance:
         return variance
 
 
-def umap(sdata, seqsm_key, umap1=0, umap2=1, n=5, return_axes=False, **kwargs):
+def umap(sdata, var, umap1=0, umap2=1, n=5, return_axes=False, **kwargs):
     """
     Plot the UMAP of the data.
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object.
-    seqsm_key : str
+    var : str
         The key of the SeqSM object to use.
     umap1 : int
         The first UMAP to plot.
     umap2 : int
         The second UMAP to plot.
     color : str
         The color of the points.
     n : int
         The number of points to plot.
 
     Returns
     -------
     None
     """
-    umap_data = sdata.seqsm[seqsm_key]
+    umap_data = sdata.seqsm[var]
     xs = umap_data[:, umap1]
     ys = umap_data[:, umap2]
     scalex = 1.0 / (xs.max() - xs.min())
     scaley = 1.0 / (ys.max() - ys.min())
     ax = plt.scatter(xs * scalex, ys * scaley, **kwargs)
     plt.xlabel("UMAP{}".format(1))
     plt.ylabel("UMAP{}".format(2))
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_gia.py` & `eugene_tools-0.1.1/eugene/plot/_gia.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,76 +1,100 @@
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from os import PathLike
 from ._utils import _save_fig
 import matplotlib.pyplot as plt
 from matplotlib.lines import Line2D
+from typing import Optional, Union, Sequence, Mapping, List
 
 def positional_gia_plot(
     sdata,
     keys: list,
-    id_key: str = "id",
+    id_var: str = "id",
     xlab: str = "Position",
     ylab: str = "Predicted Score",
-    ylim: tuple = None,
-    save: PathLike = None,
+    ylim: Optional[tuple] = None,
+    save: Optional[PathLike] = None,
     return_axes: bool = False,
 ):
-    """
-    Plot a lineplot for each position of the sequence after implanting a feature.
+    """Plot a lineplot for each position of the sequence after implanting a feature.
 
-    Assumes that the value corresponding to each seqsm_key in the sdata.uns dictionary
+    Assumes that the value corresponding to each seqsm_var in the sdata.uns dictionary
     has the same shape, namely (L, ) where L are the positions where a feature was implanted
     and scores were calculated using a model. Plots the scores as a line plot with a 95% CI
     corresponding to the number of sequences used to make the plot.
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object with sequences and scores to plot
-    seqsm_keys : list
-        The keys in the sdata.uns dictionary that contain the scores to plot
+    id_var : str
+        The name of the variable in sdata.obs to use as the x-axis
     xlab : str
         The x-axis label
     ylab : str
         The y-axis label
     save : PathLike
         The path to save the figure to
     return_axes : bool
         Whether to return the matplotlib axes object
     """
     concat_df = pd.DataFrame()
     for key in keys:
-        df = pd.DataFrame(index=sdata[id_key].values, data=sdata[key].values).melt(
+        df = pd.DataFrame(index=sdata[id_var].values, data=sdata[key].values).melt(
             var_name=xlab, value_name=ylab, ignore_index=False
         )
         df["feature"] = key
         concat_df = pd.concat([concat_df, df])
     concat_df.reset_index(drop=True, inplace=True)
     g = sns.lineplot(data=concat_df, x=xlab, y=ylab, hue="feature")
     if ylim is not None:
         g.set(ylim=ylim)
     if save:
         _save_fig(save)
     if return_axes:
         return g
 
+
 def distance_cooperativity_gia_plot(
-    sdata,
-    results_key="cooperativity",
-    distance_key="distance",
-    col_names=None,
-    cols_to_plot=None,
-    motif_a_name="",
-    motif_b_name="",
-):
-    cooperativity_df = pd.DataFrame(np.median(sdata[results_key], axis=1))
-    cooperativity_df["distance"] = [int(d[1:]) for d in sdata[distance_key].values]
-    cooperativity_df[f"relative_to_{motif_a_name}"] = [d[0] for d in sdata[distance_key].values]
+    sdata: np.ndarray,
+    results_var: str = "cooperativity",
+    distance_var: str = "distance",
+    col_names: Optional[List[str]] = None,
+    cols_to_plot: Optional[List[str]] = None,
+    motif_a_name: str = "",
+    motif_b_name: str = "",
+) -> None:
+    """Plot the median predicted cooperativity as a function of motif pair distance.
+
+    Parameters
+    ----------
+    sdata : np.ndarray
+        The input data array.
+    results_var : str, optional
+        The name of the variable containing the cooperativity results, by default "cooperativity".
+    distance_var : str, optional
+        The name of the variable containing the motif pair distances, by default "distance".
+    col_names : List[str], optional
+        The names of the columns in the input data array, by default None.
+    cols_to_plot : List[str], optional
+        The names of the columns to plot, by default None.
+    motif_a_name : str, optional
+        The name of the first motif, by default "".
+    motif_b_name : str, optional
+        The name of the second motif, by default "".
+
+    Returns
+    -------
+    None
+    """
+    cooperativity_df = pd.DataFrame(np.median(sdata[results_var], axis=1))
+    cooperativity_df["distance"] = [int(d[1:]) for d in sdata[distance_var].values]
+    cooperativity_df[f"relative_to_{motif_a_name}"] = [d[0] for d in sdata[distance_var].values]
     if col_names is not None:
         cooperativity_df.columns = col_names + ["distance", f"relative_to_{motif_a_name}"]
     else:
         col_names = cooperativity_df.columns[:-2]
 
     # Plot the results
     labels = []
@@ -100,8 +124,9 @@
     )
 
     # Set the x-axis label to "Distance from motif B to motif A"
     plt.ylabel("Median predicted cooperativity")
     plt.xlabel("Motif pair distance")
     plt.title(f"{motif_a_name}/{motif_b_name} cooperativity")
 
-    plt.show()
+    plt.show()
+
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_regression.py` & `eugene_tools-0.1.1/eugene/plot/_regression.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,57 @@
+import matplotlib.pyplot as plt
 import numpy as np
 import xarray as xr
 from os import PathLike
-import matplotlib.pyplot as plt
-from typing import Union, Sequence
-from sklearn.metrics import r2_score, mean_squared_error
-from scipy.stats import spearmanr, pearsonr
-from ._utils import _create_matplotlib_axes, _save_fig
+from scipy.stats import pearsonr, spearmanr
+from sklearn.metrics import mean_squared_error, r2_score
+from typing import Optional, Sequence, Union
+
 from .. import settings
+from ._utils import _create_matplotlib_axes, _save_fig
 
 
 def _plot_performance_scatter(
-    sdata,
-    target_key: str,
-    prediction_key: str,
+    sdata: xr.Dataset,
+    target_var: str,
+    prediction_var: str,
     metrics: Union[str, Sequence[str]] = ["r2", "mse", "pearsonr", "spearmanr"],
-    groupby=None,
+    groupby: Optional[str] = None,
     figsize: tuple = (8, 8),
-    save: PathLike = None,
-    ax: bool = None,
+    save: Optional[PathLike] = None,
+    ax: Optional[bool] = None,
     **kwargs,
-) -> None:
-    """
-    Plot a scatter plot of the performance of the model on a subset of the sequences.
+) -> Optional[plt.Axes]:
+    """Plot a scatter plot of the performance of the model on a subset of the sequences.
 
     Classic predicted vs observed scatterplot that will be annotated with r2, mse and spearman correlation.
     If a groupby key is passed, the scatterplot will be colored according to group.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    target_key : str
-        Name of the target_key variable.
-    prediction_key : str
-        Name of the prediction_key variable.
+    target_var : str
+        Name of the target_var variable.
+    prediction_var : str
+        Name of the prediction_var variable.
     metrics : str or list of str
         Metrics to plot. Should be the string name of the metric used in PL
     **kwargs
 
     Returns
     -------
-    None
+    
 
     Note
     ----
     This function uses Matplotlib as opposed to Seaborn.
     """
-    target = sdata[target_key].to_numpy()
-    prediction = sdata[prediction_key].to_numpy()
+    target = sdata[target_var].to_numpy()
+    prediction = sdata[prediction_var].to_numpy()
 
     nan_mask = ~np.isnan(target)
     target = target[nan_mask]
     prediction = prediction[nan_mask]
 
     r2 = r2_score(target, prediction) if "r2" in metrics else None
     mse = mean_squared_error(target, prediction) if "mse" in metrics else None
@@ -62,18 +62,18 @@
     if "c" in kwargs:
         if kwargs["c"] in sdata.data_vars.keys():
             kwargs["c"] = sdata[kwargs["c"]]
     ax = _create_matplotlib_axes(1, subplot_size=figsize) if ax is None else ax
     if groupby is not None:
         i = 0
         print("Group", "R2", "MSE", "Pearsonr", "Spearmanr")
-        seqs_annot = sdata[[groupby, target_key, prediction_key]].to_dataframe()
+        seqs_annot = sdata[[groupby, target_var, prediction_var]].to_dataframe()
         for group, data in seqs_annot.groupby(groupby):
-            target = data[target_key]
-            prediction = data[prediction_key]
+            target = data[target_var]
+            prediction = data[prediction_var]
             group_r2 = r2_score(target, prediction) if "r2" in metrics else None
             group_mse = mean_squared_error(
                 target, prediction if "mse" in metrics else None
             )
             group_pearsr = (
                 pearsonr(target, prediction)[0] if "pearsonr" in metrics else None
             )
@@ -88,16 +88,16 @@
             ax.legend()
     else:
         im = ax.scatter(
             target, prediction, edgecolor="black", linewidth=0.1, s=10, **kwargs
         )
     if "c" in kwargs:
         plt.colorbar(im, location="bottom", label=kwargs["c"].name)
-    ax.set_xlabel(target_key)
-    ax.set_ylabel(prediction_key)
+    ax.set_xlabel(target_var)
+    ax.set_ylabel(prediction_var)
     ax.text(
         1.02, 0.95, f"$R^2$: {r2:.2f}", transform=plt.gca().transAxes, fontsize=16
     ) if r2 is not None else None
     ax.text(
         1.02, 0.90, f"MSE: {mse:.2f}", transform=plt.gca().transAxes, fontsize=16
     ) if mse is not None else None
     ax.text(
@@ -124,58 +124,58 @@
     ax.set_ylim(lims)
     if save is not None:
         _save_fig(save)
     return ax
 
 
 def performance_scatter(
-    sdata,
-    target_keys: Union[str, Sequence[str]],
-    prediction_keys: Union[str, Sequence[str]],
-    seq_idx: Union[Sequence[int], np.ndarray] = None,
+    sdata: xr.Dataset,
+    target_vars: Union[str, Sequence[str]],
+    prediction_vars: Union[str, Sequence[str]],
+    seq_idx: Optional[Union[Sequence[int], np.ndarray]] = None,
     rc_context: dict = settings.rc_context,
     return_axes: bool = False,
     **kwargs,
-) -> None:
-    """
-    Plot a scatter plot of the performance of the model on a subset of the sequences.
+) -> Optional[plt.Axes]:
+    """Plot a scatter plot of the performance of the model on a subset of the sequences.
 
     Classic predicted vs observed scatterplot that will be annotated with r2, mse and spearman correlation.
     If a groupby key is passed, the scatterplot will be colored according to group.
 
     Parameters
     ----------
     sdata : SeqData
         SeqData object.
-    target_key : str
-        Name of the target_key variable.
-    prediction_key : str
-        Name of the prediction_key variable.
+    target_var : str
+        Name of the target_var variable.
+    prediction_var : str
+        Name of the prediction_var variable.
     seq_idx : list of int
         List of indices of sequences to plot.
     **kwargs
 
     Returns
     -------
     None
     """
     if seq_idx is not None:
         sdata = sdata[seq_idx]
-    if isinstance(target_keys, str) and isinstance(prediction_keys, str):
-        target_keys = [target_keys]
-        prediction_keys = [prediction_keys]
-    if type(target_keys) is list and type(prediction_keys) is list:
-        assert len(target_keys) == len(prediction_keys)
+    if isinstance(target_vars, str) and isinstance(prediction_vars, str):
+        target_vars = [target_vars]
+        prediction_vars = [prediction_vars]
+    if type(target_vars) is list and type(prediction_vars) is list:
+        assert len(target_vars) == len(prediction_vars)
     else:
-        target_keys = [target_keys]
-        prediction_keys = [prediction_keys]
+        target_vars = [target_vars]
+        prediction_vars = [prediction_vars]
     with plt.rc_context(rc_context):
-        for target_key, prediction_key in zip(target_keys, prediction_keys):
-            targs = sdata[target_key].values
+        for target_var, prediction_var in zip(target_vars, prediction_vars):
+            targs = sdata[target_var].values
             nan_mask = xr.DataArray(np.isnan(targs), dims=["_sequence"])
             print(f"Dropping {int(nan_mask.sum().values)} sequences with NaN targets.")
             sdata = sdata.where(~nan_mask, drop=True)
             ax = _plot_performance_scatter(
-                sdata, target_key=target_key, prediction_key=prediction_key, **kwargs
+                sdata, target_var=target_var, prediction_var=prediction_var, **kwargs
             )
     if return_axes:
         return ax
+
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_seq.py` & `eugene_tools-0.1.1/eugene/plot/_seq.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import numpy as np
 import pandas as pd
 import seaborn as sns
 import logomaker as lm
 from os import PathLike
 import matplotlib as mpl
-from typing import Union
+from typing import Union, Sequence, Optional, List
 from tqdm.auto import tqdm
 from ._utils import _save_fig
 import matplotlib.pyplot as plt
 from matplotlib.axes import Axes
 from ._utils import _collapse_pos
-
+import xarray as xr
 
 vocab_dict = {"DNA": ["A", "C", "G", "T"], "RNA": ["A", "C", "G", "U"]}
 
 
 def _plot_seq_features(
     ax: Axes,
     seq: str,
     annots: pd.DataFrame,
     additional_annots: list = [],
 ):
-    """
-    Plot sequence features using matplotlib.
+    """Plot sequence features using matplotlib.
 
     This uses basic matplotlib rectangles and lines to plot sequence features
     as blocks. Can be used along with importance scores to give a visual of where the
     a prior known features of a sequence are
 
     Parameters
     ----------
@@ -99,20 +98,19 @@
 
 
 def _plot_seq_logo(
     ax: Axes,
     seq: str,
     attrs: np.ndarray = None,
     highlight: list = [],
-    threshold: float = None,
+    threshold: Optional[float] = None,
     ylab="Importance Score",
     **kwargs,
 ):
-    """
-    Plot sequence logo using plot_weights_given_ax function from viz_sequence
+    """Plot sequence logo using plot_weights_given_ax function from viz_sequence
 
     This allows for the plotting of sequence logos using the viz_sequence package.
 
     Parameters
     ----------
     ax : matplotlib.axes.Axes
         The axes object to plot on
@@ -173,47 +171,45 @@
     ax.set_xlabel("Sequence Position")
     ax.set_ylabel(ylab)
     if threshold is not None:
         ax.hlines(1, len(seq), threshold / 10, color="red")
 
 
 def seq_track_features(
-    sdata,
+    sdata: xr.Dataset,
     seq_id: str,
-    uns_key: str = None,
+    uns_var: Optional[str] = None,
     additional_annotations: list = ["Score", "Strand"],
-    pred_key: str = None,
-    threshold: float = None,
+    pred_var: Optional[str] = None,
+    threshold: Optional[float] = None,
     highlight: list = [],
     cmap=None,
     norm=None,
     return_axes: bool = False,
-    save: str = None,
+    save: Optional[str] = None,
     **kwargs,
 ):
-    """
-    Function to plot tracks from a SeqData object using matplotlib and function
-    from viz_sequence package.
+    """Function to plot tracks from a SeqData object using matplotlib and function from the viz_sequence package.
 
     This function allows users to also add features from the pos_annot attribute,
     which is not currently available with seq_track function.
 
     This also allows users to just plot the sequences with no importance scores, which is
     currently not available with seq_track function.
 
 
     Parameters
     ----------
     sdata : SeqData object
         The SeqData object to plot
     seq_id : str
         The ID of the sequence to plot
-    uns_key : str
+    uns_var : str
         The key in the SeqData.uns dictionary to use to get the nucleotide scores
-    pred_key : str
+    pred_var : str
         The key in the SeqData.seqs_annot
     threshold : float
         The threshold to use to draw a cut-off line
     highlight : list
         A list of positions to highlight in the sequence
     cmap : str
         The name of the colormap to use
@@ -235,15 +231,15 @@
     seq_idx = np.where(sdata.seqs_annot.index == seq_id)[0][0]
     seq = sdata.seqs[seq_idx]
     p_annot = (
         sdata.pos_annot.df[sdata.pos_annot.df["Chromosome"] == seq_id]
         if sdata.pos_annot is not None
         else None
     )
-    attrs = sdata.uns[uns_key][seq_idx] if uns_key in sdata.uns.keys() else None
+    attrs = sdata.uns[uns_var][seq_idx] if uns_var in sdata.uns.keys() else None
 
     # Define subplots
     _, ax = (
         plt.subplots(2, 1, figsize=(12, 4), sharex=True)
         if p_annot is not None
         else plt.subplots(1, 1, figsize=(12, 4))
     )
@@ -270,16 +266,16 @@
             highlight=highlight,
             threshold=threshold,
             **kwargs,
         )
 
     # Add title
     title = seq_id
-    if pred_key is not None:
-        model_pred = sdata.seqs_annot[pred_key].iloc[seq_idx]
+    if pred_var is not None:
+        model_pred = sdata.seqs_annot[pred_var].iloc[seq_idx]
         if cmap is not None:
             color = cmap(norm(model_pred))
         else:
             color = "black"
         title += ": {}".format(str(round(model_pred, 3)))
     else:
         color = "black"
@@ -289,73 +285,71 @@
     if save is not None:
         _save_fig(save)
 
 
 def multiseq_track_features(
     sdata,
     seq_ids: list,
-    attr_keys: str = None,
-    ylabs: list = None,
+    attr_vars: Optional[str] = None,
+    ylabs: Optional[list] = None,
     width=None,
     height=None,
     return_axes: bool = False,
-    save: str = None,
+    save: Optional[str] = None,
     **kwargs,
 ):
-    """
-    Wrapper around seq_track_features function to plot multiple tracks from a SeqData object
-    using matplotlib and viz_sequence. This function allows users to also add features from the
+    """Wrapper around seq_track_features function to plot multiple tracks from a SeqData object
+    
+    Uses matplotlib and viz_sequence. This function allows users to also add features from the
     pos_annot attribute
 
     Parameters
     ----------
     sdata : SeqData object
         The SeqData object to plot
     seq_ids : list
         The IDs of the sequences to plot
-    uns_key : str
+    attr_vars : list
         The key in the SeqData.uns dictionary to use to get the nucleotide scores
-    pred_key : str
-        The key in the SeqData.seqs_annot
-    threshold : float
-        The threshold to use to draw a cut-off line
-    highlight : list
-        A list of positions to highlight in the sequence
-    cmap : str
-        The name of the colormap to use
-    norm : str
-        The name of the normalization to use
+    ylabs : list
+        The y-axis labels to use for each importance score
+    width : int
+        The width of the figure to plot
+    height : int
+        The height of the figure to plot
     return_axes : bool
         Whether to return the axes object
+    save : str
+        The path to save the figure to
     **kwargs : dict
         Additional keyword arguments to pass to vizsequence call
 
     Returns
     -------
     ax : matplotlib.axes.Axes
         The axes object
     """
     if isinstance(seq_ids, str):
         seq_ids = [seq_ids]
-    if isinstance(attr_keys, str):
-        attr_keys = [attr_keys]
-    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(attr_keys)
+    if isinstance(attr_vars, str):
+        attr_vars = [attr_vars]
+    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(attr_vars)
     seq_idx = np.where(sdata.seqs_annot.index.isin(seq_ids))[0]
     seqs = sdata.seqs[seq_idx]
     fig_width = (
         len(seq_ids) * int(len(seqs[0]) / 20) if width is None else width
     )  # make each sequence width proportional to its length and multiply by the number of sequences
     fig_height = (
-        len(attr_keys) * 4 if height is None else height
-    )  # make each sequence height proportional to the number of attr_keys
-    _, ax = plt.subplots(len(attr_keys), len(seq_ids), figsize=(fig_width, fig_height))
-    for i, uns_key in tqdm(enumerate(attr_keys), desc="Importance values", position=0):
+        len(attr_vars) * 4 if height is None else height
+    )  # make each sequence height proportional to the number of attr_vars
+    _, ax = plt.subplots(len(attr_vars), len(seq_ids), figsize=(fig_width, fig_height))
+    for i, uns_var in tqdm(enumerate(attr_vars), desc="Importance values", position=0):
         for j, seq in enumerate(seqs):
             attrs = (
-                sdata.uns[uns_key][seq_idx[j]] if uns_key in sdata.uns.keys() else None
+                sdata.uns[uns_var][seq_idx[j]] if uns_var in sdata.uns.keys() else None
             )
             _plot_seq_logo(
                 ax.flatten()[i * len(seq_ids) + j],
                 seq,
                 attrs=attrs,
                 ylab=ylabs[i],
             )
@@ -367,45 +361,46 @@
     if return_axes:
         return ax
     if save is not None:
         _save_fig(save)
 
 
 def seq_track(
-    sdata,
+    sdata: xr.Dataset,
     seq_id: str,
-    attrs_key: str,
-    id_key="id",
+    attrs_var: str,
+    id_var="id",
     vocab: str = "DNA",
     highlights: list = [],
     highlight_colors: list = ["lavenderblush", "lightcyan", "honeydew"],
     title: str = "",
     ylab: str = "Saliency",
     xlab: str = "Position",
     return_ax: bool = False,
-    save: PathLike = None,
+    save: Optional[PathLike] = None,
     **kwargs,
 ):
-    """
-    Plot a track of the importance scores for a sequence using the logomaker package
+    """Plot a track of the importance scores for a sequence using the logomaker package
 
     This function is a wrapper around the logomaker Logo function. See the logomaker documentation
     for more details on the kwargs that can be passed to this function.
 
     Currently does no allow for features to be plotted (users must do them themselves on returned axes) or
     for sequence only plotting (i.e. importance scores must be passed in through the uns key)
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object to plot the logo for
     seq_id : str
         The ID of the sequence to plot
-    uns_key : str
-        The key in the sdata.uns dictionary that contains the importance scores
+    attrs_var : str
+        The var in the xarray dataset to use to get the importance scores
+    id_var : str
+        The var in the xarray dataset to use to get the sequence ids
     vocab : str
         The vocabulary to use for the sequence
     highlights : list
         A list of positions to highlight in the sequence
     highlight_colors : list
         A list of colors to use for the highlights
     title : str
@@ -422,16 +417,16 @@
     ax : matplotlib.axes._subplots.AxesSubplot
         The matplotlib axes object
     """
     if isinstance(highlights, tuple):
         highlights = [highlights]
     if isinstance(highlight_colors, str):
         highlight_colors = [highlight_colors] * len(highlights)
-    seq_idx = np.where(sdata[id_key].to_numpy() == seq_id)[0]
-    attrs = sdata[attrs_key][seq_idx].squeeze()
+    seq_idx = np.where(sdata[id_var].to_numpy() == seq_id)[0]
+    attrs = sdata[attrs_var][seq_idx].squeeze()
     viz_seq = pd.DataFrame(attrs.T, columns=vocab_dict[vocab])
     viz_seq.index.name = "pos"
     y_max = np.max(viz_seq.values)
     y_min = np.min(viz_seq.values)
     nn_logo = lm.Logo(viz_seq, **kwargs)
 
     # style using Logo methods
@@ -458,43 +453,42 @@
     if save is not None:
         _save_fig(save)
     if return_ax:
         return nn_logo.ax
 
 
 def multiseq_track(
-    sdata,
+    sdata: xr.Dataset,
     seq_ids: list,
-    attrs_keys: str,
-    id_key="id",
-    ylabs: list = None,
-    width: int = None,
-    height: int = None,
+    attrs_vars: Union[str, Sequence[str]],
+    id_var="id",
+    ylabs: Optional[list] = None,
+    width: Optional[int] = None,
+    height: Optional[int] = None,
     return_axes: bool = False,
-    save: str = None,
+    save: Optional[str] = None,
     **kwargs,
 ):
-    """
-    Plot the saliency tracks for multiple sequences across multiple importance scores in one plot.
+    """Plot the saliency tracks for multiple sequences across multiple importance scores in one plot.
 
     Wraps the seq_track function to plot multiple sequences at once across multiple importance scores.
 
     Attempts to make each sequence width proportional to its length and multiply by the number of sequences
     if no width is passed in.
 
-    Attempts to make each sequence height proportional to the number of attr_keys passed in (the number of different
+    Attempts to make each sequence height proportional to the number of attr_vars passed in (the number of different
     importance scores to plot) if no height is passed in.
 
     Parameters
     ----------
-    sdata : SeqData
+    sdata : xr.Dataset
         The SeqData object with sequences and importances to plot a logo for
     seq_ids : list
         The sequence ids to plot
-    attr_keys : list
+    attr_vars : list
         The keys in the sdata.uns dictionary that contain the importance scores to plot
     ylabs : list
         The ylabs to use for each importance score
     width : int
         The width of the figure to plot
     height : int
         The height of the figure to plot
@@ -508,86 +502,89 @@
     Returns
     -------
     axes : list
         The axes objects if return_axes is True
     """
     if isinstance(seq_ids, str):
         seq_ids = [seq_ids]
-    if isinstance(attrs_keys, str):
-        attrs_keys = [attrs_keys]
+    if isinstance(attrs_vars, str):
+        attrs_vars = [attrs_vars]
     if isinstance(ylabs, str):
         ylabs = [ylabs]
-    example_attr = sdata[attrs_keys[0]][0]
+    example_attr = sdata[attrs_vars[0]][0]
     seq_len = example_attr.sizes["length"]
-    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(attrs_keys)
+    ylabs = ylabs if ylabs is not None else ["Importance Score"] * len(attrs_vars)
     fig_width = len(seq_ids) * int(len(seq_len) / 20) if width is None else width
-    fig_height = len(attrs_keys) * 4 if height is None else height
-    _, ax = plt.subplots(len(attrs_keys), len(seq_ids), figsize=(fig_width, fig_height))
-    for i, attrs_key in tqdm(
-        enumerate(attrs_keys),
+    fig_height = len(attrs_vars) * 4 if height is None else height
+    _, ax = plt.subplots(len(attrs_vars), len(seq_ids), figsize=(fig_width, fig_height))
+    for i, attrs_var in tqdm(
+        enumerate(attrs_vars),
         desc="Importance values",
         position=0,
-        total=len(attrs_keys),
+        total=len(attrs_vars),
     ):
         for j, seq_id in enumerate(seq_ids):
             seq_track(
                 sdata,
                 seq_id=seq_id,
-                attrs_key=attrs_key,
-                id_key=id_key,
+                attrs_var=attrs_var,
+                id_var=id_var,
                 ax=ax.flatten()[i * len(seq_ids) + j],
                 ylab=ylabs[i],
                 title=seq_id,
                 save=None,
                 **kwargs,
             )
     plt.tight_layout()
     if save is not None:
         _save_fig(save)
     if return_axes:
         return ax
 
 
 def filter_viz(
-    sdata,
+    sdata: xr.Dataset,
     filter_num: Union[str, int],
-    pfms_key: str,
+    pfms_var: str,
     vocab: str = "DNA",
-    title: str = None,
+    title: Optional[str] = None,
     return_ax: bool = False,
-    save: str = None,
+    save: Optional[str] = None,
     **kwargs,
 ):
-    """
-    Plot the PFM for a single filter in a SeqData object's uns dictionary as a PWM logo
+    """Plot the PFM for a single filter in a SeqData object's uns dictionary as a PWM logo
 
     This function also uses logomaker to generate the PWM and plot it. Check out the logomaker documentation
     for more information on how to style the plot.
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object with sequences and pfms to plot a logo for
     filter_num : str or int
         The filter id to plot
-    uns_key : str
-        The key in the sdata.uns dictionary that contains the pfms to plot
+    pfms_var : str
+        The var in the xarray dataset to use to get the pfms
     vocab : str
         The vocabulary to use for the logo
     title : str
         The title to use for the plot, defaults to the filter id if None
     return_ax : bool
         Whether to return the matplotlib axes object
+    save : str
+        The path to save the figure to
+    **kwargs : dict
+        Additional keyword arguments to pass to the logomaker Logo function
 
     Returns
     -------
     ax : matplotlib.axes.Axes
         The axes object if return_ax is True
     """
-    pfm = sdata[pfms_key][filter_num].squeeze()
+    pfm = sdata[pfms_var][filter_num].squeeze()
     pfm = pd.DataFrame(pfm, columns=vocab_dict[vocab])
     vocab = vocab_dict[vocab]
     pfm.fillna(1, inplace=True)
     info_mat = lm.transform_matrix(
         pfm,
         from_type="counts",
         to_type="information",
@@ -606,45 +603,44 @@
     if save is not None:
         _save_fig(save)
     if return_ax:
         return logo.ax
 
 
 def multifilter_viz(
-    sdata,
+    sdata: xr.Dataset,
     filter_nums: list,
-    pfms_key: str,
-    num_rows: int = None,
-    num_cols: int = None,
-    titles: list = None,
+    pfms_var: str,
+    num_rows: Optional[int] = None,
+    num_cols: Optional[int] = None,
+    titles: Optional[list] = None,
     figsize=(12, 10),
-    save: PathLike = None,
+    save: Optional[PathLike] = None,
     **kwargs,
 ):
-    """
-    Plot multiple filters in a SeqData object's uns dictionary as PWM logos.
+    """Plot multiple filters in a SeqData object's uns dictionary as PWM logos.
 
     This function wraps filter_viz. Getting the figure to look nice it more of an art
     than a science. In experimenting so far, I've found that a 8x4 grid with a (12, 10)
     figure size works well.
 
     Parameters
     ----------
     sdata : SeqData
         The SeqData object with sequences and pfms to plot a logo for
     filter_nums : list
         The filter ids to plot
+    pfms_var : str
+        The var in the xarray dataset to use to get the pfms
     num_rows : int
         The number of rows to use for the figure
     num_cols : int
         The number of columns to use for the figure
-    uns_key : str
+    uns_var : str
         The key in the sdata.uns dictionary that contains the pfms to plot
-    titles : list
-        The titles to use for the plots, defaults to the filter ids if None
     figsize : tuple
         The figure size to use for the plot
     save : PathLike
         The path to save the figure to
 
     Returns
     -------
@@ -655,15 +651,15 @@
     _, ax = plt.subplots(num_rows, num_cols, figsize=figsize)
     for i in range(num_rows):
         for j in range(num_cols):
             filter_num = filter_nums[i * num_cols + j]
             filter_viz(
                 sdata,
                 filter_num=filter_num,
-                pfms_key=pfms_key,
+                pfms_var=pfms_var,
                 ax=ax.flatten()[i * num_cols + j],
                 title=titles[i * num_cols + j] if titles is not None else filter_num,
                 save=None,
                 **kwargs,
             )
 
     plt.tight_layout()
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_summary.py` & `eugene_tools-0.1.1/eugene/plot/_summary.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from os import PathLike
-from typing import Union
+from typing import Union, Sequence, Optional
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 from sklearn.metrics import r2_score, mean_squared_error
 from sklearn.metrics import (
     accuracy_score,
     roc_auc_score,
@@ -11,15 +11,15 @@
     precision_score,
     recall_score,
     f1_score,
 )
 from scipy.stats import spearmanr, pearsonr, kendalltau
 from ._utils import _plot_seaborn, _save_fig
 from .. import settings
-
+import xarray as xr
 
 metric_dict = {
     "r2": r2_score,
     "mse": mean_squared_error,
     "spearman": spearmanr,
     "pearson": pearsonr,
     "kendall": kendalltau,
@@ -30,35 +30,35 @@
     "recall": recall_score,
     "f1": f1_score,
 }
 
 
 def _model_performances_across_groups(
     sdataframe: pd.DataFrame,
-    target_key: str,
-    prediction_keys: list = None,
-    prediction_groups: list = None,
-    groupby: str = None,
+    target_var: str,
+    prediction_vars: Optional[list] = None,
+    prediction_groups: Optional[list] = None,
+    groupby: Optional[str] = None,
     metrics: str = "r2",
     clf_thresh: float = 0,
     **kwargs
 ):
     """
     Calculate model performance for a metric or set of metrics across groups.
 
     Compares a target column to a set of prediction column in sdataframe
     and calculates the performance of the model for each group in groupby.
 
     Parameters
     ----------
     sdataframe : pd.DataFrame
-        A dataframe containing the target and prediction columns in target_key and prediction_keys respectively.
-    target_key : str
+        A dataframe containing the target and prediction columns in target_var and prediction_vars respectively.
+    target_var : str
         The name of the column in sdataframe containing the target values.
-    prediction_keys : list, optional
+    prediction_vars : list, optional
         A list of the names of the columns in sdataframe containing the prediction values.
         If None, all columns containing "predictions" in their name will be used.
     prediction_groups : list, optional
         A list of the names of the groups for each prediction column.
     groupby : str, optional
         The name of the column in sdataframe to group by. If None, the prediction_groups will be used.
     metrics : str, optional
@@ -70,24 +70,24 @@
     Returns
     -------
     pd.DataFrame
         A dataframe containing the calculated metrics for each group.
     """
     if isinstance(metrics, str):
         metrics = [metrics]
-    prediction_keys = (
+    prediction_vars = (
         sdataframe.columns[sdataframe.columns.str.contains("predictions")]
-        if prediction_keys is None
-        else prediction_keys
+        if prediction_vars is None
+        else prediction_vars
     )
     conc = pd.DataFrame()
     for group, data in sdataframe.groupby(groupby):
-        predicts = data[prediction_keys]
+        predicts = data[prediction_vars]
         bin_predicts = (predicts >= clf_thresh).astype(int)
-        true = data[target_key]
+        true = data[target_var]
         scores = pd.DataFrame()
         for metric in metrics:
             func = metric_dict[metric]
             if metric in ["r2", "mse"]:
                 scores = pd.concat(
                     [
                         scores,
@@ -132,32 +132,32 @@
             scores["prediction_groups"] = prediction_groups
         conc = pd.concat([conc, scores])
     return conc
 
 
 def _model_performances(
     sdataframe: pd.DataFrame,
-    target_key: str,
-    prediction_keys: list = None,
-    prediction_groups: list = None,
+    target_var: str,
+    prediction_vars: Optional[list] = None,
+    prediction_groups: Optional[list] = None,
     metrics: str = "r2",
     clf_thresh: float = 0,
 ):
     """
     Calculate model performance for a metric or set of metrics.
 
     Uses columns from a passed in dataframe to calcuate a set of metrics.
 
     Parameters
     ----------
     sdataframe : pd.DataFrame
-        A dataframe containing the target and prediction columns in target_key and prediction_keys respectively.
-    target_key : str
+        A dataframe containing the target and prediction columns in target_var and prediction_vars respectively.
+    target_var : str
         The name of the column in sdataframe containing the target values.
-    prediction_keys : list, optional
+    prediction_vars : list, optional
         A list of the names of the columns in sdataframe containing the prediction values.
         If None, all columns containing "predictions" in their name will be used.
     prediction_groups : list, optional
         A list of the names of the groups for each prediction column.
     groupby : str, optional
         The name of the column in sdataframe to group by. If None, the prediction_groups will be used.
     metrics : str, optional
@@ -167,16 +167,16 @@
     Returns
     -------
     pd.DataFrame
         A dataframe containing the calculated metrics.
     """
     if isinstance(metrics, str):
         metrics = [metrics]
-    true = sdataframe[target_key]
-    predicts = sdataframe[prediction_keys]
+    true = sdataframe[target_var]
+    predicts = sdataframe[prediction_vars]
     bin_predicts = (predicts >= clf_thresh).astype(int)
     scores = pd.DataFrame()
     for metric in metrics:
         func = metric_dict[metric]
         if metric in ["r2", "mse"]:
             scores = pd.concat(
                 [
@@ -220,39 +220,39 @@
     if prediction_groups is not None:
         scores["prediction_groups"] = prediction_groups
     return scores
 
 
 def performance_summary(
     sdata,
-    target_key: str,
-    prediction_keys: list = None,
-    prediction_groups: list = None,
-    groupby: str = None,
+    target_var: str,
+    prediction_vars: Optional[list] = None,
+    prediction_groups: Optional[list] = None,
+    groupby: Optional[str] = None,
     add_swarm: bool = False,
     size: int = 5,
     metrics: Union[str, list] = "r2",
     orient: str = "v",
     rc_context=settings.rc_context,
     return_axes: bool = False,
-    save: PathLike = None,
+    save: Optional[PathLike] = None,
     **kwargs
 ):
     """
     Plot a performance summary across model predictions for a passed in metric
 
     Uses model predictions and targets to calculate a set of metrics and plot them.
 
     Parameters
     ----------
     sdata : pd.DataFrame
-        A dataframe containing the target and prediction columns in target_key and prediction_keys respectively.
-    target_key : str
+        A dataframe containing the target and prediction columns in target_var and prediction_vars respectively.
+    target_var : str
         The name of the column in sdataframe containing the target values.
-    prediction_keys : list, optional
+    prediction_vars : list, optional
         A list of the names of the columns in sdataframe containing the prediction values.
         If None, all columns containing "predictions" in their name will be used.
     prediction_groups : list, optional
         A list of the names of the groups for each prediction column.
     groupby : str, optional
         The name of the column in sdataframe to group by. If None, the prediction_groups will be used.
     add_swarm : bool, optional
@@ -272,43 +272,43 @@
     **kwargs
         Additional keyword arguments to pass to sns.violinplot.
 
     Returns
     -------
     ax : matplotlib.axes.Axes
     """
-    prediction_keys = prediction_keys = (
-        [k for k in sdata.keys() if "preds" in k]
-        if prediction_keys is None
-        else prediction_keys
+    prediction_vars = prediction_vars = (
+        [k for k in sdata.vars() if "preds" in k]
+        if prediction_vars is None
+        else prediction_vars
     )
     sdataframe = (
-        sdata[["id"] + [target_key] + prediction_keys].to_dataframe().set_index("id")
+        sdata[["id"] + [target_var] + prediction_vars].to_dataframe().set_index("id")
     )
     if groupby is None:
         scores = _model_performances(
-            sdataframe, target_key, prediction_keys, prediction_groups, metrics
+            sdataframe, target_var, prediction_vars, prediction_groups, metrics
         )
     else:
         scores = _model_performances_across_groups(
-            sdataframe, target_key, prediction_keys, prediction_groups, groupby, metrics
+            sdataframe, target_var, prediction_vars, prediction_groups, groupby, metrics
         )
     with plt.rc_context(rc_context):
         ax = _plot_seaborn(
             scores,
-            keys=metrics,
+            vars=metrics,
             func=sns.boxplot,
             groupby="prediction_groups" if groupby is None else groupby,
             orient=orient,
             **kwargs
         )
         if add_swarm:
             _plot_seaborn(
                 scores,
-                keys=metrics,
+                vars=metrics,
                 func=sns.swarmplot,
                 groupby="prediction_groups" if groupby is None else groupby,
                 orient=orient,
                 size=size,
                 edgecolor="black",
                 linewidth=2,
                 ax=ax,
```

### Comparing `eugene_tools-0.1.0/eugene/plot/_utils.py` & `eugene_tools-0.1.1/eugene/plot/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.0/eugene/preprocess/_seqdata.py` & `eugene_tools-0.1.1/eugene/preprocess/_seqdata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,190 @@
 import os
 import sys
-from typing import Optional
+from typing import Any, Dict, Generic, List, Literal, Optional, Type, Union, cast
 
-bin_dir = os.path.dirname(sys.executable)
-os.environ["PATH"] += os.pathsep + bin_dir
 import dask.array as da
 import dask_ml as dml
 import numpy as np
 import seqpro as sp
 import xarray as xr
 from sklearn.preprocessing import StandardScaler
 
+bin_dir = os.path.dirname(sys.executable)
+os.environ["PATH"] += os.pathsep + bin_dir
+
+alphabets ={
+    "DNA": sp.alphabets.DNA,
+    "RNA": sp.alphabets.RNA,
+}
+
+
+def make_unique_ids_sdata(
+    sdata: xr.Dataset,
+    id_var: str = "id",
+    copy: bool = False,
+) -> Optional[xr.Dataset]:
+    """Make a set of unique ids for each sequence in a SeqData object and store as new xarray variable. 
+
+    Expects that the dimension for the number of sequences is named "_sequence". Otherwise,
+    it will fail. Will also overwrite any existing variable with the same name.
+
+    Parameters
+    ----------
+    sdata : xr.Dataset
+        SeqData object.
+    id_var : str, optional
+        Name of the variable to store the ids in, by default "id"
+    copy : bool, optional
+        Whether to return a copy of the SeqData object, by default False
 
-def make_unique_ids_sdata(sdata, id_var="id", copy=False):
-    """Make unique ids for each sequence in a sdata object."""
+    Returns
+    -------
+    xr.Dataset
+        SeqData object with unique ids. If copy is True, a copy of the SeqData
+        object is returned, else the original SeqData object is modified in place.
+    """
     sdata = sdata.copy() if copy else sdata
     n_digits = len(str(sdata.dims["_sequence"]))
     sdata[id_var] = xr.DataArray(
         [
             "seq{num:0{width}}".format(num=i, width=n_digits)
             for i in range(sdata.dims["_sequence"])
         ],
         dims=["_sequence"],
     )
     return sdata if copy else None
 
 
 def pad_seqs_sdata(
-    sdata, length, seq_key="seq", pad="right", pad_value="N", copy=False
-):
-    """Pad sequences in a SeqData object."""
+    sdata: xr.Dataset,
+    length: int,
+    seq_var: str = "seq", 
+    pad: Literal["left", "both", "right"] = "right",
+    pad_value: Optional[str] = None,
+    copy: bool = False,
+) -> Optional[xr.Dataset]:
+    """Pad sequences in a SeqData object.
+    
+    Wraps the pad_seqs function from SeqPro on the sequences in a SeqData object. Automatically
+    adds a new variable to the SeqData object with the padded sequences called "{seq_var}_padded".
+    Assumes that the dimension for the number of sequences is named "_sequence" and will add dimension
+    called length to the padded sequences. Will also overwrite any existing variable with the same name.
+
+    Parameters
+    ----------
+    sdata : xr.Dataset
+        SeqData object.
+    length : int
+        Length to pad or truncate sequences to.
+    seq_var : str, optional
+        Name of the variable holding the sequences, by default "seq"
+    pad : Literal["left", "both", "right"], optional
+        How to pad. If padding on both sides and an odd amount of padding is needed, 1
+        more pad value will be on the right side, by default "right"
+    pad_val : str, optional
+        Single character to pad sequences with. Needed for string input. Ignored for OHE
+        sequences, by default None
+    copy : bool, optional
+        Whether to return a copy of the SeqData object, by default False
+
+    Returns
+    -------
+    xr.Dataset
+        SeqData object with padded sequences. If copy is True, a copy of the SeqData
+        object is returned, else the original SeqData object is modified in place.
+    """
     sdata = sdata.copy() if copy else sdata
-    padded_seqs = sp.pad_seqs(
-        seqs=sdata["seq"].values, pad=pad, pad_value=pad_value, length=length
-    )
-    sdata[f"{seq_key}_padded"] = xr.DataArray(padded_seqs, dims=["_sequence", "length"])
+    padded_seqs = sp.pad_seqs(seqs=sdata["seq"].values, pad=pad, pad_value=pad_value, length=length)
+    sdata[f"{seq_var}_padded"] = xr.DataArray(padded_seqs, dims=["_sequence", "length"])
     return sdata if copy else None
 
 
 def ohe_seqs_sdata(
-    sdata, alphabet="DNA", seq_key="seq", ohe_key="ohe_seq", fill_value=0, copy=False
-):
+    sdata: xr.Dataset,
+    alphabet: str = "DNA",
+    seq_var: str = "seq",
+    ohe_var: str = "ohe_seq",
+    fill_value: Union[int, float] = 0,
+    copy: bool = False,
+) -> Optional[xr.Dataset]:
+    """One-hot encode sequences in a SeqData object.
+    
+    Wraps the ohe function from SeqPro on the sequences in a SeqData object. Automatically
+    adds a new variable to the SeqData object with the one-hot encoded sequences called "ohe_seq".
+    with dimensions ()"_sequence", "length", "_ohe"). Will also overwrite any existing variable
+    with the same name.
+
+    Parameters
+    ----------
+    sdata : xr.Dataset
+        SeqData object.
+    alphabet : str, optional
+        Alphabet to use for one-hot encoding, by default "DNA"
+    seq_var : str, optional
+        Name of the variable holding the sequences to be encoded, by default "seq"
+    ohe_var : str, optional
+        Name of the variable to store the one-hot encoded sequences in, by default "ohe_seq"
+    fill_value : Union[int, float], optional
+        Value to fill the one-hot encoded sequences with, by default 0
+    copy : bool, optional
+        Whether to return a copy of the SeqData object, by default False
+    
+    Returns
+    -------
+    xr.Dataset
+        SeqData object with one-hot encoded sequences. If copy is True, a copy of the SeqData
+        object is returned, else the original SeqData object is modified in place.
+    """
     sdata = sdata.copy() if copy else sdata
-    ohe_seqs = sp.ohe(sdata[seq_key].values, sp.ALPHABETS[alphabet])
+    ohe_seqs = sp.ohe(sdata[seq_var].values, alphabet=alphabets[alphabet])
     if fill_value != 0:
         ohe_seqs = ohe_seqs.astype(type(fill_value))
-        ohe_seqs[(ohe_seqs == 0).all(-1)] = np.array(
-            np.repeat(fill_value, ohe_seqs.shape[-1]), dtype=type(fill_value)
-        )
-    sdata[ohe_key] = xr.DataArray(ohe_seqs, dims=["_sequence", "length", "_ohe"])
-
+        ohe_seqs[(ohe_seqs == 0).all(-1)] = np.array(np.repeat(fill_value, ohe_seqs.shape[-1]), dtype=type(fill_value))
+    sdata[ohe_var] = xr.DataArray(ohe_seqs, dims=["_sequence", "length", "_ohe"])
     return sdata if copy else None
 
 
 def train_test_chrom_split(
-    sdata: xr.Dataset, test_chroms: list[str], train_key="train_val"
+    sdata: xr.Dataset, 
+    test_chroms: List[str],
+    train_var: str = "train_val",
 ):
     """Add a variable labeling sequences as part of the train or test split based on chromosome.
 
     Parameters
     ----------
     sdata : xr.Dataset
+        SeqData object.
     test_chroms : list[str]
         List of chromosomes to put into test split.
-    train_key : str, optional
+    train_var : str, optional
         Name of the variable holding the labels such that True = train and False = test, by default "train_val"
     """
     train_mask = (~sdata.chrom.isin(test_chroms)).compute()
-    sdata[train_key] = train_mask
+    sdata[train_var] = train_mask
 
 
 def train_test_random_split(
     sdata: xr.Dataset,
     dim: str,
-    train_key="train_val",
-    groups=None,
-    test_size=0.1,
+    train_var: str = "train_val",
+    groups: Optional[Any] = None,
+    test_size: float = 0.1,
     random_state: Optional[int] = None,
 ):
     """Add a variable labeling sequences as part of the train or test split, splitting randomly.
 
     Parameters
     ----------
     sdata : xr.Dataset
+        SeqData object.
     dim : str
         Dimension to split randomly.
-    train_key : str, optional
+    train_var : str, optional
         Name of the variable holding the labels such that True = train and False = test, by default "train_val"
     groups : ArrayLike, optional
         Groups to stratify the splits by, by default None
     test_size : float, optional
         Proportion of data to put in the test set, by default 0.1
     random_state : int, optional
         Random seed, by default None
@@ -98,32 +193,33 @@
         n_splits=1, test_size=test_size, random_state=random_state
     )
     train_idx, test_idx = next(
         splitter.split(da.arange(sdata.sizes[dim]), groups=groups)
     )
     train_mask = np.full(sdata.sizes[dim], False)
     train_mask[train_idx] = True
-    sdata[train_key] = train_mask
+    sdata[train_var] = xr.DataArray(train_mask, dims=[dim])
 
 
 def train_test_homology_split(
     sdata: xr.Dataset,
     seq_var: str,
-    train_key="train_val",
-    test_size=0.1,
-    nucleotide=True,
+    train_var: str = "train_val",
+    test_size: float = 0.1,
+    nucleotide: bool = True,
 ):
     """Add a variable labeling sequences as part of the train or test split, splitting by homology.
 
     Parameters
     ----------
     sdata : xr.Dataset
+        SeqData object.
     seq_var : str
         Variable containing the sequences.
-    train_key : str, optional
+    train_var : str, optional
         Name of the variable holding the labels, by default "train_val"
     test_size : float, optional
         Proportion of data to put in the test set, by default 0.1
     nucleotide : bool, optional
         Whether the input sequences are nucleotides or not, by default True
 
     Raises
@@ -154,119 +250,121 @@
         prefilter=True,
         denominator="shortest",
     )
     train_idx, test_idx = map(np.array, outs)
     train_group = np.full(sdata.sizes[sdata.attrs["sequence_dim"]], "removed")
     train_group[train_idx] = "train"
     train_group[test_idx] = "val"
-    sdata[train_key] = train_group
+    sdata[train_var] = train_group
 
 
 def clamp_targets_sdata(
-    sdata,
-    target_keys: list,
+    sdata: xr.Dataset,
+    target_vars: Union[str, List[str]],
     percentile: float = 0.995,
-    train_key: str = None,
-    clamp_nums: list = None,
-    store_clamp_nums=False,
-    suffix=False,
-    copy=False,
+    train_var: Optional[str] = None,
+    clamp_nums: Optional[List[float]] = None,
+    store_clamp_nums: bool = False,
+    suffix: bool = False,
+    copy: bool = False,
 ):
     """
-    Clamp targets to a given percentile if they are above that percentile in a SeqData object.
+    Clamp targets to a given percentile in a SeqData object.
 
     Parameters
     ----------
-    sdata : SeqData
+    sdata : xr.Dataset
         SeqData object.
-    target_keys : list
-        List of target keys to clamp.
+    target_vars : list
+        List of target variables to clamp.
     percentile : float, optional
         Percentile to clamp to, by default 0.995
-    train_key : str, optional
+    train_var : str, optional
         Key to use if you only want to calculate percentiles on training data, by default None
     clamp_nums : list, optional
         You can provide numbers to clamp to, by default None
     store_clamp_nums : bool, optional
         Whether to store the clamp numbers in the SeqData object, by default False
+    suffix : bool, optional
+        Whether to add a suffix to the variable name, by default False
     copy : bool, optional
         Whether to return a copy of the SeqData object, by default False
 
     Returns
     -------
     SeqData
         SeqData object with clamped targets. If copy is True, a copy of the SeqData
         object is returned, else the original SeqData object is modified in place.
     """
     sdata = sdata.copy() if copy else sdata
-    if type(target_keys) is str:
-        target_keys = [target_keys]
+    if type(target_vars) is str:
+        target_vars = [target_vars]
     if clamp_nums is None:
-        if train_key is not None:
+        if train_var is not None:
             train_idx = np.where(sdata["train_val"])[0]
             clamp_nums = (
-                sdata.isel(_sequence=train_idx)[target_keys]
+                sdata.isel(_sequence=train_idx)[target_vars]
                 .to_pandas()
                 .quantile(percentile)
             )
         else:
-            clamp_nums = sdata[target_keys].to_pandas().quantile(percentile)
+            clamp_nums = sdata[target_vars].to_pandas().quantile(percentile)
     else:
-        assert len(clamp_nums) == len(target_keys)
-    for target_key in target_keys:
+        assert len(clamp_nums) == len(target_vars)
+    for target_var in target_vars:
         if suffix:
-            sdata[f"{target_key}_clamped"] = xr.DataArray(
-                sdata[target_key].to_pandas().clip(upper=clamp_nums[target_key]),
+            sdata[f"{target_var}_clamped"] = xr.DataArray(
+                sdata[target_var].to_pandas().clip(upper=clamp_nums[target_var]),
                 dims=["_sequence"],
             )
         else:
-            sdata[target_key].values = (
-                sdata[target_key].to_pandas().clip(upper=clamp_nums[target_key])
+            sdata[target_var].values = (
+                sdata[target_var].to_pandas().clip(upper=clamp_nums[target_var])
             )
     if store_clamp_nums:
         sdata["clamp_nums"] = xr.DataArray(clamp_nums, dims=["_targets"])
     return sdata if copy else None
 
 
 def scale_targets_sdata(
-    sdata,
-    target_keys,
-    train_key=None,
-    scaler=None,
-    return_scaler=True,
-    suffix=False,
-    copy=False,
+    sdata: xr.Dataset,
+    target_vars: Union[str, List[str]],
+    train_var: Optional[str] = None,
+    scaler: Optional[StandardScaler] = None,
+    return_scaler: bool = False,
+    suffix: bool = False,
+    copy: bool = False,
 ):
     """
     Scale targets in a SeqData object.
     """
     sdata = sdata.copy() if copy else sdata
-    if type(target_keys) is str:
-        target_keys = [target_keys]
-    if train_key is not None:
-        scale_data = sdata.isel(_sequence=np.where(sdata[train_key])[0])[
-            target_keys
+    if type(target_vars) is str:
+        target_vars = [target_vars]
+    if train_var is not None:
+        scale_data = sdata.isel(_sequence=np.where(sdata[train_var])[0])[
+            target_vars
         ].to_pandas()
     else:
-        scale_data = sdata[target_keys].to_pandas()
-    to_scale = sdata[target_keys].to_pandas()
-    if len(target_keys) == 1:
+        scale_data = sdata[target_vars].to_pandas()
+    to_scale = sdata[target_vars].to_pandas()
+    if len(target_vars) == 1:
         scale_data = scale_data.values.reshape(-1, 1)
         to_scale.values.reshape(-1, 1)
     if scaler is None:
         scaler = StandardScaler()
         scaler.fit(scale_data)
-    assert scaler.n_features_in_ == len(target_keys)
+    assert scaler.n_features_in_ == len(target_vars)
     to_scale = scaler.transform(to_scale)
-    for i, target_key in enumerate(target_keys):
+    for i, target_var in enumerate(target_vars):
         if suffix:
-            sdata[f"{target_key}_scaled"] = xr.DataArray(
+            sdata[f"{target_var}_scaled"] = xr.DataArray(
                 to_scale[:, i], dims=["_sequence"]
             )
         else:
-            sdata[target_key].values = to_scale[:, i]
+            sdata[target_var].values = to_scale[:, i]
     if return_scaler and copy:
         return scaler, sdata
     elif return_scaler and not copy:
         return scaler
     else:
         return sdata if copy else None
```

### Comparing `eugene_tools-0.1.0/eugene/train/_fit.py` & `eugene_tools-0.1.1/eugene/train/_fit.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,90 @@
 import os
 from os import PathLike
-from typing import Dict, List, Type, Union
+from typing import Dict, List, Type, Union, Literal, Optional
 
 import seqdata as sd
 import xarray as xr
+from ..models import SequenceModule
 from pytorch_lightning import LightningModule, Trainer, seed_everything
 from pytorch_lightning.callbacks import ModelCheckpoint
 from pytorch_lightning.callbacks.early_stopping import EarlyStopping
 from pytorch_lightning.callbacks.lr_monitor import LearningRateMonitor
 from pytorch_lightning.loggers import CSVLogger, Logger, TensorBoardLogger, WandbLogger
 from torch.utils.data import DataLoader
 
 from eugene import settings
 
-# Note that CSVLogger is currently hanging training with SequenceModule right now
-# Note that if you use wandb logger, it comes with a few extra steps. Show a notebook for this
 LOGGER_REGISTRY: Dict[str, Type[Logger]] = {
     "csv": CSVLogger,
     "tensorboard": TensorBoardLogger,
     "wandb": WandbLogger,
 }
 
 
 def fit(
     model: LightningModule,
     train_dataloader: DataLoader,
     val_dataloader: DataLoader = None,
     epochs: int = 10,
-    gpus: int = None,
+    gpus: Optional[int] = None,
     logger: Union[str, Logger] = "tensorboard",
-    log_dir: PathLike = None,
-    name: str = None,
-    version: str = None,
+    log_dir: Optional[PathLike] = None,
+    name: Optional[str] = None,
+    version: Optional[str] = None,
     early_stopping_metric: str = "val_loss_epoch",
-    early_stopping_patience=5,
-    early_stopping_verbose=False,
-    model_checkpoint_k=1,
+    early_stopping_patience: int = 5,
+    early_stopping_verbose: bool = False,
+    model_checkpoint_k: int = 1,
     model_checkpoint_monitor: str = "val_loss_epoch",
-    seed: int = None,
+    seed: Optional[int] = None,
     return_trainer: bool = False,
     **kwargs,
-):
+) -> Optional[Trainer]:
+    """Fit a model using PyTorch Lightning.
+
+    This is a generic fit function that can be used to train any PyTorch LightninngModule. All that's
+    required is a LightningModule, a training dataloader, and optionally a validation dataloader.
+
+    Parameters
+    ----------
+    model : LightningModule
+        The model to train.
+    train_dataloader : DataLoader
+        The training dataloader to use.
+    val_dataloader : DataLoader
+        The validation dataloader to use.
+    epochs : int
+        The number of epochs to train for.
+    gpus : int
+        The number of gpus to use. EUGENe will automatically use all available gpus if available.
+    logger : str or Logger
+        The logger to use. If a string, must be one of "csv", "tensorboard", or "wandb".
+    log_dir : PathLike
+        The directory to save the logs to.
+    name : str
+        The name of the experiment. Appended to the end of the log directory
+    version : str
+        The version of the experiment. Appended to the end of the log directory/name
+    early_stopping_metric : str
+        The metric to use for early stopping.
+    early_stopping_patience : int
+        The number of epochs to wait before stopping.
+    early_stopping_verbose : bool
+        Whether to print early stopping messages.
+    seed : int
+        The seed to use for reproducibility.
+    kwargs : dict
+        Additional varword arguments to pass to the PL Trainer.
+
+    Returns
+    -------
+    trainer : Trainer
+        The PyTorch Lightning Trainer object.
+    """
     # Set-up a seed
     seed_everything(seed, workers=True) if seed is not None else print("No seed set")
 
     # Logger
     logger = LOGGER_REGISTRY[logger](save_dir=log_dir, name=name, version=version)
 
     # Set-up callbacks
@@ -83,138 +123,142 @@
     trainer.fit(
         model, train_dataloaders=train_dataloader, val_dataloaders=val_dataloader
     )
     if return_trainer:
         return trainer
 
 
-# Have a couple of fit methods that are meant to take in a SeqData and call the above function
 def fit_sequence_module(
-    model: LightningModule,
-    sdata: "xr.Dataset",
-    seq_key: str = None,
-    target_keys: Union[str, List[str]] = None,
+    model: SequenceModule,
+    sdata: xr.Dataset,
+    seq_var: Optional[str] = None,
+    target_vars: Optional[Union[str, List[str]]] = None,
     in_memory: bool = False,
-    train_key: str = "train_val",
+    train_var: str = "train_val",
     epochs: int = 10,
-    gpus: int = None,
-    batch_size: int = None,
-    num_workers: int = None,
+    gpus: Optional[int] = None,
+    batch_size: Optional[int] = None,
+    num_workers: Optional[int] = None,
     prefetch_factor: int = None,
-    transforms=None,
-    drop_last=True,
+    transforms: Optional[Dict] = None,
+    drop_last: bool = False,
     logger: str = "tensorboard",
-    log_dir: PathLike = None,
-    name: str = None,
-    version: str = None,
+    log_dir: Optional[PathLike] = None,
+    name: Optional[str] = None,
+    version: Optional[str] = None,
     early_stopping_metric: str = "val_loss_epoch",
-    early_stopping_patience=5,
-    early_stopping_verbose=False,
-    model_checkpoint_k=1,
+    early_stopping_patience: int = 5,
+    early_stopping_verbose: bool = False,
+    model_checkpoint_k: int = 1,
     model_checkpoint_monitor: str = "val_loss_epoch",
-    seed: int = None,
+    seed: Optional[int] = None,
     return_trainer: bool = False,
     **kwargs,
-):
+) -> Optional[Trainer]:
     """
-    Train the model using PyTorch Lightning.
+    Fit a SequenceModule using PyTorch Lightning. This function is a wrapper around the fit function, but builds
+    the dataloaders from a SeqData object.
 
     Parameters
     ----------
-    model : BaseModel
+    model : 
         The model to train.
     sdata : SeqData
         The SeqData object to train on.
-    target_keys : str or list of str
-        The target keys in sdata's seqs_annot attribute to train on.
-    train_key : str
-        The key in sdata's seqs_annot attribute to split into train and validation set
+    target_vars : str or list of str
+        The target vars in sdata to use aas labels for training
+    in_memory : bool
+        Whether to load the data into memory before training. Default is False.
+    train_var : str
+        The var in sdata to use to split into train and validation set
     epochs : int
         The number of epochs to train for.
     gpus : int
         The number of gpus to use. EUGENe will automatically use all available gpus if available.
     batch_size : int
         The batch size to use.
     num_workers : int
         The number of workers to use for the dataloader.
+    prefetch_factor : int
+        The prefetch factor to use for the dataloader.
+    transforms : dict
+        The transforms to apply to the data. This should be a dictionary of the form
+        {"var": transform function to apply}. See the documentation for SeqData for more
+        information.
+    drop_last : bool
+        Whether to drop the last batch if it is smaller than the batch size.
+    logger : str or Logger
+        The logger to use. If a string, must be one of "csv", "tensorboard", or "wandb".
     log_dir : PathLike
         The directory to save the logs to.
     name : str
         The name of the experiment.
     version : str
         The version of the experiment.
-    train_dataset :Dataset
-        The training dataset to use. If None, will be created from sdata.
-    val_dataset :Dataset
-        The validation dataset to use. If None, will be created from sdata.
-    train_dataloader : DataLoader
-        The training dataloader to use. If None, will be created from train_dataset.
-    val_dataloader : DataLoader
-        The validation dataloader to use. If None, will be created from val_dataset.
-    transforms : list of str
-        The sequence transforms to apply to the data.
-    transform_kwargs : dict
-        The keyword arguments to pass to the sequence transforms.
     early_stopping_metric : str
         The metric to use for early stopping.
     early_stopping_patience : int
         The number of epochs to wait before stopping.
     early_stopping_verbose : bool
         Whether to print early stopping messages.
+    model_checkpoint_k : int
+        The number of models to save.
+    model_checkpoint_monitor : str
+        The metric to use for model checkpointing.
     seed : int
         The seed to use for reproducibility.
-    verbosity : int
-        The verbosity level.
+    return_trainer : bool
+        Whether to return the trainer object.
     kwargs : dict
-        Additional keyword arguments to pass to the PL Trainer.
+        Additional varword arguments to pass to the PL Trainer.
 
     Returns
     -------
     trainer : Trainer
         The PyTorch Lightning Trainer object.
     """
 
     # Set-up dataloaders
     batch_size = batch_size if batch_size is not None else settings.batch_size
     num_workers = num_workers if num_workers is not None else settings.dl_num_workers
-    if target_keys is not None:
-        if isinstance(target_keys, str):
-            target_keys = [target_keys]
-        if len(target_keys) == 1:
-            sdata["target"] = sdata[target_keys[0]]
+    if target_vars is not None:
+        if isinstance(target_vars, str):
+            target_vars = [target_vars]
+        if len(target_vars) == 1:
+            sdata["target"] = sdata[target_vars[0]]
         else:
             sdata["target"] = xr.concat(
-                [sdata[target_key] for target_key in target_keys], dim="_targets"
+                [sdata[target_var] for target_var in target_vars], dim="_targets"
             ).transpose("_sequence", "_targets")
         nan_mask = sdata['target'].isnull()
         if sdata["target"].ndim > 1:
             nan_mask = nan_mask.any('_targets')
         print(f"Dropping {nan_mask.sum().compute().item()} sequences with NaN targets.")
     if in_memory:
-        print(f"Loading {seq_key} and {target_keys} into memory")
-        sdata[seq_key].load()
+        print(f"Loading {seq_var} and {target_vars} into memory")
+        sdata[seq_var].load()
         sdata["target"].load()
-    sdata[train_key].load()
-    train_sdata = sdata.sel(_sequence=(sdata[train_key] == True).compute())  # noqa
-    val_sdata = sdata.sel(_sequence=(sdata[train_key] == False).compute())  # noqa
+    sdata[train_var].load()
+    train_sdata = sdata.sel(_sequence=(sdata[train_var] == True).compute())  # noqa
+    val_sdata = sdata.sel(_sequence=(sdata[train_var] == False).compute())  # noqa
     train_dataloader = sd.get_torch_dataloader(
         train_sdata,
         sample_dims=["_sequence"],
-        variables=[seq_key, "target"],
+        variables=[seq_var, "target"],
         batch_size=batch_size,
         num_workers=num_workers,
         prefetch_factor=prefetch_factor,
         transforms=transforms,
         shuffle=True,
         drop_last=drop_last,
     )
     val_dataloader = sd.get_torch_dataloader(
         val_sdata,
         sample_dims=["_sequence"],
-        variables=[seq_key, "target"],
+        variables=[seq_var, "target"],
         batch_size=batch_size,
         num_workers=num_workers,
         prefetch_factor=prefetch_factor,
         transforms=transforms,
         shuffle=False,
         drop_last=drop_last,
     )
```

