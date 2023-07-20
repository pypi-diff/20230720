# Comparing `tmp/sensai-0.1.9.tar.gz` & `tmp/sensai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sensai-0.1.9.tar", last modified: Wed Jul 20 17:00:17 2022, max compression
+gzip compressed data, was "dist/sensai-0.2.0.tar", last modified: Thu Jul 20 10:01:16 2023, max compression
```

## Comparing `sensai-0.1.9.tar` & `sensai-0.2.0.tar`

### file list

```diff
@@ -1,138 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-20 16:59:54.000000 sensai-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-20 17:00:17.000000 sensai-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3162 2022-07-20 16:59:54.000000 sensai-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-07-20 16:59:56.000000 sensai-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-07-20 16:59:56.000000 sensai-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-20 17:00:17.000000 sensai-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-07-20 16:59:56.000000 sensai-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/
--rw-r--r--   0 runner    (1001) docker     (121)     1026 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4521 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/catboost.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/clustering/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6956 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/clustering/clustering_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     6030 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/clustering/greedy_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     1221 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/clustering/sklearn_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     5492 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/columngen.py
--rw-r--r--   0 runner    (1001) docker     (121)     8755 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/data.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/data_transformation/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/data_transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    41732 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/data_transformation/dft.py
--rw-r--r--   0 runner    (1001) docker     (121)     3866 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/data_transformation/sklearn_transformer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/data_transformation/value_transformation.py
--rw-r--r--   0 runner    (1001) docker     (121)     8971 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/distance_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/ensemble/
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/ensemble/ensemble_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/ensemble/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/evaluation/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13052 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/crossval.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/evaluation/eval_stats/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/eval_stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14775 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    29332 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     9324 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)    12299 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)    50503 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/eval_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    26886 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/evaluation/evaluator_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)    11601 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/feature_importance.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/feature_selection/
--rw-r--r--   0 runner    (1001) docker     (121)     6481 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/feature_selection/rfe.py
--rw-r--r--   0 runner    (1001) docker     (121)    52421 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/featuregen.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/geoanalytics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14706 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/_globalmaptiles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6697 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geo_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     6840 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geo_coords.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6701 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/coordinate_clustering.py
--rw-r--r--   0 runner    (1001) docker     (121)     5385 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/coordinate_clustering_ground_truth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1514 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     2959 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/geometry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/geopandas/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     7507 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/local_coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/geoanalytics/map_tiles.py
--rw-r--r--   0 runner    (1001) docker     (121)    23505 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/hyperopt.py
--rw-r--r--   0 runner    (1001) docker     (121)     7005 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (121)    31793 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/local_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/minizinc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/multi_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2842 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/naive_bayes.py
--rw-r--r--   0 runner    (1001) docker     (121)    18430 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/normalisation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/pytorch_lightning/pl_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/sklearn/
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15246 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/sklearn/sklearn_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/sklearn/sklearn_classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     7891 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/sklearn/sklearn_regression.py
--rw-r--r--   0 runner    (1001) docker     (121)    19868 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tensor_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5280 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tensorflow/tf_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tensorflow/tf_mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/torch/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38875 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    26792 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2925 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_eval_util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/torch/torch_models/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/torch/torch_models/lstnet/
--rw-r--r--   0 runner    (1001) docker     (121)     8903 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/lstnet/lstnet_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12555 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/lstnet/lstnet_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/torch/torch_models/mlp/
--rw-r--r--   0 runner    (1001) docker     (121)     6112 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/mlp/mlp_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1966 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/mlp/mlp_modules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/torch/torch_models/residualffn/
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/residualffn/residualffn_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8798 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_models/residualffn/residualffn_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)      450 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)    41880 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torch_opt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3479 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/torch/torchtext.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/tracking/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tracking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2032 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tracking/azure_tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tracking/clearml_tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)      637 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tracking/mlflow_tracking.py
--rw-r--r--   0 runner    (1001) docker     (121)     1269 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/tracking/tracking_base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai/util/
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (121)    29950 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    31117 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/cache_azure.py
--rw-r--r--   0 runner    (1001) docker     (121)     3483 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/cache_mysql.py
--rw-r--r--   0 runner    (1001) docker     (121)    11784 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/datastruct.py
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      865 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/dtype.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/hash.py
--rw-r--r--   0 runner    (1001) docker     (121)     2271 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     5267 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/io.py
--rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)     5209 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/pandas.py
--rw-r--r--   0 runner    (1001) docker     (121)     7749 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/pickle.py
--rw-r--r--   0 runner    (1001) docker     (121)     9387 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/plot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/profiling.py
--rw-r--r--   0 runner    (1001) docker     (121)     7492 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/sequences.py
--rw-r--r--   0 runner    (1001) docker     (121)    19371 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/string.py
--rw-r--r--   0 runner    (1001) docker     (121)     1203 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/time.py
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/util/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)    34982 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/vector_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    14692 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/vectoriser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-07-20 16:59:56.000000 sensai-0.1.9/src/sensai/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-07-20 17:00:16.000000 sensai-0.1.9/src/sensai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-07-20 17:00:17.000000 sensai-0.1.9/src/sensai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-07-20 17:00:16.000000 sensai-0.1.9/src/sensai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      396 2022-07-20 17:00:16.000000 sensai-0.1.9/src/sensai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-20 17:00:16.000000 sensai-0.1.9/src/sensai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 10:01:01.000000 sensai-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 10:01:16.000000 sensai-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-20 10:01:01.000000 sensai-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-20 10:01:01.000000 sensai-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 10:01:01.000000 sensai-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:01:16.000000 sensai-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-07-20 10:01:01.000000 sensai-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/catboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/clustering/clustering_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/clustering/greedy_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/clustering/sklearn_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/columngen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8749 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/data_transformation/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/data_transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42094 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/data_transformation/dft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/data_transformation/sklearn_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/data_transformation/value_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/distance_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/ensemble/ensemble_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/ensemble/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/crossval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/evaluation/eval_stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/eval_stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30015 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13380 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51278 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/eval_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26972 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/evaluation/evaluator_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/feature_importance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/feature_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/feature_selection/rfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52421 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/featuregen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/geoanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/_globalmaptiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geo_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6840 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geo_coords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/coordinate_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/coordinate_clustering_ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/geopandas/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/local_coords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/geoanalytics/map_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23505 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/hyperopt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31787 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/local_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/minizinc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/multi_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/naive_bayes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18430 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/normalisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/pytorch_lightning/pl_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15846 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/sklearn/sklearn_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/sklearn/sklearn_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7891 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/sklearn/sklearn_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/sklearn_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19868 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tensor_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tensorflow/tf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tensorflow/tf_mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38883 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26792 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_eval_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/torch/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/torch/torch_models/lstnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/lstnet/lstnet_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/lstnet/lstnet_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/torch/torch_models/mlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/mlp/mlp_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/mlp/mlp_modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/torch/torch_models/residualffn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/residualffn/residualffn_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_models/residualffn/residualffn_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41880 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torch_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/torch/torchtext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/tracking/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tracking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tracking/azure_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tracking/clearml_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tracking/mlflow_tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/tracking/tracking_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30119 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31117 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/cache_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/cache_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15278 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/datastruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/jscode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8809 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14553 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19907 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/util/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/vector_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14692 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/vectoriser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-07-20 10:01:01.000000 sensai-0.2.0/src/sensai/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 10:01:16.000000 sensai-0.2.0/src/sensai.egg-info/top_level.txt
```

### Comparing `sensai-0.1.9/README.md` & `sensai-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/setup.py` & `sensai-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 import functools
 import re
 from typing import Iterable, Dict
 from glob import glob
 
 from setuptools import setup, find_namespace_packages
 
-tf_requirements = ['tensorflow==1.15.0']
-torch_requirements = ['torch==1.4.0', 'torchtext==0.5.0']
-lightgbm_requirements = ['lightgbm==2.3.0']
-geoanalytics_requirements = ['networkx==2.4', 'Shapely~=1.7.0', 'geopandas==0.7.0', 'utm==0.7.0']
-
-
 # list of dependencies where ==/~= dependencies (used in requirements.txt and for the extras in requirements_*.txt) are relaxed:
 # any later version is OK (as long as we are not aware of a concrete limitation - and once we are, we shall define
 # the respective upper bound below)
 DEPS_VERSION_LOWER_BOUND = [
     # main
     "pandas", "scipy", "numpy", "scikit-learn", "seaborn", "typing-extensions",
     # extra "torch"
@@ -69,15 +63,15 @@
 setup(
     name='sensai',
     package_dir={"": "src"},
     license="MIT",
     url="https://github.com/jambit/sensAI",
     packages=find_namespace_packages(where="src"),
     include_package_data=True,
-    version='0.1.9',
+    version='0.2.0',
     description='Library for sensible AI',
     install_requires=relaxed_requirements_from_file("requirements.txt"),
     dependency_links=["https://download.pytorch.org/whl/torch_stable.html"],
     setup_requires=["wheel"],
     extras_require=extras_require,
     author='jambit GmbH'
 )
```

### Comparing `sensai-0.1.9/src/sensai/__init__.py` & `sensai-0.2.0/src/sensai/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from . import columngen
-from . import data_transformation
-from . import featuregen
-from . import hyperopt
-from . import local_search
-from . import naive_bayes
-from . import nearest_neighbors
-from . import sklearn
-from . import util
-from .data import InputOutputData
-from .data_transformation import DataFrameTransformer, RuleBasedDataFrameTransformer
-from .ensemble import AveragingVectorRegressionModel
-from .evaluation.eval_stats import eval_stats_classification, eval_stats_regression
-from .normalisation import NormalisationMode
-from .tensor_model import TensorToTensorRegressionModel, TensorToScalarRegressionModel, \
-    TensorToTensorClassificationModel, TensorToScalarClassificationModel
-from .vector_model import VectorModelBase, VectorModel, VectorRegressionModel, VectorClassificationModel
-
-__version__ = "0.1.9"
-
-# The following submodules are not imported by default to avoid necessarily requiring their dependencies:
-# tensorflow
-# torch
-# lightgbm
-# catboost
-# geoanalytics
-# xgboost
+from . import columngen
+from . import data_transformation
+from . import featuregen
+from . import hyperopt
+from . import local_search
+from . import naive_bayes
+from . import nearest_neighbors
+from . import sklearn
+from . import util
+from .data import InputOutputData
+from .data_transformation import DataFrameTransformer, RuleBasedDataFrameTransformer
+from .ensemble import AveragingVectorRegressionModel
+from .evaluation.eval_stats import eval_stats_classification, eval_stats_regression
+from .normalisation import NormalisationMode
+from .tensor_model import TensorToTensorRegressionModel, TensorToScalarRegressionModel, \
+    TensorToTensorClassificationModel, TensorToScalarClassificationModel
+from .vector_model import VectorModelBase, VectorModel, VectorRegressionModel, VectorClassificationModel
+
+__version__ = "0.2.0"
+
+# The following submodules are not imported by default to avoid necessarily requiring their dependencies:
+# tensorflow
+# torch
+# lightgbm
+# catboost
+# geoanalytics
+# xgboost
```

### Comparing `sensai-0.1.9/src/sensai/catboost.py` & `sensai-0.2.0/src/sensai/catboost.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/clustering/clustering_base.py` & `sensai-0.2.0/src/sensai/clustering/clustering_base.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/clustering/sklearn_clustering.py` & `sensai-0.2.0/src/sensai/clustering/sklearn_clustering.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/columngen.py` & `sensai-0.2.0/src/sensai/columngen.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/data.py` & `sensai-0.2.0/src/sensai/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Tuple, Sequence, TypeVar, List, Generic
 
 import numpy as np
 import pandas as pd
 import scipy.stats
 from sklearn.model_selection import StratifiedShuffleSplit
 
-from sensai.util.string import ToStringMixin
+from .util.string import ToStringMixin
 
 log = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
 
 class BaseInputOutputData(Generic[T], ABC):
```

### Comparing `sensai-0.1.9/src/sensai/data_transformation/dft.py` & `sensai-0.2.0/src/sensai/data_transformation/dft.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,28 @@
 import logging
 import re
 from abc import ABC, abstractmethod
 from typing import List, Sequence, Union, Dict, Callable, Any, Optional, Set
 
 import numpy as np
 import pandas as pd
+import sklearn
 from sklearn.preprocessing import OneHotEncoder
 
 from .sklearn_transformer import SkLearnTransformerProtocol
 from ..columngen import ColumnGenerator
 from ..util import flattenArguments, countNotNone
 from ..util.pandas import DataFrameColumnChangeTracker
 from ..util.pickle import setstate
 from ..util.string import orRegexGroup, ToStringMixin
 
 from typing import TYPE_CHECKING
 
+from ..util.version import Version
+
 if TYPE_CHECKING:
     from ..featuregen import FeatureGenerator
 
 log = logging.getLogger(__name__)
 
 
 class DataFrameTransformer(ABC, ToStringMixin):
@@ -196,14 +199,17 @@
 
     def findFirstTransformerByType(self, cls) -> Optional[DataFrameTransformer]:
         for dft in self.dataFrameTransformers:
             if isinstance(dft, cls):
                 return dft
         return None
 
+    def append(self, t: DataFrameTransformer):
+        self.dataFrameTransformers.append(t)
+
 
 class DFTRenameColumns(RuleBasedDataFrameTransformer):
     def __init__(self, columnsMap: Dict[str, str]):
         """
         :param columnsMap: dictionary mapping old column names to new names
         """
         super().__init__()
@@ -367,19 +373,25 @@
             self._columnNameRegex = orRegexGroup(columns)
             self._columnsToEncode = columns
         self.inplace = inplace
         self.arrayValuedResult = arrayValuedResult
         self.handleUnknown = "ignore" if ignoreUnknown else "error"
         if categories is not None:
             if type(categories) == dict:
-                self.oneHotEncoders = {col: OneHotEncoder(categories=[np.sort(categories)], sparse=False, handle_unknown=self.handleUnknown) for col, categories in categories.items()}
+                self.oneHotEncoders = {col: OneHotEncoder(categories=[np.sort(categories)], handle_unknown=self.handleUnknown, **self._sparseKwargs()) for col, categories in categories.items()}
             else:
                 if len(columns) != len(categories):
                     raise ValueError(f"Given categories must have the same length as columns to process")
-                self.oneHotEncoders = {col: OneHotEncoder(categories=[np.sort(categories)], sparse=False, handle_unknown=self.handleUnknown) for col, categories in zip(columns, categories)}
+                self.oneHotEncoders = {col: OneHotEncoder(categories=[np.sort(categories)], handle_unknown=self.handleUnknown, **self._sparseKwargs()) for col, categories in zip(columns, categories)}
+
+    def _sparseKwargs(self, sparse=False):
+        if Version(sklearn).isAtLeast(1, 2):
+            return dict(sparse_output=sparse)
+        else:
+            return dict(sparse=sparse)
 
     def __setstate__(self, state):
         if "arrayValuedResult" not in state:
             state["arrayValuedResult"] = False
         super().__setstate__(state)
 
     def _toStringAdditionalEntries(self) -> Dict[str, Any]:
@@ -389,15 +401,15 @@
 
     def _fit(self, df: pd.DataFrame):
         if self._columnsToEncode is None:
             self._columnsToEncode = [c for c in df.columns if re.fullmatch(self._columnNameRegex, c) is not None]
             if len(self._columnsToEncode) == 0:
                 log.warning(f"{self} does not apply to any columns, transformer has no effect; regex='{self._columnNameRegex}'")
         if self.oneHotEncoders is None:
-            self.oneHotEncoders = {column: OneHotEncoder(categories=[np.sort(df[column].unique())], sparse=False, handle_unknown=self.handleUnknown) for column in self._columnsToEncode}
+            self.oneHotEncoders = {column: OneHotEncoder(categories=[np.sort(df[column].unique())], handle_unknown=self.handleUnknown, **self._sparseKwargs()) for column in self._columnsToEncode}
         for columnName in self._columnsToEncode:
             self.oneHotEncoders[columnName].fit(df[[columnName]])
 
     def _apply(self, df: pd.DataFrame):
         if len(self._columnsToEncode) == 0:
             return df
```

### Comparing `sensai-0.1.9/src/sensai/data_transformation/sklearn_transformer.py` & `sensai-0.2.0/src/sensai/data_transformation/sklearn_transformer.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/data_transformation/value_transformation.py` & `sensai-0.2.0/src/sensai/data_transformation/value_transformation.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/distance_metric.py` & `sensai-0.2.0/src/sensai/distance_metric.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/ensemble/ensemble_base.py` & `sensai-0.2.0/src/sensai/ensemble/ensemble_base.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/ensemble/models.py` & `sensai-0.2.0/src/sensai/ensemble/models.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/evaluation/__init__.py` & `sensai-0.2.0/src/sensai/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/evaluation/crossval.py` & `sensai-0.2.0/src/sensai/evaluation/crossval.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_base.py` & `sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,16 @@
             if metric.bounds == (0, 1):
                 xTick = 0.1
                 if bins is None:
                     numBins = 10 if cdf else 20
                 else:
                     numBins = bins
                 bins = np.linspace(0, 1, numBins+1)
+            else:
+                bins = "auto"
 
         values = self._valuesByMetricName[metricName]
         title = metricName
         if subtitle is not None:
             title += "\n" + subtitle
         plot = HistogramPlot(values, bins=bins, stat=stat, kde=kde, cdf=cdf, cdfComplementary=cdfComplementary, **kwargs).title(title)
         if xTick is not None:
```

### Comparing `sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_classification.py` & `sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,40 +60,45 @@
         return balanced_accuracy_score(y_true=y_true, y_pred=y_predicted)
 
 
 class ClassificationMetricAccuracyWithoutLabels(ClassificationMetric):
     """
     Accuracy score with set of data points limited to the ones where the ground truth label is not one of the given labels
     """
-    def __init__(self, *labels: Any, probabilityThreshold=None):
+    def __init__(self, *labels: Any, probabilityThreshold=None, zeroValue=0.0):
         """
         :param labels: one or more labels which are not to be considered (all data points where the ground truth is
             one of these labels will be ignored)
         :param probabilityThreshold: a probability threshold: the probability of the most likely class must be at least this value for a data point
             to be considered in the metric computation (analogous to :class:`ClassificationMetricAccuracyMaxProbabilityBeyondThreshold`)
+        :param zeroValue: the metric value to assume for the case where the condition never applies (no countable instances without
+            the given label/beyond the given threshold)
         """
         if probabilityThreshold is not None:
             nameAdd = f", p_max >= {probabilityThreshold}"
         else:
             nameAdd = ""
         name = f"{ClassificationMetricAccuracy.name}Without[{','.join(map(str, labels))}{nameAdd}]"
         super().__init__(name, requiresProbabilities=probabilityThreshold is not None)
         self.labels = set(labels)
         self.probabilityThreshold = probabilityThreshold
+        self.zeroValue = zeroValue
 
     def _computeValue(self, y_true, y_predicted, y_predictedClassProbabilities):
         y_true = np.array(y_true)
         y_predicted = np.array(y_predicted)
         indices = []
         for i, (trueLabel, predictedLabel) in enumerate(zip(y_true, y_predicted)):
             if trueLabel not in self.labels:
                 if self.probabilityThreshold is not None:
                     if y_predictedClassProbabilities[predictedLabel].iloc[i] < self.probabilityThreshold:
                         continue
                 indices.append(i)
+        if len(indices) == 0:
+            return self.zeroValue
         return accuracy_score(y_true=y_true[indices], y_pred=y_predicted[indices])
 
     def getPairedMetrics(self) -> List[TMetric]:
         if self.probabilityThreshold is not None:
             return [ClassificationMetricRelFreqMaxProbabilityBeyondThreshold(self.probabilityThreshold)]
         else:
             return []
@@ -152,15 +157,15 @@
         labels = y_predictedClassProbabilities.columns
         labelToColIdx = {l: i for i, l in enumerate(labels)}
         relFreq = RelativeFrequencyCounter()
         for i, probabilities in enumerate(y_predictedClassProbabilities.values.tolist()):
             classIdx_predicted = np.argmax(probabilities)
             prob_predicted = probabilities[classIdx_predicted]
             if prob_predicted >= self.threshold:
-                classIdx_true = labelToColIdx[y_true[i]]
+                classIdx_true = labelToColIdx.get(y_true[i], -1)  # -1 if true class is unknown to model (did not appear in training data)
                 relFreq.count(classIdx_predicted == classIdx_true)
         if relFreq.numTotal == 0:
             return self.zeroValue
         else:
             return relFreq.getRelativeFrequency()
 
     def getPairedMetrics(self) -> List[TMetric]:
@@ -530,14 +535,19 @@
 
     def getRecall(self):
         return self._frac(self.tp, self.tp + self.fn)
 
     def getF1(self):
         return self._frac(self.tp, self.tp + 0.5 * (self.fp + self.fn))
 
+    def getRelFreqPositive(self):
+        positive = self.tp + self.fp
+        negative = self.tn + self.fn
+        return positive / (positive + negative)
+
 
 class BinaryClassificationProbabilityThresholdVariationData:
     def __init__(self, evalStats: ClassificationEvalStats):
         self.thresholds = np.linspace(0, 1, 101)
         self.counts: List[BinaryClassificationCounts] = []
         for threshold in self.thresholds:
             self.counts.append(BinaryClassificationCounts.fromEvalStats(evalStats, threshold=threshold))
@@ -548,17 +558,19 @@
         if subtitle is not None:
             title += "\n" + subtitle
         plt.title(title)
         plt.xlabel("probability threshold")
         precision = [c.getPrecision() for c in self.counts]
         recall = [c.getRecall() for c in self.counts]
         f1 = [c.getF1() for c in self.counts]
+        rfPositive = [c.getRelFreqPositive() for c in self.counts]
         plt.plot(self.thresholds, precision, label="precision")
         plt.plot(self.thresholds, recall, label="recall")
         plt.plot(self.thresholds, f1, label="F1-score")
+        plt.plot(self.thresholds, rfPositive, label="rel. freq. positive")
         plt.legend()
         return fig
 
     def plotCounts(self, subtitle=None):
         fig = plt.figure()
         title = "Probability Threshold-Dependent Counts"
         if subtitle is not None:
```

### Comparing `sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_clustering.py` & `sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_clustering.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/evaluation/eval_stats/eval_stats_regression.py` & `sensai-0.2.0/src/sensai/evaluation/eval_stats/eval_stats_regression.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 from typing import List, Sequence, Optional
 
 import numpy as np
 from matplotlib import pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap
 
 from .eval_stats_base import PredictionEvalStats, Metric, EvalStatsCollection, PredictionArray, EvalStatsPlot
+from ...vector_model import VectorRegressionModel, InputOutputData
 from ...util.plot import HistogramPlot
 
 log = logging.getLogger(__name__)
 
 
 class RegressionMetric(Metric["RegressionEvalStats"], ABC):
-    def computeValueForEvalStats(self, evalStats: "RegressionEvalStats"):
-        return self.computeValue(np.array(evalStats.y_true), np.array(evalStats.y_predicted))
+    def computeValueForEvalStats(self, evalStats: "RegressionEvalStats", model: VectorRegressionModel = None, ioData: InputOutputData = None):
+        return self.computeValue(np.array(evalStats.y_true), np.array(evalStats.y_predicted), model=model, ioData=ioData)
 
     @classmethod
     @abstractmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         pass
 
     @classmethod
     def computeErrors(cls, y_true: np.ndarray, y_predicted: np.ndarray):
         return y_predicted - y_true
 
     @classmethod
@@ -30,76 +31,76 @@
         return np.abs(cls.computeErrors(y_true, y_predicted))
 
 
 class RegressionMetricMAE(RegressionMetric):
     name = "MAE"
 
     @classmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         return np.mean(cls.computeAbsErrors(y_true, y_predicted))
 
 
 class RegressionMetricMSE(RegressionMetric):
     name = "MSE"
 
     @classmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         residuals = y_predicted - y_true
         return np.sum(residuals * residuals) / len(residuals)
 
 
 class RegressionMetricRMSE(RegressionMetric):
     name = "RMSE"
 
     @classmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         errors = cls.computeErrors(y_true, y_predicted)
         return np.sqrt(np.mean(errors * errors))
 
 
 class RegressionMetricRRSE(RegressionMetric):
     name = "RRSE"
 
     @classmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         mean_y = np.mean(y_true)
         residuals = y_predicted - y_true
         mean_deviation = y_true - mean_y
         return np.sqrt(np.sum(residuals * residuals) / np.sum(mean_deviation * mean_deviation))
 
 
 class RegressionMetricR2(RegressionMetric):
     name = "R2"
 
-    def computeValue(self, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         rrse = RegressionMetricRRSE.computeValue(y_true, y_predicted)
         return 1.0 - rrse*rrse
 
 
 class RegressionMetricPCC(RegressionMetric):
     name = "PCC"
 
-    def computeValue(self, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         cov = np.cov([y_true, y_predicted])
         return cov[0][1] / np.sqrt(cov[0][0] * cov[1][1])
 
 
 class RegressionMetricStdDevAE(RegressionMetric):
     name = "StdDevAE"
 
     @classmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         return np.std(cls.computeAbsErrors(y_true, y_predicted))
 
 
 class RegressionMetricMedianAE(RegressionMetric):
     name = "MedianAE"
 
     @classmethod
-    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray):
+    def computeValue(cls, y_true: np.ndarray, y_predicted: np.ndarray, model: VectorRegressionModel = None, ioData: InputOutputData = None):
         return np.median(cls.computeAbsErrors(y_true, y_predicted))
 
 
 class RegressionEvalStats(PredictionEvalStats["RegressionMetric"]):
     """
     Collects data for the evaluation of predicted continuous values and computes corresponding metrics
     """
@@ -108,30 +109,36 @@
     HEATMAP_COLORMAP_FACTORY = lambda self: LinearSegmentedColormap.from_list("whiteToRed", ((0, (1, 1, 1)), (1/len(self.y_predicted), (1, 0.96, 0.96)), (1, (0.7, 0, 0))), len(self.y_predicted))
     HEATMAP_DIAGONAL_COLOR = "green"
     HEATMAP_ERROR_BOUNDARY_VALUE = None
     HEATMAP_ERROR_BOUNDARY_COLOR = (0.8, 0.8, 0.8)
     SCATTER_PLOT_POINT_COLOR = (0, 0, 1, 0.05)
 
     def __init__(self, y_predicted: Optional[PredictionArray] = None, y_true: Optional[PredictionArray] = None,
-            metrics: Sequence["RegressionMetric"] = None, additionalMetrics: Sequence["RegressionMetric"] = None):
+            metrics: Sequence["RegressionMetric"] = None, additionalMetrics: Sequence["RegressionMetric"] = None,
+            model: VectorRegressionModel = None, ioData: InputOutputData = None):
         """
         :param y_predicted: the predicted values
         :param y_true: the true values
         :param metrics: the metrics to compute for evaluation; if None, use default metrics
         :param additionalMetrics: the metrics to additionally compute
         """
+        self.model = model
+        self.ioData = ioData
 
         if metrics is None:
             metrics = [RegressionMetricRRSE(), RegressionMetricR2(),
                        RegressionMetricMAE(), RegressionMetricMSE(), RegressionMetricRMSE(),
                        RegressionMetricStdDevAE()]
         metrics = list(metrics)
 
         super().__init__(y_predicted, y_true, metrics, additionalMetrics=additionalMetrics)
 
+    def computeMetricValue(self, metric: RegressionMetric) -> float:
+        return metric.computeValueForEvalStats(self, model=self.model, ioData=self.ioData)
+
     def getMSE(self):
         return self.computeMetricValue(RegressionMetricMSE())
 
     def getRRSE(self):
         """Gets the root relative squared error"""
         return self.computeMetricValue(RegressionMetricRRSE())
```

### Comparing `sensai-0.1.9/src/sensai/evaluation/eval_util.py` & `sensai-0.2.0/src/sensai/evaluation/eval_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -242,19 +242,20 @@
         :param isRegression: whether to create a regression model cross-validator. Either this or model have to be specified
         :return: an evaluator
         """
         return createVectorModelCrossValidator(self.inputOutputData, model=model, isRegression=isRegression, params=self.crossValidatorParams)
 
     def performSimpleEvaluation(self, model: TModel, createPlots=True, showPlots=False, logResults=True, resultWriter: ResultWriter = None,
             additionalEvaluationOnTrainingData=False, fitModel=True, writeEvalStats=False,
-            trackedExperiment: TrackedExperiment = None) -> TEvalData:
+            trackedExperiment: TrackedExperiment = None, evaluator: Optional[TEvaluator] = None) -> TEvalData:
         if showPlots and not createPlots:
             raise ValueError("showPlots=True requires createPlots=True")
         resultWriter = self._resultWriterForModel(resultWriter, model)
-        evaluator = self.createEvaluator(model)
+        if evaluator is None:
+            evaluator = self.createEvaluator(model)
         if trackedExperiment is not None:
             evaluator.setTrackedExperiment(trackedExperiment)
         log.info(f"Evaluating {model} via {evaluator}")
         if fitModel:
             evaluator.fitModel(model)
 
         def gatherResults(evalResultData: VectorModelEvaluationData, resultWriter, subtitlePrefix=""):
@@ -285,28 +286,29 @@
     @staticmethod
     def _resultWriterForModel(resultWriter: Optional[ResultWriter], model: TModel) -> Optional[ResultWriter]:
         if resultWriter is None:
             return None
         return resultWriter.childWithAddedPrefix(model.getName() + "_")
 
     def performCrossValidation(self, model: TModel, showPlots=False, logResults=True, resultWriter: Optional[ResultWriter] = None,
-            trackedExperiment: TrackedExperiment = None) -> TCrossValData:
+            trackedExperiment: TrackedExperiment = None, crossValidator: Optional[TCrossValidator] = None) -> TCrossValData:
         """
         Evaluates the given model via cross-validation
 
         :param model: the model to evaluate
         :param showPlots: whether to show plots that visualise evaluation results (combining all folds)
         :param logResults: whether to log evaluation results
         :param resultWriter: a writer with which to store text files and plots. The evaluated model's name is added to each filename
             automatically
         :param trackedExperiment: a tracked experiment with which results shall be associated
         :return: cross-validation result data
         """
         resultWriter = self._resultWriterForModel(resultWriter, model)
-        crossValidator = self.createCrossValidator(model)
+        if crossValidator is None:
+            crossValidator = self.createCrossValidator(model)
         if trackedExperiment is not None:
             crossValidator.setTrackedExperiment(trackedExperiment)
         crossValidationData = crossValidator.evalModel(model)
         aggStatsByVar = {varName: crossValidationData.getEvalStatsCollection(predictedVarName=varName).aggMetricsDict()
                 for varName in crossValidationData.predictedVarNames}
         df = pd.DataFrame.from_dict(aggStatsByVar, orient="index")
         strEvalResults = df.to_string()
@@ -346,28 +348,35 @@
         :param writeVisitorResults: whether to collect results from visitors (if any) after the comparison
         :param writeCSV: whether to write metrics table to CSV files
         :return: the comparison results
         """
         # collect model evaluation results
         statsList = []
         resultByModelName = {}
+        evaluator = None
+        crossValidator = None
         for i, model in enumerate(models, start=1):
             modelName = model.getName()
             log.info(f"Evaluating model {i}/{len(models)} named '{modelName}' ...")
             if useCrossValidation:
                 if not fitModels:
                     raise ValueError("Cross-validation necessitates that models be trained several times; got fitModels=False")
-                crossValData = self.performCrossValidation(model, resultWriter=resultWriter if writeIndividualResults else None)
+                if crossValidator is None:
+                    crossValidator = self.createCrossValidator(model)
+                crossValData = self.performCrossValidation(model, resultWriter=resultWriter if writeIndividualResults else None,
+                    crossValidator=crossValidator)
                 modelResult = ModelComparisonData.Result(crossValData=crossValData)
                 resultByModelName[modelName] = modelResult
                 evalStatsCollection = crossValData.getEvalStatsCollection()
                 statsDict = evalStatsCollection.aggMetricsDict()
             else:
+                if evaluator is None:
+                    evaluator = self.createEvaluator(model)
                 evalData = self.performSimpleEvaluation(model, resultWriter=resultWriter if writeIndividualResults else None,
-                    fitModel=fitModels)
+                    fitModel=fitModels, evaluator=evaluator)
                 modelResult = ModelComparisonData.Result(evalData=evalData)
                 resultByModelName[modelName] = modelResult
                 evalStats = evalData.getEvalStats()
                 statsDict = evalStats.metricsDict()
             statsDict["modelName"] = modelName
             statsList.append(statsDict)
             if visitors is not None:
@@ -428,15 +437,15 @@
 
         # write visitor results
         if visitors is not None and writeVisitorResults:
             resultCollector = EvaluationResultCollector(showPlots=False, resultWriter=resultWriter)
             for visitor in visitors:
                 visitor.collectResults(resultCollector)
 
-        return ModelComparisonData(resultsDF, resultByModelName)
+        return ModelComparisonData(resultsDF, resultByModelName, evaluator=evaluator, crossValidator=crossValidator)
 
     def compareModelsCrossValidation(self, models: Sequence[TModel], resultWriter: Optional[ResultWriter] = None) -> "ModelComparisonData":
         """
         Compares several models via cross-validation
 
         :param models: the models to compare
         :param resultWriter: a writer with which to store results of the comparison
@@ -723,17 +732,20 @@
 
 class ModelComparisonData:
     @dataclass
     class Result:
         evalData: Union[VectorClassificationModelEvaluationData, VectorRegressionModelEvaluationData] = None
         crossValData: Union[VectorClassificationModelCrossValidationData, VectorRegressionModelCrossValidationData] = None
 
-    def __init__(self, resultsDF: pd.DataFrame, resultsByModelName: Dict[str, Result]):
+    def __init__(self, resultsDF: pd.DataFrame, resultsByModelName: Dict[str, Result], evaluator: Optional[VectorModelEvaluator] = None,
+            crossValidator: Optional[VectorModelCrossValidator] = None):
         self.resultsDF = resultsDF
         self.resultByModelName = resultsByModelName
+        self.evaluator = evaluator
+        self.crossValidator = crossValidator
 
     def getBestModelName(self, metricName: str) -> str:
         idx = np.argmax(self.resultsDF[metricName])
         return self.resultsDF.index[idx]
 
     def getBestModel(self, metricName: str) -> Union[VectorClassificationModel, VectorRegressionModel, VectorModelBase]:
         result = self.resultByModelName[self.getBestModelName(metricName)]
@@ -841,15 +853,15 @@
         :param cdf: whether to additionally plot, for each distribution, the cumulative distribution function
         :param cdfComplementary: whether to plot the complementary cdf, provided that ``cdf`` is True
         """
         for modelName in self.getModelNames():
             evalStatsCollection = self.getEvalStatsCollection(modelName)
             for metricName in evalStatsCollection.getMetricNames():
                 # plot distribution
-                fig = evalStatsCollection.plotDistribution(metricName, cdf=cdf, cdfComplementary=cdfComplementary)
+                fig = evalStatsCollection.plotDistribution(metricName, subtitle=modelName, cdf=cdf, cdfComplementary=cdfComplementary)
                 resultWriter.writeFigure(f"{modelName}_dist-{metricName}", fig)
                 # scatter plot with paired metrics
                 metric = evalStatsCollection.getMetricByName(metricName)
                 for pairedMetric in metric.getPairedMetrics():
                     if evalStatsCollection.hasMetric(pairedMetric):
                         fig = evalStatsCollection.plotScatter(metric.name, pairedMetric.name)
                         resultWriter.writeFigure(f"{modelName}_scatter-{metric.name}-{pairedMetric.name}", fig)
```

### Comparing `sensai-0.1.9/src/sensai/evaluation/evaluator.py` & `sensai-0.2.0/src/sensai/evaluation/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from .eval_stats.eval_stats_classification import ClassificationEvalStats, ClassificationMetric
 from .eval_stats.eval_stats_regression import RegressionEvalStats, RegressionEvalStatsCollection, RegressionMetric
 from ..data import DataSplitter, DataSplitterFractional, InputOutputData
 from ..data_transformation import DataFrameTransformer
 from ..tracking import TrackingMixin, TrackedExperiment
 from ..util.string import ToStringMixin
 from ..util.typing import PandasNamedTuple
-from ..vector_model import VectorClassificationModel, VectorModel, VectorModelBase, VectorModelFittableBase
+from ..vector_model import VectorClassificationModel, VectorModel, VectorModelBase, VectorModelFittableBase, VectorRegressionModel
 
 log = logging.getLogger(__name__)
 
 TModel = TypeVar("TModel", bound=VectorModel)
 TEvalStats = TypeVar("TEvalStats", bound=EvalStats)
 TEvalStatsCollection = TypeVar("TEvalStatsCollection", bound=EvalStatsCollection)
 
@@ -296,23 +296,25 @@
         if params is not None:
             return params
         elif len(kwArgsOldParams) > 0:
             return VectorRegressionModelEvaluatorParams.fromOldKwArgs(**kwArgsOldParams)
         else:
             return VectorRegressionModelEvaluatorParams()
 
-    def _evalModel(self, model: VectorModelBase, data: InputOutputData) -> VectorRegressionModelEvaluationData:
+    def _evalModel(self, model: VectorRegressionModel, data: InputOutputData) -> VectorRegressionModelEvaluationData:
         if not model.isRegressionModel():
             raise ValueError(f"Expected a regression model, got {model}")
         evalStatsByVarName = {}
         predictions, groundTruth = self._computeOutputs(model, data)
         for predictedVarName in predictions.columns:
             evalStats = RegressionEvalStats(y_predicted=predictions[predictedVarName], y_true=groundTruth[predictedVarName],
                 metrics=self.params.metrics,
-                additionalMetrics=self.params.additionalMetrics)
+                additionalMetrics=self.params.additionalMetrics,
+                model=model,
+                ioData=data)
             evalStatsByVarName[predictedVarName] = evalStats
         return VectorRegressionModelEvaluationData(evalStatsByVarName, data, model)
 
     def computeTestDataOutputs(self, model: VectorModelBase) -> Tuple[pd.DataFrame, pd.DataFrame]:
         """
         Applies the given model to the test data
 
@@ -359,15 +361,15 @@
             fractionalSplitTestFraction for fractional split (default)
         :param fractionalSplitTestFraction: [if dataSplitter is None, test data must be obtained via split] the fraction of the data to use for testing/evaluation;
         :param fractionalSplitRandomSeed: [if dataSplitter is none, test data must be obtained via split] the random seed to use for the fractional split of the data
         :param fractionalSplitShuffle: [if dataSplitter is None, test data must be obtained via split] whether to randomly (based on randomSeed) shuffle the dataset before
             splitting it
         :param additionalMetrics: additional metrics to apply
         :param computeProbabilities: whether to compute class probabilities
-        :param binaryPositiveLabel: the positive class label for binary classification; if GUESS, true to detect from labels;
+        :param binaryPositiveLabel: the positive class label for binary classification; if GUESS, try to detect from labels;
             if None, no detection (non-binary classification)
         """
         super().__init__(dataSplitter, fractionalSplitTestFraction=fractionalSplitTestFraction, fractionalSplitRandomSeed=fractionalSplitRandomSeed,
             fractionalSplitShuffle=fractionalSplitShuffle)
         self.additionalMetrics = additionalMetrics
         self.computeProbabilities = computeProbabilities
         self.binaryPositiveLabel = binaryPositiveLabel
```

### Comparing `sensai-0.1.9/src/sensai/evaluation/evaluator_clustering.py` & `sensai-0.2.0/src/sensai/evaluation/evaluator_clustering.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/feature_importance.py` & `sensai-0.2.0/src/sensai/feature_importance.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from abc import ABC, abstractmethod
 from typing import Dict, Union, Sequence, List, Tuple, Optional
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from matplotlib import pyplot as plt
-from sklearn.inspection import permutation_importance
 
 from .data import InputOutputData
 from .evaluation.crossval import VectorModelCrossValidationData
 from .util.deprecation import deprecated
 from .util.plot import MATPLOTLIB_DEFAULT_FIGURE_SIZE
 from .util.string import ToStringMixin
 from .vector_model import VectorModel
@@ -174,14 +173,15 @@
 
     def getAggregatedFeatureImportance(self) -> FeatureImportance:
         return FeatureImportance(self.getAggregatedFeatureImportanceDict())
 
 
 def computePermutationFeatureImportanceDict(model, ioData: InputOutputData, scoring, numRepeats: int, randomState,
         excludeInputPreprocessors=False, numJobs=None):
+    from sklearn.inspection import permutation_importance
     if excludeInputPreprocessors:
         inputs = model.computeModelInputs(ioData.inputs)
         model = copy.copy(model)
         model.removeInputPreprocessors()
     else:
         inputs = ioData.inputs
     featureNames = inputs.columns
```

### Comparing `sensai-0.1.9/src/sensai/feature_selection/rfe.py` & `sensai-0.2.0/src/sensai/feature_selection/rfe.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass
 from typing import Union, List
 
 import matplotlib.pyplot as plt
 import numpy as np
 
 from sensai import VectorModel, InputOutputData
+from sensai.data_transformation import DFTKeepColumns, DFTColumnFilter
 from sensai.evaluation import VectorModelCrossValidatorParams, createVectorModelCrossValidator
 from sensai.feature_importance import FeatureImportanceProvider, AggregatedFeatureImportance
 from sensai.util.plot import ScatterPlot
 
 log = logging.getLogger(__name__)
 
 
@@ -33,14 +34,16 @@
     until n features remain and returns these features as the result.
     """
     def __init__(self, crossValidatorParams: VectorModelCrossValidatorParams, minFeatures=1):
         """
         :param crossValidatorParams: the parameters for cross-validation
         :param minFeatures: the minimum number of features to evaluate
         """
+        if not crossValidatorParams.returnTrainedModels:
+            raise ValueError("crossValidatorParams: returnTrainedModels is required to be enabled")
         self.crossValidatorParams = crossValidatorParams
         self.minFeatures = minFeatures
 
     @dataclass
     class Step:
         metricValue: float
         features: List[str]
@@ -77,41 +80,55 @@
             Plots the metric values vs. the number of features for each step of the elimination
 
             :return: the figure
             """
             return ScatterPlot(self.getNumFeaturesArray(), self.getMetricValuesArray(), c_opacity=1, x_label="number of features",
                 y_label=f"cross-validation mean metric value ({self.metricName})").fig
 
-    def run(self, model: Union[VectorModel, FeatureImportanceProvider], ioData: InputOutputData, metricName: str, minimise: bool) -> Result:
+    def run(self, model: Union[VectorModel, FeatureImportanceProvider], ioData: InputOutputData, metricName: str,
+            minimise: bool, removeInputPreprocessors=False) -> Result:
         """
         Runs the optimisation for the given model and data.
 
         :param model: the model
         :param ioData: the data
         :param metricName: the metric to optimise
         :param minimise: whether the metric shall be minimsed; if False, maximise.
+        :param removeInputPreprocessors: whether to remove input preprocessors from the model and create input data
+            only once during the entire experiment; this is usually reasonable only if all input preprocessors are not
+            trained on the input data or if, for any given data split/fold, the preprocessor learning outcome is likely
+            to be largely similar.
         :return: a result object, which provides access to the selected features and data on all elimination steps
         """
         metricKey = f"mean[{metricName}]"
 
-        model = copy(model)
-        model.fitInputOutputData(ioData, fitPreprocessors=True, fitModel=False)
-        inputs = model.computeModelInputs(ioData.inputs)
-        model.removeInputPreprocessors()
-        ioData = InputOutputData(inputs, ioData.outputs)
+        dftColumnFilter = None
+        if removeInputPreprocessors:
+            model = copy(model)
+            model.fitInputOutputData(ioData, fitPreprocessors=True, fitModel=False)
+            inputs = model.computeModelInputs(ioData.inputs)
+            model.removeInputPreprocessors()
+            ioData = InputOutputData(inputs, ioData.outputs)
+            features = list(inputs.columns)
+        else:
+            features = None  # can only be obtained after having fitted the model initially (see below)
+        dftColumnFilter = DFTColumnFilter()
+        model.withFeatureTransformers(dftColumnFilter, add=True)
 
-        features = list(inputs.columns)
         steps = []
         while True:
             # evaluate model
             crossValidator = createVectorModelCrossValidator(ioData, model=model, params=self.crossValidatorParams)
             crossValData = crossValidator.evalModel(model)
             aggMetricsDict = crossValData.getEvalStatsCollection().aggMetricsDict()
             metricValue = aggMetricsDict[metricKey]
 
+            if features is None:
+                features = crossValData.trainedModels[0].getModelInputVariableNames()
+
             steps.append(self.Step(metricValue=metricValue, features=features))
 
             # eliminate feature(s)
             log.info(f"Model performance with {len(features)} features: {metricKey}={metricValue}")
             aggImportance = AggregatedFeatureImportance(*crossValData.trainedModels)
             fi = aggImportance.getAggregatedFeatureImportance()
             tuples = fi.getSortedTuples()
@@ -123,15 +140,16 @@
                         break
                     eliminatedFeatures.append(fname)
                 log.info(f"Eliminating {len(eliminatedFeatures)} features with 0 importance: {eliminatedFeatures}")
             else:
                 eliminatedFeatures = [tuples[0][0]]
                 log.info(f"Eliminating feature {eliminatedFeatures[0]}")
             features = [f for f in features if f not in eliminatedFeatures]
-            ioData.inputs = ioData.inputs[features]
+            dftColumnFilter.keep = features
+
             log.info(f"{len(features)} features remain")
 
             if len(features) < self.minFeatures:
                 log.info("Minimum number of features reached/exceeded")
                 break
 
         return self.Result(steps, metricName, minimise)
```

### Comparing `sensai-0.1.9/src/sensai/featuregen.py` & `sensai-0.2.0/src/sensai/featuregen.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/_globalmaptiles.py` & `sensai-0.2.0/src/sensai/geoanalytics/_globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/geo_coords.py` & `sensai-0.2.0/src/sensai/geoanalytics/geo_coords.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/geopandas/coordinate_clustering.py` & `sensai-0.2.0/src/sensai/geoanalytics/geopandas/coordinate_clustering.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/geopandas/coordinate_clustering_ground_truth.py` & `sensai-0.2.0/src/sensai/geoanalytics/geopandas/coordinate_clustering_ground_truth.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/geopandas/coordinates.py` & `sensai-0.2.0/src/sensai/geoanalytics/geopandas/coordinates.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/geopandas/geometry.py` & `sensai-0.2.0/src/sensai/geoanalytics/geopandas/geometry.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/geopandas/graph.py` & `sensai-0.2.0/src/sensai/geoanalytics/geopandas/graph.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/local_coords.py` & `sensai-0.2.0/src/sensai/geoanalytics/local_coords.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/geoanalytics/map_tiles.py` & `sensai-0.2.0/src/sensai/geoanalytics/map_tiles.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/hyperopt.py` & `sensai-0.2.0/src/sensai/hyperopt.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/lightgbm.py` & `sensai-0.2.0/src/sensai/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/local_search.py` & `sensai-0.2.0/src/sensai/local_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple, Callable, Type, Sequence, TypeVar, Generic
 
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 
-from sensai.util.aggregation import RelativeFrequencyCounter
+from .util.aggregation import RelativeFrequencyCounter
 
 log = logging.getLogger(__name__)
 
 
 class SATemperatureSchedule(ABC):
     """
     Describes how temperature changes as the annealing process goes on.
```

### Comparing `sensai-0.1.9/src/sensai/minizinc.py` & `sensai-0.2.0/src/sensai/minizinc.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/multi_model.py` & `sensai-0.2.0/src/sensai/multi_model.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/naive_bayes.py` & `sensai-0.2.0/src/sensai/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/nearest_neighbors.py` & `sensai-0.2.0/src/sensai/nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/normalisation.py` & `sensai-0.2.0/src/sensai/normalisation.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/pytorch_lightning/pl_models.py` & `sensai-0.2.0/src/sensai/pytorch_lightning/pl_models.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/sklearn/sklearn_base.py` & `sensai-0.2.0/src/sensai/sklearn/sklearn_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,17 +154,20 @@
                     outputTransformer=copy.deepcopy(self.sklearnOutputTransformer))
             model.fit(inputs, outputs[predictedVarName], **self.fitArgs)
             self.models[predictedVarName] = model
 
     def _predictSkLearn(self, inputs: pd.DataFrame) -> pd.DataFrame:
         results = {}
         for varName in self.models:
-            results[varName] = self.models[varName].predict(inputs)
+            results[varName] = self._predictSkLearnSingleModel(self.models[varName], inputs)
         return pd.DataFrame(results)
 
+    def _predictSkLearnSingleModel(self, model, inputs: pd.DataFrame) -> np.ndarray:
+        return model.predict(inputs)
+
     def getSkLearnModel(self, predictedVarName=None):
         if predictedVarName is None:
             if len(self.models) > 1:
                 raise ValueError(f"Must provide predicted variable name (one of {self.models.keys()})")
             return next(iter(self.models.values()))
         return self.models[predictedVarName]
 
@@ -199,36 +202,40 @@
 
     def _predictSkLearn(self, inputs: pd.DataFrame) -> pd.DataFrame:
         Y = self.model.predict(inputs)
         return pd.DataFrame(Y, columns=self.getModelOutputVariableNames())
 
 
 class AbstractSkLearnVectorClassificationModel(VectorClassificationModel, ABC):
-    def __init__(self, modelConstructor, useBalancedClassWeights=False, **modelArgs):
+    def __init__(self, modelConstructor, useBalancedClassWeights=False, useLabelEncoding=False, **modelArgs):
         """
         :param modelConstructor: the sklearn model constructor
         :param modelArgs: arguments to be passed to the sklearn model constructor
         :param useBalancedClassWeights: whether to compute class weights from the training data and apply the corresponding weight to
             each data point such that the sum of weights for all classes is equal. This is achieved by applying a weight proportional
             to the reciprocal frequency of the class in the (training) data. We scale weights such that the smallest weight (of the
             largest class) is 1, ensuring that weight counts still reasonably correspond to data point counts.
             Note that weighted data points may not be supported for all types of models.
+        :param useLabelEncoding: whether to replace original class labels with 0-based index in sorted list of labels (a.k.a. label
+            encoding), which is required by some sklearn-compatible implementations (particularly xgboost)
         """
         super().__init__()
         self.modelConstructor = modelConstructor
         self.sklearnInputTransformer = None
-        self.sklearnOutputTransformer = None
         self.modelArgs = modelArgs
         self.fitArgs = {}
         self.useBalancedClassWeights = useBalancedClassWeights
+        self.useLabelEncoding = useLabelEncoding
         self.model = None
 
     def __setstate__(self, state):
-        setstate(AbstractSkLearnVectorClassificationModel, self, state, newDefaultProperties={"useComputedClassWeights": False},
-            renamedProperties={"useComputedClassWeights": "useBalancedClassWeights"})
+        setstate(AbstractSkLearnVectorClassificationModel, self, state, newOptionalProperties=["labelEncoder"],
+            newDefaultProperties={"useComputedClassWeights": False, "useLabelEncoder": False},
+            renamedProperties={"useComputedClassWeights": "useBalancedClassWeights"},
+            removedProperties=["sklearnOutputTransformer"])
 
     def _toStringExcludes(self) -> List[str]:
         return super()._toStringExcludes() + ["modelConstructor", "sklearnInputTransformer", "sklearnOutputTransformer",
             "modelArgs", "model"]
 
     def _toStringAdditionalEntries(self) -> Dict[str, Any]:
         d = super()._toStringAdditionalEntries()
@@ -242,23 +249,14 @@
         """
         :param sklearnInputTransformer: an optional sklearn preprocessor for transforming inputs
         :return: self
         """
         self.sklearnInputTransformer = sklearnInputTransformer
         return self
 
-    def withSkLearnOutputTransformer(self, sklearnOutputTransformer):
-        """
-        :param sklearnOutputTransformer: an optional sklearn preprocessor for transforming the target labels
-        :return: self
-        """
-        raise Exception("This is currently not supported for classifiers")  # TODO add support
-        self.sklearnOutputTransformer = sklearnOutputTransformer
-        return self
-
     def _updateModelArgs(self, inputs: pd.DataFrame, outputs: pd.DataFrame):
         """
         Designed to be overridden in order to make input data-specific changes to modelArgs
 
         :param inputs: the training input data
         :param outputs: the training output data
         """
@@ -274,32 +272,47 @@
         """
         pass
 
     def _fitClassifier(self, inputs: pd.DataFrame, outputs: pd.DataFrame):
         inputs = self._transformInput(inputs, fit=True)
         self._updateModelArgs(inputs, outputs)
         self._updateFitArgs(inputs, outputs)
-        self.model = createSkLearnModel(self.modelConstructor, self.modelArgs, self.sklearnOutputTransformer)
+        self.model = createSkLearnModel(self.modelConstructor, self.modelArgs)
         log.info(f"Fitting sklearn classifier of type {self.model.__class__.__name__}")
         kwargs = dict(self.fitArgs)
         if self.useBalancedClassWeights:
             class2weight = self._computeClassWeights(outputs)
             classes = outputs.iloc[:, 0]
             weights = np.array([class2weight[cls] for cls in classes])
             weights = weights / np.min(weights)
             kwargs["sample_weight"] = weights
+
         outputValues = np.ravel(outputs.values)
+        if self.useLabelEncoding:
+            outputValues = self._encodeLabels(outputValues)
         self.model.fit(inputs, outputValues, **kwargs)
 
     def _transformInput(self, inputs: pd.DataFrame, fit=False) -> pd.DataFrame:
         return _applySkLearnInputTransformer(inputs, self.sklearnInputTransformer, fit)
 
+    def _encodeLabels(self, y: np.ndarray):
+        d = {l: i for i, l in enumerate(self._labels)}
+        vfn = np.vectorize(lambda x: d[x])
+        return vfn(y)
+
+    def _decodeLabels(self, y: np.ndarray):
+        d = dict(enumerate(self._labels))
+        vfn = np.vectorize(lambda x: d[x])
+        return vfn(y)
+
     def _predict(self, x: pd.DataFrame):
         inputValues = self._transformInput(x)
         Y = self.model.predict(inputValues)
+        if self.useLabelEncoding:
+            Y = self._decodeLabels(Y)
         return pd.DataFrame(Y, columns=self._predictedVariableNames)
 
     def _predictClassProbabilities(self, x: pd.DataFrame):
         inputValues = self._transformInput(x)
         Y = self.model.predict_proba(inputValues)
         return pd.DataFrame(Y, columns=self._labels)
```

### Comparing `sensai-0.1.9/src/sensai/sklearn/sklearn_classification.py` & `sensai-0.2.0/src/sensai/sklearn/sklearn_classification.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/sklearn/sklearn_regression.py` & `sensai-0.2.0/src/sensai/sklearn/sklearn_regression.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/tensor_model.py` & `sensai-0.2.0/src/sensai/tensor_model.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/tensorflow/tf_base.py` & `sensai-0.2.0/src/sensai/tensorflow/tf_base.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/tensorflow/tf_mlp.py` & `sensai-0.2.0/src/sensai/tensorflow/tf_mlp.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_base.py` & `sensai-0.2.0/src/sensai/torch/torch_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,15 +573,15 @@
             nnOptimiserParamsInstance = NNOptimiserParams.fromDictOrInstance(nnOptimiserParams)
         if nnOptimiserParamsInstance.lossEvaluator is None:
             lossFunction = NNLossEvaluatorClassification.LossFunction.defaultForOutputMode(outputMode)
             nnOptimiserParamsInstance.lossEvaluator = NNLossEvaluatorClassification(lossFunction)
 
         self.outputMode = outputMode
         self.normalisationMode = normalisationMode
-        self.nnOptimiserParams: NNOptimiserParams = nnOptimiserParams
+        self.nnOptimiserParams: NNOptimiserParams = nnOptimiserParamsInstance
         self.modelClass = modelClass
         self.modelArgs = modelArgs
         self.modelKwArgs = modelKwArgs
         self.model: Optional[VectorTorchModel] = None
         self.inputTensoriser: Optional[Tensoriser] = None
         self.outputTensoriser: Optional[Tensoriser] = None
         self.torchDataSetProviderFactory: Optional[TorchDataSetProviderFactory] = None
```

### Comparing `sensai-0.1.9/src/sensai/torch/torch_data.py` & `sensai-0.2.0/src/sensai/torch/torch_data.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_enums.py` & `sensai-0.2.0/src/sensai/torch/torch_enums.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_eval_util.py` & `sensai-0.2.0/src/sensai/torch/torch_eval_util.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_models/lstnet/lstnet_models.py` & `sensai-0.2.0/src/sensai/torch/torch_models/lstnet/lstnet_models.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_models/lstnet/lstnet_modules.py` & `sensai-0.2.0/src/sensai/torch/torch_models/lstnet/lstnet_modules.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_models/mlp/mlp_models.py` & `sensai-0.2.0/src/sensai/torch/torch_models/mlp/mlp_models.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_models/mlp/mlp_modules.py` & `sensai-0.2.0/src/sensai/torch/torch_models/mlp/mlp_modules.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_models/residualffn/residualffn_models.py` & `sensai-0.2.0/src/sensai/torch/torch_models/residualffn/residualffn_models.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_models/residualffn/residualffn_modules.py` & `sensai-0.2.0/src/sensai/torch/torch_models/residualffn/residualffn_modules.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torch_opt.py` & `sensai-0.2.0/src/sensai/torch/torch_opt.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/torch/torchtext.py` & `sensai-0.2.0/src/sensai/torch/torchtext.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-from typing import Dict, Generator, Tuple, Optional, Union
-
-import pandas as pd
-import torch
-import torchtext
-
-from .torch_data import toTensor, TorchDataSet, TorchDataSetProvider
-
-
-class TorchtextDataSetFromDataFrame(torchtext.data.Dataset):
-    """
-    A specialisation of torchtext.data.Dataset, where the data is taken from a pandas.DataFrame
-    """
-    def __init__(self, df: pd.DataFrame, fields: Dict[str, torchtext.data.Field]):
-        """
-        :param df: the data frame from which to obtain the data
-        :param fields: a mapping from column names in the given data frame to torchtext fields, i.e.
-            the keys are the columns to read and the values are the fields to use for generated Example instances
-        """
-        examples = df.apply(self._exampleFromSeries, args=(fields,), axis=1).tolist()
-        fields = dict(fields)
-        super().__init__(examples, fields)
-
-    @classmethod
-    def _exampleFromSeries(cls, series: pd.Series, fields: Dict[str, torchtext.data.Field]):
-        return cls._exampleFromDict(series.to_dict(), fields)
-
-    @classmethod
-    def _exampleFromDict(cls, d: dict, fields: Dict[str, torchtext.data.Field]):
-        ex = torchtext.data.Example()
-        for key, field in fields.items():
-            if key not in d:
-                raise ValueError("Specified key {} was not found in "
-                                 "the input data".format(key))
-            if field is not None:
-                setattr(ex, key, field.preprocess(d[key]))
-            else:
-                setattr(ex, key, d[key])
-        return ex
-
-
-class TorchDataSetFromTorchtextDataSet(TorchDataSet):
-    def __init__(self, dataSet: torchtext.data.Dataset, inputField: str, outputField: Optional[str], cuda: bool):
-        self.outputField = outputField
-        self.inputField = inputField
-        self.dataSet = dataSet
-        self.cuda = cuda
-
-    def iterBatches(self, batchSize: int, shuffle: bool = False, inputOnly=False) -> Generator[Union[Tuple[torch.Tensor, torch.Tensor], torch.Tensor], None, None]:
-        iterator = torchtext.data.BucketIterator(self.dataSet,
-            batch_size=batchSize,
-            sort_key=lambda x: len(x.text),
-            sort_within_batch=False)
-
-        for batch in iterator:
-            x = toTensor(getattr(batch, self.inputField), self.cuda)
-            if not inputOnly and self.outputField is not None:
-                y = toTensor(getattr(batch, self.outputField), self.cuda)
-                yield x, y
-            else:
-                yield x
-
-    def size(self) -> Optional[int]:
-        return len(self.dataSet)
-
-
-class TorchDataSetProviderFromTorchtextDataSet(TorchDataSetProvider):
-    def __init__(self, dataSet: torchtext.data.Dataset, inputField: str, outputField: str, cuda: bool, modelOutputDim, inputDim=None):
-        super().__init__(modelOutputDim=modelOutputDim, inputDim=inputDim)
-        self.dataSet = dataSet
-        self.outputField = outputField
-        self.inputField = inputField
-        self.cuda = cuda
-
-    def provideSplit(self, fractionalSizeOfFirstSet: float) -> Tuple[TorchDataSet, TorchDataSet]:
-        d1, d2 = self.dataSet.split(fractionalSizeOfFirstSet)
-        return self._createDataSet(d1), self._createDataSet(d2)
-
-    def _createDataSet(self, d: torchtext.data.Dataset):
+from typing import Dict, Generator, Tuple, Optional, Union
+
+import pandas as pd
+import torch
+import torchtext
+
+from .torch_data import toTensor, TorchDataSet, TorchDataSetProvider
+
+
+class TorchtextDataSetFromDataFrame(torchtext.data.Dataset):
+    """
+    A specialisation of torchtext.data.Dataset, where the data is taken from a pandas.DataFrame
+    """
+    def __init__(self, df: pd.DataFrame, fields: Dict[str, torchtext.data.Field]):
+        """
+        :param df: the data frame from which to obtain the data
+        :param fields: a mapping from column names in the given data frame to torchtext fields, i.e.
+            the keys are the columns to read and the values are the fields to use for generated Example instances
+        """
+        examples = df.apply(self._exampleFromSeries, args=(fields,), axis=1).tolist()
+        fields = dict(fields)
+        super().__init__(examples, fields)
+
+    @classmethod
+    def _exampleFromSeries(cls, series: pd.Series, fields: Dict[str, torchtext.data.Field]):
+        return cls._exampleFromDict(series.to_dict(), fields)
+
+    @classmethod
+    def _exampleFromDict(cls, d: dict, fields: Dict[str, torchtext.data.Field]):
+        ex = torchtext.data.Example()
+        for key, field in fields.items():
+            if key not in d:
+                raise ValueError("Specified key {} was not found in "
+                                 "the input data".format(key))
+            if field is not None:
+                setattr(ex, key, field.preprocess(d[key]))
+            else:
+                setattr(ex, key, d[key])
+        return ex
+
+
+class TorchDataSetFromTorchtextDataSet(TorchDataSet):
+    def __init__(self, dataSet: torchtext.data.Dataset, inputField: str, outputField: Optional[str], cuda: bool):
+        self.outputField = outputField
+        self.inputField = inputField
+        self.dataSet = dataSet
+        self.cuda = cuda
+
+    def iterBatches(self, batchSize: int, shuffle: bool = False, inputOnly=False) -> Generator[Union[Tuple[torch.Tensor, torch.Tensor], torch.Tensor], None, None]:
+        iterator = torchtext.data.BucketIterator(self.dataSet,
+            batch_size=batchSize,
+            sort_key=lambda x: len(x.text),
+            sort_within_batch=False)
+
+        for batch in iterator:
+            x = toTensor(getattr(batch, self.inputField), self.cuda)
+            if not inputOnly and self.outputField is not None:
+                y = toTensor(getattr(batch, self.outputField), self.cuda)
+                yield x, y
+            else:
+                yield x
+
+    def size(self) -> Optional[int]:
+        return len(self.dataSet)
+
+
+class TorchDataSetProviderFromTorchtextDataSet(TorchDataSetProvider):
+    def __init__(self, dataSet: torchtext.data.Dataset, inputField: str, outputField: str, cuda: bool, modelOutputDim, inputDim=None):
+        super().__init__(modelOutputDim=modelOutputDim, inputDim=inputDim)
+        self.dataSet = dataSet
+        self.outputField = outputField
+        self.inputField = inputField
+        self.cuda = cuda
+
+    def provideSplit(self, fractionalSizeOfFirstSet: float) -> Tuple[TorchDataSet, TorchDataSet]:
+        d1, d2 = self.dataSet.split(fractionalSizeOfFirstSet)
+        return self._createDataSet(d1), self._createDataSet(d2)
+
+    def _createDataSet(self, d: torchtext.data.Dataset):
         return TorchDataSetFromTorchtextDataSet(d, self.inputField, self.outputField, self.cuda)
```

### Comparing `sensai-0.1.9/src/sensai/tracking/azure_tracking.py` & `sensai-0.2.0/src/sensai/tracking/azure_tracking.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/tracking/clearml_tracking.py` & `sensai-0.2.0/src/sensai/tracking/clearml_tracking.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/tracking/mlflow_tracking.py` & `sensai-0.2.0/src/sensai/tracking/mlflow_tracking.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/tracking/tracking_base.py` & `sensai-0.2.0/src/sensai/tracking/tracking_base.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/aggregation.py` & `sensai-0.2.0/src/sensai/util/aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,17 +49,21 @@
 
 
 class DistributionCounter(ToStringMixin):
     """
     Supports the counting of the frequencies with which (mutually exclusive) events occur
     """
     def __init__(self):
-        self.counts = collections.defaultdict(lambda: 0)
+        self.counts = collections.defaultdict(self._zero)
         self.totalCount = 0
 
+    @staticmethod
+    def _zero():
+        return 0
+
     def count(self, event: Hashable) -> None:
         """
         Increments the count of the given event
 
         :param event: the event/key whose count to increment, which must be hashable
         """
         self.totalCount += 1
```

### Comparing `sensai-0.1.9/src/sensai/util/cache.py` & `sensai-0.2.0/src/sensai/util/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,29 +208,32 @@
                 if persistedVersion == version:
                     cacheFound = True
             except EOFError:
                 log.warning(f"The cache file in {picklePath} is corrupt")
         if not cacheFound:
             self.cache = {}
         self._updateHook = DelayedUpdateHook(self.save, deferredSaveDelaySecs)
+        self._writeLock = threading.Lock()
 
     def save(self):
         """
         Saves the cache in the file whose path was provided at construction
         """
-        log.info(f"Saving cache to {self.picklePath}")
-        dumpPickle((self.version, self.cache), self.picklePath)
+        with self._writeLock:  # avoid concurrent modification while saving
+            log.info(f"Saving cache to {self.picklePath}")
+            dumpPickle((self.version, self.cache), self.picklePath)
 
     def get(self, key: TKey) -> Optional[TValue]:
         return self.cache.get(key)
 
     def set(self, key: TKey, value: TValue):
-        self.cache[key] = value
-        if self.saveOnUpdate:
-            self._updateHook.handleUpdate()
+        with self._writeLock:
+            self.cache[key] = value
+            if self.saveOnUpdate:
+                self._updateHook.handleUpdate()
 
 
 class SlicedPicklePersistentList(PersistentList):
     """
     Object handling the creation and access to sliced pickle caches
     """
     def __init__(self, directory, pickleBaseName, numEntriesPerSlice=100000):
```

### Comparing `sensai-0.1.9/src/sensai/util/cache_azure.py` & `sensai-0.2.0/src/sensai/util/cache_azure.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/cache_mysql.py` & `sensai-0.2.0/src/sensai/util/cache_mysql.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/datastruct.py` & `sensai-0.2.0/src/sensai/util/datastruct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from abc import ABC, abstractmethod
 from enum import Enum
 from typing import Sequence, Optional, TypeVar, Generic, Tuple, Dict, Any
 
 import pandas as pd
 
 from . import sequences as array_util
 from .string import ToStringMixin, dictString
 
+T = TypeVar("T")
 TKey = TypeVar("TKey")
 TValue = TypeVar("TValue")
 
 
 class Trivalent(Enum):
     TRUE = "true"
     FALSE = "false"
@@ -22,14 +24,19 @@
     def isTrue(self):
         return self == Trivalent.TRUE
 
     def isFalse(self):
         return self == Trivalent.FALSE
 
 
+class Maybe(Generic[TValue]):
+    def __init__(self, value: Optional[TValue]):
+        self.value = value
+
+
 class DeferredParams(ToStringMixin):
     """
     Represents a dictionary of parameters that is specifically designed to hold parameters that can only defined late within
     a process (i.e. not initially at construction time), e.g. because the parameters are data-dependent and therefore can only
     be determined once the data has been seen.
     """
     UNDEFINED = "__undefined__DeferredParams"
@@ -135,89 +142,197 @@
             return None
         return self.values[firstIndex:lastIndex+1]
 
     def valueSlice(self, lowestKey, highestKey) -> Optional[Sequence[TValue]]:
         return self._valueSlice(self.ceilIndex(lowestKey), self.floorIndex(highestKey))
 
 
-class SortedKeysAndValues(Generic[TKey, TValue]):
-    def __init__(self, keys: Sequence[TKey], values: Sequence[TValue]):
-        """
-        :param keys: a sorted sequence of keys
-        :param values: a sequence of corresponding values
-        """
-        if len(keys) != len(values):
-            raise ValueError("Lengths of keys and values do not match")
-        self.keys = keys
-        self.values = values
-
-    @classmethod
-    def fromSeries(cls, s: pd.Series):
-        """
-        Creates an instance from a pandas Series, using the series' index as the keys and its values as the values
-
-        :param s: the series
-        :return: an instance
-        """
-        return cls(s.index, s.values)
+class SortedKeyValueStructure(Generic[TKey, TValue], ABC):
+    @abstractmethod
+    def __len__(self):
+        pass
 
-    def floorIndex(self, key) -> Optional[int]:
+    @abstractmethod
+    def floorIndex(self, key: TKey) -> Optional[int]:
         """
         Finds the rightmost index where the key value is less than or equal to the given value
 
         :param key: the value to search for
         :return: the index or None if there is no such index
         """
-        return array_util.floorIndex(self.keys, key)
+        pass
 
-    def ceilIndex(self, key) -> Optional[int]:
+    @abstractmethod
+    def ceilIndex(self, key: TKey) -> Optional[int]:
         """
         Finds the leftmost index where the key value is greater than or equal to the given value
 
         :param key: the value to search for
         :return: the index or None if there is no such index
         """
-        return array_util.ceilIndex(self.keys, key)
+        pass
 
-    def closestIndex(self, key) -> Optional[int]:
+    @abstractmethod
+    def closestIndex(self, key: TKey) -> Optional[int]:
         """
         Finds the index where the key is closest to the given value.
         If two subsequent keys have the same distance, the smaller index is returned.
 
         :param key: the value to search for
         :return: the index or None if this object is empty.
         """
-        return array_util.closestIndex(self.keys, key)
+        pass
 
-    def floorValue(self, key) -> Optional[TValue]:
+    @abstractmethod
+    def floorValue(self, key: TKey) -> Optional[TValue]:
         """
         Returns the value for the largest index where the corresponding key is less than or equal to the given value
 
-        :param value: the value to search for
+        :param key: the key to search for
         :return: the value or None if there is no such value
         """
-        return array_util.floorValue(self.keys, key, values=self.values)
+        pass
 
-    def ceilValue(self, key) -> Optional[TValue]:
+    @abstractmethod
+    def ceilValue(self, key: TKey) -> Optional[TValue]:
         """
         Returns the value for the smallest index where the corresponding key is greater than or equal to the given value
 
-        :param value: the value to search for
+        :param key: the key to search for
         :return: the value or None if there is no such value
         """
-        return array_util.ceilValue(self.keys, key, values=self.values)
+        pass
 
-    def closestValue(self, key) -> Optional[TValue]:
+    @abstractmethod
+    def closestValue(self, key: TKey) -> Optional[TValue]:
         """
         Finds the value that is closest to the given value.
         If two subsequent values have the same distance, the smaller value is returned.
 
-        :param value: the value to search for
+        :param key: the key to search for
         :return: the value or None if this object is empty
         """
+        pass
+
+    @abstractmethod
+    def floorKeyAndValue(self, key: TKey) -> Optional[Tuple[TKey, TValue]]:
+        pass
+
+    @abstractmethod
+    def ceilKeyAndValue(self, key: TKey) -> Optional[Tuple[TKey, TValue]]:
+        pass
+
+    @abstractmethod
+    def closestKeyAndValue(self, key: TKey) -> Optional[Tuple[TKey, TValue]]:
+        pass
+
+    def interpolatedValue(self, key: TKey) -> Optional[TValue]:
+        """
+        Computes a linearly interpolated value for the given key - based on the two closest key-value pairs found in the data structure.
+        If the key is found in the data structure, the corresponding value is directly returned.
+
+        NOTE: This operation is supported only for value types that support the required arithmetic operations.
+
+        :param key: the key for which the interpolated value is to be computed.
+        :return: the interpolated value or None if the data structure does not contain floor/ceil entries for the given key
+        """
+        fkv = self.floorKeyAndValue(key)
+        ckv = self.ceilKeyAndValue(key)
+        if fkv is None or ckv is None:
+            return None
+        floorKey, floorValue = fkv
+        ceilKey, ceilValue = ckv
+        if ceilKey == floorKey:
+            return floorValue
+        else:
+            frac = (key - floorKey) / (ceilKey - floorKey)
+            return floorValue + (ceilValue - floorValue) * frac
+
+    def slice(self: T, lowerBoundKey=None, upperBoundKey=None, inner=True) -> T:
+        """
+        :param lowerBoundKey: the key defining the start of the slice (depending on inner);
+            if None, the first included entry will be the very first entry
+        :param upperBoundKey: the key defining the end of the slice (depending on inner);
+            if None, the last included entry will be the very last entry
+        :param inner: if True, the returned slice will be within the bounds; if False, the returned
+            slice is extended by one entry in both directions such that it contains the bounds (where possible)
+        :return:
+        """
+        if lowerBoundKey is not None and upperBoundKey is not None:
+            assert upperBoundKey >= lowerBoundKey
+        if lowerBoundKey is not None:
+            if inner:
+                fromIndex = self.ceilIndex(lowerBoundKey)
+                if fromIndex is None:
+                    fromIndex = len(self)  # shall return empty slice
+            else:
+                fromIndex = self.floorIndex(lowerBoundKey)
+                if fromIndex is None:
+                    fromIndex = 0
+        else:
+            fromIndex = 0
+        if upperBoundKey is not None:
+            if inner:
+                toIndex = self.floorIndex(upperBoundKey)
+                if toIndex is None:
+                    toIndex = -1  # shall return empty slice
+            else:
+                toIndex = self.ceilIndex(upperBoundKey)
+                if toIndex is None:
+                    toIndex = len(self) - 1
+        else:
+            toIndex = len(self) - 1
+        return self._createSlice(fromIndex, toIndex)
+
+    @abstractmethod
+    def _createSlice(self: T, fromIndex: int, toIndex: int) -> T:
+        pass
+
+
+class SortedKeysAndValues(Generic[TKey, TValue], SortedKeyValueStructure[TKey, TValue]):
+    def __init__(self, keys: Sequence[TKey], values: Sequence[TValue]):
+        """
+        :param keys: a sorted sequence of keys
+        :param values: a sequence of corresponding values
+        """
+        if len(keys) != len(values):
+            raise ValueError(f"Lengths of keys ({len(keys)}) and values ({len(values)}) do not match")
+        self.keys = keys
+        self.values = values
+
+    def __len__(self):
+        return len(self.keys)
+
+    @classmethod
+    def fromSeries(cls, s: pd.Series):
+        """
+        Creates an instance from a pandas Series, using the series' index as the keys and its values as the values
+
+        :param s: the series
+        :return: an instance
+        """
+        # noinspection PyTypeChecker
+        return cls(s.index, s.values)
+
+    def floorIndex(self, key) -> Optional[int]:
+        return array_util.floorIndex(self.keys, key)
+
+    def ceilIndex(self, key) -> Optional[int]:
+        return array_util.ceilIndex(self.keys, key)
+
+    def closestIndex(self, key) -> Optional[int]:
+        return array_util.closestIndex(self.keys, key)
+
+    def floorValue(self, key) -> Optional[TValue]:
+        return array_util.floorValue(self.keys, key, values=self.values)
+
+    def ceilValue(self, key) -> Optional[TValue]:
+        return array_util.ceilValue(self.keys, key, values=self.values)
+
+    def closestValue(self, key) -> Optional[TValue]:
         return array_util.closestValue(self.keys, key, values=self.values)
 
     def floorKeyAndValue(self, key) -> Optional[Tuple[TKey, TValue]]:
         idx = self.floorIndex(key)
         return None if idx is None else (self.keys[idx], self.values[idx])
 
     def ceilKeyAndValue(self, key) -> Optional[Tuple[TKey, TValue]]:
@@ -230,29 +345,41 @@
 
     def valueSliceInner(self, lowerBoundKey, upperBoundKey):
         return array_util.valueSliceInner(self.keys, lowerBoundKey, upperBoundKey, values=self.values)
 
     def valueSliceOuter(self, lowerBoundKey, upperBoundKey, fallback=False):
         return array_util.valueSliceOuter(self.keys, lowerBoundKey, upperBoundKey, values=self.values, fallbackBounds=fallback)
 
+    def _createSlice(self, fromIndex: int, toIndex: int) -> "SortedKeysAndValues":
+        return SortedKeysAndValues(self.keys[fromIndex:toIndex+1], self.values[fromIndex:toIndex+1])
+
 
-class SortedKeyValuePairs(Generic[TKey, TValue]):
+class SortedKeyValuePairs(Generic[TKey, TValue], SortedKeyValueStructure[TKey, TValue]):
     @classmethod
     def fromUnsortedKeyValuePairs(cls, unsortedKeyValuePairs: Sequence[Tuple[TKey, TValue]]):
         return cls(sorted(unsortedKeyValuePairs, key=lambda x: x[0]))
 
     def __init__(self, sortedKeyValuePairs: Sequence[Tuple[TKey, TValue]]):
         self.entries = sortedKeyValuePairs
         self._sortedKeys = SortedValues([t[0] for t in sortedKeyValuePairs])
 
+    def __len__(self):
+        return len(self.entries)
+
     def _value(self, idx: Optional[int]) -> Optional[TValue]:
         if idx is None:
             return None
         return self.entries[idx][1]
 
+    def valueForIndex(self, idx: int) -> TValue:
+        return self.entries[idx][1]
+
+    def keyForIndex(self, idx: int) -> TKey:
+        return self.entries[idx][0]
+
     def floorIndex(self, key) -> Optional[int]:
         """Finds the rightmost index where the key is less than or equal to the given key"""
         return self._sortedKeys.floorIndex(key)
 
     def floorValue(self, key) -> Optional[TValue]:
         return self._value(self.floorIndex(key))
 
@@ -273,42 +400,21 @@
 
     def closestIndex(self, key) -> Optional[int]:
         return self._sortedKeys.closestIndex(key)
 
     def closestValue(self, key) -> Optional[TValue]:
         return self._value(self.closestIndex(key))
 
-    def closestKeyAndValue(self, key):
+    def closestKeyAndValue(self, key) -> Optional[Tuple[TKey, TValue]]:
         idx = self.closestIndex(key)
         return None if idx is None else self.entries[idx]
 
     def _valueSlice(self, firstIndex, lastIndex):
         if firstIndex is None or lastIndex is None:
             return None
         return [e[1] for e in self.entries[firstIndex:lastIndex+1]]
 
     def valueSlice(self, lowestKey, highestKey) -> Optional[Sequence[TValue]]:
         return self._valueSlice(self.ceilIndex(lowestKey), self.floorIndex(highestKey))
 
-    def slice(self, lowerBoundKey=None, upperBoundKey=None, inner=True) -> "SortedKeyValuePairs":
-        """
-        :param lowerBoundKey: the key defining the start of the slice (depending on inner);
-            if None, the first included entry will be the very first entry
-        :param upperBoundKey: the key defining the end of the slice (depending on inner);
-            if None, the last included entry will be the very last entry
-        :param inner: if True, the returned slice will be within the bounds; if False, the the returned
-            slice is extended by one entry in both directions such that it contains the bounds (where possible)
-        :return:
-        """
-        if lowerBoundKey is not None:
-            fromIndex = self.ceilIndex(lowerBoundKey) if inner else self.floorIndex(lowerBoundKey)
-            if fromIndex is None:
-                fromIndex = 0
-        else:
-            fromIndex = 0
-        if upperBoundKey is not None:
-            toIndex = self.floorIndex(upperBoundKey) if inner else self.ceilIndex(upperBoundKey)
-            if toIndex is None:
-                toIndex = len(self.entries)
-        else:
-            toIndex = len(self.entries)
-        return SortedKeyValuePairs(self.entries[fromIndex:toIndex])
+    def _createSlice(self, fromIndex: int, toIndex: int) -> "SortedKeyValuePairs":
+        return SortedKeyValuePairs(self.entries[fromIndex:toIndex+1])
```

### Comparing `sensai-0.1.9/src/sensai/util/dtype.py` & `sensai-0.2.0/src/sensai/util/dtype.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/hash.py` & `sensai-0.2.0/src/sensai/util/hash.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/helper.py` & `sensai-0.2.0/src/sensai/util/helper.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/logging.py` & `sensai-0.2.0/src/sensai/util/logging.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import atexit
+from datetime import datetime
 import logging as lg
 from logging import *
 import sys
 import time
 from typing import List, Tuple
 
 import pandas as pd
 
+
 log = getLogger(__name__)
 
 LOG_DEFAULT_FORMAT = '%(levelname)-5s %(asctime)-15s %(name)s:%(funcName)s - %(message)s'
 
 
 def removeLogHandlers():
     """
@@ -30,14 +32,21 @@
     basicConfig(level=level, format=format, stream=sys.stdout)
     getLogger("matplotlib").setLevel(lg.INFO)
     getLogger("urllib3").setLevel(lg.INFO)
     getLogger("msal").setLevel(lg.INFO)
     pd.set_option('display.max_colwidth', 255)
 
 
+def datetimeTag() -> str:
+    """
+    :return: a string tag for use in log file names which contains the current date and time (compact but readable)
+    """
+    return datetime.now().strftime('%Y%m%d-%H%M%S')
+
+
 _fileLoggerPaths: List[str] = []
 _isAtExitReportFileLoggerRegistered = False
 
 
 def _atExitReportFileLogger():
     for path in _fileLoggerPaths:
         print(f"A log file was saved to {path}")
@@ -55,27 +64,77 @@
         _isAtExitReportFileLoggerRegistered = True
 
 
 class StopWatch:
     """
     Represents a stop watch for timing an execution. Constructing an instance starts the stopwatch.
     """
-    def __init__(self):
+    def __init__(self, start=True):
         self.startTime = time.time()
+        self._elapsedSecs = 0.0
+        self.isRunning = start
 
-    def restart(self):
+    def reset(self, start=True):
+        """
+        Resets the stopwatch, setting the elapsed time to zero.
+
+        :param start: whether to start the stopwatch immediately
+        """
         self.startTime = time.time()
+        self._elapsedSecs = 0.0
+        self.isRunning = start
+
+    def restart(self):
+        """
+        Resets the stopwatch (setting the elapsed time to zero) and restarts it immediately
+        """
+        self.reset(start=True)
+
+    def _getElapsedTimeSinceLastStart(self):
+        if self.isRunning:
+            return time.time() - self.startTime
+        else:
+            return 0
+
+    def pause(self):
+        """
+        Pauses the stopwatch. It can be resumed via method 'resume'.
+        """
+        self._elapsedSecs += self._getElapsedTimeSinceLastStart()
+        self.isRunning = False
+
+    def resume(self):
+        """
+        Resumes the stopwatch (assuming that it is currently paused). If the stopwatch is not paused,
+        the method has no effect (and a warning is logged).
+        """
+        if not self.isRunning:
+            self.startTime = time.time()
+            self.isRunning = True
+        else:
+            log.warning("Stopwatch is already running (resume has not effect)")
 
     def getElapsedTimeSecs(self) -> float:
-        return time.time() - self.startTime
+        """
+        Gets the total elapsed time, in seconds, on this stopwatch.
+
+        :return: the elapsed time in seconds
+        """
+        return self._elapsedSecs + self._getElapsedTimeSinceLastStart()
 
     def getElapsedTimedelta(self) -> pd.Timedelta:
+        """
+        :return: the elapsed time as a pandas.Timedelta object
+        """
         return pd.Timedelta(self.getElapsedTimeSecs(), unit="s")
 
     def getElapsedTimeString(self) -> str:
+        """
+        :return: a string representation of the elapsed time
+        """
         secs = self.getElapsedTimeSecs()
         if secs < 60:
             return f"{secs:.3f} seconds"
         else:
             return str(pd.Timedelta(secs, unit="s"))
```

### Comparing `sensai-0.1.9/src/sensai/util/math.py` & `sensai-0.2.0/src/sensai/util/math.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import math
+from typing import List
+
 import scipy.stats
 
-from .string import objectRepr
+from .string import objectRepr, ToStringMixin
 
 
-class NormalDistribution:
+class NormalDistribution(ToStringMixin):
     def __init__(self, mean=0, std=1, unitMax=False):
         """
         :param mean: the mean
         :param std: the standard deviation
         :param unitMax: if True, scales the distribution's pdf such that its maximum value becomes 1
         """
         self.unitMax = unitMax
         self.mean = mean
         self.std = std
         self.norm = scipy.stats.norm(loc=mean, scale=std)
 
+    def _toStringIncludes(self) -> List[str]:
+        return ["mean", "std", "unitMax"]
+
     def pdf(self, x):
         v = self.norm.pdf(x)
         if self.unitMax:
             v /= self.norm.pdf(self.mean)
         return v
 
     def __str__(self):
```

### Comparing `sensai-0.1.9/src/sensai/util/multiprocessing.py` & `sensai-0.2.0/src/sensai/util/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/pandas.py` & `sensai-0.2.0/src/sensai/util/pandas.py`

 * *Files 5% similar despite different names*

```diff
@@ -121,7 +121,22 @@
             arr = arr[0]
     except ValueError:
         raise ValueError(f"No array can be extracted from frame of length {len(df)} with columns {list(df.columns)}. "
                          f"Make sure that all entries have the same shape")
     if dtype is not None:
         arr = arr.astype(dtype, copy=False)
     return arr
+
+
+def removeDuplicateIndexEntries(df: pd.DataFrame):
+    """
+    Removes successive duplicate index entries by keeping only the first occurrence for every duplicate index element.
+
+    :param df: the data frame, which is assumed to have a sorted index
+    :return: the (modified) data frame with duplicate index entries removed
+    """
+    keep = [True]
+    prevItem = df.index[0]
+    for item in df.index[1:]:
+        keep.append(item != prevItem)
+        prevItem = item
+    return df[keep]
```

### Comparing `sensai-0.1.9/src/sensai/util/pickle.py` & `sensai-0.2.0/src/sensai/util/pickle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,49 @@
 import logging
 import os
 import pickle
 from typing import List, Dict, Any, Iterable
 
 import joblib
 
+from .io import isS3Path, S3Object
+
 log = logging.getLogger(__name__)
 
 
 def loadPickle(path, backend="pickle"):
-    with open(path, "rb") as f:
+    def readFile(f):
         if backend == "pickle":
-            return pickle.load(f)
+            try:
+                return pickle.load(f)
+            except:
+                log.error(f"Error loading {path}")
+                raise
         elif backend == "joblib":
             return joblib.load(f)
         else:
             raise ValueError(f"Unknown backend '{backend}'")
 
+    if isS3Path(path):
+        return readFile(S3Object(path).openFile("rb"))
+    with open(path, "rb") as f:
+        return readFile(f)
+
 
 def dumpPickle(obj, picklePath, backend="pickle", protocol=pickle.HIGHEST_PROTOCOL):
+    def openFile():
+        if isS3Path(picklePath):
+            return S3Object(picklePath).openFile("wb")
+        else:
+            return open(picklePath, "wb")
+
     dirName = os.path.dirname(picklePath)
     if dirName != "":
         os.makedirs(dirName, exist_ok=True)
-    with open(picklePath, "wb") as f:
+    with openFile() as f:
         if backend == "pickle":
             try:
                 pickle.dump(obj, f, protocol=protocol)
             except AttributeError as e:
                 failingPaths = PickleFailureDebugger.debugFailure(obj)
                 raise AttributeError(f"Cannot pickle paths {failingPaths} of {obj}: {str(e)}")
         elif backend == "joblib":
@@ -111,27 +128,28 @@
             if len(failures) > 0:
                 log.error(f"{prefix}: pickling would result in failures due to: {failures}")
             else:
                 log.info(f"{prefix}: is picklable")
 
 
 def setstate(cls, obj, state: Dict[str, Any], renamedProperties: Dict[str, str] = None, newOptionalProperties: List[str] = None,
-        newDefaultProperties: Dict[str, Any] = None) -> None:
+        newDefaultProperties: Dict[str, Any] = None, removedProperties: List[str] = None) -> None:
     """
     Helper function for safe implementations of __setstate__ in classes, which appropriately handles the cases where
     a parent class already implements __setstate__ and where it does not. Call this function whenever you would actually
     like to call the super-class' implementation.
     Unfortunately, __setstate__ is not implemented in object, rendering super().__setstate__(state) invalid in the general case.
 
     :param cls: the class in which you are implementing __setstate__
     :param obj: the instance of cls
     :param state: the state dictionary
     :param renamedProperties: a mapping from old property names to new property names
     :param newOptionalProperties: a list of names of new property names, which, if not present, shall be initialised with None
     :param newDefaultProperties: a dictionary mapping property names to their default values, which shall be added if they are not present
+    :param removedProperties: a list of names of properties that are no longer being used
     """
     # handle new/changed properties
     if renamedProperties is not None:
         for mOld, mNew in renamedProperties.items():
             if mOld in state:
                 state[mNew] = state[mOld]
                 del state[mOld]
@@ -139,36 +157,42 @@
         for mNew in newOptionalProperties:
             if mNew not in state:
                 state[mNew] = None
     if newDefaultProperties is not None:
         for mNew, mValue in newDefaultProperties.items():
             if mNew not in state:
                 state[mNew] = mValue
+    if removedProperties is not None:
+        for p in removedProperties:
+            if p in state:
+                del state[p]
     # call super implementation, if any
     s = super(cls, obj)
     if hasattr(s, '__setstate__'):
         s.__setstate__(state)
     else:
         obj.__dict__ = state
 
 
 def getstate(cls, obj, transientProperties: Iterable[str] = None, excludedProperties: Iterable[str] = None,
-        overrideProperties: Dict[str, Any] = None) -> Dict[str, Any]:
+             overrideProperties: Dict[str, Any] = None, excludedDefaultProperties: Dict[str, Any] = None) -> Dict[str, Any]:
     """
     Helper function for safe implementations of __getstate__ in classes, which appropriately handles the cases where
     a parent class already implements __getstate__ and where it does not. Call this function whenever you would actually
     like to call the super-class' implementation.
     Unfortunately, __getstate__ is not implemented in object, rendering super().__getstate__() invalid in the general case.
 
     :param cls: the class in which you are implementing __getstate__
     :param obj: the instance of cls
     :param transientProperties: transient properties which be set to None in serialisations
     :param excludedProperties: properties which shall be completely removed from serialisations
     :param overrideProperties: a mapping from property names to values specifying (new or existing) properties which are to be set;
         use this to set a fixed value for an existing property or to add a completely new property
+    :param excludedDefaultProperties: properties which shall be completely removed from serialisations, if they are set
+        to the given default value
     :return: the state dictionary, which may be modified by the receiver
     """
     s = super(cls, obj)
     if hasattr(s, '__getstate__'):
         d = s.__getstate__()
     else:
         d = obj.__dict__.copy()
@@ -179,8 +203,12 @@
     if excludedProperties is not None:
         for p in excludedProperties:
             if p in d:
                 del d[p]
     if overrideProperties is not None:
         for k, v in overrideProperties.items():
             d[k] = v
+    if excludedDefaultProperties is not None:
+        for p, v in excludedDefaultProperties.items():
+            if p in d and d[p] == v:
+                del d[p]
     return d
```

### Comparing `sensai-0.1.9/src/sensai/util/profiling.py` & `sensai-0.2.0/src/sensai/util/profiling.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai/util/sequences.py` & `sensai-0.2.0/src/sensai/util/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     floorIdx = floorIndex(arr, value)
     if floorIdx is None:
         return 0
     ceilIdx = floorIdx + 1
     if ceilIdx >= length:
         return floorIdx
     floorValue = arr[floorIdx]
-    ceilValue = arr[floorIdx]
+    ceilValue = arr[ceilIdx]
     floorDist = abs(floorValue - value)
     ceilDist = abs(ceilValue - value)
     if floorDist <= ceilDist:
         return floorIdx
     else:
         return ceilIdx
```

### Comparing `sensai-0.1.9/src/sensai/util/string.py` & `sensai-0.2.0/src/sensai/util/string.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,16 @@
     def _toStringObjectInfo(self) -> str:
         """
         Override this method to use a fully custom definition of the ``<object info>`` part in the full string
         representation ``"<class name>[<object info>]"`` to be generated.
         As soon as this method is overridden, any property-based exclusions, inclusions, etc. will have no effect
         (unless the implementation is specifically designed to make use of them - as is the default
         implementation).
+        NOTE: Overrides must not internally use super() because of a technical limitation in the proxy
+        object that is used for nested object structures.
 
         :return: a string containing the string to use for ``<object info>``
         """
         return self._toStringProperties(exclude=self._toStringExcludes(), include=self._toStringIncludes(),
             excludeExceptions=self._toStringExcludeExceptions(), includeForced=self._toStringIncludesForced(),
             additionalEntries=self._toStringAdditionalEntries())
 
@@ -345,28 +347,33 @@
         class _ToStringMixinProxy:
             """
             A proxy object which wraps a ToStringMixin to ensure that the converter is applied when creating the properties string.
             The proxy is to achieve that all ToStringMixin methods that aren't explicitly overwritten are bound to this proxy
             (rather than the original object), such that the transitive call to _toStringProperties will call the new
             implementation.
             """
+
+            # methods where we assume that they could transitively call _toStringProperties (others are assumed not to)
+            TOSTRING_METHODS_TRANSITIVELY_CALLING_TOSTRINGPROPERTIES = set(["_toStringObjectInfo"])
+
             def __init__(self, x: "ToStringMixin", converter):
                 self.x = x
                 self.converter = converter
 
             def _toStringProperties(self, *args, **kwargs):
                 return self.x._toStringProperties(*args, **kwargs, converter=self.converter)
 
             def _toStringClassName(self):
                 return self.x._toStringClassName()
 
             def __getattr__(self, attr: str):
-                if attr.startswith("_toString"):  # ToStringMixin method which we bind to use this proxy
+                if attr.startswith("_toString"):  # ToStringMixin method which we may bind to use this proxy to ensure correct transitive call
                     method = getattr(self.x.__class__, attr)
-                    return lambda *args, **kwargs: method(self, *args, **kwargs)
+                    obj = self if attr in self.TOSTRING_METHODS_TRANSITIVELY_CALLING_TOSTRINGPROPERTIES else self.x
+                    return lambda *args, **kwargs: method(obj, *args, **kwargs)
                 else:
                     return getattr(self.x, attr)
 
             def __str__(self: "ToStringMixin"):
                 return ToStringMixin.__str__(self)
```

### Comparing `sensai-0.1.9/src/sensai/vector_model.py` & `sensai-0.2.0/src/sensai/vector_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 """
 This module defines base classes for models that use pandas.DataFrames for inputs and outputs, where each data frame row represents
 a single model input or output. Since every row contains a vector of data (one-dimensional array), we refer to them as vector-based
 models. Hence the name of the module and of the central base class :class:`VectorModel`.
 """
 
 import logging
+import typing
 from abc import ABC, abstractmethod
 from typing import List, Any, Optional, Union, Type, Dict
 
 import numpy as np
 import pandas as pd
 
-from sensai.util.deprecation import deprecated
+from .util.deprecation import deprecated
 from .data import InputOutputData
 from .data_transformation import DataFrameTransformer, DataFrameTransformerChain, InvertibleDataFrameTransformer
 from .featuregen import FeatureGenerator, FeatureCollector
 from .util import markUsed
 from .util.cache import PickleLoadSaveMixin
 from .util.logging import StopWatch
 from .util.pickle import setstate, getstate
 from .util.sequences import getFirstDuplicate
 from .util.string import ToStringMixin
 
 markUsed(InputOutputData)  # for backward compatibility
 
 log = logging.getLogger(__name__)
+TVectorModelBase = typing.TypeVar("TVectorModelBase", bound="VectorModelBase")
+TVectorModel = typing.TypeVar("TVectorModel", bound="VectorModel")
+TVectorRegressionModel = typing.TypeVar("TVectorRegressionModel", bound="VectorRegressionModel")
 
 
 class VectorModelBase(ABC):
     """
     Base class for vector models, which defines the fundamental prediction interface.
     A vector model takes data frames as input, where each row represents a vector of information.
     """
@@ -43,15 +47,15 @@
     def isRegressionModel(self) -> bool:
         pass
 
     @abstractmethod
     def getPredictedVariableNames(self) -> list:
         pass
 
-    def withName(self, name: str):
+    def withName(self: TVectorModelBase, name: str) -> TVectorModelBase:
         """
         Sets the model's name.
 
         :param name: the name
         :return: self
         """
         self.setName(name)
@@ -144,65 +148,71 @@
         d = super()._toStringAdditionalEntries()
         if self._featureGenerator is not None:
             d["featureGeneratorNames"] = self._featureGenerator.getNames()
         if self._name is not None:
             d["name"] = self._name
         return d
 
-    def withRawInputTransformers(self, *transformers: Union[DataFrameTransformer, List[DataFrameTransformer]]):
+    def withRawInputTransformers(self: TVectorModel, *transformers: Union[DataFrameTransformer, List[DataFrameTransformer]]) -> TVectorModel:
         """
         Makes the model use the given transformers (removing previously set raw input transformers, if any), which
         are to be applied to the raw input data frame (prior to feature generation).
 
         :param transformers: :class:`DataFrameTransformer` instances to use (in sequence) for the transformation of inputs
         :return: self
         """
         self._rawInputTransformerChain = DataFrameTransformerChain(*transformers)
         return self
 
-    def withFeatureTransformers(self, *transformers: Union[DataFrameTransformer, List[DataFrameTransformer]]) -> __qualname__:
+    def withFeatureTransformers(self: TVectorModel, *transformers: Union[DataFrameTransformer, List[DataFrameTransformer]],
+            add=False) -> TVectorModel:
         """
-        Makes the model use the given transformers (removing previously set feature transformers, if any),
+        Makes the model use the given transformers
         which are to be applied to the data frames generated by feature generators.
         (If the model does not use feature generators, the transformers will be applied to
         whatever is produced by the raw input transformers or, if there are none, the original raw
         input data frame).
 
         :param transformers: :class:`DataFrameTransformer` instances to use (in sequence) for the transformation of features
+        :param add: whether to add the transformers to the existing transformers rather than replacing them
         :return: self
         """
-        self._featureTransformerChain = DataFrameTransformerChain(*transformers)
+        if not add:
+            self._featureTransformerChain = DataFrameTransformerChain(*transformers)
+        else:
+            for t in transformers:
+                self._featureTransformerChain.append(t)
         return self
 
     @deprecated("Use withFeatureTransformers instead; this method will be removed in a future sensAI release.")
-    def withInputTransformers(self, *inputTransformers: Union[DataFrameTransformer, List[DataFrameTransformer]]) -> __qualname__:
+    def withInputTransformers(self: TVectorModel, *inputTransformers: Union[DataFrameTransformer, List[DataFrameTransformer]]) -> TVectorModel:
         """
         Makes the model use the given feature transformers (removing previously set transformers, if any),
         i.e. it transforms the data frame that is generated by the feature generators (if any).
 
         :param inputTransformers: :class:`DataFrameTransformer` instances to use (in sequence) for the transformation of inputs
         :return: self
         """
         return self.withFeatureTransformers(*inputTransformers)
 
-    def withFeatureGenerator(self, featureGenerator: Optional[FeatureGenerator]) -> __qualname__:
+    def withFeatureGenerator(self: TVectorModel, featureGenerator: Optional[FeatureGenerator]) -> TVectorModel:
         """
         Makes the model use the given feature generator in order to obtain the model inputs.
         If the model shall use more than one feature generator, pass a :class:`MultiFeatureGenerator` which combines them or
         use the perhaps more convenient :class:`FeatureCollector` in conjunction with :meth:`withFeatureCollector`.
 
         Note: Feature computation takes place before input transformation.
 
         :param featureGenerator: the feature generator to use for input computation
         :return: self
         """
         self._featureGenerator = featureGenerator
         return self
 
-    def withFeatureCollector(self, featureCollector: FeatureCollector) -> __qualname__:
+    def withFeatureCollector(self: TVectorModel, featureCollector: FeatureCollector) -> TVectorModel:
         """
         Makes the model use the given feature collector's multi-feature generator
         in order compute the underlying model's input from the data frame that is given.
         Overrides any feature generator previously passed to :meth:`withFeatureGenerator` (if any).
 
         Note: Feature computation takes place before input transformation.
 
@@ -498,15 +508,15 @@
         if self.TOSTRING_INCLUDE_PREPROCESSORS:
             e += ["_targetTransformer"]
         return e
 
     def isRegressionModel(self) -> bool:
         return True
 
-    def withOutputTransformers(self, *outputTransformers: Union[DataFrameTransformer, List[DataFrameTransformer]]) -> __qualname__:
+    def withOutputTransformers(self: TVectorRegressionModel, *outputTransformers: Union[DataFrameTransformer, List[DataFrameTransformer]]) -> TVectorRegressionModel:
         """
         Makes the model use the given output transformers. Call with empty input to remove existing output transformers.
         The transformers are ignored during the fit phase. Not supported for rule-based models.
 
         **Important**: The output columns names of the last output transformer should be the same
         as the first one's input column names. If this fails to hold, an exception will be raised when :meth:`predict` is called.
 
@@ -527,15 +537,15 @@
         """
         # There is no reason for post processing in rule-based models
         if not self._underlyingModelRequiresFitting():
             raise Exception(f"Output transformers are not supported for model of type {self.__class__.__name__}")
         self._outputTransformerChain = DataFrameTransformerChain(*outputTransformers)
         return self
 
-    def withTargetTransformer(self, targetTransformer: Optional[InvertibleDataFrameTransformer]) -> __qualname__:
+    def withTargetTransformer(self: TVectorRegressionModel, targetTransformer: Optional[InvertibleDataFrameTransformer]) -> TVectorRegressionModel:
         """
         Makes the model use the given target transformers such that the underlying low-level model is trained on the transformed
         targets, but this high-level model still outputs the original (untransformed) values, i.e. the transformation is applied
         to targets during training and the inverse transformation is applied to the underlying model's predictions during inference.
         Hence the requirement of  the transformer being invertible.
 
         This method is not supported for rule-based models, because they are not trained and therefore the transformation
```

### Comparing `sensai-0.1.9/src/sensai/vectoriser.py` & `sensai-0.2.0/src/sensai/vectoriser.py`

 * *Files identical despite different names*

### Comparing `sensai-0.1.9/src/sensai.egg-info/SOURCES.txt` & `sensai-0.2.0/src/sensai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 src/sensai/lightgbm.py
 src/sensai/local_search.py
 src/sensai/minizinc.py
 src/sensai/multi_model.py
 src/sensai/naive_bayes.py
 src/sensai/nearest_neighbors.py
 src/sensai/normalisation.py
+src/sensai/sklearn_quantile.py
 src/sensai/tensor_model.py
 src/sensai/vector_model.py
 src/sensai/vectoriser.py
 src/sensai/xgboost.py
 src/sensai.egg-info/PKG-INFO
 src/sensai.egg-info/SOURCES.txt
 src/sensai.egg-info/dependency_links.txt
@@ -97,18 +98,21 @@
 src/sensai/util/cache_mysql.py
 src/sensai/util/datastruct.py
 src/sensai/util/deprecation.py
 src/sensai/util/dtype.py
 src/sensai/util/hash.py
 src/sensai/util/helper.py
 src/sensai/util/io.py
+src/sensai/util/jscode.py
 src/sensai/util/logging.py
 src/sensai/util/math.py
 src/sensai/util/multiprocessing.py
 src/sensai/util/pandas.py
 src/sensai/util/pickle.py
 src/sensai/util/plot.py
 src/sensai/util/profiling.py
 src/sensai/util/sequences.py
 src/sensai/util/string.py
+src/sensai/util/test.py
 src/sensai/util/time.py
-src/sensai/util/typing.py
+src/sensai/util/typing.py
+src/sensai/util/version.py
```

