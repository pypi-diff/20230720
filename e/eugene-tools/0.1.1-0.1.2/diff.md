# Comparing `tmp/eugene_tools-0.1.1.tar.gz` & `tmp/eugene_tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eugene_tools-0.1.1.tar", max compression
+gzip compressed data, was "eugene_tools-0.1.2.tar", max compression
```

## Comparing `eugene_tools-0.1.1.tar` & `eugene_tools-0.1.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1066 2023-01-26 02:27:24.000000 eugene_tools-0.1.1/LICENSE
--rw-r--r--   0        0        0     1061 2023-07-20 18:47:35.000000 eugene_tools-0.1.1/README.md
--rw-r--r--   0        0        0      584 2023-07-17 22:54:02.000000 eugene_tools-0.1.1/eugene/__init__.py
--rw-r--r--   0        0        0     6279 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/_settings.py
--rw-r--r--   0        0        0     1455 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/conftest.py
--rw-r--r--   0        0        0       73 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/dataload/__init__.py
--rw-r--r--   0        0        0     2709 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/dataload/_augment.py
--rw-r--r--   0        0        0     2263 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/dataload/_utils.py
--rw-r--r--   0        0        0      258 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/__init__.py
--rw-r--r--   0        0        0     1179 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/_evaluate.py
--rw-r--r--   0        0        0    13118 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/_predict.py
--rw-r--r--   0        0        0      991 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/_utils.py
--rw-r--r--   0        0        0        0 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/__init__.py
--rw-r--r--   0        0        0     2741 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_binary_classification.py
--rw-r--r--   0        0        0      541 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_multiclass_classification.py
--rw-r--r--   0        0        0    13629 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_profile_prediction.py
--rw-r--r--   0        0        0      745 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/evaluate/metrics/_regression.py
--rw-r--r--   0        0        0     3049 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_AdverserialModule.py
--rw-r--r--   0        0        0     8244 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_AugmentModule.py
--rw-r--r--   0        0        0     7013 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_GenerativeModule.py
--rw-r--r--   0        0        0        0 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_LanguageModule.py
--rw-r--r--   0        0        0     1204 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_hyperopt_wandb.py
--rw-r--r--   0        0        0     7154 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_language_models.py
--rw-r--r--   0        0        0     1905 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/experimental/_preprocess.py
--rw-r--r--   0        0        0      218 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/__init__.py
--rw-r--r--   0        0        0     4089 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/_attribute.py
--rw-r--r--   0        0        0     8720 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/_filters.py
--rw-r--r--   0        0        0     3703 2023-07-17 21:15:23.000000 eugene_tools-0.1.1/eugene/interpret/_generative.py
--rw-r--r--   0        0        0     6549 2023-07-20 03:46:53.000000 eugene_tools-0.1.1/eugene/interpret/_gia.py
--rw-r--r--   0        0        0    10508 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/_ProfileModule.py
--rw-r--r--   0        0        0    14478 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/_SequenceModule.py
--rw-r--r--   0        0        0      346 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/__init__.py
--rw-r--r--   0        0        0     2043 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/_utils.py
--rw-r--r--   0        0        0        0 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/__init__.py
--rw-r--r--   0        0        0     8986 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_blocks.py
--rw-r--r--   0        0        0     5621 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_initializers.py
--rw-r--r--   0        0        0    11661 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_layers.py
--rw-r--r--   0        0        0     3654 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_losses.py
--rw-r--r--   0        0        0     1827 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_metrics.py
--rw-r--r--   0        0        0    10447 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_module.py
--rw-r--r--   0        0        0       83 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_optimizers.py
--rw-r--r--   0        0        0     3311 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_regularizers.py
--rw-r--r--   0        0        0      121 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_schedulers.py
--rw-r--r--   0        0        0    12485 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_towers.py
--rw-r--r--   0        0        0     1731 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/base/_utils.py
--rw-r--r--   0        0        0      347 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/zoo/__init__.py
--rw-r--r--   0        0        0    27146 2023-07-18 15:50:10.000000 eugene_tools-0.1.1/eugene/models/zoo/_basic_models.py
--rw-r--r--   0        0        0     5615 2023-07-18 15:51:03.000000 eugene_tools-0.1.1/eugene/models/zoo/_cre_activity_predictors.py
--rw-r--r--   0        0        0     6596 2023-07-18 15:51:35.000000 eugene_tools-0.1.1/eugene/models/zoo/_profile_predictors.py
--rw-r--r--   0        0        0    18311 2023-07-18 15:54:07.000000 eugene_tools-0.1.1/eugene/models/zoo/_regulatory_classifiers.py
--rw-r--r--   0        0        0     3291 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/models/zoo/_single_cell_predictors.py
--rw-r--r--   0        0        0    13955 2023-07-18 15:56:56.000000 eugene_tools-0.1.1/eugene/models/zoo/_tf_binding_predictors.py
--rw-r--r--   0        0        0      483 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/__init__.py
--rw-r--r--   0        0        0     7410 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_catplot.py
--rw-r--r--   0        0        0     8227 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_classification.py
--rw-r--r--   0        0        0     3545 2023-07-20 03:47:25.000000 eugene_tools-0.1.1/eugene/plot/_experimental.py
--rw-r--r--   0        0        0     4458 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_gia.py
--rw-r--r--   0        0        0     6317 2023-07-20 03:47:32.000000 eugene_tools-0.1.1/eugene/plot/_regression.py
--rw-r--r--   0        0        0    21089 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_seq.py
--rw-r--r--   0        0        0    11244 2023-07-20 03:55:05.000000 eugene_tools-0.1.1/eugene/plot/_summary.py
--rw-r--r--   0        0        0     4835 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_training.py
--rw-r--r--   0        0        0     9721 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/plot/_utils.py
--rw-r--r--   0        0        0      231 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/preprocess/__init__.py
--rw-r--r--   0        0        0    12762 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/preprocess/_seqdata.py
--rw-r--r--   0        0        0      850 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/preprocess/_utils.py
--rw-r--r--   0        0        0      322 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/train/__init__.py
--rw-r--r--   0        0        0    10310 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/train/_fit.py
--rw-r--r--   0        0        0    13397 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/train/_hyperopt.py
--rw-r--r--   0        0        0       30 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/utils/__init__.py
--rw-r--r--   0        0        0      723 2023-07-17 21:15:24.000000 eugene_tools-0.1.1/eugene/utils/_utils.py
--rw-r--r--   0        0        0     1301 2023-07-20 19:30:12.000000 eugene_tools-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 eugene_tools-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-01-26 02:27:24.000000 eugene_tools-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1061 2023-07-20 18:47:35.000000 eugene_tools-0.1.2/README.md
+-rw-r--r--   0        0        0      584 2023-07-17 22:54:02.000000 eugene_tools-0.1.2/eugene/__init__.py
+-rw-r--r--   0        0        0     6279 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/_settings.py
+-rw-r--r--   0        0        0     1455 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/conftest.py
+-rw-r--r--   0        0        0       73 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/dataload/__init__.py
+-rw-r--r--   0        0        0     2709 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/dataload/_augment.py
+-rw-r--r--   0        0        0     2263 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/dataload/_utils.py
+-rw-r--r--   0        0        0      258 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/__init__.py
+-rw-r--r--   0        0        0     1179 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/_evaluate.py
+-rw-r--r--   0        0        0    13118 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/_predict.py
+-rw-r--r--   0        0        0      991 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/metrics/__init__.py
+-rw-r--r--   0        0        0     2741 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/metrics/_binary_classification.py
+-rw-r--r--   0        0        0      541 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/metrics/_multiclass_classification.py
+-rw-r--r--   0        0        0    13629 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/metrics/_profile_prediction.py
+-rw-r--r--   0        0        0      745 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/evaluate/metrics/_regression.py
+-rw-r--r--   0        0        0     3049 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_AdverserialModule.py
+-rw-r--r--   0        0        0     8244 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_AugmentModule.py
+-rw-r--r--   0        0        0     7013 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_GenerativeModule.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_LanguageModule.py
+-rw-r--r--   0        0        0     1204 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_hyperopt_wandb.py
+-rw-r--r--   0        0        0     7154 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_language_models.py
+-rw-r--r--   0        0        0     1905 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/experimental/_preprocess.py
+-rw-r--r--   0        0        0      218 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/interpret/__init__.py
+-rw-r--r--   0        0        0     4089 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/interpret/_attribute.py
+-rw-r--r--   0        0        0     8720 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/interpret/_filters.py
+-rw-r--r--   0        0        0     3703 2023-07-17 21:15:23.000000 eugene_tools-0.1.2/eugene/interpret/_generative.py
+-rw-r--r--   0        0        0     6549 2023-07-20 03:46:53.000000 eugene_tools-0.1.2/eugene/interpret/_gia.py
+-rw-r--r--   0        0        0    10508 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/_ProfileModule.py
+-rw-r--r--   0        0        0    14478 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/_SequenceModule.py
+-rw-r--r--   0        0        0      346 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/__init__.py
+-rw-r--r--   0        0        0     2043 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/_utils.py
+-rw-r--r--   0        0        0        0 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/__init__.py
+-rw-r--r--   0        0        0     8986 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_blocks.py
+-rw-r--r--   0        0        0     5621 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_initializers.py
+-rw-r--r--   0        0        0    11661 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_layers.py
+-rw-r--r--   0        0        0     3654 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_losses.py
+-rw-r--r--   0        0        0     1827 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_metrics.py
+-rw-r--r--   0        0        0    10447 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_module.py
+-rw-r--r--   0        0        0       83 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_optimizers.py
+-rw-r--r--   0        0        0     3311 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_regularizers.py
+-rw-r--r--   0        0        0      121 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_schedulers.py
+-rw-r--r--   0        0        0    12485 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_towers.py
+-rw-r--r--   0        0        0     1731 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/base/_utils.py
+-rw-r--r--   0        0        0      347 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/zoo/__init__.py
+-rw-r--r--   0        0        0    27146 2023-07-18 15:50:10.000000 eugene_tools-0.1.2/eugene/models/zoo/_basic_models.py
+-rw-r--r--   0        0        0     5615 2023-07-18 15:51:03.000000 eugene_tools-0.1.2/eugene/models/zoo/_cre_activity_predictors.py
+-rw-r--r--   0        0        0     6596 2023-07-18 15:51:35.000000 eugene_tools-0.1.2/eugene/models/zoo/_profile_predictors.py
+-rw-r--r--   0        0        0    18311 2023-07-20 19:45:23.000000 eugene_tools-0.1.2/eugene/models/zoo/_regulatory_classifiers.py
+-rw-r--r--   0        0        0     3291 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/models/zoo/_single_cell_predictors.py
+-rw-r--r--   0        0        0    13955 2023-07-18 15:56:56.000000 eugene_tools-0.1.2/eugene/models/zoo/_tf_binding_predictors.py
+-rw-r--r--   0        0        0      483 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/__init__.py
+-rw-r--r--   0        0        0     7410 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/_catplot.py
+-rw-r--r--   0        0        0     8227 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/_classification.py
+-rw-r--r--   0        0        0     3545 2023-07-20 03:47:25.000000 eugene_tools-0.1.2/eugene/plot/_experimental.py
+-rw-r--r--   0        0        0     4458 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/_gia.py
+-rw-r--r--   0        0        0     6317 2023-07-20 03:47:32.000000 eugene_tools-0.1.2/eugene/plot/_regression.py
+-rw-r--r--   0        0        0    21089 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/_seq.py
+-rw-r--r--   0        0        0    11244 2023-07-20 03:55:05.000000 eugene_tools-0.1.2/eugene/plot/_summary.py
+-rw-r--r--   0        0        0     4835 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/_training.py
+-rw-r--r--   0        0        0     9721 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/plot/_utils.py
+-rw-r--r--   0        0        0      231 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/preprocess/__init__.py
+-rw-r--r--   0        0        0    12762 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/preprocess/_seqdata.py
+-rw-r--r--   0        0        0      850 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/preprocess/_utils.py
+-rw-r--r--   0        0        0      322 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/train/__init__.py
+-rw-r--r--   0        0        0    10310 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/train/_fit.py
+-rw-r--r--   0        0        0    13397 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/train/_hyperopt.py
+-rw-r--r--   0        0        0       30 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/utils/__init__.py
+-rw-r--r--   0        0        0      723 2023-07-17 21:15:24.000000 eugene_tools-0.1.2/eugene/utils/_utils.py
+-rw-r--r--   0        0        0     1307 2023-07-20 20:00:00.000000 eugene_tools-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 eugene_tools-0.1.2/PKG-INFO
```

### Comparing `eugene_tools-0.1.1/LICENSE` & `eugene_tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/README.md` & `eugene_tools-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/__init__.py` & `eugene_tools-0.1.2/eugene/__init__.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/_settings.py` & `eugene_tools-0.1.2/eugene/_settings.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/conftest.py` & `eugene_tools-0.1.2/eugene/conftest.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/dataload/_augment.py` & `eugene_tools-0.1.2/eugene/dataload/_augment.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/dataload/_utils.py` & `eugene_tools-0.1.2/eugene/dataload/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/_evaluate.py` & `eugene_tools-0.1.2/eugene/evaluate/_evaluate.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/_predict.py` & `eugene_tools-0.1.2/eugene/evaluate/_predict.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/_utils.py` & `eugene_tools-0.1.2/eugene/evaluate/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/metrics/_binary_classification.py` & `eugene_tools-0.1.2/eugene/evaluate/metrics/_binary_classification.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/metrics/_multiclass_classification.py` & `eugene_tools-0.1.2/eugene/evaluate/metrics/_multiclass_classification.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/metrics/_profile_prediction.py` & `eugene_tools-0.1.2/eugene/evaluate/metrics/_profile_prediction.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/evaluate/metrics/_regression.py` & `eugene_tools-0.1.2/eugene/evaluate/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/experimental/_AdverserialModule.py` & `eugene_tools-0.1.2/eugene/experimental/_AdverserialModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/experimental/_AugmentModule.py` & `eugene_tools-0.1.2/eugene/experimental/_AugmentModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/experimental/_GenerativeModule.py` & `eugene_tools-0.1.2/eugene/experimental/_GenerativeModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/experimental/_hyperopt_wandb.py` & `eugene_tools-0.1.2/eugene/experimental/_hyperopt_wandb.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/experimental/_language_models.py` & `eugene_tools-0.1.2/eugene/experimental/_language_models.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/experimental/_preprocess.py` & `eugene_tools-0.1.2/eugene/experimental/_preprocess.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/interpret/_attribute.py` & `eugene_tools-0.1.2/eugene/interpret/_attribute.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/interpret/_filters.py` & `eugene_tools-0.1.2/eugene/interpret/_filters.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/interpret/_generative.py` & `eugene_tools-0.1.2/eugene/interpret/_generative.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/interpret/_gia.py` & `eugene_tools-0.1.2/eugene/interpret/_gia.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/_ProfileModule.py` & `eugene_tools-0.1.2/eugene/models/_ProfileModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/_SequenceModule.py` & `eugene_tools-0.1.2/eugene/models/_SequenceModule.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/_utils.py` & `eugene_tools-0.1.2/eugene/models/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_blocks.py` & `eugene_tools-0.1.2/eugene/models/base/_blocks.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_initializers.py` & `eugene_tools-0.1.2/eugene/models/base/_initializers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_layers.py` & `eugene_tools-0.1.2/eugene/models/base/_layers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_losses.py` & `eugene_tools-0.1.2/eugene/models/base/_losses.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_metrics.py` & `eugene_tools-0.1.2/eugene/models/base/_metrics.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_module.py` & `eugene_tools-0.1.2/eugene/models/base/_module.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_regularizers.py` & `eugene_tools-0.1.2/eugene/models/base/_regularizers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_towers.py` & `eugene_tools-0.1.2/eugene/models/base/_towers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/base/_utils.py` & `eugene_tools-0.1.2/eugene/models/base/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/zoo/_basic_models.py` & `eugene_tools-0.1.2/eugene/models/zoo/_basic_models.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/zoo/_cre_activity_predictors.py` & `eugene_tools-0.1.2/eugene/models/zoo/_cre_activity_predictors.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/zoo/_profile_predictors.py` & `eugene_tools-0.1.2/eugene/models/zoo/_profile_predictors.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/zoo/_regulatory_classifiers.py` & `eugene_tools-0.1.2/eugene/models/zoo/_regulatory_classifiers.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/zoo/_single_cell_predictors.py` & `eugene_tools-0.1.2/eugene/models/zoo/_single_cell_predictors.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/models/zoo/_tf_binding_predictors.py` & `eugene_tools-0.1.2/eugene/models/zoo/_tf_binding_predictors.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_catplot.py` & `eugene_tools-0.1.2/eugene/plot/_catplot.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_classification.py` & `eugene_tools-0.1.2/eugene/plot/_classification.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_experimental.py` & `eugene_tools-0.1.2/eugene/plot/_experimental.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_gia.py` & `eugene_tools-0.1.2/eugene/plot/_gia.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_regression.py` & `eugene_tools-0.1.2/eugene/plot/_regression.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_seq.py` & `eugene_tools-0.1.2/eugene/plot/_seq.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_summary.py` & `eugene_tools-0.1.2/eugene/plot/_summary.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_training.py` & `eugene_tools-0.1.2/eugene/plot/_training.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/plot/_utils.py` & `eugene_tools-0.1.2/eugene/plot/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/preprocess/_seqdata.py` & `eugene_tools-0.1.2/eugene/preprocess/_seqdata.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/preprocess/_utils.py` & `eugene_tools-0.1.2/eugene/preprocess/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/train/_fit.py` & `eugene_tools-0.1.2/eugene/train/_fit.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/train/_hyperopt.py` & `eugene_tools-0.1.2/eugene/train/_hyperopt.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/eugene/utils/_utils.py` & `eugene_tools-0.1.2/eugene/utils/_utils.py`

 * *Files identical despite different names*

### Comparing `eugene_tools-0.1.1/pyproject.toml` & `eugene_tools-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "eugene-tools"
 packages = [{ include = "eugene"}]
-version = "0.1.1"
+version = "0.1.2"
 description = "Elucidating the Utility of Genomic Elements with Neural Nets"
 authors = ["adamklie <aklie@ucsd.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-seqpro = "0.1.1"
-seqdata = "0.1.1"
-seqexplainer = "0.1.0"
-motifdata = "0.1.0"
-seqdatasets = "0.1.0"
-torch = "^1.12.0"
+seqpro = "^0.1.1"
+seqdata = "^0.1.1"
+seqexplainer = "^0.1.0"
+motifdata = "^0.1.0"
+seqdatasets = "^0.1.0"
+torch = ">=1.12.0"
 pytorch-lightning = "^2.0.0"
 einops = "0.6.1"
 torchinfo = "1.8.0"
 scikit-learn = "1.2.0"
 dask_ml = "2023.3.24"
 tensorboard = "2.11.2"
 matplotlib = "^3.6.2"
```

### Comparing `eugene_tools-0.1.1/PKG-INFO` & `eugene_tools-0.1.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 Metadata-Version: 2.1
 Name: eugene-tools
-Version: 0.1.1
+Version: 0.1.2
 Summary: Elucidating the Utility of Genomic Elements with Neural Nets
 Author: adamklie
 Author-email: aklie@ucsd.edu
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: docs
 Requires-Dist: Sphinx[docs] (>=6.2.1,<7.0.0) ; extra == "docs"
 Requires-Dist: dask_ml (==2023.3.24)
 Requires-Dist: einops (==0.6.1)
 Requires-Dist: graph-part (>=0.1.2,<0.2.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: motifdata (==0.1.0)
+Requires-Dist: motifdata (>=0.1.0,<0.2.0)
 Requires-Dist: myst-parser[docs] (>=2.0.0,<3.0.0) ; extra == "docs"
 Requires-Dist: nbsphinx[docs] (>=0.9.2,<0.10.0) ; extra == "docs"
 Requires-Dist: pandoc[docs] (>=2.3,<3.0) ; extra == "docs"
 Requires-Dist: pytorch-lightning (>=2.0.0,<3.0.0)
 Requires-Dist: scikit-learn (==1.2.0)
 Requires-Dist: seaborn (>=0.12.0,<0.13.0)
-Requires-Dist: seqdata (==0.1.1)
-Requires-Dist: seqdatasets (==0.1.0)
-Requires-Dist: seqexplainer (==0.1.0)
-Requires-Dist: seqpro (==0.1.1)
+Requires-Dist: seqdata (>=0.1.1,<0.2.0)
+Requires-Dist: seqdatasets (>=0.1.0,<0.2.0)
+Requires-Dist: seqexplainer (>=0.1.0,<0.2.0)
+Requires-Dist: seqpro (>=0.1.1,<0.2.0)
 Requires-Dist: sphinx-autobuild[docs] (==2021.3.14) ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.21.1,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.2.2,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinxcontrib-apidoc[docs] (>=0.3.0,<0.4.0) ; extra == "docs"
 Requires-Dist: tensorboard (==2.11.2)
-Requires-Dist: torch (>=1.12.0,<2.0.0)
+Requires-Dist: torch (>=1.12.0)
 Requires-Dist: torchinfo (==1.8.0)
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/eugene-tools.svg)](https://badge.fury.io/py/eugene-tools)
 [![Documentation Status](https://readthedocs.org/projects/eugene-tools/badge/?version=latest)](https://eugene-tools.readthedocs.io/en/latest/?badge=latest)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/eugene-tools)
 ![GitHub stars](https://img.shields.io/github/stars/cartercompbio/EUGENe)
```

