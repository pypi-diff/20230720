# Comparing `tmp/tensorflow-gnn-0.5.1.tar.gz` & `tmp/tensorflow-gnn-0.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorflow-gnn-0.5.1.tar", last modified: Mon Jun 12 14:40:09 2023, max compression
+gzip compressed data, was "tensorflow-gnn-0.6.0rc0.tar", last modified: Thu Jul 20 17:59:41 2023, max compression
```

## Comparing `tensorflow-gnn-0.5.1.tar` & `tensorflow-gnn-0.6.0rc0.tar`

### file list

```diff
@@ -1,258 +1,318 @@
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      304 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/AUTHORS
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1481 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11357 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/LICENSE
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      177 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/MANIFEST.in
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5503 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/PKG-INFO
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4203 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/README.md
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/WORKSPACE
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/package/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      412 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/package/BUILD
--rwxrwxr-x   0 mparadkar (603057) primarygroup (89939)     1577 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/package/move_generated_files.sh
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      495 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/package/tfdep.bzl
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)       38 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/setup.cfg
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7191 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/setup.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1659 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8288 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/__init__.py
--rwxrwxr-x   0 mparadkar (603057) primarygroup (89939)    17657 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3645 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/ogb_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3291 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1567 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/data/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      986 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    41551 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31879 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1354 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31688 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/datasets.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    35246 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12073 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13830 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/models.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3138 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/reader_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11388 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11598 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11249 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20856 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13080 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    39354 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32323 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1289 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1348 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3857 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_constants.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    40947 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28985 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    60355 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6176 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5885 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20524 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27804 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    56326 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    73049 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2735 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1587 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12963 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6123 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    53315 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2635 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5414 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9065 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26955 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26711 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9088 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12726 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10402 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16641 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15373 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1134 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1361 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19393 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12925 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2286 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1220 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6146 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9557 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14463 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_e2e_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5581 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13354 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6229 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1679 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19603 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15800 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6516 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5791 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27129 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25880 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25485 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10300 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2904 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3874 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16646 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    23849 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10818 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4589 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2478 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3698 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2149 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6313 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.434229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      735 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1406 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/__init__.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1871 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5488 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2513 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2407 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3720 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4320 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1648 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/layers.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1022 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1252 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27602 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26525 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      886 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1030 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11839 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19154 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      759 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      998 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16777 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/tensor_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16678 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/tensor_utils_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1285 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    34468 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    23956 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      855 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1048 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2984 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5181 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2395 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1566 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3059 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2906 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1599 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    36816 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    46770 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1446 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2225 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2915 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2157 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1296 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4911 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4242 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1013 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1023 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/examples.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11444 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2895 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2887 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4590 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8308 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/distribute_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      841 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12378 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/train.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      675 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19957 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9151 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6910 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/interfaces.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13882 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5171 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1381 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10249 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8177 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/regression.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5650 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/regression_test.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.438229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      373 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11673 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/keras_fit.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3268 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12942 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9399 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2243 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1324 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_dir.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6786 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9185 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2696 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_templates.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4916 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4245 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/padding.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2576 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4907 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1873 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/strategies.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1885 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19137 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22306 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22774 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32206 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6762 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15163 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6212 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4931 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5281 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2123 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13461 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16517 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2629 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tensorflow_gnn.bzl
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      455 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/__init__.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3368 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1375 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3926 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2080 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2700 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.proto
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8109 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1975 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats_test.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1742 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/tools/validate_graph_schema.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      272 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/BUILD
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/__init__.py
--rwxrwxr-x   0 mparadkar (603057) primarygroup (89939)     2116 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/utils/test_utils.py
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2128 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/tensorflow_gnn/version.py
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.430229 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5503 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/PKG-INFO
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)     9057 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/SOURCES.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/dependency_links.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)      459 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/entry_points.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/namespace_packages.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-06-12 14:39:07.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/not-zip-safe
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)      242 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/requires.txt
--rw-r--r--   0 mparadkar (603057) primarygroup (89939)       27 2023-06-12 14:40:09.000000 tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/top_level.txt
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      167 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/heterogeneous/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      420 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/heterogeneous/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/homogeneous/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      294 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/homogeneous/BUILD
-drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-06-12 14:40:09.442229 tensorflow-gnn-0.5.1/testdata/node_vs_edge/
--rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      295 2023-06-12 14:31:40.000000 tensorflow-gnn-0.5.1/testdata/node_vs_edge/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      304 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/AUTHORS
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1481 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11357 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/LICENSE
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      177 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/MANIFEST.in
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5322 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/PKG-INFO
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4019 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/README.md
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1392 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/WORKSPACE
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/package/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      477 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/package/BUILD
+-rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     1633 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/package/move_generated_files.sh
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      953 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/package/tfdep.bzl
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)       38 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/setup.cfg
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7305 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/setup.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2072 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9298 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/__init__.py
+-rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)    17657 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1386 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3645 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/ogb_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3291 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1567 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1141 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    41983 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31879 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1475 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    45889 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2874 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    38944 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18108 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13960 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/models.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4786 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2589 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3138 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/reader_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11411 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11598 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      840 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2230 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/__init__.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.455089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5537 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7559 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/accessors.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9061 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/accessors_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15545 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12823 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    24769 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8426 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9854 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4272 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4018 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27898 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5391 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5926 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/beam/utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    56324 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/core.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    46060 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/core_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7585 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/custom_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5659 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28756 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    30581 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/eval_dag_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6359 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3590 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_parallel.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11443 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6255 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8061 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/interfaces.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18838 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/link_samplers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14953 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/link_samplers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11911 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13508 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.455089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14334 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20785 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13080 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    39354 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32323 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11447 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/broadcast_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14107 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/broadcast_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1289 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1348 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3920 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_constants.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    40849 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28881 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    63673 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6176 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5885 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20523 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27804 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    45886 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    67747 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2735 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1587 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10963 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5892 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    62064 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2635 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6722 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10486 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27049 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26711 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    34642 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/pool_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22200 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/pool_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7818 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9088 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28826 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/readout.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    20098 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/readout_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12726 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10402 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17764 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16543 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5192 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tag_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4878 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tag_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19429 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12925 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2984 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tf_internal.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.455089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2982 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1307 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10481 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/builders.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15288 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/builders_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2888 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/initializers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2005 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/initializers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14805 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_e2e_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5740 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13602 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6490 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2016 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19666 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15800 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6681 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5907 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    38598 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    54518 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    25526 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10300 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2904 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3874 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19343 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    26710 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11360 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6587 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2478 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6795 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2149 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6313 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.447089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2880 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1356 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6852 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/distribute_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11577 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    15368 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/layers_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6262 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/losses.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5509 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/losses_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6836 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/metrics.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5301 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/metrics_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8940 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/tasks.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10842 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/tasks_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2367 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1467 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2390 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3051 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2867 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1585 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    28134 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31034 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      983 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1030 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14098 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    31982 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      999 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1285 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    33753 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    27737 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2219 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1207 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2354 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3483 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2678 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1498 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16008 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32549 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.459089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2467 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1437 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2784 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2966 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3615 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2318 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19186 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17202 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/mt_albis/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2395 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1566 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2433 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3134 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2906 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1599 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    37373 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    54358 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2399 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1446 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2263 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2990 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2157 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1296 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5260 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7798 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1013 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1023 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/examples.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12144 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2895 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2932 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4908 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8291 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/distribute_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.447089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.447089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1576 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    17093 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2697 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3158 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      801 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19958 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9151 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9286 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/interfaces.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    24069 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/orchestration.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11036 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/orchestration_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2114 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11452 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    12562 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     8859 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/link_prediction.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6188 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/link_prediction_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    11453 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/regression.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18994 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/regression_test.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.463089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      499 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13322 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/keras_fit.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2974 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    14492 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10359 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2438 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/label_fns.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1324 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_dir.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7788 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     9780 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4245 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/padding.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2576 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4907 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1873 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/strategies.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1885 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      424 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    19089 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22306 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    22774 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    32206 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     6762 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    18498 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    10322 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     4931 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     5281 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2123 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    13461 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)    16517 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2769 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tensorflow_gnn.bzl
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      455 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/__init__.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3368 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1375 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     3926 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2080 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2700 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.proto
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     7984 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1975 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats_test.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     1742 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/validate_graph_schema.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      343 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/BUILD
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/__init__.py
+-rwxr-xr-x   0 mparadkar (603057) primarygroup (89939)     2116 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/test_utils.py
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)     2131 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn/version.py
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.451089 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)     5322 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/PKG-INFO
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)    11918 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/SOURCES.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/dependency_links.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)      459 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/entry_points.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/namespace_packages.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)        1 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/not-zip-safe
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)      244 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/requires.txt
+-rw-r--r--   0 mparadkar (603057) primarygroup (89939)       22 2023-07-20 17:59:41.000000 tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/top_level.txt
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      238 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/heterogeneous/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      420 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/heterogeneous/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/homogeneous/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      294 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/homogeneous/BUILD
+drwxr-xr-x   0 mparadkar (603057) primarygroup (89939)        0 2023-07-20 17:59:41.467089 tensorflow-gnn-0.6.0rc0/testdata/node_vs_edge/
+-rw-rw-r--   0 mparadkar (603057) primarygroup (89939)      366 2023-07-20 17:52:38.000000 tensorflow-gnn-0.6.0rc0/testdata/node_vs_edge/BUILD
```

### Comparing `tensorflow-gnn-0.5.1/BUILD` & `tensorflow-gnn-0.6.0rc0/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/LICENSE` & `tensorflow-gnn-0.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/PKG-INFO` & `tensorflow-gnn-0.6.0rc0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 0.5.1
+Version: 0.6.0rc0
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
@@ -30,18 +30,14 @@
 License-File: AUTHORS
 
 # TensorFlow GNN
 
 **This is an early (alpha) release to get community feedback.** It's under
 active development and **we may break API compatibility in the future**.
 
-> **NOTE**:
-> 2023/01/11: Release 0.4.1 was yanked due to a broken merge that passed through
-> our tests. Release 0.4.0 still works, and we are working on a new release,
-> stay tuned.
 
 TensorFlow GNN is a library to build Graph Neural Networks on the TensorFlow
 platform. It contains the following components:
 
 * A high-level Keras-style API to create GNN models that can easily be composed
   with other types of models. GNNs are often used in combination with ranking,
   deep-retrieval (dual-encoders) or mixed with other types of models
```

### Comparing `tensorflow-gnn-0.5.1/README.md` & `tensorflow-gnn-0.6.0rc0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 # TensorFlow GNN
 
 **This is an early (alpha) release to get community feedback.** It's under
 active development and **we may break API compatibility in the future**.
 
-> **NOTE**:
-> 2023/01/11: Release 0.4.1 was yanked due to a broken merge that passed through
-> our tests. Release 0.4.0 still works, and we are working on a new release,
-> stay tuned.
 
 TensorFlow GNN is a library to build Graph Neural Networks on the TensorFlow
 platform. It contains the following components:
 
 * A high-level Keras-style API to create GNN models that can easily be composed
   with other types of models. GNNs are often used in combination with ranking,
   deep-retrieval (dual-encoders) or mixed with other types of models
```

### Comparing `tensorflow-gnn-0.5.1/package/move_generated_files.sh` & `tensorflow-gnn-0.6.0rc0/package/move_generated_files.sh`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
   else
     # If run by "bazel run", $(pwd) is the .runfiles dir that contains all the
     # data dependencies.
     GENFILES=$(pwd)
   fi
 
   FILES="
+    tensorflow_gnn/experimental/sampler/eval_dag_pb2.py
     tensorflow_gnn/proto/graph_schema_pb2.py
     tensorflow_gnn/proto/examples_pb2.py
     tensorflow_gnn/sampler/sampling_spec_pb2.py
     tensorflow_gnn/sampler/subgraph_pb2.py
     tensorflow_gnn/tools/sampled_stats_pb2.py
   "
   for FILE in ${FILES}; do
```

### Comparing `tensorflow-gnn-0.5.1/setup.py` & `tensorflow-gnn-0.6.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,23 +164,25 @@
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     namespace_packages=[],
     install_requires=[
-        'apache-beam<2.47.0',
         'google-vizier>=0.0.13',
         'ml-collections',
         'networkx',
         'pyarrow',
         # pylint:disable=g-line-too-long
-        'tensorflow>=2.9.0; platform_machine != "arm64" or platform_system != "Darwin"',
-        'tensorflow-macos>=2.9.0; platform_machine == "arm64" and platform_system == "Darwin"',
+        'tensorflow>=2.10.0; platform_machine != "arm64" or platform_system != "Darwin"',
+        'tensorflow-macos>=2.10.0; platform_machine == "arm64" and platform_system == "Darwin"',
         # pylint:enable=g-line-too-long
+        # TODO(b/283835852): Unpin beam version when all supported TF versions
+        # enable protobuf >=3.20
+        'apache-beam<2.47.0',
     ],
     python_requires='>=3.8,<4',
     packages=find_namespace_packages(
         exclude=['examples*', 'package*', 'testdata*'],
     ),
     include_package_data=True,
     package_data={'': ['*.proto']},
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/BUILD`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
+load("@rules_license//rules:license.bzl", "license")
 
-package(default_visibility = ["//visibility:public"])
+package(
+    default_applicable_licenses = [":license"],
+    default_visibility = ["//visibility:public"],
+)
+
+license(
+    name = "license",
+    package_name = "tensorflow_gnn",
+    license_kinds = [
+        "@rules_license//licenses/spdx:Apache-2.0",
+    ],
+)
 
 licenses(["notice"])
 
 exports_files(["LICENSE"])
 
 config_setting(
     name = "no_tfgnn_py_deps",
@@ -14,34 +26,38 @@
 
 pytype_strict_library(
     name = "tensorflow_gnn",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
     visibility = ["//visibility:public"],
     deps = [
-        "//tensorflow_gnn:version",
+        ":version",
         "//tensorflow_gnn/experimental",
         "//tensorflow_gnn/graph:adjacency",
         "//tensorflow_gnn/graph:batching_utils",
+        "//tensorflow_gnn/graph:broadcast_ops",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
         "//tensorflow_gnn/graph:graph_tensor_encode",
         "//tensorflow_gnn/graph:graph_tensor_io",
         "//tensorflow_gnn/graph:graph_tensor_ops",
         "//tensorflow_gnn/graph:graph_tensor_pprint",
         "//tensorflow_gnn/graph:graph_tensor_random",
         "//tensorflow_gnn/graph:normalization_ops",
         "//tensorflow_gnn/graph:padding_ops",
+        "//tensorflow_gnn/graph:pool_ops",
         "//tensorflow_gnn/graph:preprocessing_common",
+        "//tensorflow_gnn/graph:readout",
         "//tensorflow_gnn/graph:schema_utils",
         "//tensorflow_gnn/graph:schema_validation",
         "//tensorflow_gnn/graph:tag_utils",
         "//tensorflow_gnn/graph:tensor_utils",
         "//tensorflow_gnn/keras",
         "//tensorflow_gnn/proto:graph_schema",
+        "//tensorflow_gnn/sampler",
     ],
 )
 
 pytype_strict_library(
     name = "version",
     srcs = ["version.py"],
     srcs_version = "PY3",
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,30 +20,35 @@
 
     import tensorflow_gnn as tfgnn
 
 The various data types provided by the GNN library have corresponding schemas
 similar to `tf.TensorSpec`. For example, a `FieldSpec` describes an instance of
 `Field`, and a `GraphTensorSpec` describes an instance of `GraphTensor`.
 """
+# pylint: disable=line-too-long
 
 from tensorflow_gnn import experimental  # Exposed as submodule. pylint: disable=unused-import
 from tensorflow_gnn import keras  # Exposed as submodule. pylint: disable=unused-import
+from tensorflow_gnn import sampler  # Exposed as submodule. pylint: disable=unused-import
 from tensorflow_gnn import version
 from tensorflow_gnn.graph import adjacency
 from tensorflow_gnn.graph import batching_utils
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import graph_constants
 from tensorflow_gnn.graph import graph_tensor
 from tensorflow_gnn.graph import graph_tensor_encode
 from tensorflow_gnn.graph import graph_tensor_io
 from tensorflow_gnn.graph import graph_tensor_ops
 from tensorflow_gnn.graph import graph_tensor_pprint
 from tensorflow_gnn.graph import graph_tensor_random
 from tensorflow_gnn.graph import normalization_ops
 from tensorflow_gnn.graph import padding_ops
+from tensorflow_gnn.graph import pool_ops
 from tensorflow_gnn.graph import preprocessing_common
+from tensorflow_gnn.graph import readout
 from tensorflow_gnn.graph import schema_utils
 from tensorflow_gnn.graph import schema_validation
 from tensorflow_gnn.graph import tag_utils
 from tensorflow_gnn.graph import tensor_utils
 from tensorflow_gnn.proto import graph_schema
 
 # Package version.
@@ -139,40 +144,50 @@
 
 # Pretty-printing.
 graph_tensor_to_values = graph_tensor_pprint.graph_tensor_to_values
 
 # Random generation.
 random_graph_tensor = graph_tensor_random.random_graph_tensor
 
-# Operations.
+# Broadcast and pool.
+broadcast_node_to_edges = broadcast_ops.broadcast_node_to_edges
+broadcast_context_to_nodes = broadcast_ops.broadcast_context_to_nodes
+broadcast_context_to_edges = broadcast_ops.broadcast_context_to_edges
+broadcast = broadcast_ops.broadcast_v2
+pool_edges_to_node = pool_ops.pool_edges_to_node
+pool_nodes_to_context = pool_ops.pool_nodes_to_context
+pool_edges_to_context = pool_ops.pool_edges_to_context
+pool = pool_ops.pool_v2
+get_registered_reduce_operation_names = pool_ops.get_registered_reduce_operation_names
+
+# Misc operations.
 mask_edges = graph_tensor_ops.mask_edges
 add_self_loops = graph_tensor_ops.add_self_loops
-broadcast_node_to_edges = graph_tensor_ops.broadcast_node_to_edges
-is_graph_tensor = graph_tensor_ops.is_graph_tensor
-pool_edges_to_node = graph_tensor_ops.pool_edges_to_node
-broadcast_context_to_nodes = graph_tensor_ops.broadcast_context_to_nodes
-broadcast_context_to_edges = graph_tensor_ops.broadcast_context_to_edges
-pool_nodes_to_context = graph_tensor_ops.pool_nodes_to_context
-pool_edges_to_context = graph_tensor_ops.pool_edges_to_context
-broadcast = graph_tensor_ops.broadcast
-pool = graph_tensor_ops.pool
 gather_first_node = graph_tensor_ops.gather_first_node
-get_registered_reduce_operation_names = (
-    graph_tensor_ops.get_registered_reduce_operation_names)
-register_reduce_operation = graph_tensor_ops.register_reduce_operation
 shuffle_features_globally = graph_tensor_ops.shuffle_features_globally
 combine_values = graph_tensor_ops.combine_values
 reorder_nodes = graph_tensor_ops.reorder_nodes
 shuffle_nodes = graph_tensor_ops.shuffle_nodes
 node_degree = graph_tensor_ops.node_degree
+convert_to_line_graph = graph_tensor_ops.convert_to_line_graph
 
 # Normalization operations.
 softmax = normalization_ops.softmax
 softmax_edges_per_node = normalization_ops.softmax_edges_per_node
 
+# Readout.
+validate_graph_tensor_spec_for_readout = readout.validate_graph_tensor_spec_for_readout
+validate_graph_tensor_for_readout = readout.validate_graph_tensor_for_readout
+add_readout_from_first_node = readout.add_readout_from_first_node
+structured_readout = readout.structured_readout
+structured_readout_into_feature = readout.structured_readout_into_feature
+# DO NOT USE the obsolete aliases `readout_named*`.
+readout_named = readout.structured_readout
+readout_named_into_feature = readout.structured_readout_into_feature
+
 # Schema conversion and I/O functions.
 parse_schema = schema_utils.parse_schema
 read_schema = schema_utils.read_schema
 write_schema = schema_utils.write_schema
 check_compatible_with_schema_pb = schema_utils.check_compatible_with_schema_pb
 create_graph_spec_from_schema_pb = schema_utils.create_graph_spec_from_schema_pb
 create_schema_pb_from_graph_spec = schema_utils.create_schema_pb_from_graph_spec
@@ -184,30 +199,40 @@
 validate_schema = schema_validation.validate_schema
 check_required_features = schema_validation.check_required_features
 assert_constraints = schema_validation.assert_constraints
 
 # Tensor Validation Utils
 check_scalar_graph_tensor = graph_tensor.check_scalar_graph_tensor
 check_homogeneous_graph_tensor = graph_tensor.check_homogeneous_graph_tensor
+get_homogeneous_node_and_edge_set_name = graph_tensor.get_homogeneous_node_and_edge_set_name
+get_aux_type_prefix = graph_tensor.get_aux_type_prefix
+
+# Type check helpers
+is_dense_tensor = tensor_utils.is_dense_tensor
 is_ragged_tensor = tensor_utils.is_ragged_tensor
+is_graph_tensor = graph_tensor_ops.is_graph_tensor
 
 # Prune imported module symbols so they're not accessible implicitly,
 # except those meant to be used as subpackages, like tfgnn.keras.*.
 # Please use the same order as for the import statements at the top.
 del version
 del adjacency
 del batching_utils
+del broadcast_ops
 del graph_constants
 del graph_tensor
 del graph_tensor_encode
 del graph_tensor_io
 del graph_tensor_ops
 del graph_tensor_pprint
 del graph_tensor_random
 del normalization_ops
 del padding_ops
+del pool_ops
 del preprocessing_common
+del readout
 del schema_utils
 del schema_validation
 del tag_utils
 del tensor_utils
 del graph_schema
+
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/convert_ogb_dataset.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/ogb/ogb_lib.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/ogb/ogb_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/converters/triples_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/converters/triples_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/data/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/BUILD`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_contrib_test", "pytype_strict_library")
 
 licenses(["notice"])
 
-package(default_visibility = ["//visibility:public"])
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = ["//visibility:public"],
+)
+
+GOOGLE_INTERNAL_UNIGRAPH_DEPENDENCIES = []
 
 pytype_strict_library(
     name = "unigraph",
     srcs = ["unigraph.py"],
     srcs_version = "PY3ONLY",
     deps = [
         "//third_party/py/apache_beam",
         "//third_party/py/pyarrow",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
         "//tensorflow_gnn/proto:graph_schema_py_proto",
-    ],
+    ] + GOOGLE_INTERNAL_UNIGRAPH_DEPENDENCIES,
 )
 
 pytype_strict_contrib_test(
     name = "unigraph_test",
     srcs = ["unigraph_test.py"],
     data = [
         "@tensorflow_gnn//testdata/heterogeneous",
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,22 +37,20 @@
 
 from absl import logging
 import apache_beam as beam
 import pyarrow
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.proto import graph_schema_pb2
-# Placeholder for Google-internal record file format pipeline import
-# Placeholder for Google-internal sorted string file format pipeline import
-# Placeholder for Google-internal sorted string file format utils
-
+# Placeholder for optional Google-internal record file format pipeline import
+# Placeholder for optional Google-internal record file format import
+# Placeholder for optional Google-internal sorted string file format utils
 try:
-  # pytype: disable=import-error
-  import google.cloud.bigquery_storage_v1 as bq_storage  # pylint: disable=g-import-not-at-top
-  # pytype: enable=import-error
+  # pylint: disable-next=g-import-not-at-top
+  import google.cloud.bigquery_storage_v1 as bq_storage  # pytype: disable=import-error
 except ImportError:
   bq_storage = None
 
 
 # Special constant column names required to be present in the node and edge
 # tabular files. As BigQuery doesn't support the `#` character in column names,
 # the special constant column names for BigQuery tables are the same without
@@ -280,41 +278,50 @@
     A dict set type to set name to PCollection of tf.Example of the features.
     Node sets have items of type (node-id, Example).
     Edge sets have items of type (source-id, target-id, Example).
   """
   pcoll_dict = {}
   for set_type, set_name, fset in tfgnn.iter_sets(schema):
 
+    # Save the collection for output.
+    set_dict = pcoll_dict.setdefault(set_type, {})
     if fset.metadata.HasField("filename"):
       pcoll = (
           rcoll
           | f"ReadFile/{set_name}" >> ReadUnigraphPieceFromFile(
               set_type, set_name, fset, graph_dir))
+      set_dict[set_name] = pcoll
     elif fset.metadata.HasField("bigquery"):
       pcoll = (
           rcoll | f"ReadBigQuery/{set_name}" >> ReadUnigraphPieceFromBigQuery(
               set_name,
               fset,
               gcs_location=gcs_location,
               bigquery_reader=bigquery_reader))
-
-    # Save the collection for output.
-    set_dict = pcoll_dict.setdefault(set_type, {})
-    set_dict[set_name] = pcoll
+      set_dict[set_name] = pcoll
 
   return pcoll_dict
 
 
 def is_edge_reversed(schema_edge_set: graph_schema_pb2.EdgeSet):
   for kv in schema_edge_set.metadata.extra:
     if kv.key == "edge_type" and kv.value == "reversed":
       return True
   return False
 
 
+# Needed for cloud storage paths to be treated like absolute paths
+# instead of being spuriously joined with a directory.
+# TODO(b/287083322): Identify if there's a library to check cloud URLs.
+def _is_complete_path(path: str) -> bool:
+  return (os.path.isabs(path)
+          or path.startswith("gs://")
+          or path.startswith("s3://"))
+
+
 class ReadUnigraphPieceFromFile(beam.PTransform):
   """Read a unigraph node/edge/context component from a file.
 
   Returns a PCollection object representing the Unigraph component.
   """
 
   def __init__(self, fset_type: str, fset_name: str,
@@ -338,15 +345,15 @@
     self.graph_dir = graph_dir
 
     if not self.fset.HasField("metadata") and not self.fset.metadata.HasField(
         "filename"):
       raise ValueError(f"{fset_name} does not specify a file: {fset}")
 
     self.filename = fset.metadata.filename
-    if not os.path.isabs(self.filename):
+    if not _is_complete_path(self.filename):
       if not self.graph_dir:
         raise ValueError(f"{self.filename} does not specify a full path "
                          "and graph_dir is None.")
       self.filename = os.path.join(self.graph_dir, self.filename)
 
     self.converters = build_converter_from_schema(self.fset.features)
 
@@ -884,24 +891,25 @@
     else:
       converters = None
     csv_records = csv.DictReader(gfile.GFile(file_path, "r"))
     for csv_record in csv_records:
       yield _csv_fields_to_example(csv_record.items(), converters=converters)
 
   @staticmethod
-  def fn_iter_from_file(file_format) -> Callable[
+  def fn_iter_from_file(file_format) -> Callable[  # pylint: disable=missing-function-docstring
       [str, Union[None, graph_schema_pb2.NodeSet, graph_schema_pb2.EdgeSet]],
       Iterable[Example]]:
-    return {
-        # Iterator for Google-internal data file type.
+    lookup = {
         "csv": DictStreams.iter_csv_examples,
         "tfrecord": DictStreams.iter_tfrecord_examples,
         # "capacitor": lambda path, fset: raise ValueError("Not implemented")
         # "recordio": lambda path, fset: raise ValueError("Not implemented")
-    }[file_format]
+    }
+        # Iterator for Google-internal data file type.
+    return lookup[file_format]
 
   @staticmethod
   def iter_records_from_filepattern(
       filepattern: str,
       fset: Optional[
           Union[graph_schema_pb2.NodeSet, graph_schema_pb2.EdgeSet]] = None
       ) -> Iterable[Example]:
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/data/unigraph_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/data/unigraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 ```
 
 This is the preferred way to expose individual functions on track to inclusion
 into the stable public interface of TensorFlow GNN.
 
 Beyond these symbols, there are also experimental sub-libraries that
 need to be imported separately (`from tensorflow_gnn.experimental import foo`).
-This is for special cases only.
+That is for special cases only.
 """
 
+from tensorflow_gnn.graph import readout
 from tensorflow_gnn.graph import tensor_utils
 
+context_readout_into_feature = readout.context_readout_into_feature
 segment_random_index_shuffle = tensor_utils.segment_random_index_shuffle
 
+del readout
 del tensor_utils
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/datasets.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/datasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,20 +10,28 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Infrastructure and implementation of in-memory graph data.
 
+Instantiating an object will download a dataset, and cache it locally. The
+datasets will be cached on ~/data/ogb (for "ogbn-" and "ogbl-" datasets), which
+can be overridden by setting environment variable `OGB_CACHE_DIR`; and on
+~/data/planetoid (for "cora", "citeseer", "pubmed"), which can be overridden by
+environment variable `PLANETOID_CACHE_DIR`.
+
 High-level Abstract Classes:
 
   * `InMemoryGraphData`: provides nodes, edges, and features, for a
      homogeneous or a heteregenous graph.
   * `NodeClassificationGraphData`: an `InMemoryGraphData` that also provides
     list of {train, test, validation} nodes, as well as their labels.
+  * `LinkPredictionGraphData`: an `InMemoryGraphData` that also provides lists
+    of edges in {train, test, validation} partitions.
 
 
 `InMemoryGraphData` implementations can provide
 
   * a single GraphTensor for training on one big graph (e.g., for node
     classification with `tf_trainer.py` or `keras_trainer.py`),
   * a big graph from which in-memory sampling (e.g., `int_arithmetic_sampler`)
@@ -45,14 +53,19 @@
 
     * `OgbnData`: Wraps node classification graph data from OGB, i.e., with
       name prefix of "ogbn-", such as, "ogbn-arxiv".
 
     * `PlanetoidGraphData`: wraps graph data that are popularized by GCN paper
       (cora, citeseer, pubmed).
 
+  * Link prediction (inheriting `LinkPredictionGraphData`)
+
+    * `OgblData`: Wraps link prediction graph data from OGB, i.e., with name
+      prefix of "ogbl-", such as, "ogbl-ddi".
+
 
 # Usage Example.
 
 ```
 graph_data = datasets.OgbnData('ogbn-arxiv')
 
 # Optionally, make graph undirected.
@@ -92,46 +105,57 @@
 ```
 graph_data = (
     datasets.OgbnData('ogbn-arxiv').with_undirected_edges(True)
     .with_self_loops(True))
 graph_tensor = graph_data.as_graph_tensor()
 ```
 """
+import abc
 import copy
 import functools
+import io
+import json
 import os
 import pickle
 import sys
-from typing import Any, List, Mapping, MutableMapping, NamedTuple, Tuple, Union, Optional
+from typing import Any, List, Mapping, NamedTuple, Tuple, Union, Optional, Callable
 import urllib.request
 
 import numpy as np
-import ogb.linkproppred
-import ogb.nodeproppred
-
 import scipy
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.experimental.in_memory import reader_utils
+from tensorflow_gnn.experimental.sampler import interfaces
 
 
-class InMemoryGraphData:
+# Given node-set-name, must return feature lookup or None.
+NodeFeaturesLookupFactory = Callable[
+    [tfgnn.NodeSetName], None|interfaces.KeyToFeaturesAccessor]
+
+
+class InMemoryGraphData(abc.ABC):
   """Abstract class for hold a graph data in-memory (nodes, edges, features).
 
   Subclasses must implement methods `node_features_dicts()`, `node_counts()`,
   `edge_lists()`, `node_sets()`, and optionally, `context()`. They inherit
   methods `graph_schema()`, `edge_sets()`, and `as_graph_tensor()` based on
   those.
   """
 
   def __init__(self, make_undirected: bool = False,
                add_self_loops: bool = False):
     self._make_undirected = make_undirected
     self._add_self_loops = add_self_loops
 
+  @property
+  def name(self) -> str:
+    """Returns name of dataset object. Can be overridden to return data name."""
+    return self.__class__.__name__
+
   def with_undirected_edges(self, make_undirected: bool) -> 'InMemoryGraphData':
     """Returns same graph data but with undirected edges added (or removed).
 
     Subsequent calls to `.graph_schema()` and to `.as_graph_tensor()` will be
     affected. Specifically, the generated output `tfgnn.GraphTensor` (by
     `.as_graph_tensor()`) will reverse all homogeneous edge sets (where its
     source node set equals its target node set). Suppose edge `(i, j)` is
@@ -149,24 +173,35 @@
 
     If make_undirected == False:
 
       * output of `.as_graph_tensor()` will contain, for each edge set "EdgeSet"
         (returned by `.edge_sets()`) a new edge-set "rev_EdgeSet" that reverses
         the "EdgeSet".
       * output of `.graph_schema()`. will have both "EdgeSet" and "rev_EdgeSet".
-
+      * `with_reverse_edge_sets()` is an equivalent and a more explicit method
+        to add reverse edge sets to the graph tensor and its schema.
     Args:
       make_undirected: If True, subsequent calls to `.graph_schema()` and
         `.as_graph_tensor()` will export an undirected graph. If False, a
         directed graph (with additional "rev_*" edges).
     """
     modified = copy.copy(self)
     modified._make_undirected = make_undirected  # pylint: disable=protected-access -- same class.
     return modified
 
+  def with_reverse_edge_sets(self) -> 'InMemoryGraphData':
+    """Returns same graph data but with reverse edge sets added."""
+
+    # Calling `with_undirected_edges` with `False` input automatically makes the
+    # output of `.as_graph_tensor()` to contain, for each edge set "EdgeSet"
+    # (returned by `.edge_sets()`) a new edge-set "rev_EdgeSet" that reverses
+    # the "EdgeSet". Similarly, output of `.graph_schema()`. will have both
+    # "EdgeSet" and "rev_EdgeSet".
+    return self.with_undirected_edges(False)
+
   def with_self_loops(self, add_self_loops: bool) -> 'InMemoryGraphData':
     """Returns same graph data but with self-loops added (or removed).
 
     If add_self_loops == True, then subsequent calls to `.as_graph_tensor()`
     will contain edges `[(i, i) for i in range(N_j)]`, for each homogeneous edge
     set j, where `N_j` is the number of nodes in node set connected by edge set
     `j`.
@@ -179,40 +214,43 @@
       add_self_loops: If set, self-loops will be amended on subsequent calls to
       `.as_graph_tensor()`. If not, no self-loops will be automatically added.
     """
     modified = copy.copy(self)
     modified._add_self_loops = add_self_loops  # pylint: disable=protected-access -- same class.
     return modified
 
+  @abc.abstractmethod
   def node_counts(self) -> Mapping[tfgnn.NodeSetName, int]:
     """Returns total number of graph nodes per node set."""
     raise NotImplementedError()
 
+  @abc.abstractmethod
   def node_features_dicts(self) -> Mapping[
-      tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
     """Returns 2-level dict: NodeSetName->FeatureName->Feature tensor.
 
     For every node set (`"x"`), feature tensor must have leading dimension equal
     to number of nodes in node set (`.node_counts()["x"]`). Other dimensions are
     dataset specific.
     """
     raise NotImplementedError()
 
+  @abc.abstractmethod
   def edge_lists(self) -> Mapping[
       Tuple[tfgnn.NodeSetName, tfgnn.EdgeSetName, tfgnn.NodeSetName],
       tf.Tensor]:
     """Returns dict from "edge type tuple" to int Tensor of shape (2, num_edges).
 
     "edge type tuple" string three-tuple:
       `(source node set name, edge set name, target node set name)`.
     where `edge set name` must be unique.
     """
     raise NotImplementedError()
 
-  def node_sets(self) -> MutableMapping[tfgnn.NodeSetName, tfgnn.NodeSet]:
+  def node_sets(self) -> Mapping[tfgnn.NodeSetName, tfgnn.NodeSet]:
     """Returns node sets of entire graph (dict: node set name -> NodeSet)."""
     node_counts = self.node_counts()
     features_dicts = self.node_features_dicts()
     node_set_names = set(node_counts.keys()).union(features_dicts.keys())
     return (
         {name: tfgnn.NodeSet.from_fields(sizes=as_tensor([node_counts[name]]),
                                          features=features_dicts.get(name, {}))
@@ -246,15 +284,15 @@
       schema.edge_sets[edge_set_name].target = dst_node_set_name
       if not self._make_undirected:
         schema.edge_sets['rev_' + edge_set_name].source = dst_node_set_name
         schema.edge_sets['rev_' + edge_set_name].target = src_node_set_name
 
     return schema
 
-  def edge_sets(self) -> MutableMapping[tfgnn.EdgeSetName, tfgnn.EdgeSet]:
+  def edge_sets(self) -> Mapping[tfgnn.EdgeSetName, tfgnn.EdgeSet]:
     """Returns edge sets of entire graph (dict: edge set name -> EdgeSet)."""
     edge_sets = {}
     node_counts = self.node_counts() if self._add_self_loops else None
     for edge_type, edge_list in self.edge_lists().items():
       (source_node_set_name, edge_set_name, target_node_set_name) = edge_type
 
       if self._make_undirected and source_node_set_name == target_node_set_name:
@@ -273,25 +311,81 @@
         edge_sets['rev_' + edge_set_name] = tfgnn.EdgeSet.from_fields(
             sizes=tf.shape(edge_list)[1:2],
             adjacency=tfgnn.Adjacency.from_indices(
                 source=(target_node_set_name, edge_list[1]),
                 target=(source_node_set_name, edge_list[0])))
     return edge_sets
 
+  def create_node_features_lookup_factory(self) -> NodeFeaturesLookupFactory:
+    return functools.partial(
+        _node_features_lookup, node_sets=dict(self.node_sets()), cache={},
+        resource_prefix=self.name)
+
+  def save(self, filename: str):
+    """Superclasses can save themselves to disk."""
+    raise NotImplementedError()
+
+
+class _Accessor(tf.keras.layers.Layer, interfaces.KeyToFeaturesAccessor):
+  """Wraps `NodeSet` with `call` that can select features for node subsets."""
+
+  def __init__(self, node_set: tfgnn.NodeSet, resource_name: str):
+    super().__init__()
+    self._node_set = node_set
+    self._resource_name = resource_name
+
+  def call(self, keys: tf.RaggedTensor) -> interfaces.Features:
+    """Gathers features corresponding to (tf.int) node keys."""
+    return {feature_name: tf.gather(feature_value, keys)
+            for feature_name, feature_value in self._node_set.features.items()
+            if feature_name != '#id'}
+
+  @property
+  def resource_name(self) -> str:
+    return self._resource_name
+
+
+def _node_features_lookup(
+    node_set_name: tfgnn.NodeSetName,
+    *,
+    node_sets: dict[tfgnn.NodeSetName, tfgnn.NodeSet],
+    cache: dict[tfgnn.NodeSetName, _Accessor],
+    resource_prefix: str,
+    ) -> interfaces.KeyToFeaturesAccessor:
+  if node_set_name in cache:
+    return cache[node_set_name]
+  cache[node_set_name] = _Accessor(
+      node_sets[node_set_name], f'{resource_prefix}/nodes/{node_set_name}')
+  return cache[node_set_name]
+
 
 class NodeSplit(NamedTuple):
   """Contains 1D int tensors holding positions of {train, valid, test} nodes.
 
   This is returned by `NodeClassificationGraphData.node_split()`
   """
   train: tf.Tensor
   validation: tf.Tensor
   test: tf.Tensor
 
 
+class EdgeSplit(NamedTuple):
+  """Contains positive and negative edges in {train, test, valid} partitions.
+
+  Each `tf.Tensor` will be of shape `[2, num_edges]` with dtype int64.
+  """
+  # Only need positive edges for training. The (entire) graph compliment can be
+  # used for negative edges.
+  train_edges: tf.Tensor
+  validation_edges: tf.Tensor
+  test_edges: tf.Tensor
+  negative_validation_edges: tf.Tensor
+  negative_test_edges: tf.Tensor
+
+
 class NodeClassificationGraphData(InMemoryGraphData):
   """Adapts `InMemoryGraphData` for node classification settings.
 
   Subclasses should information for node classification: (node labels, name of
   node set, and partitions train:validation:test nodes).
   """
 
@@ -357,69 +451,77 @@
 
     return dataset
 
   @property
   def splits(self) -> List[str]:
     return copy.copy(self._splits)
 
+  @abc.abstractmethod
   def num_classes(self) -> int:
     """Number of node classes. Max of `labels` should be `< num_classes`."""
     raise NotImplementedError('num_classes')
 
+  @abc.abstractmethod
   def node_split(self) -> NodeSplit:
     """`NodeSplit` with attributes `train`, `validation`, `test` set.
 
     The attributes are set to indices of the `labeled_nodeset`. Specifically,
     they correspond to leading dimension of features of the node set.
     """
     raise NotImplementedError()
 
+  @abc.abstractmethod
   def labels(self) -> tf.Tensor:
     """int vector containing labels for train & validation nodes.
 
     Size of vector is number of nodes in the labeled node set. In particular:
     `self.labels().shape[0] == self.node_counts()[self.labeled_nodeset]`.
     Specifically, the vector has as many entries as there are nodes belonging to
     the node set that this task aims to predict labels for.
 
     Entry `labels()[i]` will be -1 iff `i in self.node_split().test`. Otherwise,
     `labels()[i]` will be int in range [`0`, `self.num_classes() - 1`].
     """
     raise NotImplementedError()
 
+  @abc.abstractmethod
   def test_labels(self) -> tf.Tensor:
     """Like the above but contains no -1's.
 
     Every {train, valid, test} node will have its class label.
     """
     raise NotImplementedError()
 
   @property
+  @abc.abstractmethod
   def labeled_nodeset(self) -> tfgnn.NodeSetName:
     """Name of node set which `labels` and `node_splits` reference."""
     raise NotImplementedError()
 
+  @abc.abstractmethod
   def node_features_dicts_without_labels(self) -> Mapping[
-      tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
     raise NotImplementedError()
 
   def node_features_dicts(self) -> Mapping[
-      tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
     """Implements a method required by the base class.
 
     This method combines the data from `labels()` or `test_labels()` with the
     data from `node_features_dicts_without_labels()` into a single features
     dict.
 
     Subclasses need to implement aforementioned methods and may inherit this.
 
     Returns:
       NodeSetName -> FeatureName -> Feature Tensor.
     """
     node_features_dicts = self.node_features_dicts_without_labels()
+    node_features_dicts = {ns: dict(features)  # Shallow copy.
+                           for ns, features in node_features_dicts.items()}
     if self._use_labels_as_features:
       if 'test' in self._splits:
         node_features_dicts[self.labeled_nodeset]['label'] = self.test_labels()
       else:
         node_features_dicts[self.labeled_nodeset]['label'] = self.labels()
 
     return node_features_dicts
@@ -436,14 +538,154 @@
   def graph_schema(self) -> tfgnn.GraphSchema:
     graph_schema = super().graph_schema()
     context_features = graph_schema.context.features
     context_features['seed_nodes.' + self.labeled_nodeset].dtype = (
         tf.int64.as_datatype_enum)
     return graph_schema
 
+  def save(self, filename: str):
+    """Saves the dataset on numpy compressed (.npz) file.
+
+    The file runs once the functions,
+    (labeled_nodeset, test_labels, labels, node_split, edge_lists, node_counts,
+     node_features, num_classes),
+    composes a flat dict (keys are json-encoded arrays), then writes as numpy
+    file. Flat dict is needed as numpy only saves named arrays, not nested
+    structures.
+
+    Args:
+      filename: file path to save onto. ".npz" extension is recommended. Parent
+        directory must exist.
+    """
+    features_without_labels = self.node_features_dicts_without_labels()
+    node_split = self.node_split()
+
+    attribute_dict = {
+        ('num_classes',): self.num_classes(),
+        ('node_split', 'train'): node_split.train.numpy(),
+        ('node_split', 'test'): node_split.test.numpy(),
+        ('node_split', 'validation'): node_split.validation.numpy(),
+        ('labels',): self.labels().numpy(),
+        ('test_labels',): self.test_labels().numpy(),
+        ('labeled_nodeset',): self.labeled_nodeset,
+    }
+
+    # Edge sets.
+    for (src_name, es_name, tgt_name), es_indices in self.edge_lists().items():
+      key = ('e', '#', src_name, es_name, tgt_name)
+      attribute_dict[key] = es_indices.numpy()
+
+    for ns_name, features in features_without_labels.items():
+      for feature_name, feature_tensor in features.items():
+        attribute_dict[('n', ns_name, feature_name)] = feature_tensor.numpy()
+
+    for node_set_name, node_count in self.node_counts().items():
+      attribute_dict[('nc', node_set_name)] = node_count
+
+    bytes_io = io.BytesIO()
+    attribute_dict = {json.dumps(k): v for k, v in attribute_dict.items()}
+    np.savez_compressed(bytes_io, **attribute_dict)
+    with tf.io.gfile.GFile(filename, 'wb') as f:
+      f.write(bytes_io.getvalue())
+
+  @staticmethod
+  def load(filename: str) -> 'NodeClassificationGraphData':
+    """Loads from disk `NodeClassificationGraphData` that was `save()`ed."""
+    dataset_dict = dict(np.load(tf.io.gfile.GFile(filename, 'rb')))
+    dataset_dict = {tuple(json.loads(k)): v for k, v in dataset_dict.items()}
+    edge_lists = {}
+    node_features = {}
+    node_counts = {}
+    for key, array in dataset_dict.items():
+      # edge lists.
+      if key[0] == 'e':
+        if key[1] != '#':
+          raise ValueError('Expecting ("e", "#", ...) but got %s' % str(key))
+        src_name = key[2]
+        es_name = key[3]
+        tgt_name = key[4]
+        indices = as_tensor(array)
+        edge_lists[(src_name, es_name, tgt_name)] = indices
+      # node features.
+      if key[0] == 'n':
+        node_set_name = key[1]
+        feature_name = key[2]
+        if node_set_name not in node_features:
+          node_features[node_set_name] = {}
+        node_features[node_set_name][feature_name] = as_tensor(array)
+      if key[0] == 'nc':
+        node_counts[key[1]] = int(array)
+
+    return _PreloadedNodeClassificationGraphData(
+        num_classes=dataset_dict[('num_classes',)],
+        node_features_dicts_without_labels=node_features,
+        node_counts=node_counts,
+        edge_lists=edge_lists,
+        node_split=NodeSplit(
+            train=as_tensor(dataset_dict[('node_split', 'train')]),
+            validation=as_tensor(dataset_dict[('node_split', 'validation')]),
+            test=as_tensor(dataset_dict[('node_split', 'test')])),
+        labels=as_tensor(dataset_dict[('labels',)]),
+        test_labels=as_tensor(dataset_dict[('test_labels',)]),
+        labeled_nodeset=str(dataset_dict[('labeled_nodeset',)]))
+
+
+class _PreloadedNodeClassificationGraphData(NodeClassificationGraphData):
+  """Dataset from pre-computed attributes."""
+
+  def __init__(
+      self, num_classes: int,
+      node_features_dicts_without_labels: Mapping[
+          tfgnn.NodeSetName,
+          Mapping[tfgnn.FieldName, tf.Tensor]],
+      node_counts: Mapping[tfgnn.NodeSetName, int],
+      edge_lists: Mapping[
+          Tuple[tfgnn.NodeSetName, tfgnn.EdgeSetName, tfgnn.NodeSetName],
+          tf.Tensor],
+      node_split: NodeSplit, labels: tf.Tensor, test_labels: tf.Tensor,
+      labeled_nodeset: tfgnn.NodeSetName):
+    super().__init__()
+    self._num_classes = num_classes
+    self._node_features_dicts_without_labels = (
+        node_features_dicts_without_labels)
+    self._node_counts = node_counts
+    self._edge_lists = edge_lists
+    self._node_split = node_split
+    self._labels = labels
+    self._test_labels = test_labels
+    self._labeled_nodeset = labeled_nodeset
+
+  def num_classes(self) -> int:
+    return self._num_classes
+
+  def node_features_dicts_without_labels(self) -> Mapping[
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
+    return self._node_features_dicts_without_labels
+
+  def node_counts(self) -> Mapping[tfgnn.NodeSetName, int]:
+    return self._node_counts
+
+  def edge_lists(self) -> Mapping[
+      Tuple[tfgnn.NodeSetName, tfgnn.EdgeSetName, tfgnn.NodeSetName],
+      tf.Tensor]:
+    return self._edge_lists
+
+  def node_split(self) -> NodeSplit:
+    return self._node_split
+
+  def labels(self) -> tf.Tensor:
+    return self._labels
+
+  def test_labels(self) -> tf.Tensor:
+    return self._test_labels
+
+  @property
+  def labeled_nodeset(self) -> str:
+    return self._labeled_nodeset
+
 
 class _OgbGraph:
   """Wraps data exposed by OGB graph objects, while enforcing heterogeneity.
 
   Attributes offered by this class are consistent with the APIs of GraphData.
   """
 
@@ -494,15 +736,15 @@
   @property
   def num_nodes_dict(self) -> Mapping[tfgnn.NodeSetName, int]:
     """Maps "node set name" -> number of nodes."""
     return self._num_nodes_dict
 
   @property
   def node_feat_dict(self) -> Mapping[
-      tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
     """Maps "node set name" to dict of "feature name"->tf.Tensor."""
     return self._node_feat_dict
 
   @property
   def edge_index_dict(self) -> Mapping[
       Tuple[tfgnn.NodeSetName, tfgnn.EdgeSetName, tfgnn.NodeSetName],
       tf.Tensor]:
@@ -513,41 +755,59 @@
       Where `edges` is tf.Tensor of shape (2, num edges), with `edges[0]` and
       `edges[1]`, respectively, containing source and target node IDs (as 1D int
       tf.Tensor).
     """
     return self._edge_index_dict
 
 
+def _get_ogbn_dataset(dataset_name: str, cache_dir: Optional[str] = None):
+  """Imports ogb and returns `NodePropPredDataset`."""
+  # This is done on purpose: we only import ogb if an ogb dataset is requested.
+  import ogb.nodeproppred  # pylint: disable=g-import-not-at-top
+  return ogb.nodeproppred.NodePropPredDataset(dataset_name, root=cache_dir)
+
+
+def _get_ogbl_dataset(dataset_name: str, cache_dir: Optional[str] = None):
+  """Imports ogb and returns `LinkPropPredDataset`."""
+  # This is done on purpose: we only import ogb if an ogb dataset is requested.
+  import ogb.linkproppred  # pylint: disable=g-import-not-at-top
+  return ogb.linkproppred.LinkPropPredDataset(dataset_name, root=cache_dir)
+
+
 class OgbnData(NodeClassificationGraphData):
   """Wraps node classification graph data of ogbn-* for in-memory learning."""
 
   def __init__(self, dataset_name, cache_dir=None):
     super().__init__()
+    self._dataset_name = dataset_name
     if cache_dir is None:
       cache_dir = os.environ.get(
           'OGB_CACHE_DIR', os.path.expanduser(os.path.join('~', 'data', 'ogb')))
 
-    self.ogb_dataset = ogb.nodeproppred.NodePropPredDataset(
-        dataset_name, root=cache_dir)
+    self._ogb_dataset = _get_ogbn_dataset(dataset_name, cache_dir)
     self._graph, self._node_labels, self._node_split, self._labeled_nodeset = (
-        OgbnData._to_heterogeneous(self.ogb_dataset))
+        OgbnData._to_heterogeneous(self._ogb_dataset))
 
     # rehape from [N, 1] to [N].
     self._node_labels = self._node_labels[:, 0]
 
     # train labels (test set to -1).
     self._train_labels = np.copy(self._node_labels)
     self._train_labels[self._node_split.test] = -1
 
     self._train_labels = as_tensor(self._train_labels)
     self._node_labels = as_tensor(self._node_labels)
 
+  @property
+  def name(self) -> str:
+    return self._dataset_name
+
   @staticmethod
   def _to_heterogeneous(
-      ogb_dataset: ogb.nodeproppred.NodePropPredDataset) -> Tuple[
+      ogb_dataset: Any) -> Tuple[
           _OgbGraph,    # ogb_graph.
           np.ndarray,   # node_labels.
           NodeSplit,    # idx_split.
           str]:
     """Returns heterogeneous dicts from homogeneous or heterogeneous OGB dataset.
 
     Args:
@@ -600,18 +860,18 @@
     idx_split = ogb_dataset.get_idx_split()
     idx_split['validation'] = idx_split.pop('valid')  # Rename
     idx_split = NodeSplit(**tf.nest.map_structure(
         tf.convert_to_tensor, idx_split))
     return ogb_graph, node_labels, idx_split, tfgnn.NODES
 
   def num_classes(self) -> int:
-    return self.ogb_dataset.num_classes
+    return self._ogb_dataset.num_classes
 
   def node_features_dicts_without_labels(self) -> Mapping[
-      tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
     # Deep-copy dict (*but* without copying tf.Tensor objects).
     node_sets = self._graph.node_feat_dict
     node_sets = {node_set_name: dict(node_set.items())
                  for node_set_name, node_set in node_sets.items()}
     node_counts = self.node_counts()
     for node_set_name, count in node_counts.items():
       if node_set_name not in node_sets:
@@ -666,14 +926,15 @@
 
   [1] Yang et al, ICML'16
   [2] Kipf & Welling, ICLR'17.
   """
 
   def __init__(self, dataset_name, cache_dir=None):
     super().__init__()
+    self._dataset_name = dataset_name
     allowed_names = ('pubmed', 'citeseer', 'cora')
 
     url_template = (
         'https://github.com/kimiyoung/planetoid/blob/master/data/'
         'ind.%s.%s?raw=true')
     file_parts = ['ally', 'allx', 'graph', 'ty', 'tx', 'test.index']
     if dataset_name not in allowed_names:
@@ -720,38 +981,42 @@
     self._num_nodes = len(edge_lists)
     self._num_classes = ally.shape[1]
     self._node_labels = np.argmax(ally, axis=1)
     self._train_labels = self._node_labels + 0  # Copy.
     self._train_labels[test_idx] = -1
     self._node_labels = as_tensor(self._node_labels)
     self._train_labels = as_tensor(self._train_labels)
-    self._test_idx = tf.convert_to_tensor(np.array(test_idx, dtype='int32'))
+    self._test_idx = as_tensor(np.array(test_idx, dtype='int32'))
     self._node_split = None  # Populated on `node_split()`
 
     # Will be used to construct (sparse) adjacency matrix.
     adj_src = []
     adj_target = []
     for node, neighbors in edge_lists.items():
       adj_src.extend([node] * len(neighbors))
       adj_target.extend(neighbors)
 
     self._edge_list = as_tensor(np.stack([adj_src, adj_target], axis=0))
 
+  @property
+  def name(self) -> str:
+    return self._dataset_name
+
   @staticmethod
   def load_x(filename):
     if sys.version_info > (3, 0):
       return pickle.load(tf.io.gfile.GFile(filename, 'rb'), encoding='latin1')
     else:
       return np.load(tf.io.gfile.GFile(filename))
 
   def num_classes(self) -> int:
     return self._num_classes
 
   def node_features_dicts_without_labels(self) -> Mapping[
-      tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+      tfgnn.NodeSetName, Mapping[tfgnn.FieldName, tf.Tensor]]:
     features = {'feat': self._allx}
     features['#id'] = tf.range(self._num_nodes, dtype=tf.int32)
     return {tfgnn.NODES: features}
 
   def node_counts(self) -> Mapping[tfgnn.NodeSetName, int]:
     return {tfgnn.NODES: self._num_nodes}
 
@@ -782,20 +1047,134 @@
     return self._train_labels
 
   def test_labels(self) -> tf.Tensor:
     """int numpy array of length num_nodes containing train and test labels."""
     return self._node_labels
 
 
-def get_in_memory_graph_data(dataset_name) -> InMemoryGraphData:
+class LinkPredictionGraphData(InMemoryGraphData):
+  """Superclasses must wrap dataset of graph(s) for link-prediction tasks."""
+
+  @abc.abstractmethod
+  def edge_split(self) -> EdgeSplit:
+    """Returns edge endpoints for {train, test, valid} partitions."""
+    raise NotImplementedError()
+
+  @property
+  @abc.abstractmethod
+  def target_edgeset(self) -> tfgnn.EdgeSetName:
+    """Name of edge set over which link prediction is defined."""
+    raise NotImplementedError()
+
+  @property
+  def source_node_set_name(self) -> tfgnn.NodeSetName:
+    """Node set name of source node of (task) target_edgeset."""
+    return self.graph_schema().edge_sets[self.target_edgeset].source
+
+  @property
+  def target_node_set_name(self) -> tfgnn.NodeSetName:
+    """Node set name of target node of (task) target_edgeset."""
+    return self.graph_schema().edge_sets[self.target_edgeset].target
+
+  @property
+  def num_source_nodes(self) -> int:
+    """Number of nodes in the source endpoint of (task) target_edgeset."""
+    return self.node_counts()[self.source_node_set_name]
+
+  @property
+  def num_target_nodes(self) -> int:
+    """Number of nodes in the target endpoint of (task) target_edgeset."""
+    return self.node_counts()[self.target_node_set_name]
+
+
+class OgblData(LinkPredictionGraphData):
+  """Wraps link prediction datasets of ogbl-* for in-memory learning."""
+
+  def __init__(self, dataset_name: str, cache_dir: None|str = None):
+    super().__init__()
+    self._dataset_name = dataset_name
+    if cache_dir is None:
+      cache_dir = os.environ.get(
+          'OGB_CACHE_DIR', os.path.expanduser(os.path.join('~', 'data', 'ogb')))
+
+    self._ogb_dataset = _get_ogbl_dataset(dataset_name, cache_dir)
+
+    ogb_edge_dict = self._ogb_dataset.get_edge_split()
+    self._edge_split = EdgeSplit(
+        train_edges=as_tensor(ogb_edge_dict['train']['edge']),
+        validation_edges=as_tensor(ogb_edge_dict['train']['edge']),
+        test_edges=as_tensor(ogb_edge_dict['test']['edge']),
+        negative_validation_edges=as_tensor(ogb_edge_dict['valid']['edge_neg']),
+        negative_test_edges=as_tensor(ogb_edge_dict['test']['edge_neg']))
+
+    self._ogb_graph = _OgbGraph(self._ogb_dataset.graph)
+
+  @property
+  def name(self) -> str:
+    return self._dataset_name
+
+  def node_features_dicts(self, add_id: bool = True) -> Mapping[
+      tfgnn.NodeSetName, Mapping[str, tf.Tensor]]:
+    features = self._ogb_graph.node_feat_dict
+    # 2-level dict shallow copy. Inner value stores reference to tf.Tensor,
+    features = {node_set_name: copy.copy(features)
+                for node_set_name, features in features.items()}
+    if add_id:
+      counts = self.node_counts()
+      for node_set_name, feats in features.items():
+        feats['#id'] = tf.range(counts[node_set_name], dtype=tf.int32)
+    return features
+
+  def node_counts(self) -> Mapping[tfgnn.NodeSetName, int]:
+    return dict(self._ogb_graph.num_nodes_dict)  # Return copy.
+
+  def edge_lists(self) -> Mapping[
+      Tuple[tfgnn.NodeSetName, tfgnn.EdgeSetName, tfgnn.NodeSetName],
+      tf.Tensor]:
+    return dict(self._ogb_graph.edge_index_dict)  # Return shallow copy.
+
+  def edge_split(self) -> EdgeSplit:
+    return self._edge_split
+
+  @property
+  def target_edgeset(self) -> tfgnn.EdgeSetName:
+    return tfgnn.EDGES
+
+
+def get_in_memory_graph_data(dataset_name: str) -> InMemoryGraphData:
   if dataset_name.startswith('ogbn-'):
     return OgbnData(dataset_name)
+  elif dataset_name.startswith('ogbl-'):
+    return OgblData(dataset_name)
   elif dataset_name in ('cora', 'citeseer', 'pubmed'):
     return PlanetoidGraphData(dataset_name)
   else:
     raise ValueError('Unknown Dataset name: ' + dataset_name)
 
 
 # Shorthand. Can be replaced with: `as_tensor = tf.convert_to_tensor`.
 def as_tensor(obj: Any) -> tf.Tensor:
   """short-hand for tf.convert_to_tensor."""
   return tf.convert_to_tensor(obj)
+
+
+def load_ogbn_graph_tensor(
+    dataset_path: str, *, add_reverse_edge_sets: bool = False
+)-> tfgnn.GraphTensor:
+  """Load OGBN graph data as a graph tensor from numpy compressed (.npz) files.
+
+  To generate the .npz files from the original OGB dataset, please refer to
+  tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py
+
+  Args:
+    dataset_path: Path to the saved OGBN numpy compressed (.npz) files.
+    add_reverse_edge_sets: Flag to determine whether to add reversed edge sets.
+
+  Returns:
+    A tfgnn.GraphTensor comprising of the full OGBN graph loaded in-memory.
+  """
+  graph_data = NodeClassificationGraphData.load(dataset_path)
+  graph_data = graph_data.with_labels_as_features(True)
+  if add_reverse_edge_sets:
+    graph_data = graph_data.with_reverse_edge_sets()
+  graph_tensor = graph_data.as_graph_tensor()
+  return graph_tensor
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
 
 import numpy as np
 import scipy.sparse as ssp
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.experimental.in_memory import datasets
 from tensorflow_gnn.experimental.in_memory import reader_utils
+from tensorflow_gnn.experimental.sampler import interfaces
 from tensorflow_gnn.graph import tensor_utils as utils
 from tensorflow_gnn.sampler import sampling_spec_pb2
 
 
 def process_sampling_spec_topologically(
     sampling_spec: sampling_spec_pb2.SamplingSpec,
     *,
@@ -467,14 +468,80 @@
 
 
 class EdgeSampling(enum.Enum):
   WITH_REPLACEMENT = 'with_replacement'
   WITHOUT_REPLACEMENT = 'without_replacement'
 
 
+class EdgeSampler(tf.keras.layers.Layer, interfaces.OutgoingEdgesSampler):
+  """Samples neighbors given nodes. Follows Edge-sampling API.
+
+  To an instance, EdgeSampler you must first create `sampler = GraphSampler()`.
+  Then:
+
+  ```python
+  edge_sampler = sampler.make_edge_sampler(
+      sampling_spec_pb2.SamplingOp(
+          edge_set_name="nameOfEdgeSet", sample_size=10))
+  ```
+
+  Finally, you may invoke as:
+
+  ```python
+  nodes = tf.ragged.constant([[0, 1], [2]])
+  edges = edge_sampler(nodes)  # Must be dict with keys "#source" and "#target".
+
+  print(edges['#source'])  # Should print ragged tensor with source node IDs,
+                           # e.g., [[0, 0, 0, 1, 1], [2]], if node 0 has 3
+                           # connections, node 1 has 2 connections, and node 2
+                           # has only one connection.
+  print(edges['#target'])  # Must be same shape as above, e.g.,
+                           # [[5, 6, 7, 8, 9], [20]], implying sampled edges
+                           # 0-5, 0-6, 0-7, 1-8, 1-9, and 2-20.
+  ```
+  """
+
+  def __init__(
+      self, sampler: 'GraphSampler', sample_size: int,
+      edge_set_name: tfgnn.EdgeSetName,
+      sampling_mode: Optional[EdgeSampling] = None):
+    super().__init__()
+    self._sampler = sampler
+    self._edge_set_name = edge_set_name
+    self._sample_size = sample_size
+    self._sampling_mode = sampling_mode
+
+  def call(self, source_node_ids: Union[tf.Tensor, tf.RaggedTensor]) -> Mapping[
+      str, tf.RaggedTensor]:
+    endpoint_spec = tf.RaggedTensorSpec(
+        shape=[None], dtype=source_node_ids.dtype, ragged_rank=0)
+    edges_src, edges_tgt = tf.map_fn(
+        self._sample_from_tensor_node_ids, source_node_ids,
+        fn_output_signature=(endpoint_spec, endpoint_spec))
+    return {tfgnn.SOURCE_NAME: edges_src, tfgnn.TARGET_NAME: edges_tgt}
+
+  def _sample_from_tensor_node_ids(self, nodes: tf.Tensor) -> Tuple[
+      tf.Tensor, tf.Tensor]:
+    """Given dense `nodes` (of any shape), returns (num_edges, 2) Tensor."""
+    src = tf.expand_dims(nodes, -1)  # In case `nodes` is scalar.
+    tgt, valid_mask = self._sampler.sample_one_hop_with_valid_mask(
+        src, edge_set_name=self._edge_set_name, sample_size=self._sample_size,
+        sampling_mode=self._sampling_mode)
+    # Now, `tgt` has an additional dimension over `src`. The size of this
+    # (last) dimension must be equal to `self._sample_size`. Let's repeat `src`
+    # along that axis:
+    src = tf.expand_dims(src, -1) + tf.zeros_like(tgt)
+
+    # Filter only to valid tgt (and associated valid src) and return pair
+    valid_reshaped = tf.reshape(valid_mask, [-1])
+    valid_src = tf.boolean_mask(tf.reshape(src, [-1]), valid_reshaped)
+    valid_tgt = tf.boolean_mask(tf.reshape(tgt, [-1]), valid_reshaped)
+    return valid_src, valid_tgt
+
+
 class GraphSampler:
   """Yields random sub-graphs from `InMemoryGraphData`.
 
   Sub-graphs are encoded as `GraphTensor` or tf.data.Dataset. Random walks are
   performed using `TypedWalkTree`. Input data graph must be an instance of
   `Dataset`.
   """
@@ -498,14 +565,17 @@
       edges_src = edge_set.adjacency.source.numpy()  # Assumption: in-memory.
       edges_tgt = edge_set.adjacency.target.numpy()
 
       self.adjacency[edge_set_name] = ssp.csr_matrix(
           (np.ones(edges_src.shape, dtype='int8'), (edges_src, edges_tgt)),
           shape=(size_src, size_tgt))
 
+    if not edge_sets:
+      raise ValueError('graph_data has no edge-sets.')
+
     # Compute data structures required for sampling.
     self.edge_lists = {}      # Edge set name -> (optional src_ids, target_ids).
     self.degrees = {}         # Edge set name -> [deg_1, deg_2, ... deg_|V|].
     self.degrees_cumsum = {}  # Edge set name -> [0, deg_1, deg_1+deg_2. ...].
     for edge_set_name, csr_adj in self.adjacency.items():
       csr_adj = csr_adj > 0  # Binarize.
       nonzero_rows, nonzero_cols = csr_adj.nonzero()
@@ -516,20 +586,40 @@
       self.degrees[edge_set_name] = degree_vector
       self.degrees_cumsum[edge_set_name] = tf.math.cumsum(
           degree_vector, exclusive=True)
 
     if reduce_memory_footprint:
       self.adjacency = None
 
-  def make_sampling_layer(self, edge_set_name, sample_size=3,
-                          sampling_mode=None):
+  def make_edge_sampler(
+      self, sampling_op: sampling_spec_pb2.SamplingOp) -> EdgeSampler:
     """Makes layer out of `sample_one_hop`."""
-    return functools.partial(
-        self.sample_one_hop, edge_set_name=edge_set_name,
-        sample_size=sample_size, sampling_mode=sampling_mode)
+    available_edge_set_names = self.graph_data.edge_sets().keys()
+    # Validation.
+    edge_set_name = sampling_op.edge_set_name
+
+    if (sampling_op.strategy
+        != sampling_spec_pb2.SamplingStrategy.RANDOM_UNIFORM):
+      raise ValueError(
+          'int-arithmetic sampler currently only supports strategy '
+          'RANDOM_UNIFORM')
+
+    if edge_set_name is None:
+      if len(available_edge_set_names) > 1:
+        raise ValueError(
+            'You must provide `edge_set_name` as your graph has multiple edge '
+            'sets: ' + ', '.join(available_edge_set_names))
+      edge_set_name = list(available_edge_set_names)[0]
+    else:
+      if edge_set_name not in available_edge_set_names:
+        raise ValueError('Edge-set "%s" is not one of: %s' % (
+            edge_set_name, ', '.join(available_edge_set_names)))
+
+    return EdgeSampler(
+        self, sampling_op.sample_size, edge_set_name, self.sampling_mode)
 
   def sample_one_hop(
       self, source_nodes: tf.Tensor, edge_set_name: tfgnn.EdgeSetName,
       sample_size: int,
       **kwargs) -> tf.Tensor:
     """Samples one-hop from source-nodes using edge `edge_set_name`.
 
@@ -594,15 +684,15 @@
       reshaped_node_degrees = tf.reshape(node_degrees, [-1])
       reshaped_node_degrees_or_1 = tf.maximum(
           reshaped_node_degrees, tf.ones_like(reshaped_node_degrees))
       # shape=(sample_size, total_input_nodes).
       sample_upto = tf.stack([reshaped_node_degrees] * sample_size, axis=0)
 
       # [[0, 1, 2, ..., f], <repeated>].T
-      if nodes_reshaped.shape[0] is not None:
+      if nodes_reshaped.shape[0]:
         subtract_mod = tf.stack(
             [tf.range(sample_size, dtype=tf.int64)] * nodes_reshaped.shape[0],
             axis=-1)
         sample_size_x_num_input_nodes = subtract_mod.shape
       else:
         subtract_mod = tf.transpose(utils.repeat(
             tf.expand_dims(tf.range(sample_size, dtype=tf.int64), 0),
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/models.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,43 +165,43 @@
 
 
 def make_gcn_model(
     num_classes: int, *, depth: int = 3, hidden_units: int = 200,
     hidden_activation: _OptionalActivation = 'relu',
     out_activation: _OptionalActivation = None,
     kernel_regularizer: _OptionalRegularizer = None, use_bias: bool = False,
-    dropout: float = 0) -> tf.keras.Sequential:
+    add_self_loops: bool = True, dropout: float = 0) -> tf.keras.Sequential:
   """Implements GCN of Kipf & Welling (ICLR'17) as keras Model."""
   layers = []
   for i in range(depth):
     num_units = num_classes if i == depth - 1 else hidden_units
     activation = out_activation if i == depth - 1 else hidden_activation
     if dropout > 0:
       layers.append(make_map_node_features_layer(
           tf.keras.layers.Dropout(dropout)))
 
     layers.append(gcn.GCNHomGraphUpdate(
-        units=num_units, receiver_tag=tfgnn.SOURCE, add_self_loops=True,
-        name='gcn_layer_%i' % i, activation=None, use_bias=use_bias,
-        kernel_regularizer=kernel_regularizer))
+        units=num_units, receiver_tag=tfgnn.SOURCE,
+        add_self_loops=add_self_loops, name='gcn_layer_%i' % i, activation=None,
+        use_bias=use_bias, kernel_regularizer=kernel_regularizer))
 
     if activation is not None:
       layers.append(make_map_node_features_layer(
           tf.keras.layers.Activation(activation)))
 
   return tf.keras.Sequential(layers)
 
 
 def make_gatv2_model(
     num_classes: int, *, depth: int = 2,
     num_heads=8, per_head_channels=8,
     hidden_activation: _OptionalActivation = 'relu',
     kernel_regularizer: _OptionalRegularizer = None,
     out_activation: _OptionalActivation = None,
-    add_self_loops=True,
+    add_self_loops: bool = True,
     batchnorm: bool = False, dropout: float = 0) -> tf.keras.Sequential:
   """Makes GATv2 tower interleaving GATv2 conv with batchnorm and dropout."""
   layers = []
   if add_self_loops:
     layers.append(tfgnn.keras.layers.AddSelfLoops(tfgnn.EDGES))
 
   for i in range(depth):
@@ -241,18 +241,19 @@
   model = tf.keras.Sequential(layers)
 
   return model
 
 
 def make_jknet_model(
     num_classes: int, *, depth: int = 3, hidden_units: int = 200,
-    kernel_regularizer: _OptionalRegularizer = None) -> tf.keras.Model:
+    kernel_regularizer: _OptionalRegularizer = None,
+    **gcn_kwargs) -> tf.keras.Model:
   gcn_fn = functools.partial(
       make_gcn_model, hidden_units, depth, hidden_units, out_activation='relu',
-      kernel_regularizer=kernel_regularizer)
+      kernel_regularizer=kernel_regularizer, **gcn_kwargs)
   return JKNetModel(num_classes, gcn_fn, kernel_regularizer)
 
 
 class JKNetModel(tf.keras.Model):
   """Implements Jumping Knowledge Network (Xu et al, ICML 2018).
 
   The model runs a k-layer GCN, then combines all layer features (by
@@ -292,15 +293,17 @@
 class ResidualGCNModel(tf.keras.layers.Layer):
   """GCN model with residual skip connections."""
 
   def __init__(
       self,
       num_classes: int, *, depth: int = 3, hidden_units: int = 200,
       hidden_activation='relu', out_activation=None, kernel_regularizer=None,
-      batchnorm: bool = False, dropout: float = 0, **kwargs):
+      batchnorm: bool = False, dropout: float = 0,
+      add_self_loops: bool = True,
+      **kwargs):
     super().__init__(**kwargs)
     self._config = dict(
         num_classes=num_classes, depth=depth, hidden_units=hidden_units,
         out_activation=out_activation, kernel_regularizer=kernel_regularizer,
         batchnorm=batchnorm, dropout=dropout)
 
     make_batch_norm_layer = functools.partial(
@@ -326,16 +329,16 @@
       res_model.add(tf.keras.layers.Activation(hidden_activation))
       if dropout > 0:
         res_model.add(tf.keras.layers.Dropout(dropout))
       self.res_blocks.append(tf.keras.Sequential([
           make_map_node_features_layer(res_model),
           gcn.GCNHomGraphUpdate(
               units=hidden_units, receiver_tag=tfgnn.SOURCE,
-              add_self_loops=True, name='gcn_layer_A_%i' % j, activation=None,
-              kernel_regularizer=kernel_regularizer),
+              add_self_loops=add_self_loops, name='gcn_layer_A_%i' % j,
+              activation=None, kernel_regularizer=kernel_regularizer),
       ]))
 
     postnet_model = tf.keras.Sequential()
     postnet_model.add(tf.keras.layers.Dense(
         hidden_units, kernel_regularizer=kernel_regularizer))
     if batchnorm:
       postnet_model.add(make_batch_norm_layer())
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/reader_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/reader_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,14 +58,15 @@
       keep_intermediate_examples: Used for testing. It keeps tf.Example protos
         saved in memory, in attributes `node_features` and `flat_edge_list`.
       max_size (int): If given, it will limit the number of records for all
         node sets and edge sets.
       use_tqdm: If set, all node set and edge set iterators will be wrapped with
         `tqdm.tqdm`.
     """
+    super().__init__()
     self._graph_schema = graph_schema
 
     # Node Set Name -> Node ID ->  auto-incrementing int (`node_idx`)`.
     self.compression_maps: Dict[
         tfgnn.NodeSetName, Dict[bytes, int]] = collections.defaultdict(dict)
     # Node Set Name -> list of Node ID (from above) sorted per int (`node_idx`).
     self.rev_compression_maps: Dict[
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/unigraph_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/BUILD`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,25 @@
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_contrib_test", "pytype_strict_library")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_library", "pytype_strict_contrib_test", "pytype_strict_library")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
 
 licenses(["notice"])
 
-package(default_visibility = [
-    "//tensorflow_gnn:__pkg__",
-    "//tensorflow_gnn/compat:__subpackages__",
-    "//tensorflow_gnn/converters:__subpackages__",
-    "//tensorflow_gnn/examples:__subpackages__",
-    "//tensorflow_gnn/experimental:__subpackages__",
-    "//tensorflow_gnn/graph:__subpackages__",
-    "//tensorflow_gnn/keras:__subpackages__",
-])
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = [
+        "//tensorflow_gnn:__pkg__",
+        "//tensorflow_gnn/compat:__subpackages__",
+        "//tensorflow_gnn/converters:__subpackages__",
+        "//tensorflow_gnn/examples:__subpackages__",
+        "//tensorflow_gnn/experimental:__subpackages__",
+        "//tensorflow_gnn/graph:__subpackages__",
+        "//tensorflow_gnn/keras:__subpackages__",
+        "//tensorflow_gnn/sampler:__subpackages__",
+    ],
+)
 
 pytype_strict_library(
     name = "graph_constants",
     srcs = ["graph_constants.py"],
     srcs_version = "PY3",
     deps = [
         "//:expect_tensorflow_installed",
@@ -27,26 +31,30 @@
     srcs = ["graph_tensor.py"],
     srcs_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
         ":graph_piece",
         ":tensor_utils",
+        ":tf_internal",
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
     name = "graph_tensor_ops",
     srcs = ["graph_tensor_ops.py"],
     srcs_version = "PY3",
     deps = [
         ":adjacency",
+        ":broadcast_ops",
         ":graph_constants",
         ":graph_tensor",
+        ":pool_ops",
+        ":tag_utils",
         ":tensor_utils",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/keras:keras_tensors",
     ],
 )
 
 pytype_strict_library(
@@ -79,17 +87,15 @@
     name = "graph_tensor_random",
     srcs = ["graph_tensor_random.py"],
     srcs_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
         ":graph_tensor",
-        ":schema_utils",
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn/proto:graph_schema_py_proto",
     ],
 )
 
 pytype_strict_library(
     name = "graph_tensor_pprint",
     srcs = ["graph_tensor_pprint.py"],
     srcs_version = "PY3",
@@ -99,29 +105,62 @@
     ],
 )
 
 pytype_strict_library(
     name = "tensor_utils",
     srcs = ["tensor_utils.py"],
     srcs_version = "PY3",
-    deps = ["//:expect_tensorflow_installed"],
+    deps = [
+        ":tf_internal",
+        "//:expect_tensorflow_installed",
+    ],
 )
 
 tf_py_test(
     name = "tensor_utils_test",
     srcs = ["tensor_utils_test.py"],
     python_version = "PY3",
     deps = [
         ":tensor_utils",
+        "//:expect_absl_installed",
         "//:expect_numpy_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
+    name = "readout",
+    srcs = ["readout.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":adjacency",
+        ":broadcast_ops",
+        ":graph_constants",
+        ":graph_tensor",
+        ":pool_ops",
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+tf_py_test(
+    name = "readout_test",
+    srcs = ["readout_test.py"],
+    python_version = "PY3",
+    deps = [
+        ":adjacency",
+        ":graph_constants",
+        ":graph_tensor",
+        ":graph_tensor_ops",
+        ":readout",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+pytype_strict_library(
     name = "schema_utils",
     srcs = ["schema_utils.py"],
     srcs_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
         ":graph_tensor",
@@ -135,28 +174,31 @@
     srcs = ["schema_utils_test.py"],
     data = ["@tensorflow_gnn//testdata/homogeneous"],
     python_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_tensor",
         ":schema_utils",
+        "//:expect_absl_installed",
+        "//third_party/py/google/protobuf",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/proto:graph_schema_py_proto",
         "//tensorflow_gnn/utils:test_utils",
     ],
 )
 
 pytype_strict_library(
     name = "schema_validation",
     srcs = ["schema_validation.py"],
     srcs_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
         ":graph_tensor",
+        ":readout",
         ":schema_utils",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/proto:graph_schema_py_proto",
     ],
 )
 
 tf_py_test(
@@ -196,41 +238,48 @@
     srcs = ["graph_tensor_test.py"],
     python_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
         ":graph_tensor",
         ":graph_tensor_test_utils",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 tf_py_test(
     name = "graph_tensor_ops_test",
     srcs = ["graph_tensor_ops_test.py"],
     python_version = "PY3",
     deps = [
         ":adjacency",
+        ":broadcast_ops",
         ":graph_constants",
         ":graph_tensor",
         ":graph_tensor_ops",
+        ":pool_ops",
+        ":readout",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 tf_py_test(
     name = "graph_tensor_io_test",
     srcs = ["graph_tensor_io_test.py"],
     python_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
         ":graph_tensor",
         ":graph_tensor_io",
         ":schema_utils",
+        "//:expect_absl_installed",
+        "//third_party/py/google/protobuf",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/proto:graph_schema_py_proto",
     ],
 )
 
 tf_py_test(
     name = "graph_tensor_encode_test",
@@ -240,14 +289,15 @@
     deps = [
         ":graph_constants",
         ":graph_tensor",
         ":graph_tensor_encode",
         ":graph_tensor_io",
         ":graph_tensor_random",
         ":schema_utils",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/proto:graph_schema_py_proto",
         "//tensorflow_gnn/utils:test_utils",
     ],
 )
 
 tf_py_test(
@@ -255,14 +305,15 @@
     srcs = ["graph_tensor_random_test.py"],
     data = ["@tensorflow_gnn//testdata:feature_repr"],
     python_version = "PY3",
     deps = [
         ":graph_tensor",
         ":graph_tensor_random",
         ":schema_utils",
+        "//:expect_absl_installed",
         "//:expect_numpy_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/proto:graph_schema_py_proto",
         "//tensorflow_gnn/utils:test_utils",
     ],
 )
 
@@ -284,73 +335,79 @@
 pytype_strict_library(
     name = "graph_piece",
     srcs = ["graph_piece.py"],
     srcs_version = "PY3",
     deps = [
         ":graph_constants",
         ":tensor_utils",
+        ":tf_internal",
         "//:expect_tensorflow_installed",
     ],
 )
 
 tf_py_test(
     name = "graph_piece_test",
     srcs = ["graph_piece_test.py"],
     python_version = "PY3",
     deps = [
         ":graph_piece",
+        ":tf_internal",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
     name = "adjacency",
     srcs = ["adjacency.py"],
     srcs_version = "PY3",
     deps = [
         ":graph_constants",
         ":graph_piece",
         ":tensor_utils",
+        ":tf_internal",
         "//:expect_tensorflow_installed",
     ],
 )
 
 tf_py_test(
     name = "adjacency_test",
     srcs = ["adjacency_test.py"],
     python_version = "PY3",
     deps = [
         ":adjacency",
         ":graph_constants",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
     name = "normalization_ops",
     srcs = ["normalization_ops.py"],
     srcs_version = "PY3",
     deps = [
+        ":broadcast_ops",
+        ":graph_constants",
+        ":graph_tensor",
+        ":pool_ops",
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn/graph:graph_constants",
-        "//tensorflow_gnn/graph:graph_tensor",
-        "//tensorflow_gnn/graph:graph_tensor_ops",
     ],
 )
 
 tf_py_test(
     name = "normalization_ops_test",
     srcs = ["normalization_ops_test.py"],
     python_version = "PY3",
     srcs_version = "PY3",
     deps = [
         ":adjacency",
+        ":broadcast_ops",
         ":graph_constants",
         ":graph_tensor",
-        ":graph_tensor_ops",
         ":normalization_ops",
         "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
@@ -378,17 +435,18 @@
 )
 
 tf_py_test(
     name = "preprocessing_common_test",
     srcs = ["preprocessing_common_test.py"],
     python_version = "PY3",
     deps = [
+        ":graph_tensor",
         ":preprocessing_common",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn/graph:graph_tensor",
     ],
 )
 
 pytype_strict_library(
     name = "padding_ops",
     srcs = ["padding_ops.py"],
     srcs_version = "PY3",
@@ -406,20 +464,46 @@
 
 tf_py_test(
     name = "padding_ops_test",
     srcs = ["padding_ops_test.py"],
     python_version = "PY3",
     deps = [
         ":adjacency",
-        ":graph_constants",
-        ":graph_piece",
         ":graph_tensor",
         ":graph_tensor_test_utils",
         ":padding_ops",
         ":preprocessing_common",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+pytype_strict_library(
+    name = "pool_ops",
+    srcs = ["pool_ops.py"],
+    deps = [
+        ":adjacency",
+        ":graph_constants",
+        ":graph_tensor",
+        ":tag_utils",
+        ":tensor_utils",
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn/keras:keras_tensors",
+    ],
+)
+
+tf_py_test(
+    name = "pool_ops_test",
+    srcs = ["pool_ops_test.py"],
+    deps = [
+        ":adjacency",
+        ":graph_constants",
+        ":graph_tensor",
+        ":pool_ops",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
     name = "batching_utils",
     srcs = ["batching_utils.py"],
@@ -435,36 +519,81 @@
         "//:expect_tensorflow_installed",
     ],
 )
 
 pytype_strict_library(
     name = "tag_utils",
     srcs = ["tag_utils.py"],
-    deps = [":graph_constants"],
+    deps = [
+        ":graph_constants",
+        ":graph_tensor",
+    ],
+)
+
+pytype_strict_library(
+    name = "broadcast_ops",
+    srcs = ["broadcast_ops.py"],
+    deps = [
+        ":graph_constants",
+        ":graph_tensor",
+        ":tag_utils",
+        ":tensor_utils",
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+pytype_library(
+    name = "tf_internal",
+    srcs = ["tf_internal.py"],
+    tags = [
+        # Certain deps are not provided on purpose, so this cannot be a python_strict_library.
+        "ignore_for_dep=third_party.tensorflow.python.framework.type_spec_registry",
+    ],
+    deps = [
+        "//:expect_tensorflow_installed",
+        "//third_party/tensorflow/python/framework:composite_tensor",
+        "//third_party/tensorflow/python/framework:type_spec",
+    ],
 )
 
 pytype_strict_contrib_test(
     name = "tag_utils_test",
     srcs = ["tag_utils_test.py"],
     deps = [
+        ":adjacency",
         ":graph_constants",
+        ":graph_tensor",
         ":tag_utils",
         "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
     ],
 )
 
 tf_py_test(
     name = "batching_utils_test",
     size = "large",
     srcs = ["batching_utils_test.py"],
     python_version = "PY3",
     deps = [
         ":adjacency",
         ":batching_utils",
-        ":graph_constants",
         ":graph_tensor",
         ":graph_tensor_test_utils",
-        ":padding_ops",
         ":preprocessing_common",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+tf_py_test(
+    name = "broadcast_ops_test",
+    srcs = ["broadcast_ops_test.py"],
+    deps = [
+        ":adjacency",
+        ":broadcast_ops",
+        ":graph_constants",
+        ":graph_tensor",
+        "//:expect_absl_installed",
+        "//:expect_numpy_installed",
         "//:expect_tensorflow_installed",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,18 +16,15 @@
 
 from typing import Dict, Mapping, Optional, Tuple, Union
 
 import tensorflow as tf
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_piece as gp
 from tensorflow_gnn.graph import tensor_utils as utils
-
-# pylint: disable=g-direct-tensorflow-import
-from tensorflow.python.framework import type_spec
-# pylint: enable=g-direct-tensorflow-import
+from tensorflow_gnn.graph import tf_internal
 
 Field = const.Field
 FieldSpec = const.FieldSpec
 IncidentNodeTag = const.IncidentNodeTag
 NodeSetName = const.NodeSetName
 
 Index = Tuple[NodeSetName, Field]
@@ -177,15 +174,15 @@
     return self.__class__(new_data, flat_adj.spec)
 
   @staticmethod
   def _type_spec_cls():
     return HyperAdjacencySpec
 
 
-@type_spec.register('tensorflow_gnn.HyperAdjacencySpec')
+@tf_internal.type_spec_register('tensorflow_gnn.HyperAdjacencySpec')
 class HyperAdjacencySpec(gp.GraphPieceSpecBase):
   """A type spec for `tfgnn.HyperAdjacency`."""
 
   @classmethod
   def from_incident_node_sets(
       cls,
       incident_node_sets: Mapping[IncidentNodeTag, NodeSetName],
@@ -379,15 +376,15 @@
   def __repr__(self):
     return (f'Adjacency(source=(\'{self.source_name}\', '
             f'{utils.short_repr(self.source)}), '
             f'target=(\'{self.target_name}\', '
             f'{utils.short_repr(self.target)}))')
 
 
-@type_spec.register('tensorflow_gnn.AdjacencySpec')
+@tf_internal.type_spec_register('tensorflow_gnn.AdjacencySpec')
 class AdjacencySpec(HyperAdjacencySpec):
   """A type spec for `tfgnn.Adjacency`."""
 
   @classmethod
   def from_incident_node_sets(
       cls,
       source_node_set: NodeSetName,
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/adjacency_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/adjacency_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/batching_utils_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/batching_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/dict_utils_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/dict_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_constants.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Constant strings used throughout the package."""
 
-import re
 from typing import Any, List, Mapping, Optional, Sequence, Tuple, Union
 
 import tensorflow as tf
 
 # TODO(b/245729353) Migrate string constants to enums where appropriate.
 # Formatting string for feature names.
 CONTEXT_FMT = '{stype}/{fname}'
@@ -32,24 +31,23 @@
 
 # Name of the implicitly-defined set size feature, source and target index
 # features, for serialization.
 SIZE_NAME = '#size'
 SOURCE_NAME = '#source'
 TARGET_NAME = '#target'
 RESERVED_FEATURES = frozenset({SIZE_NAME, SOURCE_NAME, TARGET_NAME})
+# The pattern of feature names (present and future) that are not allowed on a
+# graph tensor and schema, for use with re.fullmatch(pattern, feature_name).
+RESERVED_FEATURE_NAME_PATTERN = r'#.*'
 
 # The conventional feature name for the hidden state (neuron activations) of
 # an edge set, a node set or the context. Not special in GraphTensor, but used
 # in some modeling libraries on top if explicit names are not needed.
 HIDDEN_STATE = 'hidden_state'
 
-# The pattern of feature names that are not allowed on a graph tensor and
-# schema.
-RESERVED_REGEX = re.compile(r'#.*')
-
 # The internal metadata key prefix to use for hyper adjacency.
 INDEX_KEY_PREFIX = '#index.'
 
 # All edges in an EdgeSet have the same number of incident nodes. Each incident
 # node is identified by a unique tag, a small integer. For ordinary graphs,
 # these are SOURCE and TARGET, by convention. Other or additional
 # numbers can be used, e.g., for hypergraphs.
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,15 @@
 from typing import cast
 from typing import List, Tuple
 
 import tensorflow as tf
 
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import tensor_utils as utils
-
-# pylint: disable=g-direct-tensorflow-import
-from tensorflow.python.framework import composite_tensor
-from tensorflow.python.framework import type_spec
-# pylint: enable=g-direct-tensorflow-import
+from tensorflow_gnn.graph import tf_internal
 
 ShapeLike = const.ShapeLike
 Field = const.Field
 FieldSpec = const.FieldSpec
 
 # Data is a multi-level nest (see tf.nest) of Tensors, RaggedTensors and
 # subclasses of the GraphPieceBase.
@@ -49,15 +45,15 @@
 def convert_to_tensor_or_ragged(value):
   """Coerce objects other than ragged tensors to tensors."""
   return (value
           if isinstance(value, (tf.RaggedTensor, GraphPieceBase))
           else tf.convert_to_tensor(value))
 
 
-class GraphPieceBase(composite_tensor.CompositeTensor, metaclass=abc.ABCMeta):
+class GraphPieceBase(tf_internal.CompositeTensor, metaclass=abc.ABCMeta):
   """The base class for all `CompositeTensors` used inside a `GraphTensor`.
 
   A `GraphPieceBase` is a `CompositeTensor` whose value is a multi-level nest of
   tensors, ragged tensors (fields) and other subclasses of the `GraphPieceBase`.
 
    - Each `GraphPiece` (subclass of `GraphPieceBase`) is a `CompositeTensor` and
      has a matching `GraphPieceSpec` (a subclass of `GraphPieceSpecBase`) as its
@@ -216,15 +212,15 @@
 
     data = tf.nest.map_structure(
         functools.partial(
             update_fn,
             shape=shape,
             indices_dtype=indices_dtype,
             metadata=metadata), data)
-    data_spec = tf.nest.map_structure(type_spec.type_spec_from_value, data)
+    data_spec = tf.nest.map_structure(tf.type_spec_from_value, data)
 
     cls_spec = cls._type_spec_cls()
     assert issubclass(cls_spec, GraphPieceSpecBase), cls_spec
     return cls(data, cls_spec(data_spec, shape, indices_dtype, metadata))
 
   def _apply(self,
              field_map_fn: Optional[FieldMapFn] = None,
@@ -247,15 +243,15 @@
     # pylint: disable=protected-access
     def update_fn(data, spec):
       if isinstance(data, GraphPieceBase):
         assert isinstance(spec, GraphPieceSpecBase)
         if piece_map_fn is None:
           return data, spec
         data = piece_map_fn(data)
-        return data, type_spec.type_spec_from_value(data)
+        return data, tf.type_spec_from_value(data)
 
       if not isinstance(data, (tf.Tensor, tf.RaggedTensor)):
         raise TypeError(
             f'Invalid type for: {data}; should be tensor or ragged tensor')
 
       if field_map_fn is None:
         return data, spec
@@ -281,15 +277,15 @@
 
     def update_fn(value):
       if isinstance(value, GraphPieceBase):
         return value._with_attributes(new_spec.shape, new_spec.indices_dtype,
                                       new_spec._metadata)
       return value
 
-    return self.__class__(
+    return self.__class__(  # pytype: disable=not-instantiable
         tf.nest.map_structure(update_fn, self._data), new_spec)
 
   @property
   def shape(self) -> tf.TensorShape:
     """A possibly-partial shape specification for this Tensor.
 
     The returned `TensorShape` is guaranteed to have a known rank, but the
@@ -365,15 +361,15 @@
     # pylint: disable=protected-access
     return self._apply(
         functools.partial(remove_batch_dimensions, self.rank),
         lambda piece: piece._merge_batch_to_components(*args, **kwargs),
         tf.TensorShape([]))
 
 
-class GraphPieceSpecBase(type_spec.BatchableTypeSpec, metaclass=abc.ABCMeta):
+class GraphPieceSpecBase(tf_internal.BatchableTypeSpec, metaclass=abc.ABCMeta):
   """The base class for TypeSpecs of GraphPieces."""
 
   __slots__ = ['_data_spec', '_shape', '_indices_dtype', '_metadata']
 
   def __init__(self,
                data_spec: DataSpec,
                shape: tf.TensorShape,
@@ -821,15 +817,15 @@
 def _assert_not_rank0_ragged(spec: _ValueSpec) -> None:
   assert not _is_ragged_rank0(spec), ('b/187011656, use `_box_spec` and '
                                       '`_unbox_spec` for batching/unbatching')
 
 
 def _assert_value_compatible_with_spec(value: _Value, spec: _ValueSpec) -> None:
   if not spec.is_compatible_with(value):
-    value_spec = type_spec.type_spec_from_value(value)
+    value_spec = tf.type_spec_from_value(value)
     raise ValueError(f'Spec {spec} is not compatible with value {value_spec}')
 
 
 def _assert_batch_shape_compatible_with_spec(batch_shape: tf.TensorShape,
                                              spec: _ValueSpec) -> None:
   """Checks that spec is compatible with the batch shape."""
   if isinstance(spec, GraphPieceSpecBase):
@@ -1006,14 +1002,15 @@
       raise ValueError('Fields batch dimensions do not match:'
                        f' batch_rank={batch_rank},'
                        f' 1st field shape: {fields[0].shape},'
                        f' 2nd field shape: {field.shape}')
   return result
 
 
+@tf.autograph.experimental.do_not_convert
 def check_scalar_graph_piece(piece: Union[GraphPieceBase,
                                           GraphPieceSpecBase],
                              name='This operation') -> None:
   if isinstance(piece, GraphPieceSpecBase):
     piece_name: str = piece.value_type.__name__
   else:
     piece_name: str = type(piece).__name__
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_piece_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_piece_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,15 @@
 import os
 from typing import Mapping, Tuple, Union
 
 from absl.testing import parameterized
 import numpy as np
 import tensorflow as tf
 from tensorflow_gnn.graph import graph_piece as gp
-
-# pylint: disable=g-direct-tensorflow-import
-from tensorflow.python.framework import type_spec
-# pylint: enable=g-direct-tensorflow-import
+from tensorflow_gnn.graph import tf_internal
 
 TestValue = Union[np.ndarray, tf.RaggedTensor, tf.Tensor, 'TestPiece']
 
 
 class TestPiece(gp.GraphPieceBase):
   """Graph piece implementation for a simple value as a nest."""
 
@@ -57,15 +54,15 @@
     return self._data
 
   @staticmethod
   def _type_spec_cls():
     return TestPieceSpec
 
 
-@type_spec.register('tensorflow_gnn.TestPieceSpec')
+@tf_internal.type_spec_register('tensorflow_gnn.TestPieceSpec')
 class TestPieceSpec(gp.GraphPieceSpecBase):
   """Graph piece specification."""
 
   @property
   def value_type(self):
     return TestPiece
 
@@ -395,24 +392,24 @@
     ds = ds.unbatch()
     ds = ds.batch(3, True)
     ds = ds.batch(2)
 
     itr = iter(ds)
     element = next(itr)
     self.assertAllEqual(
-        type_spec.type_spec_from_value(element.value['r']),
+        tf.type_spec_from_value(element.value['r']),
         tf.RaggedTensorSpec(
             shape=[2, 3, 3, None],
             dtype=tf.float32,
             ragged_rank=3,
             row_splits_dtype=tf.int64))
 
     element = next(itr)
     self.assertAllEqual(
-        type_spec.type_spec_from_value(element.value['r']),
+        tf.type_spec_from_value(element.value['r']),
         tf.RaggedTensorSpec(
             shape=[1, 3, 3, None],
             dtype=tf.float32,
             ragged_rank=3,
             row_splits_dtype=tf.int64))
 
   def testSpecsWithDropRemainder(self):
@@ -600,15 +597,15 @@
     self.assertAllEqual(element.value['x'],
                         tf.ragged.constant([
                             [[0, 1, 2, 3, 4, 5],
                              [0, 1, 2, 3, 4, 5, 6],
                              [0, 1, 2, 3, 4, 5, 6, 7]],
                         ]))
     self.assertAllEqual(
-        type_spec.type_spec_from_value(element.value['x']),
+        tf.type_spec_from_value(element.value['x']),
         tf.RaggedTensorSpec(
             shape=[1, 3, None],
             dtype=tf.int64,
             ragged_rank=2,
             row_splits_dtype=tf.int32))
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 # limitations under the License.
 # ==============================================================================
 """The GraphTensor composite tensor and its pieces."""
 from __future__ import annotations
 
 import abc
 import collections.abc
+import re
 from typing import Any, Callable, cast, Dict, Mapping, Optional, Sequence, Union
 
 import tensorflow as tf
 from tensorflow_gnn.graph import adjacency as adj
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_piece as gp
 from tensorflow_gnn.graph import tensor_utils as utils
-
-# pylint: disable=g-direct-tensorflow-import
-from tensorflow.python.framework import type_spec
-# pylint: enable=g-direct-tensorflow-import
+from tensorflow_gnn.graph import tf_internal
 
 FieldName = const.FieldName
 NodeSetName = const.NodeSetName
 EdgeSetName = const.EdgeSetName
 ShapeLike = const.ShapeLike
 Field = const.Field
 Fields = const.Fields
@@ -208,14 +206,30 @@
     }
     data_spec.update(extra_data)
     # Note that this graph piece does not use any metadata fields.
     return cls._from_data_spec(
         data_spec, shape=sizes_spec.shape[:-1], indices_dtype=sizes_spec.dtype)
 
 
+def resolve_value(graph_piece: _GraphPieceWithFeatures,
+                  *,
+                  feature_value: Optional[Field] = None,
+                  feature_name: Optional[FieldName] = None) -> Field:
+  """Resolves feature value by its name or provided value."""
+  if (feature_value is None) == (feature_name is None):
+    raise ValueError('One of feature name of feature value must be specified.')
+
+  if feature_value is not None:
+    # TODO(b/189087785): Check that the value shape is valid for `graph_piece`.
+    return feature_value
+  if feature_name is not None:
+    return graph_piece[feature_name]
+  assert False, 'This should never happen, please file a bug with TF-GNN.'
+
+
 class Context(_GraphPieceWithFeatures):
   """A composite tensor for graph context features.
 
   The items of the context are the graph components (just like the items of a
   node set are the nodes and the items of an edge set are the edges). The
   `Context` is a composite tensor. It stores features that belong to a graph
   component as a whole, not any particular node or edge. Each context feature
@@ -325,15 +339,15 @@
     return (f'Context('
             f'features={utils.short_features_repr(self.features)}, '
             f'sizes={self.sizes}, '
             f'shape={self.shape}, '
             f'indices_dtype={self.indices_dtype!r})')
 
 
-@type_spec.register('tensorflow_gnn.ContextSpec.v2')
+@tf_internal.type_spec_register('tensorflow_gnn.ContextSpec.v2')
 class ContextSpec(_GraphPieceWithFeaturesSpec):
   """A type spec for `tfgnn.Context`."""
 
   @classmethod
   def from_field_specs(
       cls,
       *,
@@ -480,15 +494,15 @@
 
   def __repr__(self):
     return (f'NodeSet('
             f'features={utils.short_features_repr(self.features)}, '
             f'sizes={self.sizes})')
 
 
-@type_spec.register('tensorflow_gnn.NodeSetSpec')
+@tf_internal.type_spec_register('tensorflow_gnn.NodeSetSpec')
 class NodeSetSpec(_NodeOrEdgeSetSpec):
   """A type spec for `tfgnn.NodeSet`."""
 
   @classmethod
   def from_field_specs(cls,
                        *,
                        features_spec: Optional[FieldsSpec] = None,
@@ -564,26 +578,26 @@
 
     Example 1:
 
     ```python
     tfgnn.EdgeSet.from_fields(
         sizes=tf.constant([3]),
         adjacency=tfgnn.Adjacency.from_indices(
-             source=("paper", [1, 2, 2]),
-             target=("paper", [0, 0, 1])))
+            source=("paper", [1, 2, 2]),
+            target=("paper", [0, 0, 1])))
     ```
 
     Example 2:
 
     ```python
-     tfgnn.EdgeSet.from_fields(
-         sizes=tf.constant([4]),
-         adjacency=tfgnn.Adjacency.from_indices(
-             source=("paper", [1, 1, 1, 2]),
-             target=("author", [0, 1, 1, 3])))
+    tfgnn.EdgeSet.from_fields(
+        sizes=tf.constant([4]),
+        adjacency=tfgnn.Adjacency.from_indices(
+            source=("paper", [1, 1, 1, 2]),
+            target=("author", [0, 1, 1, 3])))
     ```
 
     Args:
       features: A mapping from feature name to feature Tensor or RaggedTensor.
         All feature tensors must have shape `[*graph_shape, num_edges,
         *feature_shape]`, where num_edge is the number of edges in the edge set
         (could be ragged) and feature_shape is a shape of the feature value for
@@ -613,15 +627,15 @@
   def __repr__(self):
     return (f'EdgeSet('
             f'features={utils.short_features_repr(self.features)}, '
             f'sizes={self.sizes}, '
             f'adjacency={self.adjacency})')
 
 
-@type_spec.register('tensorflow_gnn.EdgeSetSpec')
+@tf_internal.type_spec_register('tensorflow_gnn.EdgeSetSpec')
 class EdgeSetSpec(_NodeOrEdgeSetSpec):
   """A type spec for `tfgnn.EdgeSet`."""
 
   @classmethod
   def from_field_specs(cls,
                        *,
                        features_spec: Optional[FieldsSpec] = None,
@@ -712,22 +726,22 @@
   Example 1:
 
   ```python
   # A homogeneous scalar graph tensor with 1 graph component, 10 nodes and 3
   # edges. Edges connect nodes 0 and 3, 5 and 7, 9 and 1. There are no features.
   tfgnn.GraphTensor.from_pieces(
       node_sets = {
-        'node': tfgnn.NodeSet.from_fields(sizes=[10], features={})},
+          'node': tfgnn.NodeSet.from_fields(sizes=[10], features={})},
       edge_sets = {
-        'edge': tfgnn.EdgeSet.from_fields(
-           sizes=[3],
-           features={},
-           adjacency=tfgnn.Adjacency.from_indices(
-             source=('node', [0, 5, 9]),
-             target=('node', [3, 7, 1])))})
+          'edge': tfgnn.EdgeSet.from_fields(
+              sizes=[3],
+              features={},
+              adjacency=tfgnn.Adjacency.from_indices(
+                  source=('node', [0, 5, 9]),
+                  target=('node', [3, 7, 1])))})
   ```
 
   All graph pieces provide a mapping interface to access their features by name
   as `graph_piece[feature_name]`. Each graph piece feature has the shape
   `[*graph_shape, num_items, *feature_shape]`, where `graph_shape` is the shape
   of the GraphTensor, `num_items` is the number of items in a piece (number of
   graph components, number of nodes in a node set or edges in an edge set). The
@@ -757,15 +771,15 @@
       context=tfgnn.Context.from_fields(
           features={'venue': [1980519, 9756463]}),
       node_sets={
           'author': tfgnn.NodeSet.from_fields(sizes=[2, 2], features={}),
           'paper': tfgnn.NodeSet.from_fields(
               sizes=[3, 1], features={'year': [2018, 2017, 2017, 2022]})},
       edge_sets={
-          'is_writen': tfgnn.EdgeSet.from_fields(
+          'is_written': tfgnn.EdgeSet.from_fields(
               sizes=[4, 2],
               features={},
               adjacency=tfgnn.Adjacency.from_indices(
                   source=('paper', [0, 1, 1, 0, 2, 3]),
                   target=('author', [0, 0, 1, 2, 3, 3])))})
   ```
 
@@ -776,16 +790,17 @@
 
   Example 3:
 
   ```python
   # The year of publication of the first article in each venue from the
   # previous example.
   papers = venues.node_sets['paper']
-  years_by_venue = tf.RaggedTensor.from_row_lengths(papers['year'],
-                                                    papers.sizes)
+  years_by_venue = tf.RaggedTensor.from_row_lengths(
+      papers['year'], papers.sizes
+  )
   first_paper_year = tf.reduce_min(years_by_venue, -1)  # [2017, 2022]
   ```
 
   The GraphTensor, as a composite tensor, can be used directly in a
   tf.data.Dataset, as an input or output of a Keras Layer or a tf.function,
   and so on. As any other tensor, the GraphTensor has an associated type
   specification object, a GraphTensorSpec, that holds the `tf.TensorSpec` and
@@ -835,15 +850,15 @@
     if isinstance(context.spec, ContextSpec) and isinstance(
         indicative_piece.spec, _NodeOrEdgeSetSpec):
       # Reevaluate context sizes from the node or edge set sizes. The latter are
       # directly set by user, whereas the context sizes are indirectly inferred
       # from the context feature shapes or set to zero-shaped tensor if the
       # context has no features.
       context_sizes = tf.ones_like(indicative_piece.sizes,
-                                   context.indices_dtype)
+                                   indicative_piece.indices_dtype)
       context = context.from_fields(
           features=context.features, sizes=context_sizes)
 
     assert isinstance(indicative_piece, _GraphPieceWithFeatures)
     return cls._from_data(
         data={
             GraphTensor._DATAKEY_CONTEXT: context,
@@ -1079,17 +1094,17 @@
           for set_name, edge_set in self.edge_sets.items()
       }
 
     return self.__class__.from_pieces(new_context, new_node_sets, new_edge_sets)
 
   def remove_features(
       self,
-      context: Optional[Sequence[NodeSetName]] = None,
-      node_sets: Optional[Mapping[NodeSetName, Sequence[NodeSetName]]] = None,
-      edge_sets: Optional[Mapping[NodeSetName, Sequence[EdgeSetName]]] = None,
+      context: Optional[Sequence[FieldName]] = None,
+      node_sets: Optional[Mapping[NodeSetName, Sequence[FieldName]]] = None,
+      edge_sets: Optional[Mapping[NodeSetName, Sequence[FieldName]]] = None,
   ) -> 'GraphTensor':
     """Returns a new GraphTensor with some features removed.
 
     The graph topology and the other features remain unchanged.
 
     Example 1. Removes the id feature from node set 'node.a'.
 
@@ -1185,15 +1200,15 @@
     # so we truncate it but still keep it unique.
     return (f'GraphTensor(\n'
             f'  context={self.context},\n'
             f'  node_set_names={list(self.node_sets.keys())},\n'
             f'  edge_set_names={list(self.edge_sets.keys())})')
 
 
-@type_spec.register('tensorflow_gnn.GraphTensorSpec')
+@tf_internal.type_spec_register('tensorflow_gnn.GraphTensorSpec')
 class GraphTensorSpec(gp.GraphPieceSpecBase):
   """A type spec for `tfgnn.GraphTensor`."""
 
   @classmethod
   def from_piece_specs(
       cls,
       context_spec: Optional[ContextSpec] = None,
@@ -1493,15 +1508,15 @@
 
   # Featureless edges with no sizes are okay because we can compute sizes
   # from the adjacency source and target.
   # This is impossible for node sets with no features
   if node_features is None and node_set_sizes is None:
     raise ValueError('node_set_sizes must be provided if node_features is not')
 
-  if tf.rank(source) != 1 or tf.rank(target) != 1:
+  if source.shape.rank != 1 or target.shape.rank != 1:
     raise ValueError('source and target must be rank-1 dense tensors')
 
   node_features, num_nodes = _fields_and_size_from_fieldorfields(
       node_features, HIDDEN_STATE)
   edge_features, _ = _fields_and_size_from_fieldorfields(
       edge_features, HIDDEN_STATE)
   context_features, _ = _fields_and_size_from_fieldorfields(
@@ -1533,15 +1548,81 @@
       context=Context.from_fields(
           features=context_features,
           sizes=tf.ones_like(node_sizes),
       ),
   )
 
 
-def check_homogeneous_graph_tensor(graph: Union[GraphTensor, GraphTensorSpec],
-                                   name='This operation') -> None:
-  """Raises ValueError unless there is exactly one node set and edge set."""
+def get_aux_type_prefix(set_name: const.SetName) -> Optional[str]:
+  """Returns type prefix of aux node or edge set names, or `None` if non-aux.
+
+  Auxiliary node sets and edge sets in a `tfgnn.GraphTensor` have names that
+  begin with an underscore `_` (preferred) or any of the characters `#`, `!`,
+  `%`, `.`, `^`, and `~` (reserved for future use). They store structural
+  information needed by helper functions like `tfgnn.structured_readout()`,
+  beyond the node sets and edge sets that represent graph data from the
+  application domain.
+
+  By convention, the names of auxiliary graph pieces begin with a type prefix
+  that contains the leading special character and all letters, digits and
+  underscores following it.
+
+  Users can define their own aux types and handle them in their own code.
+  The TF-GNN library uses the following types:
+
+    * `"_readout"` and (rarely) `"_shadow"`, for `tfgnn.structured_readout()`.
+
+  See the named function(s) for how the respective types of auxiliary edge sets
+  and node sets are formed.
+
+  Args:
+    set_name: The name of a node set or edge set in a `tfgnn.GraphTensor`,
+      `tfgnn.GraphTensorSpec` or `tfgnn.GraphSchema`.
+
+  Returns:
+    For an auxiliary node set or edge set, a non-empty prefix that identifies
+    its type; for other node sets or edge sets, `None`.
+  """
+  match = re.match(r'[_#!%.^~][a-zA-Z0-9_]*', set_name)
+  if match:
+    return match.group()
+
+
+def get_homogeneous_node_and_edge_set_name(
+    graph: Union[GraphTensor, GraphTensorSpec],
+    name: str = 'This operation') -> tuple[str, str]:
+  """Returns the sole `node_set_name, edge_set_name` or raises `ValueError`.
+
+  By default, this function ignores auxiliary node sets and edge sets for which
+  `tfgnn.get_aux_type_prefix(set_name) is not None` (e.g., those needed for
+  `tfgnn.structured_readout()`), as appropriate for model-building code.
+
+  Args:
+    graph: the `GraphTensor` or `GraphTensorSpec` to check.
+    name: Optionally, the name of the operation (library function, class, ...)
+      to mention in the user-visible error message in case an exception is
+      raised.
+
+  Returns:
+    A tuple `node_set_name, edge_set_name` with the unique node set and edge
+    set, resp., in `graph` for which `tfgnn.get_aux_type_prefix(set_name)` is
+    `None`.
+  """
   spec = get_graph_tensor_spec(graph)
-  if len(spec.node_sets_spec) != 1 or len(spec.edge_sets_spec) != 1:
+  node_set_names = [node_set_name for node_set_name in spec.node_sets_spec
+                    if not get_aux_type_prefix(node_set_name)]
+  edge_set_names = [edge_set_name for edge_set_name in spec.edge_sets_spec
+                    if not get_aux_type_prefix(edge_set_name)]
+  if len(node_set_names) != 1 or len(edge_set_names) != 1:
     raise ValueError(
         f'{name} requires a graph with 1 node set and 1 edge set '
-        f'but got {len(spec.node_sets_spec)} and {len(spec.edge_sets_spec)}')
+        f'but got {len(node_set_names)} node sets and '
+        f'{len(edge_set_names)} edge sets.')
+  return node_set_names[0], edge_set_names[0]
+
+
+def check_homogeneous_graph_tensor(
+    graph: Union[GraphTensor, GraphTensorSpec],
+    name: str = 'This operation') -> None:
+  """Raises ValueError when tfgnn.get_homogeneous_node_and_edge_set_name() does.
+  """
+  _ = get_homogeneous_node_and_edge_set_name(graph, name=name)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_encode_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_encode_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
       _check_size_fields(spec, flat_fields) if validate else None):
     flat_fields = _restore_types(spec, prefix, flat_fields)
     return tf.identity(_unflatten_graph_fields(spec, flat_fields, prefix or ''))
 
 
 def get_io_spec(spec: gt.GraphTensorSpec,
                 prefix: Optional[str] = None,
-                validate: bool = False) -> Dict[str, IOFeature]:
+                validate: bool = True) -> Dict[str, IOFeature]:
   """Returns tf.io parsing features for `GraphTensorSpec` type spec.
 
   This function returns a mapping of `tf.train.Feature` names to configuration
   objects that can be used to parse instances of `tf.train.Example` (see
   https://www.tensorflow.org/api_docs/python/tf/io). The resulting mapping can
   be used with `tf.io.parse_example()` for reading the individual fields of a
   `GraphTensor` instance. This essentially forms our encoding of a `GraphTensor`
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_io_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_io_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_ops_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_ops_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,483 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for gt.GraphTensor extension type (go/tf-gnn-api)."""
-
 import collections
-import functools
 from typing import Mapping, Union
 
 from absl.testing import parameterized
-# TODO(b/266817638): Remove when fixed
-from packaging import version
 import tensorflow as tf
 from tensorflow_gnn.graph import adjacency as adj
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
 from tensorflow_gnn.graph import graph_tensor_ops as ops
-
-partial = functools.partial
+from tensorflow_gnn.graph import pool_ops
+from tensorflow_gnn.graph import readout
 
 as_tensor = tf.convert_to_tensor
 as_ragged = tf.ragged.constant
 
 GraphPiece = Union[gt.Context, gt.NodeSet, gt.EdgeSet]
 
 
-class PoolingTest(tf.test.TestCase, parameterized.TestCase):
-  """Tests for pooling operations."""
-
-  @parameterized.parameters([
-      dict(
-          description='max pooling of edge features to source and targed nodes',
-          pooling='max',
-          node_set=gt.NodeSet.from_fields(sizes=as_tensor([1, 2]), features={}),
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([2, 2]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  const.SOURCE: ('node', as_tensor([0, 0, 1, 2])),
-                  const.TARGET: ('node', as_tensor([0, 0, 2, 1]))
-              }),
-              features={
-                  'scalar':
-                      as_tensor([1., 2., 3., 4.]),
-                  'ragged':
-                      as_ragged(
-                          [[[1, 8], [2, 7]], [[3, 6]], [[4, 5]], [[5, 4]]],
-                          ragged_rank=1)
-              }),
-          expected_source_fields={
-              'scalar':
-                  as_tensor([2., 3., 4.]),
-              'ragged':
-                  as_ragged([[[3, 8], [2, 7]], [[4, 5]], [[5, 4]]],
-                            ragged_rank=1),
-          },
-          expected_target_fields={
-              'scalar':
-                  as_tensor([2., 4., 3.]),
-              'ragged':
-                  as_ragged([[[3, 8], [2, 7]], [[5, 4]], [[4, 5]]],
-                            ragged_rank=1),
-          }),
-      dict(
-          description='max_no_inf pooling of edge features to connected nodes',
-          pooling='max_no_inf',
-          node_set=gt.NodeSet.from_fields(sizes=as_tensor([3]), features={}),
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([4]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  const.SOURCE: ('node', as_tensor([1, 1, 2, 2])),
-                  const.TARGET: ('node', as_tensor([0, 0, 1, 1]))
-              }),
-              features={
-                  'scalar':
-                      as_tensor([1., 2., 3., 4.]),
-                  'ragged':
-                      as_ragged(
-                          [[[1, 8], [2, 7]], [[3, 6]], [[4, 5]], [[5, 4]]],
-                          ragged_rank=1)
-              }),
-          expected_source_fields={
-              'scalar':
-                  as_tensor([0., 2., 4.]),
-              'ragged':
-                  as_ragged([[], [[3, 8], [2, 7]], [[5, 5]]], ragged_rank=1),
-          },
-          expected_target_fields={
-              'scalar':
-                  as_tensor([2., 4., 0.]),
-              'ragged':
-                  as_ragged([[[3, 8], [2, 7]], [[5, 5]], []], ragged_rank=1),
-          }),
-      dict(
-          description='sum pooling of edge features to source and targed nodes',
-          pooling='sum',
-          node_set=gt.NodeSet.from_fields(sizes=as_tensor([1, 2]), features={}),
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([2, 3]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
-              }),
-              features={
-                  'scalar':
-                      as_tensor([1., 2., 3., 4., 5.]),
-                  'vector':
-                      as_tensor([[1., 5.], [2., 4.], [3., 3.], [4., 2.],
-                                 [5., 1.]]),
-                  'matrix':
-                      as_tensor([[[1.]], [[2.]], [[3.]], [[4.]], [[5.]]]),
-                  'ragged.1':
-                      as_ragged([[1, 2], [], [3, 4], [], [5]]),
-                  'ragged.2':
-                      as_ragged([[[1], [2]], [], [[3]], [], []])
-              }),
-          expected_source_fields={
-              'scalar':
-                  as_tensor([1. + 2. + 3., 0., 4. + 5.]),
-              'vector':
-                  as_tensor([[1. + 2. + 3., 5. + 4. + 3.], [0., 0.],
-                             [4. + 5., 2. + 1.]]),
-              'matrix':
-                  as_tensor([[[1. + 2. + 3.]], [[0.]], [[4. + 5.]]]),
-              'ragged.1':
-                  as_ragged([[1 + 3, 2 + 4], [], [5]]),
-              'ragged.2':
-                  as_ragged([[[1 + 3], [2]], [], []]),
-          },
-          expected_target_fields={
-              'scalar':
-                  as_tensor([3. + 4. + 5., 2., 1.]),
-              'vector':
-                  as_tensor([[3. + 4. + 5., 3. + 2. + 1.], [2., 4.], [1., 5.]]),
-              'matrix':
-                  as_tensor([[[3. + 4. + 5.]], [[2.]], [[1.]]]),
-              'ragged.1':
-                  as_ragged([[3 + 5, 4], [], [1, 2]]),
-              'ragged.2':
-                  as_ragged([[[3]], [], [[1], [2]]]),
-          })
-  ])
-  def testEdgeFieldToNode(self, description: str, pooling: str,
-                          node_set: gt.NodeSet, edge_set: gt.EdgeSet,
-                          expected_source_fields: Mapping[str, const.Field],
-                          expected_target_fields: Mapping[str, const.Field]):
-    del description
-    graph = gt.GraphTensor.from_pieces(
-        node_sets={'node': node_set}, edge_sets={'edge': edge_set})
-
-    for fname, expected in expected_source_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.pool_edges_to_node(
-              graph, 'edge', const.SOURCE, pooling, feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.pool(graph, const.SOURCE, edge_set_name='edge',
-                   reduce_type=pooling, feature_name=fname))
-    for fname, expected in expected_target_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.pool_edges_to_node(
-              graph, 'edge', const.TARGET, pooling, feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.pool(graph, const.TARGET, edge_set_name='edge',
-                   reduce_type=pooling, feature_name=fname))
-
-  @parameterized.parameters([
-      dict(
-          description='sum pooling of node features to context, 1 component',
-          pooling='sum',
-          node_set=gt.NodeSet.from_fields(
-              sizes=as_tensor([3]),
-              features={
-                  'scalar': as_tensor([1., 2., 3]),
-                  'vector': as_tensor([[1., 0.], [2., 0.], [3., 0.]]),
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]]]),
-                  'ragged.1': as_ragged([[1, 2], [3], []])
-              }),
-          expected_context_fields={
-              'scalar': as_tensor([1. + 2. + 3.]),
-              'vector': as_tensor([[1. + 2. + 3., 0. + 0. + 0.]]),
-              'matrix': as_tensor([[[1. + 2. + 3.]]]),
-              'ragged.1': as_ragged([[1 + 3, 2]])
-          }),
-      dict(
-          description='sum pooling of node features to context, 2 components',
-          pooling='sum',
-          node_set=gt.NodeSet.from_fields(
-              sizes=as_tensor([2, 1]),
-              features={
-                  'scalar': as_tensor([1., 2., 3]),
-                  'vector': as_tensor([[1., 0.], [2., 0.], [3., 0.]]),
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]]]),
-                  'ragged.1': as_ragged([[1, 2], [3], []]),
-                  'ragged.2': as_ragged([[[1, 2], []], [[3]], []])
-              }),
-          expected_context_fields={
-              'scalar': as_tensor([1. + 2., 3.]),
-              'vector': as_tensor([[1. + 2., 0. + 0.], [3., 0.]]),
-              'matrix': as_tensor([[[1. + 2.]], [[3.]]]),
-              'ragged.1': as_ragged([[1 + 3, 2], []]),
-              'ragged.2': as_ragged([[[1 + 3, 2], []], []])
-          })
-  ])
-  def testNodeFieldToContext(self, description: str, pooling: str,
-                             node_set: gt.NodeSet,
-                             expected_context_fields: Mapping[str,
-                                                              const.Field]):
-    del description
-    graph = gt.GraphTensor.from_pieces(node_sets={'node': node_set})
-
-    for fname, expected in expected_context_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.pool_nodes_to_context(graph, 'node', pooling, feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.pool(graph, const.CONTEXT, node_set_name='node',
-                   reduce_type=pooling, feature_name=fname))
-
-  @parameterized.parameters([
-      dict(
-          description='max pooling of edge features to graph context',
-          pooling='max',
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([3]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  0: ('node', as_tensor([0, 0, 0])),
-              }),
-              features={
-                  'scalar': as_tensor([1., 2., 3]),
-                  'vector': as_tensor([[1., 0.], [2., 0.], [3., 0.]]),
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]]]),
-                  'ragged.1': as_ragged([[1, 2], [3], []])
-              }),
-          expected_context_fields={
-              'scalar': as_tensor([3.]),
-              'vector': as_tensor([[3., 0.]]),
-              'matrix': as_tensor([[[3.]]]),
-              'ragged.1': as_ragged([[3, 2]])
-          }),
-      dict(
-          description='min pooling of node features to graph context',
-          pooling='min',
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([2, 1]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  0: ('node', as_tensor([0, 0, 0])),
-              }),
-              features={
-                  'scalar': as_tensor([1., 2., 3]),
-                  'vector': as_tensor([[1., 0.], [2., 0.], [3., 0.]]),
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]]]),
-                  'ragged.1': as_ragged([[1, 2], [3], []]),
-                  'ragged.2': as_ragged([[[1, 2], []], [[3]], []])
-              }),
-          expected_context_fields={
-              'scalar': as_tensor([1., 3.]),
-              'vector': as_tensor([[1., 0.], [3., 0.]]),
-              'matrix': as_tensor([[[1.]], [[3.]]]),
-              'ragged.1': as_ragged([[1, 2], []]),
-              'ragged.2': as_ragged([[[1, 2], []], []])
-          })
-  ])
-  def testEdgeFieldToContext(self, description: str, pooling: str,
-                             edge_set: gt.EdgeSet,
-                             expected_context_fields: Mapping[str,
-                                                              const.Field]):
-    del description
-    graph = gt.GraphTensor.from_pieces(edge_sets={'edge': edge_set})
-
-    for fname, expected in expected_context_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.pool_edges_to_context(graph, 'edge', pooling, feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.pool(graph, const.CONTEXT, edge_set_name='edge',
-                   reduce_type=pooling, feature_name=fname))
-
-
-class BroadcastingTest(tf.test.TestCase, parameterized.TestCase):
-  """Tests for broadcasting operations."""
-
-  @parameterized.parameters([
-      dict(
-          description='source and target node features to edges broadcasting',
-          node_set=gt.NodeSet.from_fields(
-              sizes=as_tensor([3]),
-              features={
-                  'scalar': as_tensor([1., 2., 3]),
-                  'vector': as_tensor([[1., 3.], [2., 2.], [3., 1.]]),
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]]]),
-                  'ragged': as_ragged([[1, 2], [3], []])
-              }),
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([2, 2]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
-              }),
-              features={}),
-          expected_source_fields={
-              'scalar':
-                  as_tensor([1., 1., 1., 3., 3.]),
-              'vector':
-                  as_tensor([[1., 3.], [1., 3.], [1., 3.], [3., 1.], [3., 1.]]),
-              'matrix':
-                  as_tensor([[[1.]], [[1.]], [[1.]], [[3.]], [[3.]]]),
-              'ragged':
-                  as_ragged([[1, 2], [1, 2], [1, 2], [], []])
-          },
-          expected_target_fields={
-              'scalar':
-                  as_tensor([3., 2., 1., 1., 1.]),
-              'vector':
-                  as_tensor([[3., 1.], [2., 2.], [1., 3.], [1., 3.], [1., 3.]]),
-              'matrix':
-                  as_tensor([[[3.]], [[2.]], [[1.]], [[1.]], [[1.]]]),
-              'ragged':
-                  as_ragged([[], [3], [1, 2], [1, 2], [1, 2]])
-          })
-  ])
-  def testEdgeFieldFromNode(self, description: str, node_set: gt.NodeSet,
-                            edge_set: gt.EdgeSet,
-                            expected_source_fields: Mapping[str, const.Field],
-                            expected_target_fields: Mapping[str, const.Field]):
-    del description
-    graph = gt.GraphTensor.from_pieces(
-        node_sets={'node': node_set}, edge_sets={'edge': edge_set})
-
-    for fname, expected in expected_source_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.broadcast_node_to_edges(
-              graph, 'edge', const.SOURCE, feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.broadcast(
-              graph, const.SOURCE, edge_set_name='edge', feature_name=fname))
-    for fname, expected in expected_target_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.broadcast_node_to_edges(
-              graph, 'edge', const.TARGET, feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.broadcast(
-              graph, const.TARGET, edge_set_name='edge', feature_name=fname))
-
-  @parameterized.parameters([
-      dict(
-          description='context features to nodes broadcasting, 1 component',
-          context=gt.Context.from_fields(features={
-              'scalar': as_tensor([1]),
-              'vector': as_tensor([[1., 2.]]),
-              'matrix': as_tensor([[[1., 2., 3.], [4., 5., 6.]]]),
-              'ragged': as_ragged([[[], [1], [], [2, 3]]]),
-          }),
-          node_set=gt.NodeSet.from_fields(sizes=as_tensor([3]), features={}),
-          expected_node_fields={
-              'scalar':
-                  as_tensor([1] * 3),
-              'vector':
-                  as_tensor([[1., 2.]] * 3),
-              'matrix':
-                  as_tensor([[[1., 2., 3.], [4., 5., 6.]]] * 3),
-              'ragged':
-                  as_ragged([[[], [1], [], [2, 3]], [[], [1], [], [2, 3]],
-                             [[], [1], [], [2, 3]]]),
-          }),
-      dict(
-          description='context features to nodes broadcasting, 2 components',
-          context=gt.Context.from_fields(features={
-              'scalar': as_tensor([1, 2]),
-              'vector': as_tensor([[1.], [2.]]),
-              'ragged': as_ragged([[[], [1], []], [[1], [], [2]]]),
-          }),
-          node_set=gt.NodeSet.from_fields(sizes=as_tensor([3, 2]), features={}),
-          expected_node_fields={
-              'scalar':
-                  as_tensor([1, 1, 1, 2, 2]),
-              'vector':
-                  as_tensor([[1.], [1.], [1.], [2.], [2.]]),
-              'ragged':
-                  as_ragged([[[], [1], []], [[], [1], []], [[], [1], []],
-                             [[1], [], [2]], [[1], [], [2]]]),
-          })
-  ])
-  def testNodeFieldFromContext(self, description: str, context: gt.Context,
-                               node_set: gt.NodeSet,
-                               expected_node_fields: Mapping[str, const.Field]):
-    del description
-    graph = gt.GraphTensor.from_pieces(
-        context=context, node_sets={'node': node_set})
-
-    for fname, expected in expected_node_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.broadcast_context_to_nodes(graph, 'node', feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.broadcast(
-              graph, const.CONTEXT, node_set_name='node', feature_name=fname))
-
-  @parameterized.parameters([
-      dict(
-          description='context features to edges broadcasting, 1 component',
-          context=gt.Context.from_fields(features={
-              'scalar': as_tensor([1]),
-              'vector': as_tensor([[1., 2.]]),
-              'matrix': as_tensor([[[1., 2., 3.], [4., 5., 6.]]]),
-              'ragged': as_ragged([[[], [1], [], [2, 3]]]),
-          }),
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([3]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  0: ('node', as_tensor([0, 0, 0])),
-              }),
-              features={}),
-          expected_edge_fields={
-              'scalar':
-                  as_tensor([1] * 3),
-              'vector':
-                  as_tensor([[1., 2.]] * 3),
-              'matrix':
-                  as_tensor([[[1., 2., 3.], [4., 5., 6.]]] * 3),
-              'ragged':
-                  as_ragged([[[], [1], [], [2, 3]], [[], [1], [], [2, 3]],
-                             [[], [1], [], [2, 3]]]),
-          }),
-      dict(
-          description='context features to nodes broadcasting, 2 components',
-          context=gt.Context.from_fields(features={
-              'scalar': as_tensor([1, 2]),
-              'vector': as_tensor([[1.], [2.]]),
-              'ragged': as_ragged([[[], [1], []], [[1], [], [2]]]),
-          }),
-          edge_set=gt.EdgeSet.from_fields(
-              sizes=as_tensor([3, 2]),
-              adjacency=adj.HyperAdjacency.from_indices({
-                  0: ('node', as_tensor([0, 0, 0, 0, 0])),
-              }),
-              features={}),
-          expected_edge_fields={
-              'scalar':
-                  as_tensor([1, 1, 1, 2, 2]),
-              'vector':
-                  as_tensor([[1.], [1.], [1.], [2.], [2.]]),
-              'ragged':
-                  as_ragged([[[], [1], []], [[], [1], []], [[], [1], []],
-                             [[1], [], [2]], [[1], [], [2]]]),
-          })
-  ])
-  def testEdgeFieldFromContext(self, description: str, context: gt.Context,
-                               edge_set: gt.EdgeSet,
-                               expected_edge_fields: Mapping[str, const.Field]):
-    del description
-    graph = gt.GraphTensor.from_pieces(
-        context=context, edge_sets={'edge': edge_set})
-
-    for fname, expected in expected_edge_fields.items():
-      self.assertAllEqual(
-          expected,
-          ops.broadcast_context_to_edges(graph, 'edge', feature_name=fname))
-      self.assertAllEqual(
-          expected,
-          ops.broadcast(
-              graph, const.CONTEXT, edge_set_name='edge', feature_name=fname))
-
-
 class FirstNodeOpsTest(tf.test.TestCase, parameterized.TestCase):
   """Tests for operations on first nodes per component (e.g., root nodes)."""
 
   @parameterized.parameters([
       dict(
           description='1 component',
           node_set=gt.NodeSet.from_fields(
@@ -540,171 +90,190 @@
 
 
 class ShuffleOpsTest(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.parameters([
       dict(
           description='scalar',
-          context=gt.Context.from_fields(features={
-              'scalar': as_tensor([1, 2, 3]),
-          }),
+          context=gt.Context.from_fields(
+              features={
+                  'scalar': as_tensor([1, 2, 3]),
+              }
+          ),
           node_set=gt.NodeSet.from_fields(
               sizes=as_tensor([2, 1]),
               features={
-                  'scalar': as_tensor([1., 2., 3]),
-              }),
+                  'scalar': as_tensor([1.0, 2.0, 3]),
+              },
+          ),
           edge_set=gt.EdgeSet.from_fields(
               sizes=as_tensor([2, 3]),
               adjacency=adj.HyperAdjacency.from_indices({
                   const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
+                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0])),
               }),
               features={
-                  'scalar': as_tensor([1., 2., 3., 4., 5.]),
-              }),
-          expected_fields={
-              gt.Context: {
-                  'scalar': [2, 1, 3]
+                  'scalar': as_tensor([1.0, 2.0, 3.0, 4.0, 5.0]),
               },
-              gt.NodeSet: {
-                  'scalar': [2., 1., 3.]
-              },
-              gt.EdgeSet: {
-                  'scalar': [5., 2., 3., 1., 4.]
-              },
-          }),
+          ),
+          expected_fields={
+              gt.Context: {'scalar': [2, 1, 3]},
+              gt.NodeSet: {'scalar': [2.0, 1.0, 3.0]},
+              gt.EdgeSet: {'scalar': [5.0, 2.0, 3.0, 1.0, 4.0]},
+          },
+      ),
       dict(
           description='vector',
-          context=gt.Context.from_fields(features={
-              'vector': as_tensor([[1], [2], [3]]),
-          }),
+          context=gt.Context.from_fields(
+              features={
+                  'vector': as_tensor([[1], [2], [3]]),
+              }
+          ),
           node_set=gt.NodeSet.from_fields(
               sizes=as_tensor([2, 1]),
               features={
-                  'vector': as_tensor([[1., 3.], [2., 2.], [3., 1.]]),
-              }),
+                  'vector': as_tensor([[1.0, 3.0], [2.0, 2.0], [3.0, 1.0]]),
+              },
+          ),
           edge_set=gt.EdgeSet.from_fields(
               sizes=as_tensor([2, 3]),
               adjacency=adj.HyperAdjacency.from_indices({
                   const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
+                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0])),
               }),
               features={
-                  'vector':
-                      as_tensor([[1., 5.], [2., 4.], [3., 3.], [4., 2.],
-                                 [5., 1.]]),
-              }),
-          expected_fields={
-              gt.Context: {
-                  'vector': [[2], [1], [3]]
-              },
-              gt.NodeSet: {
-                  'vector': [[2., 2.], [1., 3.], [3., 1.]]
+                  'vector': as_tensor([
+                      [1.0, 5.0],
+                      [2.0, 4.0],
+                      [3.0, 3.0],
+                      [4.0, 2.0],
+                      [5.0, 1.0],
+                  ]),
               },
+          ),
+          expected_fields={
+              gt.Context: {'vector': [[2], [1], [3]]},
+              gt.NodeSet: {'vector': [[2.0, 2.0], [1.0, 3.0], [3.0, 1.0]]},
               gt.EdgeSet: {
-                  'vector': [[5., 1.], [2., 4.], [3., 3.], [1., 5.], [4., 2.]]
+                  'vector': [
+                      [5.0, 1.0],
+                      [2.0, 4.0],
+                      [3.0, 3.0],
+                      [1.0, 5.0],
+                      [4.0, 2.0],
+                  ]
               },
-          }),
+          },
+      ),
       dict(
           description='matrix',
           context=gt.Context.from_fields(),
           node_set=gt.NodeSet.from_fields(
               sizes=as_tensor([2, 1]),
               features={
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]]]),
-              }),
+                  'matrix': as_tensor([[[1.0]], [[2.0]], [[3.0]]]),
+              },
+          ),
           edge_set=gt.EdgeSet.from_fields(
               sizes=as_tensor([2, 3]),
               adjacency=adj.HyperAdjacency.from_indices({
                   const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
+                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0])),
               }),
               features={
-                  'matrix': as_tensor([[[1.]], [[2.]], [[3.]], [[4.]], [[5.]]]),
-              }),
-          expected_fields={
-              gt.NodeSet: {
-                  'matrix': [[[2.]], [[1.]], [[3.]]]
+                  'matrix': as_tensor(
+                      [[[1.0]], [[2.0]], [[3.0]], [[4.0]], [[5.0]]]
+                  ),
               },
+          ),
+          expected_fields={
+              gt.NodeSet: {'matrix': [[[2.0]], [[1.0]], [[3.0]]]},
               gt.EdgeSet: {
-                  'matrix': [[[5.]], [[2.]], [[3.]], [[1.]], [[4.]]]
+                  'matrix': [[[5.0]], [[2.0]], [[3.0]], [[1.0]], [[4.0]]]
               },
-          }),
+          },
+      ),
       dict(
           description='ragged.1',
-          context=gt.Context.from_fields(features={
-              'ragged.1': as_ragged([[[], [1], []], [[1], [3], [4], [2]]]),
-          }),
+          context=gt.Context.from_fields(
+              features={
+                  'ragged.1': as_ragged([[[], [1], []], [[1], [3], [4], [2]]]),
+              }
+          ),
           node_set=gt.NodeSet.from_fields(
               sizes=as_tensor([2, 1]),
               features={
-                  'ragged.1':
-                      as_ragged([[[1, 2], [4, 4], [5, 5]], [[3, 3]], []]),
-              }),
+                  'ragged.1': as_ragged(
+                      [[[1, 2], [4, 4], [5, 5]], [[3, 3]], []]
+                  ),
+              },
+          ),
           edge_set=gt.EdgeSet.from_fields(
               sizes=as_tensor([2, 3]),
               adjacency=adj.HyperAdjacency.from_indices({
                   const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
+                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0])),
               }),
               features={
                   'ragged.1': as_ragged([[[1, 2]], [], [[3, 4]], [], [[5, 5]]]),
-              }),
+              },
+          ),
           expected_fields={
               gt.Context: {
-                  'ragged.1': [[[], [4], [2]], [[1], [], [1], [3]]]
+                  'ragged.1': as_ragged([[[], [4], [2]], [[1], [], [1], [3]]])
               },
               gt.NodeSet: {
-                  'ragged.1': [[[4, 4], [5, 5], [3, 3]], [[1, 2]], []]
+                  'ragged.1': as_ragged(
+                      [[[4, 4], [5, 5], [3, 3]], [[1, 2]], []]
+                  )
               },
               gt.EdgeSet: {
-                  'ragged.1': [[[5, 5]], [], [[1, 2]], [], [[3, 4]]]
+                  'ragged.1': as_ragged([[[5, 5]], [], [[1, 2]], [], [[3, 4]]])
               },
-          }),
+          },
+      ),
       dict(
           description='ragged.2',
           context=gt.Context.from_fields(),
           node_set=gt.NodeSet.from_fields(
               sizes=as_tensor([2, 1]),
-              features={'ragged.2': as_ragged([[[1, 2, 4], []], [[3]],
-                                               [[5]]])}),
+              features={'ragged.2': as_ragged([[[1, 2, 4], []], [[3]], [[5]]])},
+          ),
           edge_set=gt.EdgeSet.from_fields(
               sizes=as_tensor([2, 3]),
               adjacency=adj.HyperAdjacency.from_indices({
                   const.SOURCE: ('node', as_tensor([0, 0, 0, 2, 2])),
-                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0]))
+                  const.TARGET: ('node', as_tensor([2, 1, 0, 0, 0])),
               }),
               features={
-                  'ragged.2':
-                      as_ragged([[[1], [2], [4]], [], [[3], [5]], [], []])
-              }),
+                  'ragged.2': as_ragged(
+                      [[[1], [2], [4]], [], [[3], [5]], [], []]
+                  )
+              },
+          ),
           expected_fields={
               gt.NodeSet: {
-                  'ragged.2': [[[1, 2, 4], [5]], [[3]], [[]]]
+                  'ragged.2': as_ragged([[[1, 2, 4], [5]], [[3]], [[]]])
               },
               gt.EdgeSet: {
-                  'ragged.2': [[[2], [4], [3]], [], [[1], [5]], [], []]
+                  'ragged.2': as_ragged(
+                      [[[2], [4], [3]], [], [[1], [5]], [], []]
+                  )
               },
-          }),
+          },
+      ),
   ])
   def testShuffleFeaturesGlobally(
       self,
       description: str,
       context: gt.Context,
       node_set: gt.NodeSet,
       edge_set: gt.EdgeSet,
       expected_fields: Mapping[GraphPiece, Mapping[str, const.Field]],
   ):
-
-    # TODO(b/266817638): Remove when fixed
-    if version.parse(tf.__version__) < version.parse(
-        '2.11.0'
-    ) and description in {'ragged.1', 'ragged.2'}:
-      self.skipTest('Bad Test')
-
     del description
     graph = gt.GraphTensor.from_pieces(
         context,
         {'node': node_set},
         {'edge': edge_set})
     shuffled = ops.shuffle_features_globally(graph, seed=8191)
 
@@ -713,181 +282,17 @@
 
     for fname, expected in expected_fields.get(gt.NodeSet, {}).items():
       self.assertAllEqual(expected, shuffled.node_sets['node'].features[fname])
 
     for fname, expected in expected_fields.get(gt.EdgeSet, {}).items():
       self.assertAllEqual(expected, shuffled.edge_sets['edge'].features[fname])
 
-
-class ReduceOpsTest(tf.test.TestCase, parameterized.TestCase):
-
-  @parameterized.parameters([
-      dict(
-          reduce_op=tf.math.unsorted_segment_max,
-          values=as_tensor([tf.float32.min, tf.float32.max,
-                            float('nan')]),
-          segment_ids=as_tensor([0, 1, 2]),
-          num_segments=3,
-          empty_set_value=-1,
-          expected_result=as_tensor(
-              [tf.float32.min, tf.float32.max,
-               float('nan')])),
-      dict(
-          reduce_op=tf.math.unsorted_segment_min,
-          values=as_tensor([tf.float32.min, tf.float32.max]),
-          segment_ids=as_tensor([0, 1]),
-          num_segments=3,
-          empty_set_value=-1,
-          expected_result=as_tensor([tf.float32.min, tf.float32.max, -1.])),
-      dict(
-          reduce_op=tf.math.unsorted_segment_max,
-          values=as_tensor([1., 2.]),
-          segment_ids=as_tensor([1, 1]),
-          num_segments=3,
-          empty_set_value=-1,
-          expected_result=as_tensor([-1., 2., -1.])),
-      dict(
-          reduce_op=tf.math.unsorted_segment_min,
-          values=as_tensor([[1., 2.], [3., 4.]]),
-          segment_ids=as_tensor([0, 2]),
-          num_segments=3,
-          empty_set_value=0,
-          expected_result=as_tensor([[1., 2.], [0., 0.], [3., 4.]])),
-      dict(
-          reduce_op=tf.math.unsorted_segment_max,
-          values=as_ragged([[1., 2., 3.], [2., 1.], [1.]]),
-          segment_ids=as_tensor([0, 0, 2]),
-          num_segments=3,
-          empty_set_value=0,
-          expected_result=as_ragged([[2., 2., 3.], [], [1.]])),
-      dict(
-          reduce_op=tf.math.unsorted_segment_min,
-          values=as_ragged([[[1., 2.], [3., 4.]], [], [[5., 6.]]],
-                           ragged_rank=1),
-          segment_ids=as_tensor([1, 2, 1]),
-          num_segments=3,
-          empty_set_value=0,
-          expected_result=as_ragged([[], [[1., 2.], [3., 4.]], []],
-                                    ragged_rank=1)),
-      dict(
-          reduce_op=tf.math.unsorted_segment_min,
-          values=tf.constant([], tf.int32, shape=[0, 2]),
-          segment_ids=tf.constant([], tf.int32),
-          num_segments=3,
-          empty_set_value=0,
-          expected_result=as_tensor([[0, 0], [0, 0], [0, 0]])),
-  ])
-  def testWithEmptySetValue(self, reduce_op: ops.UnsortedReduceOp,
-                            values: const.Field, segment_ids: tf.Tensor,
-                            num_segments: tf.Tensor, empty_set_value,
-                            expected_result):
-
-    reduce_op = ops.with_empty_set_value(reduce_op, empty_set_value)
-    self.assertAllEqual(
-        reduce_op(values, segment_ids, num_segments), expected_result)
-
-  @parameterized.parameters([
-      dict(
-          values=as_tensor([tf.float32.min, tf.float32.max, float('nan')]),
-          segment_ids=as_tensor([0, 1, 2]),
-          num_segments=3,
-          replacement_value=-1,
-          expected_result=as_tensor([-1., tf.float32.max, float('nan')])),
-      dict(
-          values=as_tensor([1., 2.]),
-          segment_ids=as_tensor([1, 1]),
-          num_segments=3,
-          replacement_value=-1,
-          expected_result=as_tensor([-1., 2., -1.])),
-      dict(
-          values=as_tensor([[1., 2.], [3., 4.]]),
-          segment_ids=as_tensor([0, 2]),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_tensor([[1., 2.], [0., 0.], [3., 4.]])),
-      dict(
-          values=as_ragged([[1., 2., 3.], [2., 1.], [tf.float32.min]]),
-          segment_ids=as_tensor([0, 0, 2]),
-          num_segments=3,
-          replacement_value=1,
-          expected_result=as_ragged([[2., 2., 3.], [], [1.]])),
-      dict(
-          values=as_ragged([[[1., 2.], [3., 4.]], [], [[5., 6.]]],
-                           ragged_rank=1),
-          segment_ids=as_tensor([1, 2, 1]),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_ragged([[], [[5., 6.], [3., 4.]], []],
-                                    ragged_rank=1)),
-      dict(
-          values=tf.constant([], tf.int32, shape=[0, 2]),
-          segment_ids=tf.constant([], tf.int32),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_tensor([[0, 0], [0, 0], [0, 0]])),
-  ])
-  def testWithMinusInfReplaced(self,
-                               values: const.Field, segment_ids: tf.Tensor,
-                               num_segments: tf.Tensor, replacement_value,
-                               expected_result):
-
-    reduce_op = ops.with_minus_inf_replaced(tf.math.unsorted_segment_max,
-                                            replacement_value)
-    self.assertAllEqual(
-        reduce_op(values, segment_ids, num_segments), expected_result)
-
-  @parameterized.parameters([
-      dict(
-          values=as_tensor([tf.float32.min, tf.float32.max, float('nan')]),
-          segment_ids=as_tensor([0, 1, 2]),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_tensor([tf.float32.min, 0., float('nan')])),
-      dict(
-          values=as_tensor([1., 2.]),
-          segment_ids=as_tensor([1, 1]),
-          num_segments=3,
-          replacement_value=-1,
-          expected_result=as_tensor([-1., 1., -1.])),
-      dict(
-          values=as_tensor([[1., 2.], [3., 4.]]),
-          segment_ids=as_tensor([0, 2]),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_tensor([[1., 2.], [0., 0.], [3., 4.]])),
-      dict(
-          values=as_ragged([[1., 2., 3.], [2., 1.], [tf.float32.max]]),
-          segment_ids=as_tensor([0, 0, 2]),
-          num_segments=3,
-          replacement_value=1,
-          expected_result=as_ragged([[1., 1., 3.], [], [1.]])),
-      dict(
-          values=as_ragged([[[1., 2.], [3., 4.]], [], [[5., 6.]]],
-                           ragged_rank=1),
-          segment_ids=as_tensor([1, 2, 1]),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_ragged([[], [[1., 2.], [3., 4.]], []],
-                                    ragged_rank=1)),
-      dict(
-          values=tf.constant([], tf.int32, shape=[0, 2]),
-          segment_ids=tf.constant([], tf.int32),
-          num_segments=3,
-          replacement_value=0,
-          expected_result=as_tensor([[0, 0], [0, 0], [0, 0]])),
-  ])
-  def testWithPlusInfReplaced(self,
-                              values: const.Field, segment_ids: tf.Tensor,
-                              num_segments: tf.Tensor, replacement_value,
-                              expected_result):
-
-    reduce_op = ops.with_plus_inf_replaced(tf.math.unsorted_segment_min,
-                                           replacement_value)
-    self.assertAllEqual(
-        reduce_op(values, segment_ids, num_segments), expected_result)
+  def testTFLite(self):
+    # TODO(b/277938756): Implement when tf.random.shuffle is supported.
+    self.skipTest('Shuffling ops are unsupported in TFLite.')
 
 
 def as_tensor_list(l):
   return [tf.convert_to_tensor(x) for x in l]
 
 
 def as_ragged_list(l):
@@ -1052,14 +457,20 @@
       offset_edges += es
 
     self.assertAllEqual(offset_nodes, sum(node_sizes))
     self.assertAllEqual(offset_edges, sum(edge_sizes))
     self.assertAllEqual(offset_new_edges, sum(expected_edge_sizes))
 
 
+class _ReorderNodes(tf.keras.layers.Layer):
+
+  def call(self, graph, permutations):
+    return ops.reorder_nodes(graph, permutations)
+
+
 class ReorderNodesTest(tf.test.TestCase, parameterized.TestCase):
   _heterogeneous = gt.GraphTensor.from_pieces(
       node_sets={
           'A':
               gt.NodeSet.from_fields(
                   sizes=[2, 2], features={
                       's': ['a', 'b', 'c', 'd'],
@@ -1174,14 +585,38 @@
 
     result = ops.reorder_nodes(graph, {'A': [2, 3, 0, 1], 'B': [2, 0, 1]})
     self.assertAllEqual(result.node_sets['A']['s'], ['c', 'd', 'a', 'b'])
     self.assertAllEqual(result.node_sets['B']['s'], ['z', 'x', 'y'])
     self.assertAllEqual(result.edge_sets['A->B'].adjacency.source, [2, 3, 0, 1])
     self.assertAllEqual(result.edge_sets['A->B'].adjacency.target, [1, 2, 0, 1])
 
+  def testTFLite(self):
+    test_graph_dict = {'fa': tf.range(10)}
+    inputs = {'fa': tf.keras.Input([1], None, 'fa', tf.int32)}
+    graph_in = _MakeGraphTensor()(inputs)
+    node_permuter = _ReorderNodes()
+    graph_out = node_permuter(
+        graph_in, {'a': tf.constant([9, 8, 7, 6, 5, 4, 3, 2, 1, 0]),
+                   'b': tf.constant([9, 8, 7, 6, 5, 4, 3, 2, 1, 0])})
+    outputs = tf.keras.layers.Layer(name='final_edge_adjacency')(
+        graph_out.edge_sets['aa'].adjacency[const.SOURCE]
+    )
+    model = tf.keras.Model(inputs, outputs)
+    expected = model(test_graph_dict).numpy()
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith('2.10.'):
+      self.skipTest('GNN models are unsupported in TFLite until TF 2.11 but '
+                    f'got TF {tf.__version__}')
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner('serving_default')
+    obtained = signature_runner(**test_graph_dict)['final_edge_adjacency']
+    self.assertAllEqual(expected, obtained)
 
 _SEED = 42
 
 
 class ShuffleNodesTest(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.named_parameters([('adjacency',
@@ -1201,20 +636,30 @@
             'node':
                 gt.NodeSet.from_fields(
                     sizes=[2],
                     features={
                         's': ['a', 'b'],
                         'v': [[1, 2], [3, 4]],
                         'r': as_ragged([[1], [2, 3]]),
-                    })
+                    }),
+            '_readout':  # To be ignored.
+                gt.NodeSet.from_fields(
+                    sizes=[2],
+                    features={'label': [42, 105]}),
         },
         edge_sets={
             'edge':
                 gt.EdgeSet.from_fields(
                     sizes=[3], adjacency=adjacency, features={'s': [1, 2, 3]}),
+            '_readout/thingy':
+                gt.EdgeSet.from_fields(
+                    sizes=[2],
+                    adjacency=adj.Adjacency.from_indices(
+                        source=('node', [0, 1]),
+                        target=('_readout', [0, 1]))),
         })
     a_first_count = 0
     for _ in range(30):
       result = ops.shuffle_nodes(graph, seed=_SEED)
       self.assertAllEqual(result.context['s'], ['x'])
       edge_set = result.edge_sets['edge']
       self.assertAllEqual(edge_set.features['s'], [1, 2, 3])
@@ -1230,14 +675,20 @@
       else:
         self.assertAllEqual(features['s'], ['b', 'a'])
         self.assertAllEqual(features['v'], [[3, 4], [1, 2]])
         self.assertAllEqual(features['r'], as_ragged([[2, 3], [1]]))
         self.assertAllEqual(edge_set.adjacency[const.SOURCE], [0, 1, 1])
         self.assertAllEqual(edge_set.adjacency[const.TARGET], [1, 0, 1])
 
+      # Readout is invariant to the shuffling of "all" node sets by default.
+      self.assertAllEqual(result.node_sets['_readout']['label'], [42, 105])
+      self.assertAllEqual(
+          readout.structured_readout(result, 'thingy', feature_name='s'),
+          ['a', 'b'])
+
     self.assertBetween(a_first_count, 1, 29)
 
   @parameterized.parameters([
       dict(node_sets=()),
       dict(node_sets=('1')),
       dict(node_sets=('2')),
       dict(node_sets=('1', '2')),
@@ -1334,17 +785,22 @@
         self.assertAllEqual(adjacency.source, [0, 1, 3, 2])
         self.assertAllEqual(adjacency.target, [1, 0, 2, 3])
       else:
         assert False, permutation
 
     self.assertLen(unique_permutations, 4)
 
+  def testTFLite(self):
+    # TODO(b/277938756): Implement when tf.random.shuffle is supported.
+    self.skipTest('Shuffling ops are unsupported in TFLite.')
+
 
 class NodeDegreeTest(tf.test.TestCase, parameterized.TestCase):
   """Tests for computing degree of each node w.r.t. one side of an edge set."""
+
   @parameterized.parameters([
       dict(
           description='varying degrees for receiver nodes',
           node_sets={
               'a': gt.NodeSet.from_fields(
                   sizes=as_tensor([4]),
                   features={'s': [1, 2, 3, 4]}),
@@ -1399,14 +855,20 @@
       self.assertAllEqual(get, expected)
 
     for edge_set_name, expected in expected_target_degree.items():
       get = ops.node_degree(graph, edge_set_name, const.TARGET)
       self.assertAllEqual(get, expected)
 
 
+class _MaskEdges(tf.keras.layers.Layer):
+
+  def call(self, graph, edge_set_name, mask, masked_edge_set_name):
+    return ops.mask_edges(graph, edge_set_name, mask, masked_edge_set_name)
+
+
 class EdgeMaskingTest(tf.test.TestCase, parameterized.TestCase):
   """Tests for edge-masking operations over a scalar GraphTensor."""
 
   @parameterized.named_parameters(
       dict(
           testcase_name='EdgeSetWVariousFeatures',
           graph=gt.GraphTensor.from_pieces(
@@ -1773,10 +1235,492 @@
                     )),
         })
     with self.assertRaisesRegex(
         tf.errors.InvalidArgumentError,
         r'boolean_edge_mask should have the same shape with the adjacency.*'):
       ops.mask_edges(graph, 'edges', as_tensor([True, False]), 'masked')
 
+  def testTFLite(self):
+    test_graph_dict = {'fa': tf.range(10)}
+    inputs = {'fa': tf.keras.Input([1], None, 'fa', tf.int32)}
+    graph_in = _MakeGraphTensor()(inputs)
+    edge_masker = _MaskEdges()
+    graph_out = edge_masker(
+        graph_in,
+        'aa',
+        tf.convert_to_tensor([True, False, True, True]),
+        'masked_aa')
+    outputs = tf.keras.layers.Layer(name='final_edge_adjacency')(
+        graph_out.edge_sets['masked_aa'].adjacency[const.SOURCE]
+    )
+    model = tf.keras.Model(inputs, outputs)
+    expected = model(test_graph_dict).numpy()
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith('2.10.'):
+      self.skipTest('GNN models are unsupported in TFLite until TF 2.11 but '
+                    f'got TF {tf.__version__}')
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner('serving_default')
+    obtained = signature_runner(**test_graph_dict)['final_edge_adjacency']
+    self.assertAllEqual(expected, obtained)
+
+
+class _MakeLineGraphTargetToSource(tf.keras.layers.Layer):
+
+  def call(self, graph):
+    return ops.convert_to_line_graph(
+        graph,
+        connect_from=const.TARGET,
+        connect_to=const.SOURCE,)
+
+
+class LineGraphTest(tf.test.TestCase, parameterized.TestCase):
+
+  def _make_test_graph(self, add_readout=False):
+    return _MakeGraphTensor()(
+        {'fa': tf.range(10)},
+        add_readout=add_readout
+    )
+
+  def testContextFeatures(self):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(graph_tensor)
+    for feature_name, feature in graph_tensor.context.features.items():
+      self.assertAllEqual(line_graph.context[feature_name], feature)
+
+  def testNodeFeatures(self):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(graph_tensor)
+    for edge_set_name, edge_set in graph_tensor.edge_sets.items():
+      for feature_name, feature in edge_set.features.items():
+        self.assertAllEqual(
+            line_graph.node_sets[edge_set_name][feature_name], feature
+        )
+
+  def testEdgeFeatures(self):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        use_node_features_as_line_graph_edge_features=True
+    )
+    self.assertCountEqual(
+        line_graph.edge_sets,
+        ['aa=>aa', 'aa=>ab', 'ab=>ba', 'ba=>aa', 'ba=>ab'],
+    )
+
+    def _assert_features_equal(
+        node_set_name, edge_set_name, node_used_for_edge
+    ):
+      node_set = graph_tensor.node_sets[node_set_name]
+      edge_set = line_graph.edge_sets[edge_set_name]
+      for feature_name, node_feature in node_set.features.items():
+        edge_feature = edge_set[feature_name]
+        if node_used_for_edge:
+          self.assertAllEqual(
+              edge_feature, tf.gather(node_feature, node_used_for_edge)
+          )
+        else:
+          self.assertEqual(tf.size(edge_feature), 0)
+
+    _assert_features_equal('a', 'aa=>aa', [0, 0])
+    _assert_features_equal('a', 'aa=>ab', [0, 1])
+    _assert_features_equal('a', 'ba=>aa', [8])
+    _assert_features_equal('a', 'ba=>ab', [7, 8])
+    _assert_features_equal('b', 'ab=>ba', [0, 0, 1, 1, 1, 1, 1, 1, 9])
+
+  def testResultIsAdjacency(self):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_from=const.TARGET,
+        connect_to=const.SOURCE,
+    )
+    for edge_set in line_graph.edge_sets.values():
+      self.assertIsInstance(edge_set.adjacency, adj.Adjacency)
+
+  @parameterized.named_parameters([('', True), ('NonBacktracking', False)])
+  def testConnectivityTargetToSource(self, backtracking: bool):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_from=const.TARGET,
+        connect_to=const.SOURCE,
+        non_backtracking=not backtracking,
+    )
+    self.assertCountEqual(
+        line_graph.edge_sets,
+        ['aa=>aa', 'aa=>ab', 'ab=>ba', 'ba=>aa', 'ba=>ab'],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>aa'].adjacency[const.SOURCE],
+        tf.constant([0] * backtracking + [0]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>aa'].adjacency[const.TARGET],
+        tf.constant([0] * backtracking + [1]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>ab'].adjacency[const.SOURCE],
+        tf.constant([0, 1]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>ab'].adjacency[const.TARGET],
+        tf.constant([0, 2]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ab=>ba'].adjacency[const.SOURCE],
+        tf.constant([1, 1, 0, 0, 0, 2, 2, 2] + [4] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ab=>ba'].adjacency[const.TARGET],
+        tf.constant([0, 3, 1, 2, 4, 1, 2, 4] + [5] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>aa'].adjacency[const.SOURCE],
+        tf.constant([5]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>aa'].adjacency[const.TARGET],
+        tf.constant([3]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>ab'].adjacency[const.SOURCE],
+        tf.constant([0] + [5] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>ab'].adjacency[const.TARGET],
+        tf.constant([3] + [4] * backtracking),
+    )
+
+  @parameterized.named_parameters([('', True), ('NonBacktracking', False)])
+  def testConnectivityTargetToTarget(self, backtracking: bool):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_from=const.TARGET,
+        connect_to=const.TARGET,
+        non_backtracking=not backtracking,
+    )
+    self.assertCountEqual(
+        line_graph.edge_sets,
+        ['aa=>aa', 'aa=>ba', 'ab=>ab', 'ba=>aa', 'ba=>ba'],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>aa'].adjacency[const.SOURCE],
+        tf.constant([0, 1, 2, 3] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>aa'].adjacency[const.TARGET],
+        tf.constant([0, 1, 2, 3] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>ba'].adjacency[const.SOURCE],
+        tf.constant([]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['aa=>ba'].adjacency[const.TARGET],
+        tf.constant([]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ab=>ab'].adjacency[const.SOURCE],
+        tf.constant([1, 0] * backtracking + [0, 2] + [2, 3, 4] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ab=>ab'].adjacency[const.TARGET],
+        tf.constant([1, 0] * backtracking + [2, 0] + [2, 3, 4] * backtracking),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>aa'].adjacency[const.SOURCE],
+        tf.constant([]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>aa'].adjacency[const.TARGET],
+        tf.constant([]),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>ba'].adjacency[const.SOURCE],
+        tf.constant(
+            [4, 2] * backtracking + [2, 3] + [3, 1, 0, 5] * backtracking
+        ),
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['ba=>ba'].adjacency[const.TARGET],
+        tf.constant(
+            [4, 2] * backtracking + [3, 2] + [3, 1, 0, 5] * backtracking
+        ),
+    )
+
+  def testConnectOriginalFeatures(self):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_with_original_nodes=True,
+    )
+    for node_set_name, node_set in graph_tensor.node_sets.items():
+      for feature_name, feature in node_set.features.items():
+        self.assertAllEqual(
+            line_graph.node_sets[f'original/{node_set_name}'][feature_name],
+            feature,
+        )
+
+  def testOriginalToLineGraph(self):
+    """The original/to/... edges have the correct endpoints."""
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_with_original_nodes=True,
+    )
+    bcast = broadcast_ops.broadcast_node_to_edges(
+        line_graph,
+        'original/to/aa',
+        const.SOURCE,
+        feature_value=2 ** tf.range(10),
+    )
+    summed_messages = pool_ops.pool_edges_to_node(
+        line_graph,
+        'original/to/aa',
+        const.TARGET,
+        'sum',
+        feature_value=bcast,
+    )
+    # In node set 'aa' of the line graph, each node receives the unique value
+    # from the source node of the original edge it represents.
+    self.assertAllEqual(
+        summed_messages,
+        2 ** graph_tensor.edge_sets['aa'].adjacency[const.SOURCE]
+    )
+
+  def testSendLineGraphToOriginal(self):
+    """The original/from/... edges have the correct endpoints."""
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_with_original_nodes=True,
+    )
+    bcast = broadcast_ops.broadcast_node_to_edges(
+        line_graph,
+        'original/from/ba',
+        const.TARGET,
+        feature_value=2 ** tf.range(10),
+    )
+    summed_messages = pool_ops.pool_edges_to_node(
+        line_graph,
+        'original/from/ba',
+        const.SOURCE,
+        'sum',
+        feature_value=bcast,
+    )
+    # In node set 'ba' of the line graph, each node receives the unique value
+    # from the target node of the original edge it represents.
+    self.assertAllEqual(
+        summed_messages,
+        2 ** graph_tensor.edge_sets['ba'].adjacency[const.TARGET]
+    )
+
+  def testConnectOriginalEdges(self):
+    graph_tensor = self._make_test_graph()
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor,
+        connect_with_original_nodes=True,
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['original/to/aa'].adjacency[const.SOURCE],
+        graph_tensor.edge_sets['aa'].adjacency[const.SOURCE],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['original/from/aa'].adjacency[const.TARGET],
+        graph_tensor.edge_sets['aa'].adjacency[const.TARGET],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['original/to/ab'].adjacency[const.SOURCE],
+        graph_tensor.edge_sets['ab'].adjacency[const.SOURCE],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['original/from/ab'].adjacency[const.TARGET],
+        graph_tensor.edge_sets['ab'].adjacency[const.TARGET],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['original/to/ba'].adjacency[const.SOURCE],
+        graph_tensor.edge_sets['ba'].adjacency[const.SOURCE],
+    )
+    self.assertAllEqual(
+        line_graph.edge_sets['original/from/ba'].adjacency[const.TARGET],
+        graph_tensor.edge_sets['ba'].adjacency[const.TARGET],
+    )
+
+  def testAuxiliaryNodeSetError(self):
+    graph_tensor = self._make_test_graph(add_readout=True)
+    edge_sets = dict(graph_tensor.edge_sets)
+    del edge_sets['_readout/testE']
+    graph_tensor = gt.GraphTensor.from_pieces(
+        context=graph_tensor.context,
+        node_sets=graph_tensor.node_sets,
+        edge_sets=edge_sets,
+    )
+    with self.assertRaises(ValueError):
+      ops.convert_to_line_graph(graph_tensor)
+
+  def testAuxiliaryEdgeSetError(self):
+    graph_tensor = self._make_test_graph(add_readout=True)
+    node_sets = dict(graph_tensor.node_sets)
+    del node_sets['_readout']
+    graph_tensor = gt.GraphTensor.from_pieces(
+        context=graph_tensor.context,
+        node_sets=node_sets,
+        edge_sets=graph_tensor.edge_sets,
+    )
+    with self.assertRaises(ValueError):
+      ops.convert_to_line_graph(graph_tensor)
+
+  def testNoAuxiliaryLineGraph(self):
+    graph_tensor = self._make_test_graph(add_readout=True)
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor, connect_with_original_nodes=True
+    )
+    self.assertCountEqual(
+        line_graph.node_sets,
+        ['aa', 'ab', 'ba', 'original/a', 'original/b', '_readout'],
+    )
+    self.assertCountEqual(
+        line_graph.edge_sets,
+        [
+            'original/from/aa',
+            'original/to/aa',
+            'original/from/ab',
+            'original/to/ab',
+            'original/from/ba',
+            'original/to/ba',
+            '_readout/testE',
+            'aa=>aa',
+            'aa=>ab',
+            'ab=>ba',
+            'ba=>aa',
+            'ba=>ab',
+        ],
+    )
+
+  def testNonBacktrackingAuxiliary(self):
+    graph_tensor = self._make_test_graph(add_readout=True)
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor, connect_with_original_nodes=True
+    )
+    line_graph_nb = ops.convert_to_line_graph(
+        graph_tensor, connect_with_original_nodes=True, non_backtracking=True
+    )
+    for edge_set_name in line_graph_nb.edge_sets:
+      if edge_set_name not in [
+          'aa=>aa',
+          'aa=>ab',
+          'ab=>ba',
+          'ba=>aa',
+          'ba=>ab',
+      ]:
+        self.assertAllEqual(
+            line_graph.edge_sets[edge_set_name].adjacency.source,
+            line_graph_nb.edge_sets[edge_set_name].adjacency.source,
+        )
+        self.assertAllEqual(
+            line_graph.edge_sets[edge_set_name].adjacency.target,
+            line_graph_nb.edge_sets[edge_set_name].adjacency.target,
+        )
+
+  def testStructuredReadout(self):
+    graph_tensor = self._make_test_graph(add_readout=True)
+    line_graph = ops.convert_to_line_graph(
+        graph_tensor, connect_with_original_nodes=True
+    )
+    readout_f2 = readout.structured_readout(line_graph, 'testE',
+                                            feature_name='f2')
+    self.assertAllEqual(readout_f2, [100, 102, 101, 109])
+
+  def testTFLite(self):
+    test_graph_dict = {'fa': tf.range(10)}
+    inputs = {'fa': tf.keras.Input([1], None, 'fa', tf.int32)}
+    graph_in = _MakeGraphTensor()(inputs)
+    linegraph_maker = _MakeLineGraphTargetToSource()
+    graph_out = linegraph_maker(graph_in)
+    outputs = tf.keras.layers.Layer(name='final_edge_adjacency')(
+        graph_out.edge_sets['ab=>ba'].adjacency.source
+    )
+    model = tf.keras.Model(inputs, outputs)
+    expected = model(test_graph_dict).numpy()
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith('2.10.'):
+      self.skipTest('GNN models are unsupported in TFLite until TF 2.11 but '
+                    f'got TF {tf.__version__}')
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner('serving_default')
+    obtained = signature_runner(**test_graph_dict)['final_edge_adjacency']
+    self.assertAllEqual(expected, obtained)
+
+
+# TODO(b/274779989): Replace this layer with a more standard representation
+# of GraphTensor as a dict of plain Tensors.
+class _MakeGraphTensor(tf.keras.layers.Layer):
+
+  def call(self, inputs, *, add_readout=False):
+    node_sets = {
+        'a': gt.NodeSet.from_fields(
+            features={'fa': inputs['fa'], 'f2': 100 + tf.range(10)},
+            sizes=as_tensor([8, 2]),
+        ),
+        'b': gt.NodeSet.from_fields(
+            features={'fb': tf.range(10), 'f2': 100 + tf.range(10)},
+            sizes=as_tensor([8, 2]),
+        ),
+    }
+    edge_sets = {
+        'aa': gt.EdgeSet.from_fields(
+            features={'faa': tf.range(4), 'f2': 100 + tf.range(4)},
+            sizes=as_tensor([3, 1]),
+            adjacency=adj.HyperAdjacency.from_indices({
+                const.SOURCE: ('a', as_tensor([0, 0, 2, 8])),
+                const.TARGET: ('a', as_tensor([0, 1, 3, 9])),
+            }),
+        ),
+        'ab': gt.EdgeSet.from_fields(
+            features={'fab': tf.range(5), 'f2': 100 + tf.range(5)},
+            sizes=as_tensor([4, 1]),
+            adjacency=adj.HyperAdjacency.from_indices({
+                const.SOURCE: ('a', as_tensor([0, 2, 1, 7, 8])),
+                const.TARGET: ('b', as_tensor([1, 0, 1, 2, 9])),
+            }),
+        ),
+        'ba': gt.EdgeSet.from_fields(
+            features={'fba': tf.range(6), 'f2': 100 + tf.range(6)},
+            sizes=as_tensor([5, 1]),
+            adjacency=adj.HyperAdjacency.from_indices({
+                const.SOURCE: ('b', as_tensor([0, 1, 1, 0, 1, 9])),
+                const.TARGET: ('a', as_tensor([7, 6, 5, 5, 4, 8])),
+            }),
+        ),
+    }
+    if add_readout:
+      node_sets['_readout'] = gt.NodeSet.from_fields(
+          features={'f1': 100 + tf.range(4)},
+          sizes=as_tensor([3, 1]),
+      )
+      edge_sets['_readout/testE'] = gt.EdgeSet.from_fields(
+          features={'f1': 100 + tf.range(4)},
+          sizes=as_tensor([3, 1]),
+          adjacency=adj.HyperAdjacency.from_indices({
+              const.SOURCE: ('b', as_tensor([0, 2, 1, 9])),
+              const.TARGET: ('_readout', as_tensor([0, 1, 2, 3])),
+          }),
+      )
+    return gt.GraphTensor.from_pieces(
+        context=gt.Context.from_fields(
+            features={'fc': as_tensor([10, 11]), 'f2': as_tensor([20, 21])}
+        ),
+        node_sets=node_sets,
+        edge_sets=edge_sets,
+    )
+
 
 if __name__ == '__main__':
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_pprint_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_pprint_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 from typing import Any, Dict, List, Optional, Text, Tuple, Union
 
 import tensorflow as tf
 
 from tensorflow_gnn.graph import adjacency as adj
 from tensorflow_gnn.graph import graph_constants as gc
 from tensorflow_gnn.graph import graph_tensor as gt
-from tensorflow_gnn.graph import schema_utils
-import tensorflow_gnn.proto.graph_schema_pb2 as schema_pb2
 
 
 @tf.function
 def random_ragged_tensor(
     shape: List[Union[int, None, tf.Tensor]],
     dtype: tf.dtypes.DType,
     sample_values: Optional[List[Any]] = None,
@@ -147,14 +145,18 @@
     spec: gt.GraphTensorSpec,
     sample_dict: Optional[SampleDict] = None,
     row_lengths_range: Tuple[int, int] = (2, 8),
     row_splits_dtype: tf.dtypes.DType = tf.int32,
     validate: bool = True) -> gt.GraphTensor:
   """Generate a graph tensor from a schema, with random features.
 
+  NOTE: This function does not (yet?) support the generation of the auxiliary
+  node set for `tfgnn.structured_readout()`. It should not be included in the
+  `spec`, and if needed, should be added separately in a later step.
+
   Args:
     spec: A GraphTensorSpec instance that describes the graph tensor.
     sample_dict: A dict of (set-type, set-name, field-name) to list-of-values to
       sample from. The intended purpose is to generate random values that are
       more realistic, more representative of what the actual dataset will
       contain. You can provide such if the values aren't provided for a feature,
       random features are inserted of the right type.
@@ -248,62 +250,11 @@
   elif feature.HasField("int64_list"):
     return list(feature.int64_list.value)
   elif feature.HasField("bytes_list"):
     return list(feature.bytes_list.value)
   return []
 
 
-def _get_sample_values_dict(schema: schema_pb2.GraphSchema) -> SampleDict:
-  """Return example values for sampling."""
-  sample_dict = {}
-  for fname, feature in schema.context.features.items():
-    key = (gc.CONTEXT, None, fname)
-    sample_dict[key] = _get_feature_values(feature.sample_values)
-  for set_name, node_set in schema.node_sets.items():
-    for fname, feature in node_set.features.items():
-      key = (gc.NODES, set_name, fname)
-      sample_dict[key] = _get_feature_values(feature.sample_values)
-  for set_name, edge_set in schema.edge_sets.items():
-    for fname, feature in edge_set.features.items():
-      key = (gc.EDGES, set_name, fname)
-      sample_dict[key] = _get_feature_values(feature.sample_values)
-  return sample_dict
-
-
-def random_graph_tensor_from_schema(
-    schema: schema_pb2.GraphSchema,
-    row_lengths_range: Tuple[int, int] = (2, 8),
-    row_splits_dtype: tf.dtypes.DType = tf.int32,
-    validate: bool = True) -> gt.GraphTensor:
-  """Generate a graph tensor from a schema, with random features.
-
-  THIS FUNCTION IS DEPRECATED. TODO(b/266790186): Remove it.
-
-  If example values are provided, the corresponding graph tensor features
-  contain a sample of those values instead of fully random bogus values.
-
-  Args:
-    schema: The GraphSchema instance that describes the graph tensor.
-    row_lengths_range: Minimum and maximum values for each row lengths in a
-      ragged range.
-    row_splits_dtype: Data type for row splits.
-    validate: If true, then use assertions to check that the arguments form a
-      valid RaggedTensor. Note: these assertions incur a runtime cost, since
-      they must be checked for each tensor value.
-
-  Returns:
-    An instance of a GraphTensor.
-
-  """
-  spec = schema_utils.create_graph_spec_from_schema_pb(
-      schema, indices_dtype=row_splits_dtype)
-  return random_graph_tensor(spec=spec,
-                             sample_dict=_get_sample_values_dict(schema),
-                             row_lengths_range=row_lengths_range,
-                             row_splits_dtype=row_splits_dtype,
-                             validate=validate)
-
-
 def _assert_rank0_int(t: tf.Tensor, tensor_name: Text) -> None:
   if t.shape.rank != 0 or t.dtype not in (tf.int32, tf.int64):
     raise ValueError(f"Expected `{tensor_name}` as rank-1 integer tensor,"
                      f" got rank={t.shape.rank}, dtype={t.dtype.name}")
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_random_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_random_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,15 +127,10 @@
         while True:
           yield gr.random_graph_tensor(spec)
       return tf.data.Dataset.from_generator(generator, output_signature=spec)
 
     for graph in random_graph_tensor_generator(self.spec).take(4):
       self.assertIsInstance(graph, gt.GraphTensor)
 
-  def test_random_graph_tensor_from_schema(self):
-    # This form of generation does not require a spec, and works fine.
-    graph = gr.random_graph_tensor_from_schema(self.schema)
-    self.assertIsInstance(graph, gt.GraphTensor)
-
 
 if __name__ == '__main__':
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -373,14 +373,57 @@
                           )),
               },
           ),
       ),
   )
   def testHomogeneous(self, actual, expected):
     """Tests for homogeneous()."""
+    self.assertGraphTensorsEqual(actual, expected)
+
+  def testInGraphMode(self):
+
+    @tf.function
+    def create(source, target, node_features, edge_features, context_features):
+      return gt.homogeneous(
+          source=source,
+          target=target,
+          node_features=node_features,
+          edge_features=edge_features,
+          context_features=context_features,
+      )
+    actual = create(
+        source=tf.constant([0, 3, 4, 5]),
+        target=tf.constant([1, 2, 6, 4]),
+        node_features={'onehots': tf.eye(7)},
+        edge_features={'floats': tf.ones([4, 3])},
+        context_features={'labels': tf.zeros(5)},
+    )
+    expected = gt.GraphTensor.from_pieces(
+        context=gt.Context.from_fields(
+            features={'labels': tf.zeros(5)}, sizes=tf.constant([1])
+        ),
+        node_sets={
+            const.NODES: gt.NodeSet.from_fields(
+                features={'onehots': tf.eye(7)}, sizes=tf.constant([7])
+            )
+        },
+        edge_sets={
+            const.EDGES: gt.EdgeSet.from_fields(
+                features={'floats': tf.ones([4, 3])},
+                sizes=tf.constant([4]),
+                adjacency=adj.Adjacency.from_indices(
+                    source=(const.NODES, tf.constant([0, 3, 4, 5])),
+                    target=(const.NODES, tf.constant([1, 2, 6, 4])),
+                ),
+            ),
+        },
+    )
+    self.assertGraphTensorsEqual(actual, expected)
+
+  def assertGraphTensorsEqual(self, actual, expected):
     self.assertFieldsEqual(
         actual.node_sets['nodes'].features,
         expected.node_sets['nodes'].features,
     )
     self.assertAllEqual(actual.node_sets['nodes'].sizes,
                         expected.node_sets['nodes'].sizes)
     self.assertFieldsEqual(
@@ -625,14 +668,55 @@
         'GraphTensor has no feature edge_sets\\[\'ba\'\\]\\[\'xyz\'\\]'):
       _ = graph.remove_features(edge_sets={
           'ab': ['fab', 'f2'],
           'ba': ['fba', 'xyz', 'f2']
       })
 
 
+class ResolveValueTest(tu.GraphTensorTestBase):
+  """Tests for resolve_value()."""
+
+  @parameterized.named_parameters(
+      ('Context', gt.Context.from_fields(
+          sizes=as_tensor([1, 1]),
+          features={
+              'feat': as_tensor([[1, 2], [3, 4]]),
+              'other': as_tensor([[9], [9]]),
+          })),
+      ('NodeSet', gt.NodeSet.from_fields(
+          sizes=as_tensor([1, 1]),
+          features={
+              'feat': as_tensor([[1, 2], [3, 4]]),
+              'other': as_tensor([[9], [9]]),
+          })),
+      ('EdgeSet', gt.EdgeSet.from_fields(
+          sizes=as_tensor([1, 1]),
+          features={
+              'feat': as_tensor([[1, 2], [3, 4]]),
+              'other': as_tensor([[9], [9]]),
+          },
+          adjacency=adj.HyperAdjacency.from_indices({
+              const.SOURCE: ('a', as_tensor([0, 1])),
+              const.TARGET: ('b', as_tensor([1, 0]))
+          }))))
+  def test(self, graph_piece):
+    self.assertAllEqual(
+        [[1, 2], [3, 4]],
+        gt.resolve_value(graph_piece, feature_name='feat'))
+    feature_value = as_tensor([[5, 6], [7, 8]])
+    self.assertAllEqual(
+        [[5, 6], [7, 8]],
+        gt.resolve_value(graph_piece, feature_value=feature_value))
+    with self.assertRaisesRegex(ValueError, r'One of'):
+      gt.resolve_value(graph_piece)
+    with self.assertRaisesRegex(ValueError, r'One of'):
+      gt.resolve_value(graph_piece,
+                       feature_name='feat', feature_value=feature_value)
+
+
 class ElementsCountsTest(tf.test.TestCase, parameterized.TestCase):
 
   def testEmpty(self):
     graph = gt.GraphTensor.from_pieces()
     self.assertEqual(graph.total_num_components, 0)
     self.assertEqual(graph.spec.total_num_components, 0)
 
@@ -1107,14 +1191,79 @@
     self.assertAllEqual(edge.sizes, tf.constant([], shape=(0, 1)))
     self.assertAllEqual(edge['f'], as_ragged([],
                                              dtype=tf.float32,
                                              ragged_rank=1))
     self.assertAllEqual(edge.adjacency[const.SOURCE],
                         as_ragged([], dtype=tf.int64, ragged_rank=1))
 
+  def testTFLite(self):
+    test_graph_dict = {
+        'node_features': tf.constant([[1.], [2.], [3.]], tf.float32),
+        'node_row_lengths': tf.constant([2, 1], tf.int32),
+        'edge_row_lengths': tf.constant([2, 1], tf.int32),
+        'edge_source': tf.constant([0, 1, 0], tf.int32),
+        'edge_target': tf.constant([1, 0, 0], tf.int32),
+    }
+    inputs = {
+        'node_features': tf.keras.Input([1], None, 'node_features', tf.float32),
+        'node_row_lengths': tf.keras.Input(
+            [], None, 'node_row_lengths', tf.int32),
+        'edge_source': tf.keras.Input([], None, 'edge_source', tf.int32),
+        'edge_target': tf.keras.Input([], None, 'edge_target', tf.int32),
+        'edge_row_lengths': tf.keras.Input(
+            [], None, 'edge_row_lengths', tf.int32),
+    }
+    outputs = _MakeGraphTensorMerged()(inputs)
+    model = tf.keras.Model(inputs=inputs, outputs=outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = [0, 1, 2]
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith('2.10.'):
+      self.skipTest('GNN models are unsupported in TFLite until TF 2.11 but '
+                    f'got TF {tf.__version__}')
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner('serving_default')
+    obtained = signature_runner(
+        **test_graph_dict)['private__make_graph_tensor_merged']
+    self.assertAllClose(expected, obtained)
+
+
+# TODO(b/274779989): Replace this layer with a more standard representation
+# of GraphTensor as a dict of plain Tensors.
+class _MakeGraphTensorMerged(tf.keras.layers.Layer):
+  """Makes a homogeneous GraphTensor of rank 0 with two components."""
+
+  def call(self, inputs):
+    node_features = tf.RaggedTensor.from_row_lengths(
+        inputs['node_features'], inputs['node_row_lengths'])
+    edge_source = tf.RaggedTensor.from_row_lengths(
+        inputs['edge_source'], inputs['edge_row_lengths'])
+    edge_target = tf.RaggedTensor.from_row_lengths(
+        inputs['edge_target'], inputs['edge_row_lengths'])
+    graph = gt.GraphTensor.from_pieces(
+        node_sets={
+            'nodes':
+                gt.NodeSet.from_fields(
+                    sizes=tf.expand_dims(inputs['node_row_lengths'], -1),
+                    features={const.HIDDEN_STATE: node_features})
+        },
+        edge_sets={
+            'edges':
+                gt.EdgeSet.from_fields(
+                    sizes=tf.expand_dims(inputs['edge_row_lengths'], -1),
+                    adjacency=adj.Adjacency.from_indices(
+                        ('nodes', edge_source),
+                        ('nodes', edge_target)),)
+        }).merge_batch_to_components()
+    return graph.edge_sets['edges'].adjacency.source
+
 
 class NumComponentsTest(tu.GraphTensorTestBase):
   """Tests for GraphTensor tranformations."""
 
   @parameterized.parameters([
       dict(features={}, shape=[], expected=0),
       dict(features={'a': as_tensor([2])}, shape=[], expected=1),
@@ -1204,14 +1353,53 @@
     self.assertAllEqual(context.num_components, 0)
     graph = gt.GraphTensor.from_pieces(context, node_sets={'node': node_set})
     self.assertAllEqual(graph.context.num_components, expected)
     self.assertAllEqual(graph.context.total_num_components,
                         tf.reduce_sum(expected))
 
 
+@tf.function(input_signature=[tf.TensorSpec(shape=[None], dtype=tf.int32)])
+def node_set_sizes_to_test_results(inputs):
+  context = gt.Context.from_fields(sizes=tf.ones_like(inputs))
+  nodes = gt.NodeSet.from_fields(sizes=inputs)
+  graph = gt.GraphTensor.from_pieces(context=context,
+                                     node_sets={'nodes': nodes})
+  return tf.stack([
+      graph.total_num_components,
+      graph.num_components,
+      graph.node_sets['nodes'].total_size,
+  ], axis=0)
+
+
+class NodeSetSizesToTestResults(tf.keras.layers.Layer):
+
+  def call(self, sizes):
+    return node_set_sizes_to_test_results(sizes)
+
+
+class SizesTFLiteTest(tf.test.TestCase):
+
+  def testTFLite(self):
+    test_tensor = tf.constant([2, 2])
+    inputs = tf.keras.Input([], None, 'node_sizes', tf.int32)
+    outputs = NodeSetSizesToTestResults()(inputs)
+    model = tf.keras.Model(inputs, outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = [2, 2, 4]
+
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner('serving_default')
+    obtained = signature_runner(
+        node_sizes=test_tensor)['node_set_sizes_to_test_results']
+    self.assertAllClose(expected, obtained)
+
+
 class CheckScalarGraphTensorTest(tf.test.TestCase):
 
   def testSuccess(self):
     graph_tensor = gt.GraphTensor.from_pieces(node_sets={
         'nodes': gt.NodeSet.from_fields(sizes=[1], features={'f': [[1.]]})
     })
     gt.check_scalar_graph_tensor(graph_tensor)  # Doesn't raise.
@@ -1221,50 +1409,97 @@
         'nodes': gt.NodeSet.from_fields(sizes=[[1]], features={'f': [[[1.]]]})
     })
     with self.assertRaisesRegex(ValueError,
                                 r'My test code requires.*got `rank=1`'):
       gt.check_scalar_graph_tensor(graph_tensor, 'My test code')
 
 
+class GetAuxTypePrefixTest(tf.test.TestCase, parameterized.TestCase):
+
+  @parameterized.parameters(
+      ('_readout', '_readout'),
+      ('_readout/source/1', '_readout'),
+      ('_readout:train', '_readout'),
+      ('_readout:train/seed', '_readout'),
+      ('#reserved/x', '#reserved'),
+      ('!reserved/x', '!reserved'),
+      ('%reserved/x', '%reserved'),
+      ('.reserved/x', '.reserved'),
+      ('^reserved/x', '^reserved'),
+      ('~reserved/x', '~reserved'),
+  )
+  def testType(self, set_name, expected):
+    actual = gt.get_aux_type_prefix(set_name)
+    self.assertEqual(expected, actual)
+
+  @parameterized.parameters(
+      ('video',),
+      ('User',),
+      ('49ers',),
+      ('-dashed-',),
+  )
+  def testNone(self, set_name):
+    actual = gt.get_aux_type_prefix(set_name)
+    self.assertIsNone(actual)
+
+
 class CheckHomogeneousGraphTensorTest(tf.test.TestCase, parameterized.TestCase):
 
-  def testSuccess(self):
-    graph = _make_test_graph_from_num_pieces(1, 1)
-    gt.check_homogeneous_graph_tensor(graph)  # Doesn't raise.
-    gt.check_homogeneous_graph_tensor(graph.spec)  # Doesn't raise.
+  @parameterized.named_parameters(('', False), ('WithReadout', True))
+  def testSuccess(self, add_readout):
+    graph = _make_test_graph_from_num_pieces(1, 1, add_readout=add_readout)
+    expected = ('atoms_0', 'bonds_0')
+    # These calls don't raise.
+    self.assertEqual(expected,
+                     gt.get_homogeneous_node_and_edge_set_name(graph))
+    self.assertEqual(expected,
+                     gt.get_homogeneous_node_and_edge_set_name(graph.spec))
 
   @parameterized.named_parameters(
-      ('ZeroNodeSets', 0, 0), ('ThreeNodeSets', 3, 1), ('ZeroEdgeSets', 1, 0),
-      ('SevenEdgeSets', 1, 7), ('ManyPieces', 4, 5))
-  def testFailure(self, num_node_sets, num_edge_sets):
-    graph = _make_test_graph_from_num_pieces(num_node_sets, num_edge_sets)
+      ('ZeroNodeSets', 0, 0),
+      ('ThreeNodeSets', 3, 1),
+      ('ZeroEdgeSetsButReadout', 1, 0, True),
+      ('SevenEdgeSets', 1, 7),
+      ('ManyPieces', 4, 5),
+      ('ManyPiecesAndReadout', 4, 5, True))
+  def testFailure(self, num_node_sets, num_edge_sets, add_readout=False):
+    graph = _make_test_graph_from_num_pieces(num_node_sets, num_edge_sets,
+                                             add_readout)
     with self.assertRaisesRegex(ValueError,
                                 r'a graph with 1 node set and 1 edge set'):
-      gt.check_homogeneous_graph_tensor(graph)
+      gt.get_homogeneous_node_and_edge_set_name(graph)
     with self.assertRaisesRegex(ValueError,
                                 r'a graph with 1 node set and 1 edge set'):
-      gt.check_homogeneous_graph_tensor(graph.spec)
+      gt.get_homogeneous_node_and_edge_set_name(graph.spec)
 
 
-def _make_test_graph_from_num_pieces(num_node_sets, num_edge_sets):
+def _make_test_graph_from_num_pieces(num_node_sets, num_edge_sets, add_readout):
   # pylint: disable=g-complex-comprehension
-  return gt.GraphTensor.from_pieces(
-      node_sets={
-          f'atoms_{i}': gt.NodeSet.from_fields(
-              sizes=[2, 1], features={'f': [[1.], [2.], [3.]]})
-          for i in range(num_node_sets)
-      },
-      edge_sets={
-          f'bonds_{j}': gt.EdgeSet.from_fields(
-              sizes=as_tensor([2, 0]),
-              adjacency=adj.Adjacency.from_indices(
-                  source=('atoms_1', as_ragged([[0, 1], []])),
-                  target=('atoms_1', as_ragged([[1, 2], []]))))
-          for j in range(num_edge_sets)
-      })
+  node_sets = {
+      f'atoms_{i}': gt.NodeSet.from_fields(
+          sizes=[2, 1], features={'f': [[1.], [2.], [3.]]})
+      for i in range(num_node_sets)
+  }
+  edge_sets = {
+      f'bonds_{j}': gt.EdgeSet.from_fields(
+          sizes=[2, 0],
+          adjacency=adj.Adjacency.from_indices(
+              source=('atoms_0', [0, 2]),
+              target=('atoms_0', [1, 2])))
+      for j in range(num_edge_sets)
+  }
+  if add_readout:
+    node_sets['_readout'] = gt.NodeSet.from_fields(sizes=[1, 1])
+    edge_sets['_readout/seed'] = gt.EdgeSet.from_fields(
+        sizes=[1, 1],
+        adjacency=adj.Adjacency.from_indices(
+            source=('atoms_0', [1, 2]),
+            target=('atoms_0', [0, 2])))
+
+  return gt.GraphTensor.from_pieces(node_sets=node_sets, edge_sets=edge_sets)
 
 
 class SpecRelaxationTest(tu.GraphTensorTestBase):
 
   def _get_context_spec(self, num_components: Optional[int]) -> gt.ContextSpec:
     return gt.ContextSpec.from_field_specs(
         features_spec={
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/graph_tensor_test_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/graph_tensor_test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/normalization_ops_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/normalization_ops_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from absl.testing import parameterized
 import tensorflow as tf
 from tensorflow_gnn.graph import adjacency as adj
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
-from tensorflow_gnn.graph import graph_tensor_ops as ops
 from tensorflow_gnn.graph import normalization_ops
 
 
 ct = tf.constant
 rt = tf.ragged.constant
 
 
@@ -131,20 +131,54 @@
        tf.concat(
            [tf.repeat(ct([0.0116, 0.6364, 0.0861, 0.0316, 0.234]), 5),
             ct([])],
            axis=0)),
   )
   def testSoftmax(self, gt_input, want):
     """Unit tests for the softmax function."""
-    broadcasted = ops.broadcast_node_to_edges(
+    broadcasted = broadcast_ops.broadcast_node_to_edges(
         gt_input, 'edges', const.SOURCE, feature_name=const.HIDDEN_STATE)
     got = normalization_ops.softmax_edges_per_node(
         gt_input, 'edges', const.TARGET, feature_value=broadcasted)
     self.assertAllClose(got, want, atol=.001)
 
+  def testSoftmaxMultipleEdgeSets(self):
+    """Tests softmax() across multiple edge sets."""
+    graph_tensor = gt.GraphTensor.from_pieces(
+        node_sets={
+            'air': gt.NodeSet.from_fields(sizes=[3],),
+            'ground': gt.NodeSet.from_fields(sizes=[2],)
+        },
+        edge_sets={
+            'aa': gt.EdgeSet.from_fields(
+                sizes=[4],
+                adjacency=adj.Adjacency.from_indices(
+                    ('air', [0, 1, 2, 1]),
+                    ('air', [1, 2, 1, 0]))),
+            'ga': gt.EdgeSet.from_fields(
+                sizes=[3],
+                adjacency=adj.Adjacency.from_indices(
+                    ('ground', [0, 1, 0]),
+                    ('air', [2, 0, 2]))),
+        })
+    edge_set_names = ['aa', 'ga']
+    # Feature values log(x_i) are chosen such that sum(x_i) == 100
+    # at each target node.
+    feature_values = [tf.math.log(tf.constant([60., 50., 40., 20.])),
+                      tf.math.log(tf.constant([25., 80., 25.]))]
+    expected_aa = tf.constant([0.6, 0.5, 0.4, 0.2])
+    expected_ga = tf.constant([0.25, 0.8, 0.25])
+    actual = normalization_ops.softmax(
+        graph_tensor, const.TARGET,
+        edge_set_name=edge_set_names, feature_value=feature_values)
+    self.assertLen(actual, len(edge_set_names))
+    actual_aa, actual_ga = actual
+    self.assertAllClose(actual_aa, expected_aa)
+    self.assertAllClose(actual_ga, expected_ga)
+
   @parameterized.product(
       # The descriptive names are meant to make test output easier to read.
       relation=['EdgeToNode', 'EdgeToContext', 'NodeToContext'],
       value=['Balanced', 'Huge', 'Tiny'])
   def testSoftmaxGradient(self, relation, value):
     """Tests softmax() and its derivative, also for large offsets."""
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
   Context, node or edge features of the appended fake components are filled with
   user-provided scalar values or with zeros if the latter are not specified.
   Fake edges are created such that each fake node has an approximately uniform
   number of incident edges (this behavior is not guaranteed and may change in
   the future).
 
+  NOTE(b/275338236): This operation is not available in TFLite (last checked
+  for TF 2.12).
+
   Args:
     graph_tensor: scalar graph tensor (rank=0) to pad.
     size_constraints: target total sizes for each graph piece. Must define the
       target number of graph components (`.total_num_components`), target total
       number of items for each node set (`.total_num_nodes[node_set_name]`) and
       likewise for each edge set (`.total_num_edges[edge_set_name]`).
       If `min_nodes_per_component` is set, the inserted graph components satisfy
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/padding_ops_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/padding_ops_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/preprocessing_common_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/preprocessing_common_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_utils_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Graph schema validation routines.
+"""Graph schema validation routines."""
 
-This module provides a simple container for the ragged tensors associated with
-multiple sets of nodes, edges, and graph-global data. See go/graph-tensor for
-details.
-"""
-
-from typing import List
+import re
+from typing import List, Optional, Sequence
 
 from absl import logging  # TODO(blais): Remove, see below.
 import tensorflow as tf
 from tensorflow_gnn.graph import adjacency as adj
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
+from tensorflow_gnn.graph import readout
 from tensorflow_gnn.graph import schema_utils as su
 import tensorflow_gnn.proto.graph_schema_pb2 as schema_pb2
 
 
 # The supported data types. Note that these are currently limited to the ones
 # supported by `tensorflow.Example` but we can eventually extend the list by
 # adding casting transformations, and supporting other data formats for
@@ -41,36 +38,46 @@
   """A schema validation error.
 
   This exception is raised if in the course of validating the schema for
   correctness some errors are found.
   """
 
 
-def validate_schema(schema: schema_pb2.GraphSchema) -> List[Exception]:
+def validate_schema(
+    schema: schema_pb2.GraphSchema,
+    readout_node_sets: Optional[Sequence[const.NodeSetName]] = None,
+) -> List[Exception]:
   """Validates the correctness of a graph schema instance.
 
   `GraphSchema` configuration messages are created by users in order to describe
   the topology of a graph. This function checks various aspects of the schema
   for correctness, e.g. prevents usage of reserved feature names, ensures given
   shapes are fully-defined, ensures set name references are found, etc.
 
   Args:
     schema: An instance of the graph schema.
+    readout_node_sets: By default, this function checks the "_readout" node set,
+      if present, if it meets the requirements of `tfgnn.structured_readout()`.
+      That's sufficient for most cases. Optionally, you can pass a list of
+      `readout_node_set` names to (a) require their presence and (b) check them.
+
   Returns:
     A list of exceptions describing optional warnings.
     Render those to your favorite stream (or ignore).
+
   Raises:
     ValidationError: If a validation check fails.
   """
   _validate_schema_feature_dtypes(schema)
   _validate_schema_shapes(schema)
   _validate_schema_descriptions(schema)
   _validate_schema_reserved_feature_names(schema)
   _validate_schema_context_references(schema)
   _validate_schema_node_set_references(schema)
+  _validate_schema_readout(schema, readout_node_sets)
   return _warn_schema_scalar_shapes(schema)
 
 
 def check_required_features(requirements: schema_pb2.GraphSchema,
                             actual: schema_pb2.GraphSchema):
   """Checks the requirements of a given schema against another.
 
@@ -225,15 +232,15 @@
         raise ValidationError(
             "Feature '{}' from {} set '{}' is reserved".format(
                 name, set_type, set_name))
 
   # TODO(blais): Make this compulsory after we remove the hardcoded
   # feature names from the sampler.
   for set_type, set_name, feature_name, feature in su.iter_features(schema):
-    if const.RESERVED_REGEX.match(feature_name):
+    if re.fullmatch(const.RESERVED_FEATURE_NAME_PATTERN, feature_name):
       logging.error("Invalid %s feature name '%s' on set '%s': reserved names "
                     "are not allowed", set_type, feature_name, set_name)
 
 
 def _validate_schema_context_references(schema: schema_pb2.GraphSchema):
   """Verify the cross-references to context features from node and edge sets."""
   for set_name, node_set in schema.node_sets.items():
@@ -264,14 +271,35 @@
     for feature_name in edge_set.source, edge_set.target:
       if feature_name not in schema.node_sets:
         raise ValidationError(
             "Edge set '{}' referencing unknown node set '{}'".format(
                 set_name, feature_name))
 
 
+def _validate_schema_readout(
+    schema: schema_pb2.GraphSchema,
+    readout_node_sets: Optional[Sequence[const.NodeSetName]] = None,
+) -> None:
+  """Applies validate_graph_tensor_spec_for_readout()."""
+  if readout_node_sets is None:
+    if "_readout" not in schema.node_sets:
+      return
+    readout_node_sets = ["_readout"]
+
+  spec = su.create_graph_spec_from_schema_pb(schema)
+  for readout_node_set in readout_node_sets:
+    try:
+      readout.validate_graph_tensor_spec_for_readout(
+          spec, readout_node_set=readout_node_set)
+    except (ValueError, KeyError) as e:
+      raise ValidationError(
+          "tfgnn.validate_graph_tensor_spec_for_readout(..., "
+          f"readout_node_set='{readout_node_set}') failed: {e}") from e
+
+
 # TODO(blais): This code could eventually be folded into the various
 # constructors of `GraphTensor` pieces.
 def assert_constraints(graph: gt.GraphTensor) -> tf.Operation:
   """Validate the shape constaints of a graph's features at runtime.
 
   This code returns a TensorFlow op with debugging assertions that ensure the
   parsed data has valid shape constraints for a graph. This can be instantiated
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/schema_validation_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/schema_validation_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,14 +247,54 @@
             source: "queries"
         }
       }
     """, schema_pb2.GraphSchema())
     with self.assertRaises(sv.ValidationError):
       sv._validate_schema_node_set_references(empty_target_schema)
 
+  def test_validate_schema_readout(self):
+    schema = text_format.Parse("""
+      node_sets {
+        key: "queries"
+      }
+      node_sets {
+        key: "documents"
+      }
+      node_sets {
+        key: "_readout"
+      }
+      edge_sets {
+        key: "_readout/foo"
+        value {
+          source: "queries"
+          target: "_readout"
+        }
+      }
+    """, schema_pb2.GraphSchema())
+    sv._validate_schema_readout(schema, readout_node_sets=['_readout'])
+    sv._validate_schema_readout(schema)
+
+    schema_without = copy.copy(schema)
+    del schema_without.edge_sets['_readout/foo']
+    del schema_without.node_sets['_readout']
+    sv._validate_schema_readout(schema_without)
+
+    with self.assertRaisesRegex(
+        sv.ValidationError,
+        r'lacks auxiliary node set.*_readout:train'):
+      sv._validate_schema_readout(
+          schema, readout_node_sets=['_readout', '_readout:train'])
+
+    bad_schema = copy.copy(schema)
+    bad_schema.edge_sets['_readout/foo'].target = 'documents'
+    with self.assertRaisesRegex(
+        sv.ValidationError,
+        r'validate_graph_tensor_spec_for_readout'):
+      sv._validate_schema_readout(bad_schema)
+
 
 class SchemaTests(tf.test.TestCase):
 
   def test_check_required_features__missing_feature(self):
     required = text_format.Parse("""
       node_sets {
         key: "queries"
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tag_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-# Copyright 2021 The TensorFlow GNN Authors. All Rights Reserved.
+# Copyright 2023 The TensorFlow GNN Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Utilities related to the IncidentNodeTag values."""
+"""Contrastive losses.
 
-from tensorflow_gnn.graph import graph_constants as const
+Users of TF-GNN can use these layers by importing them next to the core library:
 
+```python
+import tensorflow_gnn as tfgnn
+from tensorflow_gnn.models import contrastive_losses
+```
+"""
+from tensorflow_gnn.models.contrastive_losses import layers
+from tensorflow_gnn.models.contrastive_losses import tasks
 
-def reverse_tag(tag):
-  """Flips tfgnn.SOURCE to tfgnn.TARGET and vice versa."""
-  if tag == const.TARGET:
-    return const.SOURCE
-  elif tag == const.SOURCE:
-    return const.TARGET
-  else:
-    raise ValueError(
-        f"Expected tag tfgnn.SOURCE ({const.SOURCE}) "
-        f"or tfgnn.TARGET ({const.TARGET}), got: {tag}")
+CorruptionSpec = layers.CorruptionSpec
+DeepGraphInfomaxLogits = layers.DeepGraphInfomaxLogits
+DropoutFeatures = layers.DropoutFeatures
+ShuffleFeaturesGlobally = layers.ShuffleFeaturesGlobally
+
+BarlowTwinsTask = tasks.BarlowTwinsTask
+DeepGraphInfomaxTask = tasks.DeepGraphInfomaxTask
+VicRegTask = tasks.VicRegTask
+
+del layers
+del tasks
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utils for tensors and ragged tensors."""
 from typing import List, Optional, Text, Union, Mapping
 
-from keras.engine import keras_tensor as kt
 import tensorflow as tf
 
+from tensorflow_gnn.graph import tf_internal
+
 Value = Union[tf.Tensor, tf.RaggedTensor]
 ValueSpec = Union[tf.TensorSpec, tf.RaggedTensorSpec]
 
 
 def dims_list(tensor: tf.Tensor) -> List[Union[int, tf.Tensor]]:
   """Lists tensor dimensions with a preference for statically known sizes."""
   static = tensor.shape.as_list()
@@ -38,15 +39,14 @@
 
   if is_dense_tensor(value):
     return dims_list(value)[0]
 
   raise ValueError(f'Unsupported type {type(value).__name__}')
 
 
-# LINT.IfChange
 def row_lengths_to_row_ids(
     row_lengths: tf.Tensor,
     sum_row_lengths_hint: Optional[int] = None) -> tf.Tensor:
   """Converts rank-1 ragged row lengths to row ids.
 
   For XLA compatibility `sum_row_lengths_hint` has to be provided to guarantee
   statically (compile-time) known result size.
@@ -72,15 +72,14 @@
   sum_row_lengths = tf.reduce_sum(
       row_lengths) if sum_row_lengths_hint is None else sum_row_lengths_hint
 
   cuts = tf.math.unsorted_segment_sum(
       tf.ones_like(row_starts), row_starts, sum_row_lengths + 1)
   result = tf.math.cumsum(cuts, exclusive=False)
   return result[:sum_row_lengths]
-# LINT.ThenChange(../models/gpt_gnn/tensor_utils.py)
 
 
 def segment_random_index_shuffle(
     *, segment_ids: tf.Tensor, seed: Optional[int] = None) -> tf.Tensor:
   """Returns a global permutation that shuffles randomly within each segment.
 
   XLA compatible.
@@ -290,14 +289,17 @@
 
   This function allows to restore static dimension sizes without relying on the
   tensorflow shape inference. If `value` is a dense tensor, the result tensor
   has `result.shape[0] == nrows`. If `value` is a ragged tensor, the
   `result.nrows() == nrows`. Function checks at runtime that `value` allows
   that update.
 
+  NOTE(b/275338236): This operation is not available in TFLite (last checked
+  for TF 2.12).
+
   Args:
     value: dense tensor (`rank > 0`) or ragged tensor that allows static
       `nrows`.
     nrows: static number of rows.
 
   Returns:
     Tensor that is equal to the input tensor but with static number of rows.
@@ -449,20 +451,18 @@
     validation_ops = []
 
   with tf.control_dependencies(validation_ops):
     diff = fill(spec, nrows=diff_size, value=padding_value)
     return tf.concat([value, diff], axis=0)
 
 
-# LINT.IfChange
 def _assert_rank1_int(t: tf.Tensor, tensor_name: Text) -> None:
   if t.shape.rank != 1 or t.dtype not in (tf.int32, tf.int64):
     raise ValueError(f'Expected `{tensor_name}` as rank-1 integer tensor,'
                      f' got rank={t.shape.rank}, dtype={t.dtype.name}')
-# LINT.ThenChange(../models/gpt_gnn/tensor_utils.py)
 
 
 def with_undefined_outer_dimension(spec: ValueSpec) -> ValueSpec:
   """Sets outer most shape dimension to None (undefined)."""
   if spec.shape.rank == 0:
     raise ValueError('The `spec` must have rank>0, got scalar (rank=0)')
 
@@ -481,22 +481,23 @@
         row_splits_dtype=spec.row_splits_dtype)
 
   raise ValueError(f'Unsupported type {type(spec).__name__}')
 
 
 def is_ragged_tensor(value: Value) -> bool:
   """Returns whether a tensor (TF or Keras) is a RaggedTensor."""
-  return isinstance(value, (tf.RaggedTensor, kt.RaggedKerasTensor))
+  return isinstance(value, (tf.RaggedTensor, tf_internal.RaggedKerasTensor))
 
 
 def is_dense_tensor(value: Value) -> bool:
+  """Returns whether a tensor (TF or Keras) is a Tensor."""
   if isinstance(value, tf.Tensor):
     return True
 
-  if isinstance(value, kt.KerasTensor):
+  if isinstance(value, tf_internal.KerasTensor):
     # KerasTensor is the base class for all Keras tensors, including the
     # RaggedKerasTensor. Below we rely on the type spec to resolve actual type.
     return isinstance(value.type_spec, tf.TensorSpec)
 
   return False
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/graph/tensor_utils_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/graph/tensor_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/BUILD`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
 
 licenses(["notice"])
 
-package(default_visibility = [
-    ":__subpackages__",
-    "//tensorflow_gnn:__pkg__",
-    "//tensorflow_gnn/graph:__subpackages__",
-])
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = [
+        ":__subpackages__",
+        "//tensorflow_gnn:__pkg__",
+        "//tensorflow_gnn/graph:__subpackages__",
+    ],
+)
 
 pytype_strict_library(
     name = "keras",
     srcs = ["__init__.py"],
     deps = [
         ":builders",
+        ":initializers",
         ":keras_tensors",
         "//tensorflow_gnn/keras/layers",
     ],
 )
 
 tf_py_test(
     name = "keras_e2e_test",
@@ -34,28 +38,31 @@
     srcs = ["keras_tensors.py"],
     srcs_version = "PY3",
     deps = [
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/graph:adjacency",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
+        "//tensorflow_gnn/graph:tf_internal",
     ],
 )
 
 tf_py_test(
     name = "keras_tensors_test",
     srcs = ["keras_tensors_test.py"],
     python_version = "PY3",
     deps = [
         ":keras_tensors",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/graph:adjacency",
+        "//tensorflow_gnn/graph:broadcast_ops",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
-        "//tensorflow_gnn/graph:graph_tensor_ops",
+        "//tensorflow_gnn/graph:pool_ops",
     ],
 )
 
 pytype_strict_library(
     name = "builders",
     srcs = ["builders.py"],
     srcs_version = "PY3",
@@ -77,10 +84,31 @@
         ":builders",
         "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn/graph:adjacency",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
         "//tensorflow_gnn/keras/layers:convolutions",
+        "//tensorflow_gnn/keras/layers:graph_update",
         "//tensorflow_gnn/keras/layers:next_state",
     ],
 )
+
+pytype_strict_library(
+    name = "initializers",
+    srcs = ["initializers.py"],
+    srcs_version = "PY3",
+    deps = [
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+tf_py_test(
+    name = "initializers_test",
+    srcs = ["initializers_test.py"],
+    python_version = "PY3",
+    deps = [
+        ":initializers",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+    ],
+)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/builders_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -10,213 +10,228 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for graph_update Keras layers."""
 
-import collections
+import enum
 import os
 
 from absl.testing import parameterized
 import tensorflow as tf
-
 from tensorflow_gnn.graph import adjacency as adj
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
-from tensorflow_gnn.keras import builders
 from tensorflow_gnn.keras.layers import convolutions
+from tensorflow_gnn.keras.layers import graph_ops
+from tensorflow_gnn.keras.layers import graph_update
 from tensorflow_gnn.keras.layers import next_state as next_state_lib
 
-IdentityLayer = tf.keras.layers.Layer
 
+class ReloadModel(int, enum.Enum):
+  """Controls how to reload a model for further testing after saving."""
+  SKIP = 0
+  SAVED_MODEL = 1
+  KERAS = 2
 
-class ConvGNNBuilderTest(tf.test.TestCase, parameterized.TestCase):
 
-  def testHomogeneousCase(self):
-    input_graph = _make_test_graph_with_singleton_node_sets(
-        [("node", [1.])], [("node", "node", [100.])])
-    gnn_builder = builders.ConvGNNBuilder(
-        lambda _: convolutions.SimpleConv(IdentityLayer()),
-        lambda _: next_state_lib.NextStateFromConcat(IdentityLayer()))
-    graph = gnn_builder.Convolve()(input_graph)
-    self.assertAllEqual([[1., 1., 1.]],
-                        graph.node_sets["node"][const.HIDDEN_STATE])
-    self.assertAllEqual([[100.]],
-                        graph.edge_sets["node->node"][const.HIDDEN_STATE])
-
-  def testNoDuplicateNodeSets(self):
-    calls_for_node_sets = collections.defaultdict(lambda: 0)
-    def nodes_next_state_factory(node_set_name):
-      calls_for_node_sets[node_set_name] += 1
-      return next_state_lib.NextStateFromConcat(IdentityLayer())
-    input_graph = _make_test_graph_with_singleton_node_sets(
-        [("node", [1.])], [("node", "node", [100.])])
-    gnn_builder = builders.ConvGNNBuilder(
-        lambda _: convolutions.SimpleConv(IdentityLayer()),
-        nodes_next_state_factory)
-    graph = gnn_builder.Convolve(["node", "node", "node"])(input_graph)
-    self.assertDictEqual({"node": 1}, calls_for_node_sets)
-    self.assertAllEqual([[1., 1., 1.]],
-                        graph.node_sets["node"][const.HIDDEN_STATE])
-    self.assertAllEqual([[100.]],
-                        graph.edge_sets["node->node"][const.HIDDEN_STATE])
+class GraphUpdateTest(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.named_parameters(
-      ("Default", dict(), [1.], [2., 2., 2.]),  # Behaves like Target.
-      ("Target", dict(receiver_tag=const.TARGET), [1.], [2., 2., 2.]),
-      ("Source", dict(receiver_tag=const.SOURCE), [2., 2., 2.], [1.]))
-  def testReceiverTag(self, receiver_tag_kwarg, expected_a, expected_b):
-    def make_doubling_layer():
-      return tf.keras.layers.Dense(
-          3, use_bias=False,
-          kernel_initializer=tf.keras.initializers.Identity(gain=2.0))
+      ("InstantInit", False),
+      ("DeferredInit", True))
+  def testEndToEndWithConvolutions(self, use_deferred_init):
     input_graph = _make_test_graph_with_singleton_node_sets(
-        [("a", [1.]), ("b", [1.])], [("a", "b", [100.])])
-    if receiver_tag_kwarg:
-      # pylint: disable=g-long-lambda
-      gnn_builder = builders.ConvGNNBuilder(
-          lambda _, *, receiver_tag: convolutions.SimpleConv(
-              IdentityLayer(), receiver_tag=receiver_tag),
-          lambda _: next_state_lib.NextStateFromConcat(make_doubling_layer()),
-          **receiver_tag_kwarg)
-    else:
-      gnn_builder = builders.ConvGNNBuilder(
-          lambda _: convolutions.SimpleConv(IdentityLayer()),
-          lambda _: next_state_lib.NextStateFromConcat(make_doubling_layer()))
-    graph = gnn_builder.Convolve()(input_graph)
-    self.assertAllEqual([expected_a],
-                        graph.node_sets["a"][const.HIDDEN_STATE])
-    self.assertAllEqual([expected_b],
-                        graph.node_sets["b"][const.HIDDEN_STATE])
-    self.assertAllEqual([[100.]],  # Unchanged.
-                        graph.edge_sets["a->b"][const.HIDDEN_STATE])
-
-  def testModelSaving(self):
-
-    def sum_sources_conv(_):
-      return convolutions.SimpleConv(
+        [("a", [1.]), ("b", [2.]), ("c", [4.])],
+        [("a", "c", [100.]), ("b", "c", [100.]),
+         ("c", "a", [100.]), ("b", "a", [100.])])
+
+    def get_kwargs(graph_tensor_spec):
+      self.assertEqual(graph_tensor_spec, input_graph.spec)
+      conv_sum_sources = convolutions.SimpleConv(
           message_fn=tf.keras.layers.Dense(
-              1,
-              use_bias=False,
-              kernel_initializer=tf.keras.initializers.Ones()),
-          sender_edge_feature=const.HIDDEN_STATE,
+              1, use_bias=False, kernel_initializer="ones"),
           receiver_feature=None,
           reduce_type="sum")
-
-    def add_edges_state(_):
-      return next_state_lib.NextStateFromConcat(
+      conv_sum_endpoints = convolutions.SimpleConv(
+          message_fn=tf.keras.layers.Dense(
+              1, use_bias=False, kernel_initializer="ones"),
+          # receiver_feature=const.HIDDEN_STATE,  # The default.
+          reduce_type="sum")
+      state_add_edges = next_state_lib.NextStateFromConcat(
           tf.keras.layers.Dense(
-              1,
-              use_bias=False,
-              kernel_initializer=tf.keras.initializers.Ones()))
-
-    gnn_builder = builders.ConvGNNBuilder(sum_sources_conv, add_edges_state)
-    gnn_layer = tf.keras.models.Sequential([
-        gnn_builder.Convolve({"a"}),
-        gnn_builder.Convolve({"b"}),
-    ])
-    input_graph = _make_test_graph_with_singleton_node_sets([("a", [1.]),
-                                                             ("b", [2.])],
-                                                            [("a", "b", [100.]),
-                                                             ("b", "a", [10.])])
-
-    inputs = tf.keras.layers.Input(type_spec=input_graph.spec)
-    outputs = gnn_layer(inputs)
-    model = tf.keras.Model(inputs, outputs)
-
-    export_dir = os.path.join(self.get_temp_dir(), "stdlayer-tf")
-    tf.saved_model.save(model, export_dir)
-    restored_model = tf.saved_model.load(export_dir)
-    graph = restored_model(input_graph)
-
-    def node_state(node_set_name):
-      return graph.node_sets[node_set_name][const.HIDDEN_STATE]
-
-    self.assertAllEqual([[2. + 1. + 10.]], node_state("a"))
-    self.assertAllEqual([[13. + 2. + 100.]], node_state("b"))
+              1, use_bias=False, kernel_initializer="ones"))
+      double_state_add_edges = next_state_lib.ResidualNextState(
+          tf.keras.layers.Dense(
+              1, use_bias=False, kernel_initializer="ones"))
+      node_sets = {
+          "c": graph_update.NodeSetUpdate(
+              {"b->c": conv_sum_endpoints,
+               "a->c": conv_sum_sources},
+              state_add_edges),
+          "a": graph_update.NodeSetUpdate(
+              {"c->a": conv_sum_sources,
+               "b->a": conv_sum_sources},
+              double_state_add_edges)}
+      return dict(node_sets=node_sets)
 
-  def testParallelUpdates(self):
-    input_graph = _make_test_graph_with_singleton_node_sets(
-        [("a", [1.]), ("b", [2.]), ("c", [4.])], [("a", "c", [100.]),
-                                                  ("b", "c", [100.]),
-                                                  ("c", "a", [100.]),
-                                                  ("b", "a", [100.])])
-    conv_sum_sources = convolutions.SimpleConv(
-        message_fn=tf.keras.layers.Dense(
-            1, use_bias=False, kernel_initializer=tf.keras.initializers.Ones()),
-        receiver_feature=None,
-        reduce_type="sum")
-    conv_sum_endpoints = convolutions.SimpleConv(
-        message_fn=tf.keras.layers.Dense(
-            1, use_bias=False, kernel_initializer=tf.keras.initializers.Ones()),
-        # receiver_feature=const.HIDDEN_STATE,  # The default.
-        reduce_type="sum")
-    state_add_edges = next_state_lib.NextStateFromConcat(
-        tf.keras.layers.Dense(
-            1, use_bias=False, kernel_initializer=tf.keras.initializers.Ones()))
-    double_state_add_edges = next_state_lib.ResidualNextState(
-        tf.keras.layers.Dense(
-            1, use_bias=False, kernel_initializer=tf.keras.initializers.Ones()))
-
-    def convolutions_factory(edge_set: const.EdgeSetName):
-      return conv_sum_endpoints if edge_set == "b->c" else conv_sum_sources
-
-    def next_state_factory(node_set: const.NodeSetName):
-      return state_add_edges if node_set == "c" else double_state_add_edges
-
-    gnn_builder = builders.ConvGNNBuilder(convolutions_factory,
-                                          next_state_factory)
-    model = tf.keras.models.Sequential([
-        gnn_builder.Convolve({"a", "c"}),
-        gnn_builder.Convolve({"c"}),
-    ])
-    graph = model(input_graph)
+    if use_deferred_init:
+      update = graph_update.GraphUpdate(deferred_init_callback=get_kwargs)
+    else:
+      update = graph_update.GraphUpdate(**get_kwargs(input_graph.spec))
+    graph = update(input_graph)
 
     def node_state(node_set_name):
       return graph.node_sets[node_set_name][const.HIDDEN_STATE]
-
     def edge_state(edge_set_name):
       return graph.edge_sets[edge_set_name][const.HIDDEN_STATE]
 
     # Node sets are updated in parallel.
-    # 1st convolution:
-    #   a has 1, gets 1 by skipconn, 2 from b->a and 4 from c->a, totalling 8.
-    # 2nd convolution:
-    #   a has 8 and stays unchanged.
+    # a has 1, gets 1 by skipconn, 2 from b->a and 4 from c->a, totalling 8.
     self.assertAllEqual([[8.]], node_state("a"))
-    # 1st, 2nd convolutions: b has 2 and stays unchanged.
+    # b has 2 and stays unchanged.
     self.assertAllEqual([[2.]], node_state("b"))
-    # 1st convolution:
-    #   c has 4, gets 2+4 from b->c and 1 from a->c, totalling 11.
-    # 2nd convolution:
-    #   c has 11, gets 2+11 from b->c and 8 from a->c, totalling 32.
-    self.assertAllEqual([[32.]], node_state("c"))
+    # c has 4, gets 2+4 from b->c and 1 from a->c, totalling 11.
+    self.assertAllEqual([[11.]], node_state("c"))
     # Edge sets are unchanged.
     self.assertAllEqual([[100.]], edge_state("a->c"))
     self.assertAllEqual([[100.]], edge_state("b->c"))
     self.assertAllEqual([[100.]], edge_state("c->a"))
     self.assertAllEqual([[100.]], edge_state("b->a"))
 
+  @parameterized.named_parameters(
+      ("InstantInit", False, ReloadModel.SKIP),
+      ("InstantInitRestored", False, ReloadModel.SAVED_MODEL),
+      ("InstantInitRestoredKeras", False, ReloadModel.KERAS),
+      ("DeferredInit", True, ReloadModel.SKIP),
+      ("DeferredInitRestored", True, ReloadModel.SAVED_MODEL),
+      ("DeferredInitRestoredKeras", True, ReloadModel.KERAS))
+  def testEndToEndInModelWithEdgeStates(self, use_deferred_init, reload_model):
+    input_graph = _make_test_graph_with_singleton_node_sets(
+        [("a", [1.]), ("b", [2.]), ("c", [4.])],
+        [("a", "c", [100.]), ("b", "c", [100.]),
+         ("c", "a", [100.]), ("b", "a", [100.])],
+        context=[8.])
+
+    def get_kwargs(graph_tensor_spec):
+      self.assertEqual(graph_tensor_spec, input_graph.spec)
+      edge_sum_sources = graph_update.EdgeSetUpdate(
+          next_state_lib.NextStateFromConcat(
+              tf.keras.layers.Dense(
+                  1, use_bias=False, kernel_initializer="ones")),
+          node_input_tags=[const.SOURCE],
+          edge_input_feature=())
+      edge_sum_sources_context = graph_update.EdgeSetUpdate(
+          next_state_lib.NextStateFromConcat(
+              tf.keras.layers.Dense(
+                  1, use_bias=False, kernel_initializer="ones")),
+          node_input_tags=[const.SOURCE],
+          edge_input_feature=(),
+          context_input_feature=const.HIDDEN_STATE)
+      edge_sum_endpoints = graph_update.EdgeSetUpdate(
+          next_state_lib.NextStateFromConcat(
+              tf.keras.layers.Dense(
+                  1, use_bias=False,
+                  kernel_initializer="ones")),
+          # node_input_tags=[const.SOURCE, const.TARGET] is the default.
+          edge_input_feature=())
+      state_add_edges = next_state_lib.NextStateFromConcat(
+          tf.keras.layers.Dense(
+              1, use_bias=False, kernel_initializer="ones"))
+      double_state_add_edges = next_state_lib.ResidualNextState(
+          tf.keras.layers.Dense(
+              1, use_bias=False, kernel_initializer="ones"))
+      ctx_add_node_sets = next_state_lib.NextStateFromConcat(
+          tf.keras.layers.Dense(
+              1, use_bias=False, kernel_initializer="ones"))
+      edge_sets = {
+          "b->c": edge_sum_endpoints,
+          "a->c": edge_sum_sources,
+          "c->a": edge_sum_sources,
+          "b->a": edge_sum_sources_context}
+      node_sets = {
+          "c": graph_update.NodeSetUpdate(
+              {"b->c": graph_ops.Pool(const.TARGET, "sum"),
+               "a->c": graph_ops.Pool(const.TARGET, "sum")},
+              state_add_edges,
+              context_input_feature=const.HIDDEN_STATE),
+          "a": graph_update.NodeSetUpdate(
+              {"c->a": graph_ops.Pool(const.TARGET, "sum"),
+               "b->a": graph_ops.Pool(const.TARGET, "sum")},
+              double_state_add_edges)}
+      context = graph_update.ContextUpdate(
+          {node_set_name: graph_ops.Pool(const.CONTEXT, "sum")
+           for node_set_name in ["a", "b", "c"]},
+          ctx_add_node_sets, context_input_feature=())
+      return dict(edge_sets=edge_sets, node_sets=node_sets, context=context)
+
+    if use_deferred_init:
+      update = graph_update.GraphUpdate(deferred_init_callback=get_kwargs)
+    else:
+      update = graph_update.GraphUpdate(**get_kwargs(input_graph.spec))
+
+    # Build a Model around the Layer, possibly saved and restored.
+    inputs = tf.keras.layers.Input(type_spec=input_graph.spec)
+    outputs = update(inputs)
+    model = tf.keras.Model(inputs, outputs)
+    _ = model(input_graph)  # Trigger building.
+    if reload_model:
+      export_dir = os.path.join(self.get_temp_dir(), "edge-update-model")
+      model.save(export_dir, include_optimizer=False)
+      if reload_model == ReloadModel.KERAS:
+        model = tf.keras.models.load_model(export_dir)
+        # Check that from_config() worked, no fallback to a function trace, see
+        # https://www.tensorflow.org/guide/keras/save_and_serialize#how_savedmodel_handles_custom_objects
+        self.assertIsInstance(model.get_layer(index=1),
+                              graph_update.GraphUpdate)
+      else:
+        model = tf.saved_model.load(export_dir)
+
+    graph = model(input_graph)
+
+    def edge_state(edge_set_name):
+      return graph.edge_sets[edge_set_name][const.HIDDEN_STATE]
+    def node_state(node_set_name):
+      return graph.node_sets[node_set_name][const.HIDDEN_STATE]
+
+    # Edge sets are updated first.
+    self.assertAllEqual([[1.]], edge_state("a->c"))
+    self.assertAllEqual([[6.]], edge_state("b->c"))
+    self.assertAllEqual([[4.]], edge_state("c->a"))
+    self.assertAllEqual([[10.]], edge_state("b->a"))
+    # Node sets are updated in parallel after edge sets.
+    # a has 1, gets 1 by skipconn, 10 from b->a and 4 from c->a, totalling 16.
+    self.assertAllEqual([[16.]], node_state("a"))
+    # b has 2 and stays unchanged.
+    self.assertAllEqual([[2.]], node_state("b"))
+    # c has 4, gets 2+4 from b->c, 1 from a->c and 8 from context, totalling 19.
+    self.assertAllEqual([[19.]], node_state("c"))
+    # Context is updated last, gets overwritten with sum of nodes.
+    self.assertAllEqual([[16. + 2.+ 19.]],
+                        graph.context[const.HIDDEN_STATE])
+
 
-def _make_test_graph_with_singleton_node_sets(nodes, edges):
+def _make_test_graph_with_singleton_node_sets(nodes, edges, context=None):
   """Returns graph with singleton node sets and edge sets of given values."""
   # pylint: disable=g-complex-comprehension
   return gt.GraphTensor.from_pieces(
+      context=gt.Context.from_fields(
+          features=None if context is None else {
+              const.HIDDEN_STATE: tf.constant([context])}),
       node_sets={
           name: gt.NodeSet.from_fields(
               sizes=tf.constant([1]),
               features={const.HIDDEN_STATE: tf.constant([value])})
-          for name, value in nodes
-      },
+          for name, value in nodes},
       edge_sets={
           f"{src}->{dst}": gt.EdgeSet.from_fields(
               sizes=tf.constant([1]),
-              adjacency=adj.Adjacency.from_indices((src, tf.constant([0])),
-                                                   (dst, tf.constant([0]))),
+              adjacency=adj.Adjacency.from_indices(
+                  (src, tf.constant([0])),
+                  (dst, tf.constant([0]))),
               features={const.HIDDEN_STATE: tf.constant([value])})
-          for src, dst, value in edges
-      })
+          for src, dst, value in edges})
 
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_e2e_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_e2e_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,27 +42,34 @@
     self.assertIsSubclass(tfgnn.keras.layers.MapFeatures, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.MakeEmptyFeature, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.PadToTotalSizes, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.Broadcast, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.Pool, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.Readout, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.ReadoutFirstNode, Layer)
+    self.assertIsSubclass(tfgnn.keras.layers.StructuredReadout, Layer)
+    self.assertIsSubclass(tfgnn.keras.layers.StructuredReadoutIntoFeature,
+                          Layer)
+    self.assertIsSubclass(tfgnn.keras.layers.AddReadoutFromFirstNode, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.AnyToAnyConvolutionBase, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.SimpleConv, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.ItemDropout, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.NextStateFromConcat, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.ResidualNextState, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.EdgeSetUpdate, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.NodeSetUpdate, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.ContextUpdate, Layer)
     self.assertIsSubclass(tfgnn.keras.layers.GraphUpdate, Layer)
 
   def testBuilders(self):
     self.assertIsSubclass(tfgnn.keras.ConvGNNBuilder, object)
 
+  def testInitializers(self):
+    self.assertCallable(tfgnn.keras.clone_initializer)
+
 
 # An example of a custom Keras layer used by tests below.
 class AddWeightedSwappedInEdges(tf.keras.layers.Layer):
   """Adds weighted sum of coordinate-swapped neighbor states to each node."""
 
   def __init__(self, supports_get_config=True, supports_from_config=True,
                **kwargs):
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """KerasTensor specializations for GraphTensor pieces."""
-from keras.engine import keras_tensor as kt
-from keras.layers import core
 from tensorflow_gnn.graph import adjacency as adj
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
+from tensorflow_gnn.graph import tf_internal
 
 
-class GraphPieceKerasTensor(kt.KerasTensor):
+class GraphPieceKerasTensor(tf_internal.KerasTensor):
   """Base class for graph pieces Keras tensors.
 
   Each graph piece (e.g. `tfgnn.Context`, `tfgnn.NodeSet`, etc.) must define
   corresponding Keras tensor and register them with the
   `register_keras_tensor_specialization`.
 
   Keras tensors specialization is done according to the rules:
@@ -114,41 +113,42 @@
         'num_components',
         'total_num_components',
     ) + GRAPH_PIECE_PROPERTIES),
     (HyperAdjacencyKerasTensor, GRAPH_PIECE_PROPERTIES),
     (AdjacencyKerasTensor, GRAPH_PIECE_PROPERTIES + ('source', 'target'))
 ]:
   for gt_property in gt_properties:
-    core._delegate_property(cls, gt_property)
+    tf_internal.delegate_property(cls, gt_property)
 
 GRAPH_PIECE_WITH_FEATURES_METHODS = ('get_features_dict', 'replace_features')
 for cls, gt_methods in [(EdgeSetKerasTensor, GRAPH_PIECE_WITH_FEATURES_METHODS),
                         (NodeSetKerasTensor, GRAPH_PIECE_WITH_FEATURES_METHODS),
                         (ContextKerasTensor, GRAPH_PIECE_WITH_FEATURES_METHODS),
                         (GraphKerasTensor, ('remove_features',
                                             'replace_features',
                                             'merge_batch_to_components')),
                         (HyperAdjacencyKerasTensor, ('get_indices_dict',))]:
   for gt_method in gt_methods:
-    core._delegate_method(cls, gt_method)
+    tf_internal.delegate_method(cls, gt_method)
 
 # TODO(b/191957072): dispatch class methods.
 # for cls, class_methods in [
 #     (adj.Adjacency, ('from_indices',)),
 #     (adj.HyperAdjacency, ('from_indices',)),
 #     (gt.Context, ('from_fields',)),
 #     (gt.NodeSet, ('from_fields',)),
 #     (gt.EdgeSet, ('from_fields',)),
 #     (gt.GraphTensor, ('from_pieces',)),
 # ]:
 #   for class_method in class_methods:
-#     core.TFClassMethodDispatcher(cls, class_method).register(
+#     tf_internal.TFClassMethodDispatcher(cls, class_method).register(
 #         getattr(cls, class_method))
 
-kt.register_keras_tensor_specialization(adj.Adjacency, AdjacencyKerasTensor)
-kt.register_keras_tensor_specialization(adj.HyperAdjacency,
-                                        HyperAdjacencyKerasTensor)
-
-kt.register_keras_tensor_specialization(gt.GraphTensor, GraphKerasTensor)
-kt.register_keras_tensor_specialization(gt.Context, ContextKerasTensor)
-kt.register_keras_tensor_specialization(gt.NodeSet, NodeSetKerasTensor)
-kt.register_keras_tensor_specialization(gt.EdgeSet, EdgeSetKerasTensor)
+tf_internal.register_keras_tensor_specialization(adj.Adjacency,
+                                                 AdjacencyKerasTensor)
+tf_internal.register_keras_tensor_specialization(adj.HyperAdjacency,
+                                                 HyperAdjacencyKerasTensor)
+tf_internal.register_keras_tensor_specialization(gt.GraphTensor,
+                                                 GraphKerasTensor)
+tf_internal.register_keras_tensor_specialization(gt.Context, ContextKerasTensor)
+tf_internal.register_keras_tensor_specialization(gt.NodeSet, NodeSetKerasTensor)
+tf_internal.register_keras_tensor_specialization(gt.EdgeSet, EdgeSetKerasTensor)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/keras_tensors_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/keras_tensors_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 import os
 
 from typing import Mapping
 
 from absl.testing import parameterized
 import tensorflow as tf
 from tensorflow_gnn.graph import adjacency as adj
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
-from tensorflow_gnn.graph import graph_tensor_ops as ops
+from tensorflow_gnn.graph import pool_ops
 from tensorflow_gnn.keras import keras_tensors as kt
 
 as_tensor = tf.convert_to_tensor
 as_ragged = tf.ragged.constant
 
 
 class _TestBase(tf.test.TestCase, parameterized.TestCase):
@@ -143,14 +144,16 @@
         {0: ('node', as_tensor([0, 1]))})
     adjacency_input = tf.keras.Input(type_spec=adjacency.spec)
     self.assertEqual(adjacency.node_set_name(0), 'node')
     self.assertAllEqual(
         tf.keras.Model(adjacency_input, adjacency_input[0])(adjacency), [0, 1])
     self.assertIsInstance(adjacency_input.get_indices_dict(), dict)
 
+  # TODO(b/283404258): Remove {broadcast,pool}_*() support for KeradGraphTensor.
+  # Users are meant to call tfgnn.keras.layers.Broadcast and Pool instead.
   def testGraphTensorOps(self):
     example = gt.GraphTensor.from_pieces(
         gt.Context.from_fields(features={'f': as_tensor([1])}),
         node_sets={
             'node':
                 gt.NodeSet.from_fields(
                     features={'f': as_tensor([1, 2])},
@@ -168,34 +171,34 @@
         })
 
     graph_input = tf.keras.Input(type_spec=example.spec)
     self.assertIsInstance(graph_input, kt.GraphKerasTensor)
     graph_output = graph_input.replace_features(
         context={
             'f':
-                ops.pool_edges_to_context(
+                pool_ops.pool_edges_to_context(
                     graph_input, 'edge', feature_name='f') +
-                ops.pool_nodes_to_context(
+                pool_ops.pool_nodes_to_context(
                     graph_input, 'node', feature_name='f')
         },
         node_sets={
             'node': {
                 'f':
-                    ops.broadcast_context_to_nodes(
+                    broadcast_ops.broadcast_context_to_nodes(
                         graph_input, 'node', feature_name='f') +
-                    ops.pool_edges_to_node(
+                    pool_ops.pool_edges_to_node(
                         graph_input, 'edge', const.TARGET, feature_name='f')
             }
         },
         edge_sets={
             'edge': {
                 'f':
-                    ops.broadcast_context_to_edges(
+                    broadcast_ops.broadcast_context_to_edges(
                         graph_input, 'edge', feature_name='f') +
-                    ops.broadcast_node_to_edges(
+                    broadcast_ops.broadcast_node_to_edges(
                         graph_input, 'edge', const.SOURCE, feature_name='f')
             }
         },
     )
     self.assertIsInstance(graph_output, kt.GraphKerasTensor)
     features_output = {
         'context.f': graph_output.context['f'],
@@ -313,18 +316,18 @@
         kernel_initializer=tf.keras.initializers.Constant([[0., 1.], [1., 0.]]))
 
     inputs = tf.keras.layers.Input(type_spec=get_input_spec())
     graph = inputs
 
     weight = graph.edge_sets['edge']['edge_weight']
     node_state = graph.node_sets['node']['state']
-    source_value = ops.broadcast_node_to_edges(
+    source_value = broadcast_ops.broadcast_node_to_edges(
         graph, 'edge', const.SOURCE, feature_name='state')
     message = tf.multiply(weight, source_value)
-    pooled_message = ops.pool_edges_to_node(
+    pooled_message = pool_ops.pool_edges_to_node(
         graph, 'edge', const.TARGET, feature_value=message)
     node_updates = fnn(pooled_message)
     node_state += node_updates
     outputs = graph.replace_features(node_sets={'node': {'state': node_state}})
     model = tf.keras.Model(inputs, outputs)
     # Save and restore the model.
     export_dir = os.path.join(self.get_temp_dir(), 'graph-model')
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/BUILD`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
 
 licenses(["notice"])
 
-package(default_visibility = [
-    "//tensorflow_gnn:__pkg__",
-    "//tensorflow_gnn/compat:__subpackages__",
-    "//tensorflow_gnn/graph:__subpackages__",
-    "//tensorflow_gnn/keras:__subpackages__",
-])
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = [
+        "//tensorflow_gnn:__pkg__",
+        "//tensorflow_gnn/compat:__subpackages__",
+        "//tensorflow_gnn/graph:__subpackages__",
+        "//tensorflow_gnn/keras:__subpackages__",
+    ],
+)
 
 pytype_strict_library(
     name = "layers",
     srcs = ["__init__.py"],
     deps = [
         ":convolution_base",
         ":convolutions",
@@ -53,17 +56,18 @@
 
 pytype_strict_library(
     name = "convolution_base",
     srcs = ["convolution_base.py"],
     srcs_version = "PY3",
     deps = [
         "//:expect_tensorflow_installed",
+        "//tensorflow_gnn/graph:broadcast_ops",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
-        "//tensorflow_gnn/graph:graph_tensor_ops",
+        "//tensorflow_gnn/graph:pool_ops",
         "//tensorflow_gnn/graph:tag_utils",
     ],
 )
 
 tf_py_test(
     name = "convolution_base_test",
     srcs = ["convolution_base_test.py"],
@@ -80,17 +84,20 @@
 
 pytype_strict_library(
     name = "graph_ops",
     srcs = ["graph_ops.py"],
     srcs_version = "PY3",
     deps = [
         "//:expect_tensorflow_installed",
+        "//tensorflow_gnn/graph:broadcast_ops",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
         "//tensorflow_gnn/graph:graph_tensor_ops",
+        "//tensorflow_gnn/graph:pool_ops",
+        "//tensorflow_gnn/graph:readout",
     ],
 )
 
 tf_py_test(
     name = "graph_ops_test",
     srcs = ["graph_ops_test.py"],
     python_version = "PY3",
@@ -107,18 +114,18 @@
 pytype_strict_library(
     name = "graph_update",
     srcs = ["graph_update.py"],
     srcs_version = "PY3",
     deps = [
         ":next_state",
         "//:expect_tensorflow_installed",
+        "//tensorflow_gnn/graph:broadcast_ops",
         "//tensorflow_gnn/graph:dict_utils",
         "//tensorflow_gnn/graph:graph_constants",
         "//tensorflow_gnn/graph:graph_tensor",
-        "//tensorflow_gnn/graph:graph_tensor_ops",
     ],
 )
 
 tf_py_test(
     name = "graph_update_test",
     srcs = ["graph_update_test.py"],
     python_version = "PY3",
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 PadToTotalSizes = padding_ops.PadToTotalSizes
 
 AddSelfLoops = graph_ops.AddSelfLoops
 Broadcast = graph_ops.Broadcast
 Pool = graph_ops.Pool
 Readout = graph_ops.Readout
 ReadoutFirstNode = graph_ops.ReadoutFirstNode
+AddReadoutFromFirstNode = graph_ops.AddReadoutFromFirstNode
+StructuredReadout = graph_ops.StructuredReadout
+StructuredReadoutIntoFeature = graph_ops.StructuredReadoutIntoFeature
+# DO NOT USE the obsolete aliases `ReadoutNamed*`.
+ReadoutNamed = graph_ops.StructuredReadout
+ReadoutNamedIntoFeature = graph_ops.StructuredReadoutIntoFeature
 
 AnyToAnyConvolutionBase = convolution_base.AnyToAnyConvolutionBase
 SimpleConv = convolutions.SimpleConv
 
 ItemDropout = item_dropout.ItemDropout
 
 NextStateFromConcat = next_state.NextStateFromConcat
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,18 @@
 """The AnyToAnyConvolutionBase class and associated tooling."""
 
 import abc
 from typing import Any, Callable, Mapping, Optional
 
 import tensorflow as tf
 
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
-from tensorflow_gnn.graph import graph_tensor_ops as ops
+from tensorflow_gnn.graph import pool_ops
 from tensorflow_gnn.graph import tag_utils
 
 
 class AnyToAnyConvolutionBase(tf.keras.layers.Layer, abc.ABC):
   """Convenience base class for convolutions to nodes or to context.
 
   This base class simplifies the implementation of graph convolutions as Keras
@@ -286,30 +287,30 @@
         raise ValueError("Must pass edge_set_name, not node_set_name")
       name_kwarg = dict(edge_set_name=edge_set_name)
       edge_set = graph.edge_sets[edge_set_name]
       sender_node_tag = tag_utils.reverse_tag(receiver_tag)
       sender_node_set = graph.node_sets[
           edge_set.adjacency.node_set_name(sender_node_tag)]
       broadcast_from_sender_node = (
-          lambda feature_value: ops.broadcast_node_to_edges(
+          lambda feature_value: broadcast_ops.broadcast_node_to_edges(
               graph, edge_set_name, sender_node_tag,
               feature_value=feature_value))
       receiver_piece = graph.node_sets[
           edge_set.adjacency.node_set_name(receiver_tag)]
 
     # Set up the broadcast/pool ops for the receiver, plus any ops requested
     # by the subclass. The tag and name arguments conveniently encode the
     # distinction between operating over edge/node, node/context or
     # edge/context.
     def bind_receiver_args(fn):
       return lambda feature_value, **kwargs: fn(
           graph, receiver_tag, **name_kwarg,
           feature_value=feature_value, **kwargs)
-    broadcast_from_receiver = bind_receiver_args(ops.broadcast)
-    pool_to_receiver = bind_receiver_args(ops.pool)
+    broadcast_from_receiver = bind_receiver_args(broadcast_ops.broadcast_v2)
+    pool_to_receiver = bind_receiver_args(pool_ops.pool_v2)
     if self._extra_receiver_ops is None:
       extra_receiver_ops_kwarg = {}  # Pass no argument for this.
     else:
       extra_receiver_ops_kwarg = dict(
           extra_receiver_ops={name: bind_receiver_args(fn)
                               for name, fn in self._extra_receiver_ops.items()})
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolution_base_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolution_base_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions.py`

 * *Files 14% similar despite different names*

```diff
@@ -53,15 +53,17 @@
   )(graph)
   ```
 
   Init args:
     message_fn: A Keras layer that computes the individual messages from the
       combined input features (see combine_type).
     reduce_type: Specifies how to pool the messages to receivers. Defaults to
-      "sum", can be any name from tfgnn.get_registered_reduce_operation_names().
+      `"sum"`, can be any reduce_type understood by `tfgnn.pool()`, including
+      concatenations like `"sum|max"` (but mind the increased dimension of the
+      result and the growing number of model weights in the next-state layer).
     combine_type: a string understood by tfgnn.combine_values(), to specify how
       the inputs are combined before passing them to the message_fn. Defaults
       to "concat", which concatenates inputs along the last axis.
     receiver_tag:  one of `tfgnn.SOURCE`, `tfgnn.TARGET` or `tfgnn.CONTEXT`.
       Selects the receiver of the pooled messages.
       If set to `tfgnn.SOURCE` or `tfgnn.TARGET`, the layer can be called for
       an edge set and will pool results at the specified endpoint of the edges.
@@ -90,15 +92,15 @@
   def __init__(
       self,
       message_fn: tf.keras.layers.Layer,
       reduce_type: str = "sum",
       *,
       combine_type: str = "concat",
       receiver_tag: const.IncidentNodeTag = const.TARGET,
-      receiver_feature: const.FieldName = const.HIDDEN_STATE,
+      receiver_feature: Optional[const.FieldName] = const.HIDDEN_STATE,
       sender_node_feature: Optional[
           const.FieldName] = const.HIDDEN_STATE,
       sender_edge_feature: Optional[const.FieldName] = None,
       **kwargs):
     super().__init__(
         receiver_tag=receiver_tag,
         receiver_feature=receiver_feature,
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/convolutions_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/convolutions_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,18 @@
     actual = conv(input_graph, edge_set_name="edges")
     expected = tf.constant([
         [1. + sender_scale*4.],
         [2. + sender_scale*4.],
         [0.]])  # No edges.
     self.assertAllEqual(expected, actual)
 
+  def testTFLite(self):
+    self.skipTest(
+        "SimpleConv TFLite functionality is tested in models/mt_albis")
+
 
 def _make_test_graph_01into2(values):
   """Returns GraphTensor for [v0] --e0--> [v2] <-e1-- [v1] with values."""
   def maybe_features(key):
     features = {const.HIDDEN_STATE: values[key]} if key in values else {}
     return dict(features=features)
   graph = gt.GraphTensor.from_pieces(
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_ops.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_ops.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,31 +10,44 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Keras layer types for fundamental graph ops: Broadcast, Pool and Readout."""
 
-from typing import Any, Mapping, Optional
+from __future__ import annotations
+from typing import Any, Mapping, Optional, Sequence, Union
 
 import tensorflow as tf
 
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
 from tensorflow_gnn.graph import graph_tensor_ops as ops
+from tensorflow_gnn.graph import pool_ops
+from tensorflow_gnn.graph import readout
+
+Field = const.Field
+FieldName = const.FieldName
+NodeSetName = const.NodeSetName
+EdgeSetName = const.EdgeSetName
+IncidentNodeTag = const.IncidentNodeTag
+IncidentNodeOrContextTag = const.IncidentNodeOrContextTag
+GraphTensor = gt.GraphTensor
 
 
 @tf.keras.utils.register_keras_serializable(package="GNN")
 class Readout(tf.keras.layers.Layer):
   """Reads a feature out of a GraphTensor.
 
-  The Readout layer is a convenience wrapper for accessing a feature from
-  one of the edge_sets, node_sets, or the context of a GraphTensor, intended
-  for use in places such as tf.keras.Sequential that require a Keras layer
-  and do not allow for direct subscripting of the GraphTensor.
+  The `Readout` layer is a convenience wrapper for indexing into a
+  `tfgnn.GraphTensor` and retrieving a feature tensor from one of its edge sets,
+  node sets, or the context. It is intended for use in places such as
+  `tf.keras.Sequential` that require a Keras Layer and do not allow
+  subscrpting syntax like `graph_tensor.node_sets["user"]["name"]`.
 
   A location in the graph is selected by setting exactly one of the keyword
   arguments `edge_set_name=...`, `node_set_name=...` or `from_context=True`.
   From there, the keyword argument `feature_name=...` selects the feature.
 
   Both the initialization of and the call to this layer accept arguments to
   select the feature location and the feature name. The call arguments take
@@ -46,14 +59,21 @@
 
   ```python
   readout = tfgnn.keras.layers.Readout(feature_name="value")
   value = readout(graph_tensor, edge_set_name="edges")
   assert value == graph_tensor.edge_sets["edge"]["value"]
   ```
 
+  Besides this direct readout of a full feature tensor, the library also
+  supports readout that gathers feature values only from the nodes (or edges)
+  that matter for a particular task, see `tfgnn.keras.layers.StructuredReadout`.
+  See also `tfgnn.keras.layers.AddReadoutFromFirstNode` for adding the
+  necessary readout structure to handle the legacy cases that were previously
+  handled by `tfgnn.keras.layers.ReadoutFirstNode`.
+
   Init args:
     edge_set_name: If set, the feature will be read from this edge set.
       Mutually exclusive with node_set_name and from_context.
     node_set_name: If set, the feature will be read from this node set.
       Mutually exclusive with edge_set_name and from_context.
     from_context: If true, the feature will be read from the context.
       Mutually exclusive with edge_set_name and node_set_name.
@@ -69,38 +89,38 @@
 
   Returns:
     The tensor with the selected feature.
   """
 
   def __init__(self,
                *,
-               edge_set_name: Optional[gt.EdgeSetName] = None,
-               node_set_name: Optional[gt.NodeSetName] = None,
+               edge_set_name: Optional[EdgeSetName] = None,
+               node_set_name: Optional[NodeSetName] = None,
                from_context: bool = False,
-               feature_name: Optional[gt.FieldName] = None,
+               feature_name: Optional[FieldName] = None,
                **kwargs):
     super().__init__(**kwargs)
     self._location = self._get_location(node_set_name=node_set_name,
                                         edge_set_name=edge_set_name,
                                         from_context=from_context)
     self._feature_name = feature_name
 
   def get_config(self):
     config = super().get_config().copy()
     config.update(self._location)
     config["feature_name"] = self._feature_name
     return config
 
   def call(self,
-           graph: gt.GraphTensor,
+           graph: GraphTensor,
            *,
-           edge_set_name: Optional[gt.EdgeSetName] = None,
-           node_set_name: Optional[gt.NodeSetName] = None,
+           edge_set_name: Optional[EdgeSetName] = None,
+           node_set_name: Optional[NodeSetName] = None,
            from_context: bool = False,
-           feature_name: Optional[gt.FieldName] = None) -> gt.Field:
+           feature_name: Optional[FieldName] = None) -> Field:
     location = self._get_location(node_set_name=node_set_name,
                                   edge_set_name=edge_set_name,
                                   from_context=from_context)
     _check_init_call_kwargs_consistency("Readout",
                                         self._location, location)
     if not location:
       location = self._location
@@ -133,15 +153,15 @@
      that is, one of `edge_set_name=...`, `node_set_name=...` or
     `from_context=True`. If none of these has been set, the result is
     empty, and one of them must be set at call time.
     """
     return self._location
 
   @property
-  def feature_name(self) -> Optional[gt.FieldName]:
+  def feature_name(self) -> Optional[FieldName]:
     """Returns the feature_name argument to init, or None if unset."""
     return self._feature_name
 
   def _get_location(self, *, node_set_name, edge_set_name, from_context):
     """Returns dict of non-None kwargs for selecting the feature location."""
     result = dict()
     if node_set_name is not None: result.update(node_set_name=node_set_name)
@@ -190,37 +210,43 @@
   if self-connections already exist or not.
   """
 
   def __init__(self, edge_set_name):
     super().__init__()
     self._edge_set_name = edge_set_name
 
-  def call(self, graph_tensor: gt.GraphTensor) -> gt.GraphTensor:
+  def call(self, graph_tensor: GraphTensor) -> GraphTensor:
     return ops.add_self_loops(graph_tensor, self._edge_set_name)
 
   def get_config(self):
     config = super().get_config().copy()
     config["edge_set_name"] = self._edge_set_name
     return config
 
 
 @tf.keras.utils.register_keras_serializable(package="GNN")
 class ReadoutFirstNode(tf.keras.layers.Layer):
-  """Reads a feature from the first node of each graph conponent.
+  """Reads a feature from the first node of each graph component.
 
   Given a particular node set (identified by `node_set_name`), this layer
   will gather the given feature from the first node of each graph component.
 
   This is often used for rooted graphs created by sampling around the
   neighborhoods of seed nodes in a large graph: by convention, each seed node is
   the first node of its component in the respective node set, and this layer
   reads out the information it has accumulated there. (In other node sets, the
   first node may be arbitrary -- or nonexistant, in which case this operation
   must not be used and may raise an error at runtime.)
 
+  This implicit convention is inflexible and hard to validate. New models are
+  encouraged to use `tfgnn.keras.layers.StructuredReadout` instead. The
+  necessary readout structure should preferably be present in the sampled
+  dataset itself; if not, it can be added after the fact by
+  `tfgnn.keras.layers.AddReadoutFromFirstNode`.
+
   Init args:
     node_set_name: If set, the feature will be read from this node set.
     feature_name: The name of the feature to read. If unset (also in call),
       tfgnn.HIDDEN_STATE will be read.
 
   Call args:
     graph: The scalar GraphTensor to read from.
@@ -232,32 +258,32 @@
   Returns:
     A tensor of gathered feature values, one for each graph component, like a
     context feature.
   """
 
   def __init__(self,
                *,
-               node_set_name: Optional[gt.NodeSetName] = None,
-               feature_name: Optional[gt.FieldName] = None,
+               node_set_name: Optional[NodeSetName] = None,
+               feature_name: Optional[FieldName] = None,
                **kwargs):
     super().__init__(**kwargs)
     self._node_set_name = node_set_name
     self._feature_name = feature_name
 
   def get_config(self):
     config = super().get_config().copy()
     config["node_set_name"] = self._node_set_name
     config["feature_name"] = self._feature_name
     return config
 
   def call(self,
-           graph: gt.GraphTensor,
+           graph: GraphTensor,
            *,
-           node_set_name: Optional[gt.NodeSetName] = None,
-           feature_name: Optional[gt.FieldName] = None) -> gt.Field:
+           node_set_name: Optional[NodeSetName] = None,
+           feature_name: Optional[FieldName] = None) -> Field:
 
     _check_init_call_arg_consistency("ReadoutFirstNode", "node_set_name",
                                      self._node_set_name, node_set_name)
     if node_set_name is None:
       node_set_name = self._node_set_name
     if node_set_name is None:
       raise ValueError("The ReadoutFirstNode layer requires node_set_name "
@@ -280,54 +306,305 @@
     """
     if self._node_set_name is not None:
       return dict(node_set_name=self._node_set_name)
     else:
       return dict()
 
   @property
-  def feature_name(self) -> Optional[gt.FieldName]:
+  def feature_name(self) -> Optional[FieldName]:
     """Returns the feature_name argument to init, or None if unset."""
     return self._feature_name
 
 
+@tf.keras.utils.register_keras_serializable(package="GNN")
+class StructuredReadout(tf.keras.layers.Layer):
+  """Reads out a feature value from select nodes (or edges) in a graph.
+
+  This Keras layer wraps the `tfgnn.structured_readout()` function. It addresses
+  the need to read out final hidden states from a GNN computation to make
+  predictions for some nodes (or edges) of interest. Its typical usage looks
+  as follows:
+
+  ```python
+  input_graph = tf.keras.Input(type_spec=graph_tensor_spec)
+  graph = SomeGraphUpdate(...)(input_graph)  # Run your GNN here.
+  seed_node_states = tfgnn.keras.layers.StructuredReadout("seed")(graph)
+  logits = tf.keras.layers.Dense(num_classes)(seed_node_states)
+  model = tf.keras.Model(inputs, logits)
+  ```
+
+  ...where `"seed"` is a key defined by the readout structure. There can be
+  multiple of those. For example, a link prediction model could read out
+  `"source"` and `"target"` node states from the graph.
+
+  Please see the documentation of `tfgnn.structured_readout()` for the auxiliary
+  node set and edge sets that make up the readout structure which encodes how
+  values are read out from the graph. Whenever these are available, it is
+  strongly recommended to make use of them with this layer and avoid the older
+  `tfgnn.keras.layers.ReadoutFirstNode`.
+
+  Note that this layer returns a tensor shaped like a feature of the
+  `"_readout"` node set but not actually stored on it. To store it there,
+  see `tfgnn.keras.layers.StructuredReadoutIntoFeature`. To retrieve a
+  feature unchanged, see ``tfgnn.keras.layers.Readout`.
+
+  Init args:
+    key: A string key to select between possibly multiple named readouts
+      (such as `"source"` and `"target"` for link prediction). Can be fixed
+      in init, or selected for each call.
+    feature_name: The name of the feature to read. If unset (also in call),
+      `tfgnn.HIDDEN_STATE` will be read.
+    readout_node_set: A string, defaults to `"_readout"`. This is used as the
+      name for the readout node set and as a name prefix for its edge sets.
+    validate: Setting this to false disables the validity checks for the
+      auxiliary edge sets. This is stronlgy discouraged, unless great care is
+      taken to run `tfgnn.validate_graph_tensor_for_readout()` earlier on
+      structurally unchanged GraphTensors.
+
+  Call args:
+    graph: The scalar GraphTensor to read from.
+    key: Same meaning as for init. Must be passed to init, or to call,
+      or to both (with the same value).
+
+  Returns:
+    A tensor of read-out feature values, shaped like a feature of the
+    `readout_node_set`.
+  """
+
+  def __init__(self,
+               key: Optional[str] = None,
+               *,
+               feature_name: str = const.HIDDEN_STATE,
+               readout_node_set: NodeSetName = "_readout",
+               validate: bool = True,
+               **kwargs):
+    super().__init__(**kwargs)
+    self._key = key
+    self._feature_name = feature_name
+    self._readout_node_set = readout_node_set
+    self._validate = validate
+
+  def get_config(self):
+    return dict(
+        key=self._key,
+        feature_name=self._feature_name,
+        readout_node_set=self._readout_node_set,
+        validate=self._validate,
+        **super().get_config())
+
+  def call(self,
+           graph: GraphTensor,
+           *,
+           key: Optional[str] = None) -> Field:
+    _check_init_call_arg_consistency("StructuredReadout", "key",
+                                     self._key, key)
+    if key is None:
+      key = self._key
+    if key is None:
+      raise ValueError("The StructuredReadout layer requires a readout key "
+                       "to be set at init or call time")
+
+    gt.check_scalar_graph_tensor(graph, "StructuredReadout")
+    return readout.structured_readout(
+        graph,
+        key=key,
+        feature_name=self._feature_name,
+        readout_node_set=self._readout_node_set,
+        validate=self._validate)
+
+
+@tf.keras.utils.register_keras_serializable(package="GNN")
+class StructuredReadoutIntoFeature(tf.keras.layers.Layer):
+  """Reads out a feature value from select nodes (or edges) in a graph.
+
+  This Keras Layer wraps the `tfgnn.structured_readout_into_feature()` function.
+  It is is similar to `tfgnn.keras.layers.StructuredReadout` (see there),
+  except that it does not return the readout result itself but a modified
+  `GraphTensor` in which the readout result is stored as a feature on
+  the auxiliary `readout_node_set`. (See `tfgnn.structured_readout()` for more
+  information on that.)
+
+  For example, this layer can be used in data processing before training
+  to move training labels out of the input graph seen my the model (see
+  `remove_input_feature`) onto the auxiliary `readout_node_set`.
+
+  Init args:
+    key: A string key to select between possibly multiple named readouts
+      (such as `"source"` and `"target"` for link prediction). Can be fixed
+      in init, or selected for each call.
+    feature_name: The name of a feature to read out from, as with
+      `tfgnn.structured_readout()`.
+    new_feature_name: The name of the feature to add to `readout_node_set`
+      for storing the readout result. If unset, defaults to `feature_name`.
+      It is an error if the added feature already exists on `readout_node_set`
+      in the input `graph`, unless `overwrite=True` is set.
+    remove_input_feature: If set, the given `feature_name` is removed from the
+      node (or edge) set(s) that contain the value to be read out in the input
+      `GraphTensor`.
+    overwrite: If set, allows overwriting a potentially already existing
+      feature `graph.node_sets[readout_node_set][new_feature_name]`.
+    readout_node_set: A string, defaults to `"_readout"`. This is used as the
+      name for the readout node set and as a name prefix for its edge sets.
+    validate: Setting this to false disables the validity checks of
+      `tfgnn.structured_readout()`. This is strongly discouraged, unless great
+      care is taken to run `tfgnn.validate_graph_tensor_for_readout()` earlier
+      on structurally unchanged GraphTensors.
+
+  Call args:
+    graph: The scalar `GraphTensor` to read from.
+    key: Same meaning as for init. Must be passed to init, or to call,
+      or to both (with the same value).
+
+  Returns:
+    A `GraphTensor` like `graph`, with the readout result stored as
+    `.node_sets[readout_node_set][new_feature_name]` and possibly the
+    readout input feature removed (see `remove_input_feature`).
+  """
+
+  def __init__(
+      self,
+      key: Optional[str] = None,
+      *,
+      feature_name: FieldName,
+      new_feature_name: Optional[FieldName] = None,
+      remove_input_feature: bool = False,
+      overwrite: bool = False,
+      readout_node_set: NodeSetName = "_readout",
+      validate: bool = True,
+      **kwargs):
+    super().__init__(**kwargs)
+    self._key = key
+    self._feature_name = feature_name
+    self._new_feature_name = new_feature_name
+    self._remove_input_feature = remove_input_feature
+    self._overwrite = overwrite
+    self._readout_node_set = readout_node_set
+    self._validate = validate
+
+  def get_config(self):
+    return dict(
+        key=self._key,
+        feature_name=self._feature_name,
+        new_feature_name=self._new_feature_name,
+        remove_input_feature=self._remove_input_feature,
+        overwrite=self._overwrite,
+        readout_node_set=self._readout_node_set,
+        validate=self._validate,
+        **super().get_config())
+
+  def call(self,
+           graph: GraphTensor,
+           *,
+           key: Optional[str] = None) -> GraphTensor:
+    _check_init_call_arg_consistency("StructuredReadoutIntoFeature", "key",
+                                     self._key, key)
+    if key is None:
+      key = self._key
+    if key is None:
+      raise ValueError("The StructuredReadoutIntoFeature layer requires "
+                       "a readout key to be set at init or call time")
+
+    gt.check_scalar_graph_tensor(graph, "StructuredReadoutIntoFeature")
+    return readout.structured_readout_into_feature(
+        graph,
+        key=key,
+        feature_name=self._feature_name,
+        new_feature_name=self._new_feature_name,
+        remove_input_feature=self._remove_input_feature,
+        overwrite=self._overwrite,
+        readout_node_set=self._readout_node_set,
+        validate=self._validate)
+
+
+@tf.keras.utils.register_keras_serializable(package="GNN")
+class AddReadoutFromFirstNode(tf.keras.layers.Layer):
+  """Adds readout node set equivalent to `tfgnn.keras.layers.ReadoutFirstNode`.
+
+  Init args:
+    key: A key, for use with `tfgnn.keras.layers.StructuredReadout`. The input
+      graph must not already contain auxiliary edge sets for readout with this
+      key.
+    node_set_name: The name of the node set from which values are to be read
+      out.
+    readout_node_set: The name of the auxiliary node set for readout,
+      as in `tfgnn.structured_readout()`.
+
+  Call args:
+    graph: A scalar `GraphTensor`. If it contains the readout_node_set already,
+      its size in each graph component must be 1.
+
+  Returns:
+    A modified `GraphTensor` so that `tfgnn.keras.layers.StructuredReadout(key)`
+    acts like `tfgnn.keras.layers.ReadoutFirstNode(node_set_name=node_set_name)`
+    on the input graph.
+  """
+
+  def __init__(
+      self,
+      key: str,
+      *,
+      node_set_name: NodeSetName,
+      readout_node_set: NodeSetName = "_readout",
+      **kwargs):
+    super().__init__(**kwargs)
+    self._key = key
+    self._node_set_name = node_set_name
+    self._readout_node_set = readout_node_set
+
+  def get_config(self):
+    return dict(
+        key=self._key,
+        node_set_name=self._node_set_name,
+        readout_node_set=self._readout_node_set,
+        **super().get_config())
+
+  def call(self, graph: GraphTensor) -> GraphTensor:
+    gt.check_scalar_graph_tensor(graph, "AddReadoutFromFirstNode")
+    return readout.add_readout_from_first_node(
+        graph,
+        key=self._key,
+        node_set_name=self._node_set_name,
+        readout_node_set=self._readout_node_set)
+
+
 class BroadcastPoolBase(tf.keras.layers.Layer):
   """Base class to Broadcast and Pool.
 
   Broadcast and Pool work on the same "many-to-one" relationships in a
   GraphTensor, just with different directions of data flow. This base class
   provides their common handling of init and call args that specify the
   relationship:
 
-    * An edge_set_name or node_set_name specifies the "many" things that are
-      being broadcast to or pooled from. Collectively, the edge or node set name
-      is called the location.
+    * An edge_set_name or node_set_name (or a sequence thereof) specifies the
+      "many" things that are being broadcast to or pooled from. Collectively,
+      the edge or node set name is called the location.
     * An incident node tag SOURCE or TARGET or the special tag CONTEXT
       specifies the "one" thing that is being broadcast from or pooled to.
       The tag is understood relative to each edge (or node): the SOURCE or
       TARGET node incident to each edge, or the CONTEXT of the component
       to which the edge or node belongs.
       It is an error to use node_set_name with a tag other than CONTEXT.
 
   This base class also manages the feature_name used to select a feature
   at the origin of the Broadcast or Pool operation.
-  Broadcast and Pool also select a feature by name from their respective
-  origin.
 
   This base class manages tag, edge_set_name, node_set_name and feature_name
   for init, get_config and call but leaves the actual computation and
   user-visible documentation to concrete subclasses Broadcast and Pool.
   """
 
-  def __init__(self,
-               *,
-               tag: Optional[const.IncidentNodeOrContextTag] = None,
-               edge_set_name: Optional[gt.EdgeSetName] = None,
-               node_set_name: Optional[gt.NodeSetName] = None,
-               feature_name: Optional[gt.FieldName] = None,
-               **kwargs):
+  def __init__(
+      self,
+      *,
+      tag: Optional[IncidentNodeOrContextTag] = None,
+      edge_set_name: Union[Sequence[EdgeSetName], EdgeSetName, None] = None,
+      node_set_name: Union[Sequence[NodeSetName], NodeSetName, None] = None,
+      feature_name: Optional[FieldName] = None,
+      **kwargs,
+  ):
     super().__init__(**kwargs)
     self._check_tag(tag)
     self._tag = tag
     self._location = self._get_location(node_set_name=node_set_name,
                                         edge_set_name=edge_set_name)
     self._check_location(self._location, tag, required=False)
     self._feature_name = feature_name
@@ -335,19 +612,21 @@
   def get_config(self):
     config = super().get_config().copy()
     config["tag"] = self._tag
     config.update(self._location)
     config["feature_name"] = self._feature_name
     return config
 
-  def _fixup_call_args(self,
-                       tag: Optional[const.IncidentNodeOrContextTag] = None,
-                       edge_set_name: Optional[gt.EdgeSetName] = None,
-                       node_set_name: Optional[gt.NodeSetName] = None,
-                       feature_name: Optional[gt.FieldName] = None):
+  def _fixup_call_args(
+      self,
+      tag: Optional[IncidentNodeOrContextTag] = None,
+      edge_set_name: Union[Sequence[EdgeSetName], EdgeSetName, None] = None,
+      node_set_name: Union[Sequence[NodeSetName], NodeSetName, None] = None,
+      feature_name: Optional[FieldName] = None,
+  ):
     self._check_tag(tag)
     _check_init_call_arg_consistency(self._layer_name, "tag", self._tag, tag)
     if tag is None:
       tag = self._tag
     if tag is None:
       raise ValueError(f"The {self._layer_name} layer requires `tag=` "
                        "to be set at init or call time")
@@ -368,25 +647,25 @@
       feature_name = self._feature_name
     if feature_name is None:
       feature_name = const.HIDDEN_STATE
 
     return tag, edge_set_name, node_set_name, feature_name
 
   @property
-  def tag(self) -> Optional[const.IncidentNodeOrContextTag]:
+  def tag(self) -> Optional[IncidentNodeOrContextTag]:
     """Returns the tag argument to init, or None if unset."""
     return self._tag
 
   @property
-  def location(self) -> Mapping[str, str]:
+  def location(self) -> Mapping[str, Union[str, Sequence[str]]]:
     """Returns dict of kwarg to init with the node or edge set name."""
     return self._location
 
   @property
-  def feature_name(self) -> Optional[gt.FieldName]:
+  def feature_name(self) -> Optional[FieldName]:
     """Returns the feature_name argument to init, or None if unset."""
     return self._feature_name
 
   @property
   def _layer_name(self) -> str:
     """The user-visible name of the Layer class in logged messages."""
     return self.__class__.__name__
@@ -394,17 +673,26 @@
   def _check_tag(self, tag):
     if tag not in [None, const.SOURCE, const.TARGET, const.CONTEXT]:
       raise ValueError(f"The {self._layer_name} layer requires tag to be "
                        "one of tfgnn.SOURCE, tfgnn.TARGET or tfgnn.CONTEXT.")
 
   def _get_location(self, *, node_set_name, edge_set_name):
     """Returns dict of non-None kwargs for selecting the node or edge set."""
+    def clone_sequence(x):
+      if isinstance(x, Sequence) and not isinstance(x, str):
+        # Make a copy to avoid references to user-visible mutable lists.
+        return tuple(x)
+      return x
+
     result = dict()
-    if node_set_name is not None: result.update(node_set_name=node_set_name)
-    if edge_set_name is not None: result.update(edge_set_name=edge_set_name)
+    if node_set_name is not None:
+      result.update(node_set_name=clone_sequence(node_set_name))
+    if edge_set_name is not None:
+      result.update(edge_set_name=clone_sequence(edge_set_name))
+
     if len(result) > 1:
       raise ValueError(f"The {self._layer_name} layer allows at most one of "
                        "edge_set_name and node_set_name to be set.")
     return result
 
   def _check_location(self, location, tag, required=False):
     """Raises ValueError for bad location. May be None if not required."""
@@ -424,206 +712,208 @@
             "requires edge_set_name but not node_set_name")
 
 
 @tf.keras.utils.register_keras_serializable(package="GNN")
 class Broadcast(BroadcastPoolBase):
   """Broadcasts a GraphTensor feature.
 
-  This layer accepts a complete GraphTensor and returns a tensor with the
-  broadcast feature value.
+  This layer accepts a complete GraphTensor and returns a tensor (or tensors)
+  with the broadcast feature value.
 
   There are two kinds of broadcast that this layer can be used for:
 
-    * From a node set to an edge set. This is selected by specifying
-      the origin by tag `tgnn.SOURCE` or `tfgnn.TARGET` and the receiver
-      as `edge_set_name=...`; the node set name is implied.
-      The result is a tensor shaped like an edge feature in which each edge
-      has a copy of the feature that is present at its SOURCE or TARGET node.
-      From a node's point of view, SOURCE means broadcast to outgoing edges,
-      and TARGET means broadcast to incoming edges.
-    * From the context to a node set or edge set. This is selected by
-      specifying the origin by tag `tfgnn.CONTEXT` and the receiver as either
-      a `node_set_name=...` or an `edge_set_name=...`.
-      The result is a tensor shaped like a node/edge feature in which each
-      node/edge has a copy of the context feature in its graph component.
-      (For more on components, see GraphTensor.merge_batch_to_components().)
+    * From a node set to an edge set (or multiple edge sets). This is selected
+      by specifying the receiver edge set(s) as `edge_set_name=...` and the
+      sender by tag `tgnn.SOURCE` or `tfgnn.TARGET` relative to the edge set(s).
+      The node set name is implied. (In case of multiple edge sets, it must
+      agree between all of them.)
+      The result is a tensor (or list of tensors) shaped like an edge feature
+      in which each edge has a copy of the feature that is present at its
+      `SOURCE` or `TARGET` node. From a node's point of view, `SOURCE` means
+      broadcast to outgoing edges, and `TARGET` means broadcast to incoming
+      edges.
+    * From the context to one (or more) node sets or one (or more) edge sets.
+      This is selected by specifying the receiver(s) as either
+      `node_set_name=...` or `edge_set_name=...` and the sender by tag
+      `tfgnn.CONTEXT`.
+      The result is a tensor (or list of tensors) shaped like a node/edge
+      feature in which each node/edge has a copy of the context feature from
+      the graph component it belongs to. (For more on components, see
+      `tfgnn.GraphTensor.merge_batch_to_components()`.)
 
   Both the initialization of and the call to this layer accept arguments to
-  set the tag, node/edge_set_name, and the feature_name. The call
-  arguments take effect for that call only and can supply missing values,
+  set the `tag`, `node_set_name`/`edge_set_name`, and the `feature_name`. The
+  call arguments take effect for that call only and can supply missing values,
   but they are not allowed to contradict initialization arguments.
-  The feature name can be left unset to select tfgnn.HIDDEN_STATE.
+  The feature name can be left unset to select `tfgnn.HIDDEN_STATE`.
 
   Init args:
-    tag: Can be set to one of tfgnn.SOURCE, tfgnn.TARGET or tfgnn.CONTEXT.
+    tag: Can be set to one of `tfgnn.SOURCE`, `tfgnn.TARGET` or `tfgnn.CONTEXT`
+      to select the sender from which feature values are broadcast.
     edge_set_name: If set, the feature will be broadcast to this edge set
-      from the given origin. Mutually exclusive with node_set_name.
-    node_set_name: If set, the feature will be broadcast to this node set.
-      Origin must be CONTEXT. Mutually exclusive with edge_set_name.
+      (or this sequence of edge sets) from the sender given by `tag`.
+      Mutually exclusive with `node_set_name`.
+    node_set_name: If set, the feature will be broadcast to this node set
+      (or sequence of node sets). The sender must be selected as
+      `tag=tfgn.CONTEXT`. Mutually exclusive with `edge_set_name`.
     feature_name: The name of the feature to read. If unset (also in call),
-      the default state feature will be read.
+      the `tfgnn.HIDDEN_STATE` feature will be read.
 
   Call args:
-    graph: The scalar GraphTensor to read from.
+    graph: The scalar `tfgnn.GraphTensor` to read from.
     tag: Same meaning as for init. Must be passed to init, or to call,
       or to both (with the same value).
     edge_set_name, node_set_name: Same meaning as for init. One of them must
       be passed to init, or to call, or to both (with the same value).
     feature_name: Same meaning as for init. If passed to both, the value must
-      be the same. If passed to neither, tfgnn.HIDDEN_STATE is used.
+      be the same. If passed to neither, `tfgnn.HIDDEN_STATE` is used.
 
   Returns:
-    A tensor with the feature value broadcast to the target.
+    A tensor (or list of tensors) with the feature values broadcast to the
+    requested receivers.
   """
 
-  def __init__(self,
-               tag: Optional[const.IncidentNodeOrContextTag] = None,
-               *,
-               edge_set_name: Optional[gt.EdgeSetName] = None,
-               node_set_name: Optional[gt.NodeSetName] = None,
-               feature_name: Optional[gt.FieldName] = None,
-               **kwargs):
+  def __init__(
+      self,
+      tag: Optional[IncidentNodeOrContextTag] = None,
+      *,
+      edge_set_name: Union[Sequence[EdgeSetName], EdgeSetName, None] = None,
+      node_set_name: Union[Sequence[NodeSetName], NodeSetName, None] = None,
+      feature_name: Optional[FieldName] = None,
+      **kwargs,
+  ):
     super().__init__(
         tag=tag, edge_set_name=edge_set_name, node_set_name=node_set_name,
         feature_name=feature_name, **kwargs)
 
-  def call(self,
-           graph: gt.GraphTensor,
-           *,
-           tag: Optional[const.IncidentNodeOrContextTag] = None,
-           edge_set_name: Optional[gt.EdgeSetName] = None,
-           node_set_name: Optional[gt.NodeSetName] = None,
-           feature_name: Optional[gt.FieldName] = None) -> gt.Field:
+  def call(
+      self,
+      graph: GraphTensor,
+      *,
+      tag: Optional[IncidentNodeOrContextTag] = None,
+      edge_set_name: Union[Sequence[EdgeSetName], EdgeSetName, None] = None,
+      node_set_name: Union[Sequence[NodeSetName], NodeSetName, None] = None,
+      feature_name: Optional[FieldName] = None,
+  ) -> Union[list[Field], Field]:
     gt.check_scalar_graph_tensor(graph, "Broadcast")
     tag, edge_set_name, node_set_name, feature_name = self._fixup_call_args(
         tag, edge_set_name, node_set_name, feature_name)
 
-    if tag == const.CONTEXT:
-      if node_set_name is not None:
-        return ops.broadcast_context_to_nodes(
-            graph, node_set_name, feature_name=feature_name)
-      else:
-        return ops.broadcast_context_to_edges(
-            graph, edge_set_name, feature_name=feature_name)
-    else:
-      assert tag in (const.SOURCE, const.TARGET), f"Internal error: tag={tag}"
-      return ops.broadcast_node_to_edges(
-          graph, edge_set_name, tag, feature_name=feature_name)
+    return broadcast_ops.broadcast_v2(
+        graph, tag, edge_set_name=edge_set_name, node_set_name=node_set_name,
+        feature_name=feature_name)
 
 
 @tf.keras.utils.register_keras_serializable(package="GNN")
 class Pool(BroadcastPoolBase):
   """Pools a GraphTensor feature.
 
   This layer accepts a complete GraphTensor and returns a tensor with the
   result of pooling some feature.
 
   There are two kinds of pooling that this layer can be used for:
 
-    * From an edge set to a node set. This is selected by specifying the
-      origin as `edge_set_name=...` and the receiver with tag `tgnn.SOURCE`
-      or `tfgnn.TARGET`; the corresponding node set name is implied.
+    * From an edge set (or multiple edge sets) to a single node set. This is
+      selected by specifying the sender as `edge_set_name=...` and the receiver
+      with tag `tgnn.SOURCE` or `tfgnn.TARGET`; the corresponding node set name
+      is implied. (In case of multiple edge sets, it must be the same for all.)
       The result is a tensor shaped like a node feature in which each node
-      has the aggregated feature values from the edges of the edge set that
-      have it as their SOURCE or TARGET, resp.; that is, the outgoing or
+      has the aggregated feature values from the edges of the edge set(s) that
+      have it as their `SOURCE` or `TARGET`, resp.; that is, the outgoing or
       incoming edges of the node.
-    * From a node set or edge set to the context. This is selected by specifying
-      the origin as either a `node_set_name=...` or an `edge_set_name=...` and
-      the receiver with tag `tfgnn.CONTEXT`. The result is a tensor shaped
-      like a context feature in which each graph component has the aggregated
-      feature values from those nodes/edges in the selected node or edge set
-      that belong to the component.
-      (For more on components, see GraphTensor.merge_batch_to_components().)
+    * From one (or more) node sets or one (or more) edge sets to the context.
+      This is selected by specifying the sender as either `node_set_name=...`
+      or `edge_set_name=...` and the receiver with tag `tfgnn.CONTEXT`.
+      The result is a tensor shaped like a context feature in which the entry
+      for each graph component has the aggregated feature values from its
+      nodes/edges in the selected node or edge set(s). (For more on components,
+      see `tfgnn.GraphTensor.merge_batch_to_components()`.)
 
   Feature values are aggregated into a single value by a reduction function
-  from `tfgnn.get_registered_reduce_operation_names()`, see also
-  `tfgnn.register_reduce_operation()`. The pre-configured choices include
-  "sum", "mean", "max" and "min".
+  like `"sum"` or `"mean|max_no_inf"` as described for `tfgnn.pool()`; see there
+  for more details.
 
   Both the initialization of and the call to this layer accept arguments for
-  the receiver tag, the node/edge_set_name, the reduce_type and the
-  feature_name. The call arguments take effect for that call only and can
+  the receiver `tag`, the `node_set_name`/`edge_set_name`, the `reduce_type` and
+  the `feature_name`. The call arguments take effect for that call only and can
   supply missing values, but they are not allowed to contradict initialization
   arguments.
-  The feature name can be left unset to select tfgnn.HIDDEN_STATE.
+  The feature name can be left unset to select `tfgnn.HIDDEN_STATE`.
 
   Init args:
-    tag: Can be set to one of tfgnn.SOURCE, tfgnn.TARGET or tfgnn.CONTEXT
+    tag: Can be set to one of `tfgnn.SOURCE`, `tfgnn.TARGET` or `tfgnn.CONTEXT`
       to select the receiver.
-    reduce_type: Can be set to any name from
-      tfgnn.get_registered_reduce_operation_names().
+    reduce_type: Can be set to any `reduce_type` understood by `tfgnn.pool()`.
     edge_set_name: If set, the feature will be pooled from this edge set
-      to the given receiver `tag`. Mutually exclusive with node_set_name.
-    node_set_name: If set, the feature will be pooled from this node set.
-      The `tag` must be CONTEXT. Mutually exclusive with edge_set_name.
+      (or this sequence of edge sets) to the receiver given by `tag`.
+      Mutually exclusive with `node_set_name`.
+    node_set_name: If set, the feature will be pooled from this node set
+      (or sequence of node sets). The receiver must be selected as
+      `tag=tfgnn.CONTEXT`. Mutually exclusive with `edge_set_name`.
     feature_name: The name of the feature to read. If unset (also in call),
-      the default state feature will be read.
+      the `tfgnn.HIDDEN_STATE` feature will be read.
 
   Call args:
-    graph: The scalar GraphTensor to read from.
+    graph: The scalar `tfgnn.GraphTensor` to read from.
     reduce_type: Same meaning as for init. Must be passed to init, or to call,
       or to both (with the same value).
     tag: Same meaning as for init. Must be passed to init, or to call,
       or to both (with the same value).
     edge_set_name, node_set_name: Same meaning as for init. One of them must
       be passed to init, or to call, or to both (with the same value).
     feature_name: Same meaning as for init. If passed to both, the value must
-      be the same. If passed to neither, tfgnn.HIDDEN_STATE is used.
+      be the same. If passed to neither, `tfgnn.HIDDEN_STATE` is used.
 
   Returns:
     A tensor with the pooled feature value.
   """
 
-  def __init__(self,
-               tag: Optional[const.IncidentNodeOrContextTag] = None,
-               reduce_type: Optional[str] = None,
-               *,
-               edge_set_name: Optional[gt.EdgeSetName] = None,
-               node_set_name: Optional[gt.NodeSetName] = None,
-               feature_name: Optional[gt.FieldName] = None,
-               **kwargs):
+  def __init__(
+      self,
+      tag: Optional[IncidentNodeOrContextTag] = None,
+      reduce_type: Optional[str] = None,
+      *,
+      edge_set_name: Union[Sequence[EdgeSetName], EdgeSetName, None] = None,
+      node_set_name: Union[Sequence[NodeSetName], NodeSetName, None] = None,
+      feature_name: Optional[FieldName] = None,
+      **kwargs,
+  ):
     super().__init__(
         tag=tag, edge_set_name=edge_set_name, node_set_name=node_set_name,
         feature_name=feature_name, **kwargs)
     self._reduce_type = reduce_type
 
   def get_config(self):
     config = super().get_config()  # Our base class returns a private copy.
     config["reduce_type"] = self._reduce_type
     return config
 
-  def call(self,
-           graph: gt.GraphTensor,
-           *,
-           tag: Optional[const.IncidentNodeOrContextTag] = None,
-           reduce_type: Optional[str] = None,
-           edge_set_name: Optional[gt.EdgeSetName] = None,
-           node_set_name: Optional[gt.NodeSetName] = None,
-           feature_name: Optional[gt.FieldName] = None) -> gt.Field:
+  def call(
+      self,
+      graph: GraphTensor,
+      *,
+      tag: Optional[IncidentNodeOrContextTag] = None,
+      reduce_type: Optional[str] = None,
+      edge_set_name: Union[Sequence[EdgeSetName], EdgeSetName, None] = None,
+      node_set_name: Union[Sequence[NodeSetName], NodeSetName, None] = None,
+      feature_name: Optional[FieldName] = None,
+  ) -> Field:
     gt.check_scalar_graph_tensor(graph, "Pool")
     tag, edge_set_name, node_set_name, feature_name = self._fixup_call_args(
         tag, edge_set_name, node_set_name, feature_name)
 
     _check_init_call_arg_consistency(self._layer_name, "reduce_type",
                                      self._reduce_type, reduce_type)
     if reduce_type is None:
       reduce_type = self._reduce_type
     if reduce_type is None:
       raise ValueError("The Pool layer requires reduce_type "
                        "to be set at init or call time")
 
-    if tag == const.CONTEXT:
-      if node_set_name is not None:
-        return ops.pool_nodes_to_context(
-            graph, node_set_name, reduce_type, feature_name=feature_name)
-      else:
-        return ops.pool_edges_to_context(
-            graph, edge_set_name, reduce_type, feature_name=feature_name)
-    else:
-      assert tag in (const.SOURCE, const.TARGET), f"Internal error: tag={tag}"
-      return ops.pool_edges_to_node(
-          graph, edge_set_name, tag, reduce_type, feature_name=feature_name)
+    return pool_ops.pool_v2(
+        graph, tag, edge_set_name=edge_set_name, node_set_name=node_set_name,
+        reduce_type=reduce_type, feature_name=feature_name)
 
   @property
   def reduce_type(self) -> str:
     """Returns the reduce_type argument to init, or None if unset."""
     return self._reduce_type
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/graph_update.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/graph_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 """The GraphUpdate layer and its pieces."""
 
 import sys
 from typing import Any, Callable, Mapping, Optional, Sequence
 
 import tensorflow as tf
 
+from tensorflow_gnn.graph import broadcast_ops
 from tensorflow_gnn.graph import dict_utils as du
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
-from tensorflow_gnn.graph import graph_tensor_ops as ops
 from tensorflow_gnn.keras.layers import next_state as next_state_lib
 
 # pylint:disable=g-import-not-at-top
 if sys.version_info >= (3, 8):
   from typing import Protocol
 else:
   from typing_extensions import Protocol
@@ -330,21 +330,22 @@
     next_state_inputs.append(
         _get_feature_or_features(graph.edge_sets[edge_set_name],
                                  self._edge_input_feature))
     # Input from incident nodes.
     input_from_incident_nodes = {}
     if self._node_input_feature is not None:
       for node_tag in self._node_input_tags:
-        input_from_incident_nodes[node_tag] = ops.broadcast_node_to_edges(
-            graph, edge_set_name, node_tag,
-            feature_name=self._node_input_feature)
+        input_from_incident_nodes[
+            node_tag] = broadcast_ops.broadcast_node_to_edges(
+                graph, edge_set_name, node_tag,
+                feature_name=self._node_input_feature)
     next_state_inputs.append(input_from_incident_nodes)
     # Input from context.
     next_state_inputs.append(tf.nest.map_structure(
-        lambda value: ops.broadcast_context_to_edges(  # pylint: disable=g-long-lambda
+        lambda value: broadcast_ops.broadcast_context_to_edges(  # pylint: disable=g-long-lambda
             graph, edge_set_name, feature_value=value),
         _get_feature_or_features(graph.context, self._context_input_feature)))
 
     next_state_inputs = tuple(next_state_inputs)
     assert len(next_state_inputs) == 3, "Internal error"
     return self._next_state(next_state_inputs)
 
@@ -429,15 +430,15 @@
     input_from_edge_sets = {}
     for edge_set_name, input_fn in sorted(self._edge_set_inputs.items()):
       input_from_edge_sets[edge_set_name] = input_fn(
           graph, edge_set_name=edge_set_name)
     next_state_inputs.append(input_from_edge_sets)
     # Input from context.
     next_state_inputs.append(tf.nest.map_structure(
-        lambda value: ops.broadcast_context_to_nodes(  # pylint: disable=g-long-lambda
+        lambda value: broadcast_ops.broadcast_context_to_nodes(  # pylint: disable=g-long-lambda
             graph, node_set_name, feature_value=value),
         _get_feature_or_features(graph.context, self._context_input_feature)))
 
     next_state_inputs = tuple(next_state_inputs)
     assert len(next_state_inputs) == 3, "Internal error"
     return self._next_state(next_state_inputs)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/item_dropout_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/item_dropout_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """The MapFeatures layer and related definitions."""
 
-from typing import Mapping, Union
+import re
+from typing import Mapping, Optional, Union
 
 import tensorflow as tf
 
 from tensorflow_gnn.graph import dict_utils as du
 from tensorflow_gnn.graph import graph_constants as const
 from tensorflow_gnn.graph import graph_tensor as gt
 
@@ -29,14 +30,18 @@
 
   This layer transforms the feature maps of graph pieces (that is, EdgeSets,
   NodeSets, or the Context) by applying Keras Models to them. Those Models
   are built by user-supplied callbacks that receive a KerasTensor for the
   graph piece as input and return a dict of output features computed with
   the Keras functional API, see https://tensorflow.org/guide/keras/functional.
 
+  Auxiliary graph pieces (e.g., for `tfgnn.keras.layers.StructuredReadout`)
+  are skipped, unless explicitly requested via `allowed_aux_node_sets_pattern`
+  or `allowed_aux_edge_sets_pattern`.
+
   Examples:
 
   ```python
   # Hashes edge features called "id", leaves others unchanged:
   def edge_sets_fn(edge_set, *, edge_set_name):
     features = edge_set.get_features_dict()
     ids = features.pop("id")
@@ -58,30 +63,36 @@
           tf.keras.layers.Concatenate([v for _, v in sorted(features.items())]))
     else:  # There are no inputs, create an empty state.
       return tfgnn.keras.layers.MakeEmptyFeature()(node_set)
   graph = tfgnn.keras.layers.MapFeatures(node_sets_fn=node_sets_fn)(graph)
   ```
 
   ```python
-  # Doubles all feature values, with one callback used for all graph pieces.
+  # Doubles all feature values, with one callback used for all graph pieces,
+  # including auxiliary ones.
   def fn(inputs, **unused_kwargs):
     return {k: tf.add(v, v) for k, v in inputs.features.items()}
   graph = tfgnn.keras.layers.MapFeatures(
-      context_fn=fn, node_sets_fn=fn, edge_sets_fn=fn)(graph)
+      context_fn=fn, node_sets_fn=fn, edge_sets_fn=fn,
+      allowed_aux_node_sets_pattern=r".*", allowed_aux_edge_sets_pattern=r".*"
+  )(graph)
   ```
 
   When this layer is called on a GraphTensor, it transforms the feature map
   of each graph piece with the model built by the respective callbacks.
   The very first call to this layer triggers building the models. Subsequent
   calls to this layer do not use the callbacks again, but check that their
   input does not have more graph pieces or features than seen by the callbacks:
 
     * It is an error to call with a node set or edge set that was not present
       in the first call. (After the first call, it is too late to initialize
       another model for it and find out what the callback would have done.)
+      An exception is made for auxiliary node sets and edge sets: If they would
+      have been ignored in the first call anyways, they may be present in later
+      calls and get ignored there.
     * It is an error to call with a set of feature names of some graph piece
       that has changed since the first call, except for those graph pieces for
       which the callback was `None` or returned `None` to request passthrough.
       (Without this check, the model for the graph piece would silently drop
       new features, even though the callback might have handled them.)
 
   More details on the callbacks:
@@ -122,28 +133,44 @@
   for the common case of creating an empty hidden state for a latent node;
   see its documentation for details on how to use it with TPUs.
   If TPUs and shape inference are no concern, the callback can simply use
   `graph_piece.sizes` or (esp. for rank 0) graph_piece.total_size` to construct
   outputs of the right shape, but not `graph_piece.spec.total_size`, which
   breaks the dependency chain of KerasTensors.
 
+  Weight sharing between the transformation of different graph pieces is
+  possible by sharing the Keras objects between the respective callback
+  invocations.
+
+  WARNING: Weight sharing fails in `tf.keras.models.load_model()`
+  with an error message on weights missing from the checkpoint.
+  (Most users don't need to re-load their models this way.)
+
+  TODO(b/285243815): Remove warning when fixed.
+
   Init args:
     context_fn: A callback to build a Keras model for transforming context
       features. It will be called as `output = context_fn(g.context)`.
       Leaving this at the default `None` is equivalent to returning `None`.
     node_sets_fn: A callback to build a Keras model for transforming node set
       features. It will be called for every node sets as
       `node_sets_fn(g.node_sets[node_set_name], node_set_name=node_set_name)`.
       Leaving this at the default `None` is equivalent to returning `None`
       for every node set.
     edge_sets_fn: A callback to build a Keras model for transforming edge set
       features. It will be called for every edge sets as
       `edge_sets_fn(g.edge_sets[edge_set_name], edge_set_name=edge_set_name)`.
       Leaving this at the default `None` is equivalent to returning `None`
       for every edge set.
+    allowed_aux_node_sets_pattern: If set, `node_sets_fn` is also invoked for
+      those auxiliary node sets that match this pattern, according to Python's
+      `re.fullmatch(pattern, node_set_name)`.
+    allowed_aux_edge_sets_pattern: If set, `edge_sets_fn` is also invoked for
+      those auxiliary edge sets that match this pattern, according to Python's
+      `re.fullmatch(pattern, edge_set_name)`.
 
   Call args:
     graph: A GraphTensor. The very first call triggers the building of
       the models that map the various feature maps, with tensor specs
       taken from the GraphTensorSpec of the first input.
 
   Call returns:
@@ -151,14 +178,17 @@
     transformed feature maps.
   """
 
   def __init__(self,
                context_fn=None,
                node_sets_fn=None,
                edge_sets_fn=None,
+               *,
+               allowed_aux_node_sets_pattern: Optional[str] = None,
+               allowed_aux_edge_sets_pattern: Optional[str] = None,
                **kwargs):
     from_config = kwargs.pop("_from_config", False)
     if from_config:
       context_model = kwargs.pop("context_model")
       node_set_models = kwargs.pop("node_set_models")
       edge_set_models = kwargs.pop("edge_set_models")
     super().__init__(**kwargs)
@@ -180,24 +210,28 @@
       self._context_fn = None
       self._node_sets_fn = None
       self._edge_sets_fn = None
       self._context_model = context_model
       self._node_set_models = node_set_models
       self._edge_set_models = edge_set_models
       self._is_initialized = True
+    self._allowed_aux_node_sets_pattern = allowed_aux_node_sets_pattern
+    self._allowed_aux_edge_sets_pattern = allowed_aux_edge_sets_pattern
 
   def get_config(self):
     if not self._is_initialized:
       raise ValueError("Cannot get a config for saving a MapFeatures layer "
                        "before it has been built (during the first call).")
     return dict(
         context_model=self._context_model,
         # Sublayers need to be top-level objects in the config (b/209560043).
         **du.with_key_prefix(self._node_set_models, "node_set_models/"),
         **du.with_key_prefix(self._edge_set_models, "edge_set_models/"),
+        allowed_aux_node_sets_pattern=self._allowed_aux_node_sets_pattern,
+        allowed_aux_edge_sets_pattern=self._allowed_aux_edge_sets_pattern,
         **super().get_config())
 
   @classmethod
   def from_config(cls, config):
     config["node_set_models"] = du.pop_by_prefix(config, "node_set_models/")
     config["edge_set_models"] = du.pop_by_prefix(config, "edge_set_models/")
     return cls(**config, _from_config=True)
@@ -205,20 +239,24 @@
   def _init_from_spec(self, spec: gt.GraphTensorSpec):
     self._context_model = _make_model_or_none(
         self._context_fn, spec.context_spec)
 
     # All node sets seen at initialization time. Value `None` means ignore.
     self._node_set_models = {}
     for node_set_name, node_set_spec in spec.node_sets_spec.items():
+      if self._ignore_node_set(node_set_name):
+        continue
       self._node_set_models[node_set_name] = _make_model_or_none(
           self._node_sets_fn, node_set_spec, node_set_name=node_set_name)
 
     # All edge sets seen at initialization time. Value `None` means ignore.
     self._edge_set_models = {}
     for edge_set_name, edge_set_spec in spec.edge_sets_spec.items():
+      if self._ignore_edge_set(edge_set_name):
+        continue
       self._edge_set_models[edge_set_name] = _make_model_or_none(
           self._edge_sets_fn, edge_set_spec, edge_set_name=edge_set_name)
 
     self._is_initialized = True
 
   def call(self, graph: gt.GraphTensor) -> gt.GraphTensor:
     if not self._is_initialized:
@@ -232,37 +270,55 @@
       context_features = _call_model(self._context_model, graph.context,
                                      logging_name="context")
 
     node_set_features = {}
     for node_set_name, node_set in graph.node_sets.items():
       try:
         model = self._node_set_models[node_set_name]
+        if model is None: continue  # Was explicitly ignored in initialization.
       except KeyError as e:
+        if self._ignore_node_set(node_set_name):
+          continue  # Would have been ignored in initialization.
         raise KeyError(f"Unexpected node set '{node_set_name}' "
                        "not seen in first call") from e
-      if model is None: continue  # Initialized to be ignored.
       node_set_features[node_set_name] = _call_model(
           model, node_set, logging_name=f"node_set '{node_set_name}'")
 
     edge_set_features = {}
     for edge_set_name, edge_set in graph.edge_sets.items():
       try:
         model = self._edge_set_models[edge_set_name]
+        if model is None: continue  # Was explicitly ignored in initialization.
       except KeyError as e:
+        if self._ignore_edge_set(edge_set_name):
+          continue  # Would have been ignored in initialization.
         raise KeyError(f"Unexpected edge set '{edge_set_name}' "
                        "not seen in first call") from e
-      if model is None: continue  # Initialized to be ignored.
       edge_set_features[edge_set_name] = _call_model(
           model, edge_set, logging_name=f"edge_set '{edge_set_name}'")
 
     result = graph.replace_features(context=context_features,
                                     node_sets=node_set_features,
                                     edge_sets=edge_set_features)
     return result
 
+  def _ignore_node_set(self, node_set_name):
+    if not gt.get_aux_type_prefix(node_set_name):
+      return False
+    if self._allowed_aux_node_sets_pattern is None:
+      return True
+    return not re.fullmatch(self._allowed_aux_node_sets_pattern, node_set_name)
+
+  def _ignore_edge_set(self, edge_set_name):
+    if not gt.get_aux_type_prefix(edge_set_name):
+      return False
+    if self._allowed_aux_edge_sets_pattern is None:
+      return True
+    return not re.fullmatch(self._allowed_aux_edge_sets_pattern, edge_set_name)
+
 
 def _make_model_or_none(model_fn, graph_piece_spec, **kwargs):
   """Returns a Model to map this graph piece, or None to leave it alone."""
   if model_fn is None:
     return None  # This graph piece is to be left alone.
 
   graph_piece_input = tf.keras.layers.Input(type_spec=graph_piece_spec)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/map_features_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/map_features_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for MapFeatures."""
 
+import collections
 import enum
 import functools
 import os
 
 from absl.testing import parameterized
 import tensorflow as tf
 from tensorflow_gnn.graph import adjacency as adj
@@ -80,14 +81,62 @@
     self.assertAllEqual(
         [[62.], [64.]] if map_edges else [[31.], [32.]],
         edges["e_dense"])
     self.assertAllEqual(
         rc([[2], [4, 8]] if map_edges else [[1], [2, 4]]),
         edges["e_ragged"])
 
+  @parameterized.named_parameters(
+      ("Default", {}, {"ordinary_nodes": 1, "ordinary_edges": 1}),
+      ("AllowReadoutNodes",
+       {"allowed_aux_node_sets_pattern": r"_readout\W.*"},
+       {"ordinary_nodes": 1, "ordinary_edges": 1,
+        "_readout:test": 1, "_readout:train": 1}),
+      ("AllowExtraEdges",
+       {"allowed_aux_edge_sets_pattern": r"_extra.*"},
+       {"ordinary_nodes": 1, "ordinary_edges": 1, "_extra_edges": 1}))
+  def testAuxPieces(self, kwargs_to_test, expected_call_counts):
+    input_graph = gt.GraphTensor.from_pieces(
+        node_sets={
+            "ordinary_nodes": gt.NodeSet.from_fields(sizes=tf.constant([1])),
+            "_extra_nodes": gt.NodeSet.from_fields(sizes=tf.constant([1])),
+            "_readout:train": gt.NodeSet.from_fields(sizes=tf.constant([1])),
+            "_readout:test": gt.NodeSet.from_fields(sizes=tf.constant([1])),
+        },
+        edge_sets={
+            "ordinary_edges": gt.EdgeSet.from_fields(
+                sizes=tf.constant([]),
+                adjacency=adj.Adjacency.from_indices(
+                    ("ordinary_nodes", tf.constant([0])),
+                    ("ordinary_nodes", tf.constant([0])))),
+            "_extra_edges": gt.EdgeSet.from_fields(
+                sizes=tf.constant([]),
+                adjacency=adj.Adjacency.from_indices(
+                    ("_extra_nodes", tf.constant([0])),
+                    ("_extra_nodes", tf.constant([0])))),
+            "_readout:train/seed": gt.EdgeSet.from_fields(
+                sizes=tf.constant([]),
+                adjacency=adj.Adjacency.from_indices(
+                    ("ordinary_nodes", tf.constant([0])),
+                    ("_readout:train", tf.constant([0])))),
+        })
+
+    call_counts = collections.defaultdict(lambda: 0)
+    def node_sets_fn(node_set, node_set_name):
+      call_counts[node_set_name] += 1
+      return node_set.features
+    def edge_sets_fn(edge_set, edge_set_name):
+      call_counts[edge_set_name] += 1
+      return edge_set.features
+    layer = map_features.MapFeatures(node_sets_fn=node_sets_fn,
+                                     edge_sets_fn=edge_sets_fn,
+                                     **kwargs_to_test)
+    _ = layer(input_graph)
+    self.assertDictEqual(expected_call_counts, call_counts)
+
   def testFilterFeatures(self):
     input_graph = _make_scalar_test_graph()
 
     def keep_all(the_input_graph_piece):  # For context.
       return the_input_graph_piece.features  # Test this ImmutableMapping works.
     def keep_dense_fn(inputs, *, node_set_name):  # For nodes.
       self.assertEqual(node_set_name, "nodes")
@@ -294,22 +343,25 @@
     _ = layer(graph_without)
 
   @parameterized.named_parameters(
       ("EdgeSet", "edge_sets_fn", dict(edges=False), dict(edges=True)),
       ("NodeSet", "node_sets_fn",
        dict(nodes=False, edges=False), dict(nodes=True, edges=False)))
   def testCheckUnexpected(self, kwarg_to_test, make_without, make_with):
-    graph_with = _make_scalar_test_graph(**make_with)
     graph_without = _make_scalar_test_graph(**make_without)
+    graph_with_readout = _make_scalar_test_graph(**make_without, readout=True)
+    graph_with_unexpected = _make_scalar_test_graph(**make_with)
     def keep_all(graph_piece, **_):
       return graph_piece.features
     layer = map_features.MapFeatures(**{kwarg_to_test: keep_all})
     _ = layer(graph_without)  # First call defines the known graph pieces.
+    _ = layer(graph_without)  # OK to call again.
+    _ = layer(graph_with_readout)  # OK to call with new aux pieces.
     with self.assertRaisesRegex(KeyError, r"Unexpected"):
-      _ = layer(graph_with)
+      _ = layer(graph_with_unexpected)
 
   def testBatchedGraphTensorRaggedReduce(self):
     rc = tf.ragged.constant
     # Test input is a GraphTensor of shape [3].
     # Each element has components with the given number of nodes in each.
     # The nodes of each element have a "ragged_id" feature with
     # alternatingly 1 or 2 values, numbered consecutively.
@@ -381,15 +433,15 @@
     return result
 
   def get_config(self):
     return dict(start=self.start)
 
 
 def _make_scalar_test_graph(*, context=True, nodes=True, edges=True,
-                            dense=True, ragged=True):
+                            dense=True, ragged=True, readout=False):
   c = tf.constant
   rc = tf.ragged.constant
 
   context_obj = None
   if context:
     features = {
         **({"c_dense": c([[1., 2.]])} if dense else {}),
@@ -412,14 +464,21 @@
         ("nodes", c([1, 0])))
     features = {
         **({"e_dense": c([[31.], [32.]])} if dense else {}),
         **({"e_ragged": rc([[1], [2, 4]])} if ragged else {})}
     edge_sets["edges"] = gt.EdgeSet.from_fields(
         sizes=c([2]), adjacency=adjacency, features=features)
 
+  if readout:  # Independent of ordinary nodes and edges.
+    node_sets["_readout"] = gt.NodeSet.from_fields(sizes=c([1]))
+    edge_sets["_readout/seed"] = gt.EdgeSet.from_fields(
+        sizes=c([1]),
+        adjacency=adj.Adjacency.from_indices(("nodes", c([0])),
+                                             ("nodes", c([0]))))
+
   return gt.GraphTensor.from_pieces(
       context=context_obj, node_sets=node_sets, edge_sets=edge_sets)
 
 
 def _make_test_graph_for_batching(node_sizes, start_id):
   """Returns graph with "nodes" with 1 or 2 "ragged_ids"."""
   nodes_features = {}
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 ```
 
 The names of the prototypical classes above are used in type annotations
 for the benefit of human readers, but pytype cannot actually check the
 interface requirements beyond being any Keras layer.
 """
 
-from typing import Any, Tuple
+from typing import Any, Optional, Tuple
 
 import tensorflow as tf
 
 from tensorflow_gnn.graph import graph_constants as const
 
 
 # See module docstring.
@@ -163,28 +163,30 @@
     activation: An activation function (none by default), as understood by
       `tf.keras.layers.Activation`. This activation function is applied after
       the residual block and the addition. If using this, typically the
       residual block does not have an activation function on its last layer,
       or vice versa.
     skip_connection_feature_name: Controls which input from the updated graph
       piece is added back after the residual block. If the input from the
-      updated graph piece is a single tensor, that one is used. If it is
-      a dict, this key is used; defaults to `tfgnn.HIDDEN_STATE`.
+      updated graph piece is a single tensor, that tensor is used, and this arg
+      must not be set. If the input is a dict, this key is used; if unset, it
+      defaults to `tfgnn.HIDDEN_STATE`.
 
   Call returns:
     A tensor to use as the new state.
   """
 
-  def __init__(self,
-               residual_block: tf.keras.layers.Layer,
-               *,
-               activation: Any = None,
-               skip_connection_feature_name: const.FieldName
-               = const.HIDDEN_STATE,
-               **kwargs):
+  def __init__(
+      self,
+      residual_block: tf.keras.layers.Layer,
+      *,
+      activation: Any = None,
+      skip_connection_feature_name: Optional[const.FieldName] = None,
+      **kwargs,
+  ):
     super().__init__(**kwargs)
     self._residual_block = residual_block
     if isinstance(activation, tf.keras.layers.Layer):
       self._activation = activation
     else:
       self._activation = tf.keras.layers.Activation(activation)
     self._skip_connection_feature_name = skip_connection_feature_name
@@ -199,27 +201,38 @@
   def call(
       self, inputs: Tuple[
           const.FieldOrFields, const.FieldsNest, const.FieldsNest
       ]) -> const.FieldOrFields:
     # Extract the feature for a skip connection.
     self_input = inputs[0]
     if isinstance(self_input, (tf.Tensor, tf.RaggedTensor)):
+      if self._skip_connection_feature_name is not None:
+        raise KeyError(
+            "ResidualNextState() invoked with explicit skip connection feature"
+            f" '{self._skip_connection_feature_name}', but the "
+            " updated graph piece does not have this key (it's not a"
+            f" dictionary) {self_input}."
+        )
       skip_connection_feature = self_input
       skip_connection_msg = "single input"
     else:
+      if self._skip_connection_feature_name is None:
+        skip_connection_feature_name = const.HIDDEN_STATE
+      else:
+        skip_connection_feature_name = self._skip_connection_feature_name
       try:
-        skip_connection_feature = self_input[self._skip_connection_feature_name]
+        skip_connection_feature = self_input[skip_connection_feature_name]
       except KeyError as e:
         raise KeyError(
             "ResidualNextState() could not find the "
-            f"skip connection feature '{self._skip_connection_feature_name}' "
+            f"skip connection feature '{skip_connection_feature_name}' "
             f"in the features of the updated graph piece: {list(self_input)}"
         ) from e
       skip_connection_msg = (
-          f"input feature '{self._skip_connection_feature_name}'")
+          f"input feature '{skip_connection_feature_name}'")
 
     # Compute the state update.
     net = tf.nest.flatten(inputs)
     net = tf.concat(net, axis=-1)
     net = self._residual_block(net)
     if skip_connection_feature.shape[1:].num_elements() == 0:
       tf.get_logger().warning(
@@ -262,8 +275,7 @@
       single_input, = second_input.values()
     except ValueError as e:
       raise ValueError(
           "Second input to SingleInputNextState had multiple values."
           " This layer should take only a single input."
       ) from e
     return single_input
-
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/next_state_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/next_state_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     actual = next_state((tf.constant([[1.]]),
                          {const.SOURCE: {"h0": tf.constant([[2.]]),
                                          "h1": tf.constant([[3.]])},
                           const.TARGET: tf.constant([[4.]])},
                          tf.constant([[5.]])))
     self.assertAllEqual([[2., 4., 6., 8., 10.]], actual)
 
+  def testTFLite(self):
+    self.skipTest(
+        "NextStateFromConcat TFLite functionality is tested in models/mt_albis")
+
 
 class ResidualNextStateTest(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.named_parameters(
       ("SoleFeature",),
       ("DefaultFeature", const.HIDDEN_STATE),
       ("CustomFeature", "my_feature", "my_feature"))
@@ -73,14 +77,61 @@
     init_div2 = tf.keras.initializers.Constant(0.5)
     next_state = next_state_lib.ResidualNextState(
         tf.keras.layers.Dense(1, use_bias=False, kernel_initializer=init_div2))
 
     actual = next_state((first_input, second_input, third_input))
     self.assertAllEqual([[1. + 2. + 4.]], actual)
 
+  def testMissingDictionaryThrowsException(self):
+    first_input = tf.constant([[32.0]])
+    init_div2 = tf.keras.initializers.Constant(0.5)
+    next_state = next_state_lib.ResidualNextState(
+        tf.keras.layers.Dense(1, use_bias=False, kernel_initializer=init_div2),
+        skip_connection_feature_name="my_feature",
+    )
+
+    with self.assertRaises(KeyError):
+      _ = next_state((first_input))
+
+  def testTFLite(self):
+    test_input_dict = {
+        "first_input": tf.constant([[64.0]]),
+        "second_input_0": tf.constant([[8.0]]),
+        "second_input_1": tf.constant([[16.0]]),
+        "third_input": tf.constant([[32.0]]),
+    }
+    inputs = {
+        "first_input": tf.keras.Input([1], None, "first_input", tf.float32),
+        "second_input_0": tf.keras.Input(
+            [1], None, "second_input_0", tf.float32
+        ),
+        "second_input_1": tf.keras.Input(
+            [1], None, "second_input_1", tf.float32
+        ),
+        "third_input": tf.keras.Input([1], None, "third_input", tf.float32),
+    }
+    layer = next_state_lib.ResidualNextState(
+        tf.keras.layers.Dense(1, use_bias=False), name="residual_next_state")
+    outputs = layer(
+        (inputs["first_input"],
+         {"second_input_0": inputs["second_input_0"],
+          "second_input_1": inputs["second_input_1"]},
+         inputs["third_input"],))
+    model = tf.keras.Model(inputs, outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = model(test_input_dict).numpy()
+
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner("serving_default")
+    obtained = signature_runner(**test_input_dict)["residual_next_state"]
+    self.assertAllClose(expected, obtained)
+
 
 class SingleInputNextStateTest(tf.test.TestCase, parameterized.TestCase):
 
   def test_single_input(self):
     next_state = next_state_lib.SingleInputNextState()
     input_triple = (tf.constant([[1.]]),
                     {"edge": tf.constant([[2.]])},
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/padding_ops.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/padding_ops.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/keras/layers/parse_example_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/keras/layers/parse_example_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/BUILD`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,47 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
 
 licenses(["notice"])
 
+package(default_visibility = [
+    "//tensorflow_gnn:__pkg__",
+    "//tensorflow_gnn/graph:__subpackages__",
+])
+
 package_group(name = "users")
 
 pytype_strict_library(
-    name = "contrastive_losses",
+    name = "graph_sage",
     srcs = ["__init__.py"],
     srcs_version = "PY3",
     visibility = [
+        ":__subpackages__",
         ":users",
     ],
     deps = [
         ":layers",
-        "//tensorflow_gnn/models/contrastive_losses/deep_graph_infomax:layers",
-        "//tensorflow_gnn/models/contrastive_losses/deep_graph_infomax:tasks",
     ],
 )
 
 pytype_strict_library(
     name = "layers",
     srcs = ["layers.py"],
     srcs_version = "PY3",
-    visibility = [
-        ":__subpackages__",
+    deps = [
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
     ],
+)
+
+tf_py_test(
+    name = "layers_test",
+    srcs = ["layers_test.py"],
+    python_version = "PY3",
+    srcs_version = "PY3",
     deps = [
+        ":layers",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/BUILD`

 * *Files 25% similar despite different names*

```diff
@@ -1,77 +1,61 @@
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_binary", "pytype_strict_library")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "distribute_py_test")
 
 licenses(["notice"])
 
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = ["//visibility:public"],
+)
+
 pytype_strict_library(
-    name = "layers",
-    srcs = ["layers.py"],
-    srcs_version = "PY3",
+    name = "train_lib",
+    srcs = ["train.py"],
     visibility = [
-        "//tensorflow_gnn/models/contrastive_losses:__pkg__",
+        ":__subpackages__",
     ],
     deps = [
+        ":utils",
+        "//third_party/py/absl:app",
+        "//third_party/py/absl/flags",
+        "//third_party/py/absl/logging",
+        "//third_party/py/ml_collections/config_dict",
+        "//third_party/py/ml_collections/config_flags",
         "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+        "//tensorflow_gnn/models/gat_v2",
+        "//tensorflow_gnn/models/hgt",
+        "//tensorflow_gnn/models/mt_albis",
+        "//tensorflow_gnn/models/multi_head_attention",
+        "//tensorflow_gnn/models/vanilla_mpnn",
+        "//tensorflow_gnn/runner",
     ],
 )
 
-tf_py_test(
-    name = "layers_test",
-    srcs = ["layers_test.py"],
+pytype_strict_binary(
+    name = "train",
+    srcs = ["train.py"],
     python_version = "PY3",
-    srcs_version = "PY3",
-    deps = [
-        ":layers",
-        "//:expect_absl_installed",
-        "//:expect_tensorflow_installed",
-    ],
+    deps = [":train_lib"],
 )
 
 pytype_strict_library(
-    name = "tasks",
-    srcs = ["tasks.py"],
+    name = "utils",
+    srcs = ["utils.py"],
     srcs_version = "PY3",
-    visibility = [
-        "//tensorflow_gnn/models/contrastive_losses:__pkg__",
-    ],
     deps = [
-        ":layers",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
-        "//tensorflow_gnn/models/contrastive_losses:layers",
-        "//tensorflow_gnn/runner",
     ],
 )
 
 tf_py_test(
-    name = "tasks_test",
-    srcs = ["tasks_test.py"],
+    name = "utils_test",
+    srcs = ["utils_test.py"],
     python_version = "PY3",
-    srcs_version = "PY3",
-    deps = [
-        ":tasks",
-        "//:expect_absl_installed",
-        "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
-    ],
-)
-
-distribute_py_test(
-    name = "distribute_test",
-    size = "large",
-    srcs = ["distribute_test.py"],
-    shard_count = 4,
-    tags = [
-        "no_oss",  # TODO(b/238827505)
-        "nomultivm",  # TODO(b/170502145)
-    ],
-    xla_enable_strict_auto_jit = False,
     deps = [
-        ":tasks",
+        ":utils",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
-        "//tensorflow_gnn/models/vanilla_mpnn",
-        "//tensorflow_gnn/runner",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/distribute_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,17 +20,26 @@
 from absl.testing import parameterized
 import tensorflow as tf
 import tensorflow.__internal__.distribute as tfdistribute
 import tensorflow.__internal__.test as tftest
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn import runner
 from tensorflow_gnn.models import vanilla_mpnn
-from tensorflow_gnn.models.contrastive_losses.deep_graph_infomax import tasks
+from tensorflow_gnn.models.contrastive_losses import tasks
 
+_CLASSES = tuple(range(32))
 _SCHEMA = """
+  context {
+    features {
+      key: "classes"
+      value {
+        dtype: DT_INT64
+      }
+    }
+  }
   node_sets {
     key: "node"
     value {
       features {
         key: "features"
         value {
           dtype: DT_FLOAT
@@ -45,112 +54,148 @@
       source: "node"
       target: "node"
     }
   }
 """
 
 
-def _all_eager_strategy_combinations():
+def _all_eager_strategy_and_task_combinations():
   strategies = [
       # default
       tfdistribute.combinations.default_strategy,
       # MirroredStrategy
       tfdistribute.combinations.mirrored_strategy_with_gpu_and_cpu,
       tfdistribute.combinations.mirrored_strategy_with_one_cpu,
       tfdistribute.combinations.mirrored_strategy_with_one_gpu,
       # MultiWorkerMirroredStrategy
       tfdistribute.combinations.multi_worker_mirrored_2x1_cpu,
       tfdistribute.combinations.multi_worker_mirrored_2x1_gpu,
-      # TPUStrategy
-      tfdistribute.combinations.tpu_strategy,
-      tfdistribute.combinations.tpu_strategy_one_core,
-      tfdistribute.combinations.tpu_strategy_packed_var,
       # ParameterServerStrategy
       tfdistribute.combinations.parameter_server_strategy_3worker_2ps_cpu,
       tfdistribute.combinations.parameter_server_strategy_3worker_2ps_1gpu,
       tfdistribute.combinations.parameter_server_strategy_1worker_2ps_cpu,
       tfdistribute.combinations.parameter_server_strategy_1worker_2ps_1gpu,
+      # Temporarily disable TPU tests of CL (b/269648832, b/269249455).
+      # tfdistribute.combinations.tpu_strategy,
+      # tfdistribute.combinations.tpu_strategy_one_core,
+      # tfdistribute.combinations.tpu_strategy_packed_var,
+  ]
+  tasklist = [
+      tasks.DeepGraphInfomaxTask("node"),
+      tasks.BarlowTwinsTask("node"),
+      tasks.VicRegTask("node"),
+      # Multi-task: supervised & self-supervised tasks.
+      {
+          "classification": runner.RootNodeMulticlassClassification(
+              "node",
+              num_classes=len(_CLASSES),
+              label_feature_name="classes"),
+          "dgi": tasks.DeepGraphInfomaxTask("node"),
+      },
+      # Multi-task: multiple self-supervised tasks.
+      {
+          "bt": tasks.BarlowTwinsTask("node", representations_layer_name="bt"),
+          "vr": tasks.VicRegTask("node", representations_layer_name="vr"),
+      },
   ]
-  return tftest.combinations.combine(distribution=strategies)
+  return tftest.combinations.combine(distribution=strategies, task=tasklist)
+
+
+def with_readout(gt: tfgnn.GraphTensor) -> tfgnn.GraphTensor:
+  return tfgnn.experimental.context_readout_into_feature(
+      gt,
+      feature_name="classes",
+      remove_input_feature=True)
+
+
+def random_graph_tensor() -> tfgnn.GraphTensor:
+  schema = tfgnn.parse_schema(_SCHEMA)
+  gtspec = tfgnn.create_graph_spec_from_schema_pb(schema)
+  sample_dict = {(tfgnn.CONTEXT, None, "classes"): _CLASSES}
+  return with_readout(tfgnn.random_graph_tensor(gtspec, sample_dict))
 
 
-class DatasetProvider(runner.DatasetProvider):
+class DatasetProviderFromTensors(runner.DatasetProvider):
 
   def __init__(self, elements: Sequence[Any]):
     self._elements = list(elements)
 
   def get_dataset(self, _: tf.distribute.InputContext) -> tf.data.Dataset:
     return tf.data.Dataset.from_tensor_slices(self._elements)
 
 
 # TODO(b/265776928): Consider deduplication of distribute testing boilerplate.
 class DistributeTests(tf.test.TestCase, parameterized.TestCase):
 
-  @tfdistribute.combinations.generate(_all_eager_strategy_combinations())
-  def test_run(self, distribution: tf.distribute.Strategy):
-    schema = tfgnn.parse_schema(_SCHEMA)
-    gtspec = tfgnn.create_graph_spec_from_schema_pb(schema)
-    gts = [tfgnn.random_graph_tensor(gtspec) for _ in range(4)]
+  @tfdistribute.combinations.generate(
+      _all_eager_strategy_and_task_combinations()
+  )
+  def test_run(self, distribution: tf.distribute.Strategy, task: runner.Task):
+    gts = (random_graph_tensor(),) * 4
     serialized = [tfgnn.write_example(gt).SerializeToString() for gt in gts]
-    ds_provider = DatasetProvider(serialized)
+    ds_provider = DatasetProviderFromTensors(serialized)
 
-    node_sets_fn = lambda node_set, node_set_name: node_set["features"]
-    model_fn = runner.ModelFromInitAndUpdates(
-        init=tfgnn.keras.layers.MapFeatures(node_sets_fn=node_sets_fn),
-        updates=[vanilla_mpnn.VanillaMPNNGraphUpdate(
-            units=1,
-            message_dim=2,
-            receiver_tag=tfgnn.SOURCE,
-            l2_regularization=5e-4,
-            dropout_rate=0.1)])
+    def model_fn(graph_tensor_spec):
+      graph = inputs = tf.keras.layers.Input(type_spec=graph_tensor_spec)
+      graph = tfgnn.keras.layers.MapFeatures(
+          node_sets_fn=lambda node_set, node_set_name: node_set["features"]
+      )(graph)
+      graph = vanilla_mpnn.VanillaMPNNGraphUpdate(
+          units=2,
+          message_dim=3,
+          receiver_tag=tfgnn.SOURCE,
+          l2_regularization=5e-4,
+          dropout_rate=0.1)(graph)
+      return tf.keras.Model(inputs, graph)
 
     model_dir = self.create_tempdir()
 
     trainer = runner.KerasTrainer(
         strategy=distribution,
         model_dir=model_dir,
         steps_per_epoch=1,
         validation_steps=1,
         restore_best_weights=False)
 
     if isinstance(distribution, tf.distribute.TPUStrategy):
       train_padding = runner.FitOrSkipPadding(
-          gtspec,
+          gts[0].spec,
           ds_provider,
           fit_or_skip_sample_sample_size=5,
           fit_or_skip_success_ratio=0.7)
-      valid_padding = runner.TightPadding(gtspec, ds_provider)
+      valid_padding = runner.TightPadding(gts[0].spec, ds_provider)
     else:
       train_padding = None
       valid_padding = None
 
     runner.run(
         train_ds_provider=ds_provider,
         train_padding=train_padding,
         model_fn=model_fn,
         optimizer_fn=tf.keras.optimizers.Adam,
         epochs=1,
         trainer=trainer,
-        task=tasks.DeepGraphInfomaxTask("node"),
-        gtspec=gtspec,
+        task=task,
+        gtspec=gts[0].spec,
         global_batch_size=2,
         feature_processors=tuple(),
         valid_ds_provider=ds_provider,
-        valid_padding=valid_padding)
+        valid_padding=valid_padding,
+    )
 
     dataset = ds_provider.get_dataset(tf.distribute.InputContext())
     kwargs = {"examples": next(iter(dataset.batch(2)))}
 
     saved_model = tf.saved_model.load(os.path.join(model_dir, "export"))
 
     results = saved_model.signatures["serving_default"](**kwargs)
-    self.assertLen(results, 1)  # The task has a single output.
+    self.assertLen(results, len(tf.nest.flatten(task)))  # One output per task.
 
-    [result] = results.values()
     # The above distribute test verifies *only* that the `Task` runs under many
     # distribution strategies. Verify here that run and export also produce
     # finite values.
-    self.assertAllInRange(result, result.dtype.min, result.dtype.max)
+    for result in results.values():
+      self.assertAllInRange(result, result.dtype.min, result.dtype.max)
 
 
 if __name__ == "__main__":
   tfdistribute.multi_process_runner.test_main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/BUILD`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,31 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "py_strict_test")
 
 licenses(["notice"])
 
 package(
-    default_visibility = [":__subpackages__"],
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = ["//visibility:public"],
 )
 
-package_group(name = "users")
-
-pytype_strict_library(
-    name = "gat_v2",
-    srcs = ["__init__.py"],
-    srcs_version = "PY3",
-    visibility = [
-        ":__subpackages__",
-        ":users",
-    ],
-    deps = [
-        ":layers",
-    ],
-)
-
-# =============================================================================
-
 pytype_strict_library(
-    name = "layers",
-    srcs = ["layers.py"],
+    name = "datasets",
+    srcs = ["datasets.py"],
     srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
     ],
 )
 
-tf_py_test(
-    name = "layers_test",
-    srcs = ["layers_test.py"],
+py_strict_test(
+    name = "datasets_test",
+    srcs = ["datasets_test.py"],
     python_version = "PY3",
-    srcs_version = "PY3",
     deps = [
-        ":gat_v2",
+        ":datasets",
         "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 
 ```python
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.models import gat_v2
 ```
 """
 
+from tensorflow_gnn.models.gat_v2 import config_dict
 from tensorflow_gnn.models.gat_v2 import layers
 
 GATv2Conv = layers.GATv2Conv
 GATv2EdgePool = layers.GATv2EdgePool
 GATv2GraphUpdate = layers.GATv2GraphUpdate  # Deprecated.
 GATv2HomGraphUpdate = layers.GATv2HomGraphUpdate
 GATv2MPNNGraphUpdate = layers.GATv2MPNNGraphUpdate
+graph_update_get_config_dict = config_dict.graph_update_get_config_dict
+graph_update_from_config_dict = config_dict.graph_update_from_config_dict
 
 # Prune imported module symbols so they're not accessible implicitly.
+del config_dict
 del layers
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,41 +89,43 @@
       node set.
       If left unset for init, the tag must be passed at call time.
     receiver_feature: Can be set to override `tfgnn.HIDDEN_STATE` for use as
       the receiver's input feature to attention. (The attention key is derived
       from this input.)
     sender_node_feature: Can be set to override `tfgnn.HIDDEN_STATE` for use as
       the input feature from sender nodes to attention.
-      IMPORANT: Must be set to `None` for use with `receiver_tag=tfgnn.CONTEXT`
+      IMPORTANT: Must be set to `None` for use with `receiver_tag=tfgnn.CONTEXT`
       on an edge set, or for pooling from edges without sender node states.
     sender_edge_feature: Can be set to a feature name of the edge set to select
       it as an input feature. By default, this set to `None`, which disables
       this input.
       IMPORTANT: Must be set for use with `receiver_tag=tfgnn.CONTEXT`
       on an edge set.
     use_bias: If true, a bias term is added to the transformations of query and
       value inputs.
     edge_dropout: Can be set to a dropout rate for edge dropout. (When pooling
       nodes to context, it's the node's membership in a graph component that
       is dropped out.)
     attention_activation: The nonlinearity used on the transformed inputs
       before multiplying with the trained weights of the attention layer.
       This can be specified as a Keras layer, a tf.keras.activations.*
-      function, or a string understood by tf.keras.layers.Activation().
+      function, or a string understood by `tf.keras.layers.Activation()`.
       Defaults to "leaky_relu", which in turn defaults to a negative slope
       of `alpha=0.2`.
     heads_merge_type: The merge operation for combining output from
       all `num_heads` attention heads. By default, output of heads will be
       concatenated. However, GAT paper (Velickovic et al, Eq 6) recommends *only
       for output layer* to do mean across attention heads, which is acheivable
       by setting to `"mean"`.
     activation: The nonlinearity applied to the final result of attention,
       specified in the same ways as attention_activation.
-    kernel_initializer: Can be set to a `kerner_initializer` as understood
+    kernel_initializer: Can be set to a `kernel_initializer` as understood
       by `tf.keras.layers.Dense` etc.
+      An `Initializer` object gets cloned before use to ensure a fresh seed,
+      if not set explicitly. For more, see `tfgnn.keras.clone_initializer()`.
     kernel_regularizer: If given, will be used to regularize all layer kernels.
   """
 
   def __init__(self,
                *,
                num_heads: int,
                per_head_channels: int,
@@ -134,18 +136,16 @@
                sender_edge_feature: Optional[tfgnn.FieldName] = None,
                use_bias: bool = True,
                edge_dropout: float = 0.,
                attention_activation: Union[str,
                                            Callable[..., Any]] = "leaky_relu",
                heads_merge_type: str = "concat",
                activation: Union[str, Callable[..., Any]] = "relu",
-               kernel_initializer: Union[
-                   None, str, tf.keras.initializers.Initializer] = None,
-               kernel_regularizer: Union[
-                   None, str, tf.keras.regularizers.Regularizer] = None,
+               kernel_initializer: Any = None,
+               kernel_regularizer: Any = None,
                **kwargs):
     kwargs.setdefault("name", "gat_v2_conv")
     super().__init__(
         receiver_tag=receiver_tag,
         receiver_feature=receiver_feature,
         sender_node_feature=sender_node_feature,
         sender_edge_feature=sender_edge_feature,
@@ -171,43 +171,47 @@
     if self._edge_dropout > 0:
       self._edge_dropout_layer = tf.keras.layers.Dropout(self._edge_dropout)
     else:
       self._edge_dropout_layer = None
 
     self._attention_activation = tf.keras.activations.get(attention_activation)
     self._activation = tf.keras.activations.get(activation)
-    self._kernel_initializer = kernel_initializer
+    # IMPORTANT: Use with tfgnn.keras.clone_initializer(), b/268648226.
+    self._kernel_initializer = tf.keras.initializers.get(kernel_initializer)
     self._kernel_regularizer = tf.keras.regularizers.get(kernel_regularizer)
     self._heads_merge_type = heads_merge_type
 
     # Create the transformations for the query input in all heads.
     self._w_query = tf.keras.layers.Dense(
         per_head_channels * num_heads,
-        kernel_initializer=kernel_initializer,
+        kernel_initializer=tfgnn.keras.clone_initializer(
+            self._kernel_initializer),
         # This bias gets added to the attention features but not the outputs.
         use_bias=use_bias,
         kernel_regularizer=kernel_regularizer,
         name="query")
 
     # Create the transformations for value input from sender nodes and edges.
     if self.takes_sender_node_input:
       self._w_sender_node = tf.keras.layers.Dense(
           per_head_channels * num_heads,
-          kernel_initializer=kernel_initializer,
+          kernel_initializer=tfgnn.keras.clone_initializer(
+              self._kernel_initializer),
           # This bias gets added to the attention features and the outputs.
           use_bias=use_bias,
           kernel_regularizer=kernel_regularizer,
           name="value_node")
     else:
       self._w_sender_node = None
 
     if self.takes_sender_edge_input:
       self._w_sender_edge = tf.keras.layers.Dense(
           per_head_channels * num_heads,
-          kernel_initializer=kernel_initializer,
+          kernel_initializer=tfgnn.keras.clone_initializer(
+              self._kernel_initializer),
           # This bias would be redundant with self._w_sender_node.
           use_bias=use_bias and self._w_sender_node is None,
           kernel_regularizer=kernel_regularizer,
           name="value_edge")
     else:
       self._w_sender_edge = None
 
@@ -217,29 +221,33 @@
     # Create attention logits layers, one for each head. Note that we can't
     # use a single Dense layer that outputs `num_heads` units because we need
     # to apply a different attention function a_k to its corresponding
     # W_k-transformed features.
     self._attention_logits_fn = tf.keras.layers.experimental.EinsumDense(
         "...ik,ki->...i",
         output_shape=(None, num_heads, 1),  # TODO(b/205825425): (num_heads,)
-        kernel_initializer=kernel_initializer,
+        kernel_initializer=tfgnn.keras.clone_initializer(
+            self._kernel_initializer),
         kernel_regularizer=kernel_regularizer,
         name="attn_logits")
 
   def get_config(self):
     return dict(
         num_heads=self._num_heads,
         per_head_channels=self._per_head_channels,
         use_bias=self._use_bias,
         edge_dropout=self._edge_dropout,
         heads_merge_type=self._heads_merge_type,
         attention_activation=self._attention_activation,
         activation=self._activation,
-        kernel_initializer=self._kernel_initializer,
-        kernel_regularizer=tf.keras.regularizers.serialize(  # b/238163789.
+        # Regularizers and initializers need explicit serialization here
+        # (and deserialization in __init__ via .get()) due to b/238163789.
+        kernel_initializer=tf.keras.initializers.serialize(
+            self._kernel_initializer),
+        kernel_regularizer=tf.keras.regularizers.serialize(
             self._kernel_regularizer),
         **super().get_config())
 
   def convolve(self, *,
                sender_node_input: Optional[tf.Tensor],
                sender_edge_input: Optional[tf.Tensor],
                receiver_input: Optional[tf.Tensor],
@@ -408,15 +416,15 @@
       receiver_tag=receiver_tag,
       receiver_feature=receiver_feature,
       sender_edge_feature=sender_feature,
       sender_node_feature=None,
       **kwargs)
 
 
-# TODO(b/236941740): a systematic solution for adding loops.
+# TODO(b/286015280): a systematic solution for adding loops.
 def GATv2HomGraphUpdate(
     *,  # To be called like a class initializer.  pylint: disable=invalid-name
     num_heads: int,
     per_head_channels: int,
     receiver_tag: tfgnn.IncidentNodeTag,
     feature_name: str = tfgnn.HIDDEN_STATE,
     heads_merge_type: str = "concat",
@@ -447,18 +455,16 @@
     name: Optionally, a name for the layer returned.
     **kwargs: Any optional arguments to GATv2Conv, see there.
   """
   # Build a GraphUpdate for the target node set of the given edge_set_name.
   # That needs to be deferred until we see a GraphTensorSpec that tells us
   # the node_set_name.
   def deferred_init_callback(spec: tfgnn.GraphTensorSpec):
-    tfgnn.check_homogeneous_graph_tensor(spec, "GATv2HomGraphUpdate")
-    edge_set_name, = spec.edge_sets_spec.keys()
-    node_set_name = spec.edge_sets_spec[
-        edge_set_name].adjacency_spec.node_set_name(receiver_tag)
+    node_set_name, edge_set_name = tfgnn.get_homogeneous_node_and_edge_set_name(
+        spec, "GATv2HomGraphUpdate")
     node_set_updates = {
         node_set_name: tfgnn.keras.layers.NodeSetUpdate(
             {edge_set_name: GATv2Conv(
                 num_heads=num_heads, per_head_channels=per_head_channels,
                 receiver_tag=receiver_tag,
                 sender_node_feature=feature_name, receiver_feature=feature_name,
                 heads_merge_type=heads_merge_type,
@@ -481,31 +487,32 @@
   del edge_set_name  # Must be the only one anyways.
   return GATv2HomGraphUpdate(
       num_heads=num_heads, per_head_channels=per_head_channels,
       receiver_tag=tfgnn.TARGET, feature_name=feature_name, name=name, **kwargs)
 
 
 def GATv2MPNNGraphUpdate(  # To be called like a class initializer.  pylint: disable=invalid-name
+    # LINT.IfChange(GATv2MPNNGraphUpdate_args)
     *,
     units: int,
     message_dim: int,
     num_heads: int,
     heads_merge_type: str = "concat",
     receiver_tag: tfgnn.IncidentNodeTag,
     node_set_names: Optional[Collection[tfgnn.NodeSetName]] = None,
     edge_feature: Optional[tfgnn.FieldName] = None,
     l2_regularization: float = 0.0,
     edge_dropout_rate: float = 0.0,
     state_dropout_rate: float = 0.0,
     attention_activation: Union[str, Callable[..., Any]] = "leaky_relu",
     conv_activation: Union[str, Callable[..., Any]] = "relu",
     activation: Union[str, Callable[..., Any]] = "relu",
-    kernel_initializer: Union[
-        None, str, tf.keras.initializers.Initializer] = "glorot_uniform",
-    ) -> tf.keras.layers.Layer:
+    kernel_initializer: Any = "glorot_uniform",
+    # LINT.ThenChange(./config_dict.py:graph_update_get_config_dict)
+) -> tf.keras.layers.Layer:
   """Returns a GraphUpdate layer for message passing with GATv2 pooling.
 
   The returned layer performs one round of message passing between the nodes
   of a heterogeneous GraphTensor, using `gat_v2.GATv2Conv` to compute the
   messages and their pooling with attention, followed by a dense layer to
   compute the new node states from a concatenation of the old node state and
   all pooled messages.
@@ -529,22 +536,22 @@
       biases.
     edge_dropout_rate: The edge dropout rate applied during attention pooling
       of edges.
     state_dropout_rate: The dropout rate applied to the resulting node states.
     attention_activation: The nonlinearity used on the transformed inputs
       before multiplying with the trained weights of the attention layer.
       This can be specified as a Keras layer, a tf.keras.activations.*
-      function, or a string understood by tf.keras.layers.Activation().
+      function, or a string understood by `tf.keras.layers.Activation()`.
       Defaults to "leaky_relu", which in turn defaults to a negative slope
       of `alpha=0.2`.
     conv_activation: The nonlinearity applied to the result of attention on one
       edge set, specified in the same ways as attention_activation.
     activation: The nonlinearity applied to the new node states computed by
       this graph update.
-    kernel_initializer: Can be set to a `kerner_initializer` as understood
+    kernel_initializer: Can be set to a `kernel_initializer` as understood
       by `tf.keras.layers.Dense` etc.
 
   Returns:
     A GraphUpdate layer for use on a scalar GraphTensor with
     `tfgnn.HIDDEN_STATE` features on the node sets.
   """
   if message_dim % num_heads:
@@ -555,27 +562,28 @@
   regularizer = tf.keras.regularizers.l2(l2_regularization)
   def dense(units):  # pylint: disable=invalid-name
     return tf.keras.Sequential([
         tf.keras.layers.Dense(
             units,
             activation=activation,
             use_bias=True,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                kernel_initializer),
             bias_initializer="zeros",
             kernel_regularizer=regularizer,
             bias_regularizer=regularizer),
         tf.keras.layers.Dropout(state_dropout_rate)])
 
   # pylint: disable=g-long-lambda
   gnn_builder = tfgnn.keras.ConvGNNBuilder(
       lambda edge_set_name, receiver_tag: GATv2Conv(
           num_heads=num_heads, per_head_channels=per_head_channels,
           heads_merge_type=heads_merge_type,
           edge_dropout=edge_dropout_rate, receiver_tag=receiver_tag,
           sender_edge_feature=edge_feature,
           attention_activation=attention_activation, activation=conv_activation,
           kernel_regularizer=regularizer,
-          kernel_initializer=kernel_initializer),
+          kernel_initializer=tfgnn.keras.clone_initializer(kernel_initializer)),
       lambda node_set_name: tfgnn.keras.layers.NextStateFromConcat(
           dense(units)),
       receiver_tag=receiver_tag)
   return gnn_builder.Convolve(node_set_names)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gat_v2/layers_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gat_v2/layers_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.models import gat_v2
 
 
 class ReloadModel(int, enum.Enum):
   """Controls how to reload a model for further testing after saving."""
+
   SKIP = 0
   SAVED_MODEL = 1
   KERAS = 2
 
 
 class GATv2Test(tf.test.TestCase, parameterized.TestCase):
 
@@ -36,508 +37,606 @@
     """Tests that a single-headed GAT is correct given predefined weights."""
     # NOTE: Many following tests use minor variations of the explicit
     # construction of weights and results introduced here.
 
     # Construct a graph with three nodes 0, 1, 2, and six edges:
     # a cycle 0->1->2->0 (let's call it clockwise)
     # and the reverse cycle 0->2->1->0 (counterclockwise).
-    gt_input = _get_test_bidi_cycle_graph(tf.constant(
-        # Node states have dimension 4.
-        # The first three dimensions one-hot encode the node_id i.
-        # The fourth dimension holds a distinct payload value i+1.
-        [[1., 0., 0., 1.],
-         [0., 1., 0., 2.],
-         [0., 0., 1., 3.]]))
+    gt_input = _get_test_bidi_cycle_graph(
+        tf.constant(
+            # Node states have dimension 4.
+            # The first three dimensions one-hot encode the node_id i.
+            # The fourth dimension holds a distinct payload value i+1.
+            [[1.0, 0.0, 0.0, 1.0],
+             [0.0, 1.0, 0.0, 2.0],
+             [0.0, 0.0, 1.0, 3.0]]
+        )
+    )
 
     conv = gat_v2.GATv2Conv(
         num_heads=1,
         per_head_channels=4,
         receiver_tag=tfgnn.TARGET,
-        attention_activation="relu")  # Let's keep it simple.
+        attention_activation="relu",  # Let's keep it simple.
+    )
 
     _ = conv(gt_input, edge_set_name="edges")  # Build weights.
     weights = {v.name: v for v in conv.trainable_weights}
     self.assertLen(weights, 5)
     weights["gat_v2_conv/query/kernel:0"].assign(
         # The space of attention computation of the single head has dimension 4.
         # The last dimension is used only in the key to carry the node's value,
         # multiplied by 11/10.
         # The first three dimensions are used to hand-construct attention scores
         # (see the running example below) that favor the counterclockwise
         # incoming edge over the other. Recall that weight matrices are
         # multiplied from the right onto batched inputs (in rows).
         #
         # For example, the query vector of node 0 is [0, 1, 0, 0], and ...
-        [[0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [1., 0., 0., 0.],
-         [0., 0., 0., 0.]])
+        [
+            [0.0, 1.0, 0.0, 0.0],
+            [0.0, 0.0, 1.0, 0.0],
+            [1.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+        ]
+    )
     weights["gat_v2_conv/value_node/kernel:0"].assign(
         # ... the key vectors of node 1 and 2, resp., are [-1, 0, -1, 2.2]
         # and [-1, -1, 0, 3.3]. Therefore, ...
-        [[0., -1., -1., 0.],
-         [-1., 0., -1., 0.],
-         [-1., -1., 0., 0.],
-         [0., 0., 0., 1.1]])
-    log10 = tf.math.log(10.).numpy()
+        [
+            [0.0, -1.0, -1.0, 0.0],
+            [-1.0, 0.0, -1.0, 0.0],
+            [-1.0, -1.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 1.1],
+        ]
+    )
+    log10 = tf.math.log(10.0).numpy()
     weights["gat_v2_conv/attn_logits/kernel:0"].assign(
         # ... attention from node 0 to node 1 has a sum of key and query vector
         # [-1, 1, -1, 2.2], which gets turned by ReLU and the attention weights
         # below into a pre-softmax score of log(10). Likewise,
         # attention from node 0 to node 2 has a vector sum [-1, 0, 0, 3.3]
         # and pre-softmax score of 0. Altogether, this means: ...
-        [[log10], [log10], [log10], [0.]])
-    weights["gat_v2_conv/query/bias:0"].assign([0., 0., 0., 0.])
-    weights["gat_v2_conv/value_node/bias:0"].assign([0., 0., 0., 0.])
+        [[log10], [log10], [log10], [0.0]]
+    )
+    weights["gat_v2_conv/query/bias:0"].assign([0.0, 0.0, 0.0, 0.0])
+    weights["gat_v2_conv/value_node/bias:0"].assign([0.0, 0.0, 0.0, 0.0])
 
     got = conv(gt_input, edge_set_name="edges")
 
     # ... The softmax-weighed key vectors on the incoming edges of node 0
     # are  10/11 * [-1, 0, -1, 2.2]  +  1/11 * [-1, -1, 0, 3.3].
     # The final ReLU takes out the non-positive components and leaves 2 + 0.3
     # in the last component of the first row in the resulting node states.
-    want = tf.constant([[0., 0., 0., 2.3],  # Node 0.
-                        [0., 0., 0., 3.1],  # Node 1.
-                        [0., 0., 0., 1.2]])  # Node 2.
+    want = tf.constant([
+        [0.0, 0.0, 0.0, 2.3],  # Node 0.
+        [0.0, 0.0, 0.0, 3.1],  # Node 1.
+        [0.0, 0.0, 0.0, 1.2],
+    ])  # Node 2.
     self.assertAllEqual(got.shape, (3, 4))
-    self.assertAllClose(got, want, atol=.0001)
+    self.assertAllClose(got, want, atol=0.0001)
 
     # For node states with more than one feature dimension, GATv2 works in
     # parallel on the vectors from the innermost dimension, so we can repeat the
     # previous computation and an alternative with different values in the last
     # component and reversed orientation:
-    gt_input_2 = _get_test_bidi_cycle_graph(tf.constant(
-        [[[1., 0., 0., 1.], [0., 0., 1., 3.]],
-         [[0., 1., 0., 2.], [0., 1., 0., 6.]],
-         [[0., 0., 1., 3.], [1., 0., 0., 9.]]]))
+    gt_input_2 = _get_test_bidi_cycle_graph(
+        tf.constant([
+            [[1.0, 0.0, 0.0, 1.0], [0.0, 0.0, 1.0, 3.0]],
+            [[0.0, 1.0, 0.0, 2.0], [0.0, 1.0, 0.0, 6.0]],
+            [[0.0, 0.0, 1.0, 3.0], [1.0, 0.0, 0.0, 9.0]],
+        ])
+    )
     got_2 = conv(gt_input_2, edge_set_name="edges")
-    want_2 = tf.constant([[[0., 0., 0., 2.3], [0., 0., 0., 9.6]],
-                          [[0., 0., 0., 3.1], [0., 0., 0., 3.9]],
-                          [[0., 0., 0., 1.2], [0., 0., 0., 6.3]]])
+    want_2 = tf.constant([
+        [[0.0, 0.0, 0.0, 2.3], [0.0, 0.0, 0.0, 9.6]],
+        [[0.0, 0.0, 0.0, 3.1], [0.0, 0.0, 0.0, 3.9]],
+        [[0.0, 0.0, 0.0, 1.2], [0.0, 0.0, 0.0, 6.3]],
+    ])
     self.assertAllEqual(got_2.shape, (3, 2, 4))
-    self.assertAllClose(got_2, want_2, atol=.0001)
+    self.assertAllClose(got_2, want_2, atol=0.0001)
 
   @parameterized.named_parameters(
-      ("ConcatMerge", "concat"),
-      ("MeanMerge", "mean"))
+      ("ConcatMerge", "concat"), ("MeanMerge", "mean")
+  )
   def testMultihead(self, merge_type):
     """Extends testBasic with multiple attention heads."""
     # The same test graph as in the testBasic above.
-    gt_input = _get_test_bidi_cycle_graph(tf.constant(
-        [[1., 0., 0., 1.],
-         [0., 1., 0., -2.],
-         [0., 0., 1., 3.]]))
+    gt_input = _get_test_bidi_cycle_graph(
+        tf.constant(
+            [[1.0, 0.0, 0.0, 1.0],
+             [0.0, 1.0, 0.0, -2.0],
+             [0.0, 0.0, 1.0, 3.0]]
+        )
+    )
 
     conv = gat_v2.GATv2Conv(
         num_heads=2,
         per_head_channels=4,
         receiver_tag=tfgnn.TARGET,
         attention_activation=tf.keras.layers.LeakyReLU(alpha=0.0),
         use_bias=False,  # Don't create /bias variables.
-        heads_merge_type=merge_type)
+        heads_merge_type=merge_type,
+    )
 
     _ = conv(gt_input, edge_set_name="edges")  # Build weights.
     weights = {v.name: v for v in conv.trainable_weights}
     self.assertLen(weights, 3)
 
     weights["gat_v2_conv/query/kernel:0"].assign(
         # Attention head 0 uses the first four dimensions, which are used
         # in the same way as for the testBasic test above.
         # Attention head 1 uses the last four dimensions, in which we
         # now favor the clockwise incoming edges and omit the scaling by 11/10.
-        [[0., 1., 0., 0., 0., 0., 1., 0,],
-         [0., 0., 1., 0., 1., 0., 0., 0.],
-         [1., 0., 0., 0., 0., 1., 0., 0.],
-         [0., 0., 0., 0., 0., 0., 0., 0.]])
-    weights["gat_v2_conv/value_node/kernel:0"].assign(
-        [[0., -1., -1., 0., 0., -1., -1., 0.],
-         [-1., 0., -1., 0., -1., 0., -1., 0.],
-         [-1., -1., 0., 0., -1., -1., 0., 0.],
-         [0., 0., 0., 1.1, 0., 0., 0., 1.]])
-    log10 = tf.math.log(10.).numpy()
+        [
+            [0.0, 1.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0],
+            [0.0, 0.0, 1.0, 0.0, 1.0, 0.0, 0.0, 0.0],
+            [1.0, 0.0, 0.0, 0.0, 0.0, 1.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
+        ]
+    )
+    weights["gat_v2_conv/value_node/kernel:0"].assign([
+        [0.0, -1.0, -1.0, 0.0, 0.0, -1.0, -1.0, 0.0],
+        [-1.0, 0.0, -1.0, 0.0, -1.0, 0.0, -1.0, 0.0],
+        [-1.0, -1.0, 0.0, 0.0, -1.0, -1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.1, 0.0, 0.0, 0.0, 1.0],
+    ])
+    log10 = tf.math.log(10.0).numpy()
     weights["gat_v2_conv/attn_logits/kernel:0"].assign(
         # Attention head 0 works out to softmax weights 10/11 and 1/11 as above.
         # Attention head 1 creates very large pre-softmax scores that
         # work out to weights 1 and 0 within floating-point precision.
-        [[log10, 100.],
-         [log10, 100.],
-         [log10, 100.],
-         [0., 0.]])
+        [[log10, 100.0], [log10, 100.0], [log10, 100.0], [0.0, 0.0]]
+    )
 
     got = conv(gt_input, edge_set_name="edges")
 
     # Attention head 0 generates the first four output dimensions as in the
     # testBasic above, with weights 10/11 and 1/11,
     # Attention head 1 uses weights 0 and 1 (note the reversed preference).
-    want_logits = tf.constant([[0., 0., 0., -2+.3, 0., 0., 0., 3.0],
-                               [0., 0., 0., 3+.1, 0., 0., 0., 1.0],
-                               [0., 0., 0., 1-.2, 0., 0., 0., -2.0]])
+    want_logits = tf.constant([
+        [0.0, 0.0, 0.0, -2 + 0.3, 0.0, 0.0, 0.0, 3.0],
+        [0.0, 0.0, 0.0, 3 + 0.1, 0.0, 0.0, 0.0, 1.0],
+        [0.0, 0.0, 0.0, 1 - 0.2, 0.0, 0.0, 0.0, -2.0],
+    ])
 
     if merge_type == "mean":
       # Expect mean of heads, followed by activation.
       want = tf.nn.relu((want_logits[:, :4] + want_logits[:, 4:]) / 2)
     elif merge_type == "concat":
       want = tf.nn.relu(want_logits)
 
-    self.assertAllClose(got, want, atol=.0001)
+    self.assertAllClose(got, want, atol=0.0001)
 
   @parameterized.named_parameters(
       ("", ReloadModel.SKIP),
       ("Restored", ReloadModel.SAVED_MODEL),
-      ("RestoredKeras", ReloadModel.KERAS))
+      ("RestoredKeras", ReloadModel.KERAS),
+  )
   def testFullModel(self, reload_model):
     """Tests GATv2HomGraphUpdate in Model (incl. saving) with edge input."""
     # The same example as in the testBasic above, but with extra inputs
     # from edges.
     gt_input = _get_test_bidi_cycle_graph(
         # Node i has value i+1 in the last component, which will be mapped
         # into the fourth component of the value.
-        tf.constant(
-            [[1., 0., 0., 1.],  # Node 0.
-             [0., 1., 0., 2.],  # Node 1.
-             [0., 0., 1., 3.]]),  # Node 2.
+        tf.constant([
+            [1.0, 0.0, 0.0, 1.0],  # Node 0.
+            [0.0, 1.0, 0.0, 2.0],  # Node 1.
+            [0.0, 0.0, 1.0, 3.0],  # Node 2.
+        ]),
         # Edges out of node i have value 2*(i+1) for the clockwise edges favored
         # by attention and 3*(i+1) for the counterclockwise edges not favored.
-        tf.constant(
-            [[3.],  # Edge from node 0 (clockwise, not favored).
-             [6.],  # Edge from node 1 (clockwise, not favored).
-             [9.],  # Edge from node 2 (clockwise, not favored).
-             [2.],  # Edge from node 0 (counterclockwise, favored).
-             [6.],  # Edge from node 2 (counterclockwise, favored).
-             [4.]]))  # Edge from node 1 (counterclockwise, favored).
+        tf.constant([
+            [3.0],  # Edge from node 0 (clockwise, not favored).
+            [6.0],  # Edge from node 1 (clockwise, not favored).
+            [9.0],  # Edge from node 2 (clockwise, not favored).
+            [2.0],  # Edge from node 0 (counterclockwise, favored).
+            [6.0],  # Edge from node 2 (counterclockwise, favored).
+            [4.0],  # Edge from node 1 (counterclockwise, favored).
+        ]),
+    )
 
     l2reg = 1e-2
     layer = gat_v2.GATv2HomGraphUpdate(
         num_heads=1,
         per_head_channels=5,
         receiver_tag=tfgnn.TARGET,
         sender_edge_feature=tfgnn.HIDDEN_STATE,  # Activate edge input.
         kernel_regularizer=tf.keras.regularizers.l2(l2reg),
-        attention_activation="relu")
+        # Test with a non-None initializer for b/238163789.
+        kernel_initializer=tf.keras.initializers.GlorotNormal(),
+        attention_activation="relu",
+    )
 
     _ = layer(gt_input)  # Build weights.
     weights = {v.name: v for v in layer.trainable_weights}
     self.assertLen(weights, 6)
     weights["gat_v2/node_set_update/gat_v2_conv/value_edge/kernel:0"].assign(
         # Edge values are put into a new final component of the value space,
         # with the same adjustment for softmax-weighting by 1/11 or 10/11.
-        [[0., 0., 0., 0., 1.1]])
-    weights["gat_v2/node_set_update/gat_v2_conv/query/kernel:0"].assign(
-        [[0., 1., 0., 0., 0.],
-         [0., 0., 1., 0., 0.],
-         [1., 0., 0., 0., 0.],
-         [0., 0., 0., 0., 0.]])
-    weights["gat_v2/node_set_update/gat_v2_conv/value_node/kernel:0"].assign(
-        [[0., -1., -1., 0., 0.],
-         [-1., 0., -1., 0., 0.],
-         [-1., -1., 0., 0., 0.],
-         [0., 0., 0., 1.1, 0.]])
-    log10 = tf.math.log(10.).numpy()
+        [[0.0, 0.0, 0.0, 0.0, 1.1]]
+    )
+    weights["gat_v2/node_set_update/gat_v2_conv/query/kernel:0"].assign([
+        [0.0, 1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0, 0.0],
+    ])
+    weights["gat_v2/node_set_update/gat_v2_conv/value_node/kernel:0"].assign([
+        [0.0, -1.0, -1.0, 0.0, 0.0],
+        [-1.0, 0.0, -1.0, 0.0, 0.0],
+        [-1.0, -1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.1, 0.0],
+    ])
+    log10 = tf.math.log(10.0).numpy()
     weights["gat_v2/node_set_update/gat_v2_conv/attn_logits/kernel:0"].assign(
-        [[log10], [log10], [log10], [0.], [0.]])
+        [[log10], [log10], [log10], [0.0], [0.0]]
+    )
     weights["gat_v2/node_set_update/gat_v2_conv/query/bias:0"].assign(
-        [0., 0., 0., 0., 0.])
+        [0.0, 0.0, 0.0, 0.0, 0.0]
+    )
     # NOTE: There is value_node/bias but no redundant value_edge/bias.
     weights["gat_v2/node_set_update/gat_v2_conv/value_node/bias:0"].assign(
-        [0., 0., 0., 0., 0.])
+        [0.0, 0.0, 0.0, 0.0, 0.0]
+    )
 
     # Build a Model around the Layer, possibly saved and restored.
     inputs = tf.keras.layers.Input(type_spec=gt_input.spec)
     outputs = layer(inputs)
     model = tf.keras.Model(inputs, outputs)
 
     if reload_model:
       export_dir = os.path.join(self.get_temp_dir(), "edge-input-model")
       model.save(export_dir, include_optimizer=False)
       if reload_model == ReloadModel.KERAS:
         model = tf.keras.models.load_model(export_dir)
         # Check that from_config() worked, no fallback to a function trace, see
         # https://www.tensorflow.org/guide/keras/save_and_serialize#how_savedmodel_handles_custom_objects
-        self.assertIsInstance(model.get_layer(index=1),
-                              tfgnn.keras.layers.GraphUpdate)
+        self.assertIsInstance(
+            model.get_layer(index=1), tfgnn.keras.layers.GraphUpdate
+        )
       else:
         model = tf.saved_model.load(export_dir)  # Gives _UserObject
 
     got_gt = model(gt_input)
     got = got_gt.node_sets["nodes"][tfgnn.HIDDEN_STATE]
 
     # Verify kernel regularization is attached on model kernel variables.
     if not reload_model or reload_model == ReloadModel.KERAS:
       # Model.losses only works on Keras models. tf.saved_model.load(), however,
       # does not return a Keras model. See:
       # https://www.tensorflow.org/api_docs/python/tf/saved_model/load
-      kernel_variables = [v for v in model.trainable_variables
-                          if "/kernel:0" in v.name]
+      kernel_variables = [
+          v for v in model.trainable_variables if "/kernel:0" in v.name
+      ]
       self.assertLen(kernel_variables, 4)  # 4 kernel variables per `weights[]`.
-      self.assertLen(model.losses, 4)      # One loss term per kernel variable.
-      expected_model_losses = [tf.reduce_sum(v ** 2) * l2reg
-                               for v in kernel_variables]
+      self.assertLen(model.losses, 4)  # One loss term per kernel variable.
+      expected_model_losses = [
+          tf.reduce_sum(v**2) * l2reg for v in kernel_variables
+      ]
       self.assertAllClose(model.losses, expected_model_losses)
 
     # The fourth column with values x.y from nodes is analogous to the
     # testBasic test above, with the contribution x from the favored
     # input before the decimal dot and the other contribution y after.
     # The fifth column with values (2x).(3y) is from edges, with the
     # multipliers 2 and 3 used above in setting up the edge features.
-    want = tf.constant([[0., 0., 0., 2.3, 4.9],
-                        [0., 0., 0., 3.1, 6.3],
-                        [0., 0., 0., 1.2, 2.6]])
+    want = tf.constant([
+        [0.0, 0.0, 0.0, 2.3, 4.9],
+        [0.0, 0.0, 0.0, 3.1, 6.3],
+        [0.0, 0.0, 0.0, 1.2, 2.6],
+    ])
     self.assertAllEqual(got.shape, (3, 5))
-    self.assertAllClose(got, want, atol=.0001)
+    self.assertAllClose(got, want, atol=0.0001)
 
   def testConvolutionReceivers(self):
     """Tests convolution to context and equivalence to a special node set."""
 
     # An example graph with two components:
     # The first component has the example from testBasic split into a "sources"
     # node set with the first two nodes and a "targets" node set with the third
     # node and a context feature equal to the target node.
     # The second component repeats that construction, but with a variation in
     # the value of the target node / context.
     gt_input = tfgnn.GraphTensor.from_pieces(
         node_sets={
             "sources": tfgnn.NodeSet.from_fields(
                 sizes=[2, 2],
-                features={tfgnn.HIDDEN_STATE: tf.constant(
-                    [[1., 0., 0., 1.],
-                     [0., 1., 0., 2.]] * 2)}),  # Repeated for both components.
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant(
+                        [[1.0, 0.0, 0.0, 1.0],  # Repeated for both components.
+                         [0.0, 1.0, 0.0, 2.0]] * 2
+                    )
+                },
+            ),
             "targets": tfgnn.NodeSet.from_fields(
                 sizes=[1, 1],
-                features={tfgnn.HIDDEN_STATE: tf.constant(
-                    [[0., 0., 1., 3.],
-                     [1., 0., 0., 4.]])}),
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant(
+                        [[0.0, 0.0, 1.0, 3.0], [1.0, 0.0, 0.0, 4.0]]
+                    )
+                },
+            ),
         },
         context=tfgnn.Context.from_fields(
             # Same as "targets".
-            features={tfgnn.HIDDEN_STATE: tf.constant(
-                [[0., 0., 1., 3.],
-                 [1., 0., 0., 4.]])}),
+            features={
+                tfgnn.HIDDEN_STATE: tf.constant(
+                    [[0.0, 0.0, 1.0, 3.0], [1.0, 0.0, 0.0, 4.0]]
+                )
+            }
+        ),
         edge_sets={
             "edges": tfgnn.EdgeSet.from_fields(
                 sizes=[2, 2],
                 # Same as membership of "sources" in components.
                 adjacency=tfgnn.Adjacency.from_indices(
                     ("sources", tf.constant([0, 1, 2, 3])),
-                    ("targets", tf.constant([0, 0, 1, 1]))))
-        })
+                    ("targets", tf.constant([0, 0, 1, 1])),
+                ),
+            )
+        },
+    )
 
     conv = gat_v2.GATv2Conv(
         num_heads=1,
         per_head_channels=4,
         attention_activation="relu",
-        use_bias=False)
+        use_bias=False,
+    )
 
     # Build weights, then initialize as in testBasic.
     _ = conv(gt_input, node_set_name="sources", receiver_tag=tfgnn.CONTEXT)
     weights = {v.name: v for v in conv.trainable_weights}
     self.assertLen(weights, 3)
-    weights["gat_v2_conv/query/kernel:0"].assign(
-        [[0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [1., 0., 0., 0.],
-         [0., 0., 0., 0.]])
-    weights["gat_v2_conv/value_node/kernel:0"].assign(
-        [[0., -1., -1., 0.],
-         [-1., 0., -1., 0.],
-         [-1., -1., 0., 0.],
-         [0., 0., 0., 1.1]])
-    log10 = tf.math.log(10.).numpy()
+    weights["gat_v2_conv/query/kernel:0"].assign([
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0],
+    ])
+    weights["gat_v2_conv/value_node/kernel:0"].assign([
+        [0.0, -1.0, -1.0, 0.0],
+        [-1.0, 0.0, -1.0, 0.0],
+        [-1.0, -1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.1],
+    ])
+    log10 = tf.math.log(10.0).numpy()
     weights["gat_v2_conv/attn_logits/kernel:0"].assign(
-        [[log10], [log10], [log10], [0.]])
+        [[log10], [log10], [log10], [0.0]]
+    )
 
     # The convolution object can be called interchangeably for convolving
     # "sources" to context, or along "edges" to "targets" with the same
     # features as context.
-    got_context = conv(gt_input, node_set_name="sources",
-                       receiver_tag=tfgnn.CONTEXT)
-    got_targets = conv(gt_input, edge_set_name="edges",
-                       receiver_tag=tfgnn.TARGET)
-    want = tf.constant([[0., 0., 0., 1.2],  # As in testBasic for node 2.
-                        [0., 0., 0., 2.1]])  # Opposite preference.
-    self.assertAllClose(got_context, want, atol=.0001)
-    self.assertAllClose(got_targets, want, atol=.0001)
+    got_context = conv(
+        gt_input, node_set_name="sources", receiver_tag=tfgnn.CONTEXT
+    )
+    got_targets = conv(
+        gt_input, edge_set_name="edges", receiver_tag=tfgnn.TARGET
+    )
+    want = tf.constant([
+        [0.0, 0.0, 0.0, 1.2],  # As in testBasic for node 2.
+        [0.0, 0.0, 0.0, 2.1],  # Opposite preference.
+    ])
+    self.assertAllClose(got_context, want, atol=0.0001)
+    self.assertAllClose(got_targets, want, atol=0.0001)
 
     # The same object can even be used for convolving over the edge set in
     # reverse direction, that is, to "sources". The result is boring, though:
     # Every "source" gets the same value from the sole "target" of the component
     # (so softmax reduces to a no-op), which is scaled with 1.1 by the
     # bottom-right element of value_node/kernel.
-    got_sources = conv(gt_input, edge_set_name="edges",
-                       receiver_tag=tfgnn.SOURCE)
-    want_sources = tf.constant([[0., 0., 0., 3.3],
-                                [0., 0., 0., 3.3],
-                                [0., 0., 0., 4.4],
-                                [0., 0., 0., 4.4]])
-    self.assertAllClose(got_sources, want_sources, atol=.0001)
+    got_sources = conv(
+        gt_input, edge_set_name="edges", receiver_tag=tfgnn.SOURCE
+    )
+    want_sources = tf.constant([
+        [0.0, 0.0, 0.0, 3.3],
+        [0.0, 0.0, 0.0, 3.3],
+        [0.0, 0.0, 0.0, 4.4],
+        [0.0, 0.0, 0.0, 4.4],
+    ])
+    self.assertAllClose(got_sources, want_sources, atol=0.0001)
 
   def testEdgePoolReceivers(self):
     """Tests GATv2EdgePool for pooling to nodes and to context."""
     # This example is similar to testConvolutionReceivers, except that
     # the sender features are now on the edges, not the source nodes.
     gt_input = tfgnn.GraphTensor.from_pieces(
         edge_sets={
             "edges": tfgnn.EdgeSet.from_fields(
                 sizes=[2, 2],
                 adjacency=tfgnn.Adjacency.from_indices(
                     ("sources", tf.constant([0, 1, 2, 3])),
-                    ("targets", tf.constant([0, 0, 1, 1]))),
-                features={tfgnn.HIDDEN_STATE: tf.constant(
-                    [[1., 0., 0., 1.],
-                     [0., 1., 0., 2.]] * 2)}),  # Repeated for both components.
+                    ("targets", tf.constant([0, 0, 1, 1])),
+                ),
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant(
+                        [[1.0, 0.0, 0.0, 1.0], [0.0, 1.0, 0.0, 2.0]] * 2
+                    )
+                },
+            ),  # Repeated for both components.
         },
         node_sets={
-            "sources": tfgnn.NodeSet.from_fields(
-                sizes=[2, 2]),  # No features.
+            "sources": tfgnn.NodeSet.from_fields(sizes=[2, 2]),  # No features.
             "targets": tfgnn.NodeSet.from_fields(
                 sizes=[1, 1],
-                features={tfgnn.HIDDEN_STATE: tf.constant(
-                    [[0., 0., 1., 3.],
-                     [1., 0., 0., 4.]])}),
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant(
+                        [[0.0, 0.0, 1.0, 3.0], [1.0, 0.0, 0.0, 4.0]]
+                    )
+                },
+            ),
         },
         context=tfgnn.Context.from_fields(
             # Same as "targets".
-            features={tfgnn.HIDDEN_STATE: tf.constant(
-                [[0., 0., 1., 3.],
-                 [1., 0., 0., 4.]])}))
+            features={
+                tfgnn.HIDDEN_STATE: tf.constant(
+                    [[0.0, 0.0, 1.0, 3.0], [1.0, 0.0, 0.0, 4.0]]
+                )
+            }
+        ),
+    )
 
     layer = gat_v2.GATv2EdgePool(
-        num_heads=1,
-        per_head_channels=4,
-        attention_activation="relu")
+        num_heads=1, per_head_channels=4, attention_activation="relu"
+    )
 
     # Build weights, then initialize analogous to testConvolutionReceivers,
     # with "value_edge" instead of "value_node".
     _ = layer(gt_input, edge_set_name="edges", receiver_tag=tfgnn.CONTEXT)
     weights = {v.name: v for v in layer.trainable_weights}
     self.assertLen(weights, 5)
-    weights["gat_v2_edge_pool/query/kernel:0"].assign(
-        [[0., 1., 0., 0.],
-         [0., 0., 1., 0.],
-         [1., 0., 0., 0.],
-         [0., 0., 0., 0.]])
-    weights["gat_v2_edge_pool/value_edge/kernel:0"].assign(
-        [[0., -1., -1., 0.],
-         [-1., 0., -1., 0.],
-         [-1., -1., 0., 0.],
-         [0., 0., 0., 1.1]])
-    log10 = tf.math.log(10.).numpy()
+    weights["gat_v2_edge_pool/query/kernel:0"].assign([
+        [0.0, 1.0, 0.0, 0.0],
+        [0.0, 0.0, 1.0, 0.0],
+        [1.0, 0.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 0.0],
+    ])
+    weights["gat_v2_edge_pool/value_edge/kernel:0"].assign([
+        [0.0, -1.0, -1.0, 0.0],
+        [-1.0, 0.0, -1.0, 0.0],
+        [-1.0, -1.0, 0.0, 0.0],
+        [0.0, 0.0, 0.0, 1.1],
+    ])
+    log10 = tf.math.log(10.0).numpy()
     weights["gat_v2_edge_pool/attn_logits/kernel:0"].assign(
-        [[log10], [log10], [log10], [0.]])
-    weights["gat_v2_edge_pool/query/bias:0"].assign([0., 0., 0., 0.])
+        [[log10], [log10], [log10], [0.0]]
+    )
+    weights["gat_v2_edge_pool/query/bias:0"].assign([0.0, 0.0, 0.0, 0.0])
     # NOTE: There is a value_edge/bias but not value_node/bias.
-    weights["gat_v2_edge_pool/value_edge/bias:0"].assign([0., 0., 0., 0.])
+    weights["gat_v2_edge_pool/value_edge/bias:0"].assign([0.0, 0.0, 0.0, 0.0])
 
     # The EdgePool object can be called interchangeably for attention-pooling
     # the "edges" to context or to each component's unique node in "targets".
-    got_context = layer(gt_input, edge_set_name="edges",
-                        receiver_tag=tfgnn.CONTEXT)
-    got_targets = layer(gt_input, edge_set_name="edges",
-                        receiver_tag=tfgnn.TARGET)
-    want = tf.constant([[0., 0., 0., 1.2],
-                        [0., 0., 0., 2.1]])
-    self.assertAllClose(got_context, want, atol=.0001)
-    self.assertAllClose(got_targets, want, atol=.0001)
+    got_context = layer(
+        gt_input, edge_set_name="edges", receiver_tag=tfgnn.CONTEXT
+    )
+    got_targets = layer(
+        gt_input, edge_set_name="edges", receiver_tag=tfgnn.TARGET
+    )
+    want = tf.constant([[0.0, 0.0, 0.0, 1.2], [0.0, 0.0, 0.0, 2.1]])
+    self.assertAllClose(got_context, want, atol=0.0001)
+    self.assertAllClose(got_targets, want, atol=0.0001)
 
   @parameterized.named_parameters(
       ("", ReloadModel.SKIP),
       ("Restored", ReloadModel.SAVED_MODEL),
-      ("RestoredKeras", ReloadModel.KERAS))
+      ("RestoredKeras", ReloadModel.KERAS),
+  )
   def testEdgeDropout(self, reload_model):
     """Tests dropout, esp. the switch between training and inference modes."""
     # Avoid flakiness.
     tf.random.set_seed(42)
 
     # This test graph has many source nodes feeding into one target node.
     # The node features are a one-hot encoding of node ids.
     num_nodes = 32
     target_node_id = 7
     gt_input = tfgnn.GraphTensor.from_pieces(
         node_sets={
             "nodes": tfgnn.NodeSet.from_fields(
                 sizes=[num_nodes],
-                features={tfgnn.HIDDEN_STATE: tf.eye(num_nodes)}),
+                features={tfgnn.HIDDEN_STATE: tf.eye(num_nodes)},
+            ),
         },
         edge_sets={
             "edges": tfgnn.EdgeSet.from_fields(
                 sizes=[num_nodes],
                 adjacency=tfgnn.Adjacency.from_indices(
                     ("nodes", tf.constant(list(range(num_nodes)))),
-                    ("nodes", tf.constant([target_node_id] * num_nodes))))
-        })
+                    ("nodes", tf.constant([target_node_id] * num_nodes)),
+                ),
+            )
+        },
+    )
 
     # On purpose, this test is not for GATv2Conv directly, but for its
     # common usage in a GraphUpdate, to make sure the training/inference mode
     # is propagated correctly.
     layer = gat_v2.GATv2HomGraphUpdate(
         num_heads=1,
         per_head_channels=num_nodes,
         receiver_tag=tfgnn.TARGET,
-        edge_dropout=1./3.,  # Note here.
+        edge_dropout=1.0 / 3.0,  # Note here.
         activation="linear",
         attention_activation="linear",
-        use_bias=False)
+        use_bias=False,
+    )
 
     _ = layer(gt_input)  # Build weights.
     weights = {v.name: v for v in layer.trainable_weights}
     self.assertLen(weights, 3)
     # Set up equal attention to all inputs.
     weights["gat_v2/node_set_update/gat_v2_conv/query/kernel:0"].assign(
-        [[0.] * num_nodes] * num_nodes)
+        [[0.0] * num_nodes] * num_nodes
+    )
     weights["gat_v2/node_set_update/gat_v2_conv/attn_logits/kernel:0"].assign(
-        [[0.]] * num_nodes)
+        [[0.0]] * num_nodes
+    )
     # Values are one-hot node ids, scaled up to undo the softmax normalization.
     weights["gat_v2/node_set_update/gat_v2_conv/value_node/kernel:0"].assign(
-        num_nodes * tf.eye(num_nodes))
+        num_nodes * tf.eye(num_nodes)
+    )
 
     # Build a Model around the Layer, possibly saved and restored.
     inputs = tf.keras.layers.Input(type_spec=gt_input.spec)
     outputs = layer(inputs)
     model = tf.keras.Model(inputs, outputs)
     if reload_model:
       export_dir = os.path.join(self.get_temp_dir(), "dropout-model")
       model.save(export_dir, include_optimizer=False)
       if reload_model == ReloadModel.KERAS:
         model = tf.keras.models.load_model(export_dir)
         # Check that from_config() worked, no fallback to a function trace, see
         # https://www.tensorflow.org/guide/keras/save_and_serialize#how_savedmodel_handles_custom_objects
-        self.assertIsInstance(model.get_layer(index=1),
-                              tfgnn.keras.layers.GraphUpdate)
+        self.assertIsInstance(
+            model.get_layer(index=1), tfgnn.keras.layers.GraphUpdate
+        )
       else:
         model = tf.saved_model.load(export_dir)
 
     # The output is a one-hot encoding of the nodes that have been attended to.
     # For inference without dropout, it's an all-ones vector, so min = max = 1.
     # For training with dropout rate 1/3, there are some zeros (for dropped-out
     # edges) and some entries with value 3/2 (for kept edges, such that the
     # expected value remains at (1-1/3) * 3/2 == 1), so min = 0 and max = 1.5.
     def min_max(**kwargs):
       got_gt = model(gt_input, **kwargs)
       got = got_gt.node_sets["nodes"][tfgnn.HIDDEN_STATE][target_node_id]
       return [tf.reduce_min(got), tf.reduce_max(got)]
-    self.assertAllEqual(min_max(), [1., 1.])  # Inference is the default.
-    self.assertAllEqual(min_max(training=False), [1., 1.])
-    self.assertAllClose(min_max(training=True), [0., 1.5])
+
+    self.assertAllEqual(min_max(), [1.0, 1.0])  # Inference is the default.
+    self.assertAllEqual(min_max(training=False), [1.0, 1.0])
+    self.assertAllClose(min_max(training=True), [0.0, 1.5])
 
 
 def _get_test_bidi_cycle_graph(node_state, edge_state=None):
   return tfgnn.GraphTensor.from_pieces(
       node_sets={
           "nodes": tfgnn.NodeSet.from_fields(
-              sizes=[3],
-              features={tfgnn.HIDDEN_STATE: node_state}),
+              sizes=[3], features={tfgnn.HIDDEN_STATE: node_state}
+          ),
       },
       edge_sets={
           "edges": tfgnn.EdgeSet.from_fields(
               sizes=[6],
               adjacency=tfgnn.Adjacency.from_indices(
                   ("nodes", tf.constant([0, 1, 2, 0, 2, 1])),
-                  ("nodes", tf.constant([1, 2, 0, 2, 1, 0]))),
-              features=(None if edge_state is None else
-                        {tfgnn.HIDDEN_STATE: edge_state})),
-      })
+                  ("nodes", tf.constant([1, 2, 0, 2, 1, 0])),
+              ),
+              features=(
+                  None
+                  if edge_state is None
+                  else {tfgnn.HIDDEN_STATE: edge_state}
+              ),
+          ),
+      },
+  )
 
 
 # The components of GATv2MPNNGraphUpdate have been tested elsewhere.
 class GATv2MPNNGraphUpdateTest(tf.test.TestCase, parameterized.TestCase):
 
   def testBasic(self):
     input_graph = _make_test_graph_abc()
@@ -545,53 +644,153 @@
     layer = gat_v2.GATv2MPNNGraphUpdate(
         units=1,
         message_dim=message_dim,
         num_heads=2,
         receiver_tag=tfgnn.TARGET,
         node_set_names=["b"],
         edge_feature="fab",
-        kernel_initializer="ones")
+        kernel_initializer="ones",
+    )
     graph = layer(input_graph)
     # Nodes "a" and "c" are unchanged.
-    self.assertAllEqual([[1.]], graph.node_sets["a"][tfgnn.HIDDEN_STATE])
-    self.assertAllEqual([[8.]], graph.node_sets["c"][tfgnn.HIDDEN_STATE])
+    self.assertAllEqual([[1.0]], graph.node_sets["a"][tfgnn.HIDDEN_STATE])
+    self.assertAllEqual([[8.0]], graph.node_sets["c"][tfgnn.HIDDEN_STATE])
     # Node "b" receives message of dimension 6 from sender node and edge
     # in which all elements are 1+16=17. The hidden state is updated from
     # 2 to 2 + 6*17.
-    self.assertAllEqual([[2. + message_dim*17]],
-                        graph.node_sets["b"][tfgnn.HIDDEN_STATE])
+    self.assertAllEqual(
+        [[2.0 + message_dim * 17]], graph.node_sets["b"][tfgnn.HIDDEN_STATE]
+    )
 
   def testMessageUnitsNotDivisible(self):
     with self.assertRaisesRegex(
-        ValueError, r"must be divisible by num_heads, got 5 and 2"):
-      _ = gat_v2.GATv2MPNNGraphUpdate(message_dim=5, num_heads=2,
-                                      units=12, receiver_tag=tfgnn.SOURCE)
+        ValueError, r"must be divisible by num_heads, got 5 and 2"
+    ):
+      _ = gat_v2.GATv2MPNNGraphUpdate(
+          message_dim=5, num_heads=2, units=12, receiver_tag=tfgnn.SOURCE
+      )
+
+
+class GATv2TFLiteTest(tf.test.TestCase, parameterized.TestCase):
+
+  def testBasic(self):
+    test_graph_1_dict = {
+        # We care that the TFLite interpreter gives the same output as the
+        # model, which was tested separately (although not for the randomly
+        # initialized weights that we keep here).
+        "source": tf.constant([0, 1, 2, 0, 2, 1]),
+        "target": tf.constant([1, 2, 0, 2, 1, 0]),
+        "node_features": tf.constant([
+            [1.0, 0.0, 0.0, 1.0],
+            [0.0, 1.0, 0.0, 2.0],
+            [0.0, 0.0, 1.0, 3.0],
+        ]),
+        "edge_features": tf.constant([
+            [3.0],
+            [6.0],
+            [9.0],
+            [2.0],
+            [6.0],
+            [4.0]]),
+    }
+
+    layer = gat_v2.GATv2MPNNGraphUpdate(
+        units=4,
+        message_dim=4,
+        num_heads=2,
+        receiver_tag=tfgnn.TARGET,
+        node_set_names=["nodes"],
+        kernel_initializer="ones",
+        edge_feature=tfgnn.HIDDEN_STATE,
+    )
+
+    inputs = {
+        "node_features": tf.keras.Input([4], None, "node_features", tf.float32),
+        "source": tf.keras.Input([], None, "source", tf.int32),
+        "target": tf.keras.Input([], None, "target", tf.int32),
+        "edge_features": tf.keras.Input([1], None, "edge_features", tf.float32),
+    }
+    graph_in = _MakeGraphTensor()(inputs)
+    graph_out = layer(graph_in)
+    outputs = tf.keras.layers.Layer(name="final_node_states")(
+        graph_out.node_sets["nodes"][tfgnn.HIDDEN_STATE]
+    )
+    model = tf.keras.Model(inputs, outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = model(test_graph_1_dict).numpy()
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith("2.10."):
+      self.skipTest("GNN models are unsupported in TFLite until TF 2.11 but "
+                    f"got TF {tf.__version__}")
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner("serving_default")
+    obtained = signature_runner(**test_graph_1_dict)["final_node_states"]
+    self.assertAllClose(expected, obtained)
+
+
+# TODO(b/274779989): Replace this layer with a more standard representation
+# of GraphTensor as a dict of plain Tensors.
+class _MakeGraphTensor(tf.keras.layers.Layer):
+  """Makes a homogeneous GraphTensor of rank 0 with a single component."""
+
+  def call(self, inputs):
+    node_sizes = tf.shape(inputs["node_features"])[0]
+    edge_sizes = tf.shape(inputs["edge_features"])[0]
+    return tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            "nodes": tfgnn.NodeSet.from_fields(
+                sizes=tf.expand_dims(node_sizes, axis=0),
+                features={tfgnn.HIDDEN_STATE: inputs["node_features"]},
+            )
+        },
+        edge_sets={
+            "edges": tfgnn.EdgeSet.from_fields(
+                sizes=tf.expand_dims(edge_sizes, axis=0),
+                adjacency=tfgnn.Adjacency.from_indices(
+                    ("nodes", inputs["source"]), ("nodes", inputs["target"])
+                ),
+                features={tfgnn.HIDDEN_STATE: inputs["edge_features"]},
+            )
+        },
+    )
 
 
 def _make_test_graph_abc():
   return tfgnn.GraphTensor.from_pieces(
       node_sets={
           "a": tfgnn.NodeSet.from_fields(
               sizes=tf.constant([1]),
-              features={tfgnn.HIDDEN_STATE: tf.constant([[1.]])}),
+              features={tfgnn.HIDDEN_STATE: tf.constant([[1.0]])},
+          ),
           "b": tfgnn.NodeSet.from_fields(
               sizes=tf.constant([1]),
-              features={tfgnn.HIDDEN_STATE: tf.constant([[2.]])}),
+              features={tfgnn.HIDDEN_STATE: tf.constant([[2.0]])},
+          ),
           "c": tfgnn.NodeSet.from_fields(
               sizes=tf.constant([1]),
-              features={tfgnn.HIDDEN_STATE: tf.constant([[8.]])})},
+              features={tfgnn.HIDDEN_STATE: tf.constant([[8.0]])},
+          ),
+      },
       edge_sets={
           "a->b": tfgnn.EdgeSet.from_fields(
               sizes=tf.constant([1]),
               adjacency=tfgnn.Adjacency.from_indices(
-                  ("a", tf.constant([0])),
-                  ("b", tf.constant([0]))),
-              features={"fab": tf.constant([[16.]])}),
+                  ("a", tf.constant([0])), ("b", tf.constant([0]))
+              ),
+              features={"fab": tf.constant([[16.0]])},
+          ),
           "c->c": tfgnn.EdgeSet.from_fields(
               sizes=tf.constant([1]),
               adjacency=tfgnn.Adjacency.from_indices(
-                  ("c", tf.constant([0])),
-                  ("c", tf.constant([0]))))})
+                  ("c", tf.constant([0])), ("c", tf.constant([0]))
+              ),
+          ),
+      },
+  )
 
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/BUILD`

 * *Files 25% similar despite different names*

```diff
@@ -1,44 +1,83 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "py_strict_test")
 
 licenses(["notice"])
 
 package(
-    default_visibility = [":__subpackages__"],
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = ["//visibility:public"],
 )
 
-package_group(name = "users")
+pytype_strict_library(
+    name = "classification",
+    srcs = ["classification.py"],
+    srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    deps = [
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
+    ],
+)
+
+py_strict_test(
+    name = "classification_test",
+    srcs = ["classification_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":classification",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
+    ],
+)
 
 pytype_strict_library(
-    name = "gcn",
-    srcs = ["__init__.py"],
+    name = "link_prediction",
+    srcs = ["link_prediction.py"],
     srcs_version = "PY3",
-    visibility = [
-        ":__subpackages__",
-        ":users",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    deps = [
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
     ],
+)
+
+py_strict_test(
+    name = "link_prediction_test",
+    srcs = ["link_prediction_test.py"],
+    srcs_version = "PY3",
     deps = [
-        ":gcn_conv",
+        ":link_prediction",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
     ],
 )
 
 pytype_strict_library(
-    name = "gcn_conv",
-    srcs = ["gcn_conv.py"],
+    name = "regression",
+    srcs = ["regression.py"],
     srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
     ],
 )
 
-tf_py_test(
-    name = "gcn_conv_test",
-    srcs = ["gcn_conv_test.py"],
+py_strict_test(
+    name = "regression_test",
+    srcs = ["regression_test.py"],
     srcs_version = "PY3",
     deps = [
-        ":gcn_conv",
+        ":regression",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,29 +13,61 @@
 # limitations under the License.
 # ==============================================================================
 """Keras layer for Graph Convolutional Network by Kipf&Welling (2016).
 
 This file implements the fundamental transformation which can be wrapped in
 NodeSetUpdate and EdgeSetUpdate.
 """
-from typing import Optional, Union
+from typing import Any, Optional
 
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 
-_RegularizerType = Union[tf.keras.regularizers.Regularizer, str]
-
 
 @tf.keras.utils.register_keras_serializable(package='GNN>models>gcn')
 class GCNConv(tf.keras.layers.Layer):
-  """Implements the Graph Convolutional Network by Kipf&Welling (2016).
+  r"""Implements the Graph Convolutional Network by Kipf&Welling (2016).
 
   This class implements a Graph Convolutional Network from
   https://arxiv.org/abs/1609.02907 as a Keras layer that can be used
   as a convolution on an edge set in a tfgnn.keras.layers.NodeSetUpdate.
+  The original algorithm proposed in the Graph Convolutional Network paper
+  expects a symmetric graph as input. That is, if there is an edge from node i
+  to node j, there is also an edge from node j to node i. This implementation,
+  however, is able to take asymmetric graphs as input.
+
+  Let $w_{ij}$ be the weight of the edge from sender i to receiver j.
+  Let $\deg^{in}_i$ be the number of incoming edges to i (in the direction
+  of message flow, see `receiver_tag`), and $\deg^{out}_i$ the number of
+  outgoing edges from i. In a symmetric graphs, both are equal.
+
+  In this implementation, we provide multiple approaches for normalizing an edge
+  weight $w_{ij}$ in $v_{ij}$, namely `"none"`, `"in"`, `"out"`, `"in_out"`, and
+  `"in_in"`. Setting normalization to `"none"` will end up in set $v_{ij} =
+  w_{ij}$.
+  The `"in"` normalization normalizes edge weights using the in-degree of the
+  receiver node, that is:
+
+  $$v_{ij} = w_{ij} / \deg^{in}_j.$$
+
+  The `"out"` normalization normalizes edges using the out-degree of sender
+  nodes that is:
+
+  $$v_{ij} = w_{ij} / \deg^{out}_i.$$
+
+  The `"in_out"` normalization normalizes edges as follows:
+
+  $$v_{ij} = w_{ij} / (\sqrt{\deg^{out}_i} \sqrt{\deg^{in}_j}).$$
+
+  The `"in_in"` normalization normalizes the edge weights as:
+
+  $$v_{ij} = w_{ij} / (\sqrt{\deg^{in}_i} \sqrt{\deg^{in}_j}).$$
+
+  For symmetric graphs (as in the original GCN paper), `"in_out"` and `"in_in"`
+  are equal, but the latter needs to compute degrees just once.
 
   Init arguments:
     units: Number of output units for this transformation applied to sender
       node features.
     receiver_tag: This layer's result is obtained by pooling the per-edge
       results at this endpoint of each edge. The default is `tfgnn.TARGET`,
       but it is perfectly reasonable to do a convolution towards the
@@ -45,20 +77,24 @@
     activation: Keras activation to apply to the result, defaults to 'relu'.
     use_bias: Whether to add bias in the final transformation. The original
       paper doesn't use a bias, but this defaults to True to be consistent
       with Keras and other implementations.
     add_self_loops: Whether to compute the result as if a loop from each node
       to itself had been added to the edge set. The self-loop edges are added
       with an edge weight of one.
-    normalize: Whether to normalize the node features by in-degree.
-    kernel_initializer: initializer of type tf.keras.initializers .
+    kernel_initializer: Can be set to a `kernel_initializer` as understood
+      by `tf.keras.layers.Dense` etc.
+      An `Initializer` object gets cloned before use to ensure a fresh seed,
+      if not set explicitly. For more, see `tfgnn.keras.clone_initializer()`.
     node_feature: Name of the node feature to transform.
     edge_weight_feature_name: Can be set to the name of a feature on the edge
       set that supplies a scalar weight for each edge. The GCN computation uses
       it as the edge's entry in the adjacency matrix, instead of the default 1.
+    degree_normalization: Can be set to `"none"`, `"in"`, `"out"`, `"in_out"`,
+      or `"in_in"`, as explained above.
     **kwargs: additional arguments for the Layer.
 
   Call arguments:
     graph: The GraphTensor on which to apply the layer.
     edge_set_name: Edge set of `graph` over which to apply the layer.
 
   Example:
@@ -88,56 +124,58 @@
                  target=(tfgnn.NODES, tf.constant([1, 0, 3, 2],
                                                   dtype=tf.int64))))})
   gcnconv = gcn_conv.GCNConv(3)
   gcnconv(graph, edge_set_name=tfgnn.EDGES)   # Has shape=(4, 3).
   ```
   """
 
-  def __init__(self,
-               units: int,
-               *,
-               receiver_tag: tfgnn.IncidentNodeTag = tfgnn.TARGET,
-               activation='relu',
-               use_bias: bool = True,
-               add_self_loops: bool = False,
-               normalize: bool = True,
-               kernel_initializer: bool = None,
-               node_feature: Optional[str] = tfgnn.HIDDEN_STATE,
-               kernel_regularizer: Optional[_RegularizerType] = None,
-               edge_weight_feature_name: Optional[tfgnn.FieldName] = None,
-               **kwargs):
-
+  def __init__(
+      self,
+      units: int,
+      *,
+      receiver_tag: tfgnn.IncidentNodeTag = tfgnn.TARGET,
+      activation='relu',
+      use_bias: bool = True,
+      add_self_loops: bool = False,
+      kernel_initializer: Any = None,
+      node_feature: Optional[str] = tfgnn.HIDDEN_STATE,
+      kernel_regularizer: Any = None,
+      edge_weight_feature_name: Optional[tfgnn.FieldName] = None,
+      degree_normalization: str = 'in_out',
+      **kwargs,
+  ):
     super().__init__(**kwargs)
     self._filter = tf.keras.layers.Dense(
         units=units,
         activation=activation,
         use_bias=use_bias,
         kernel_regularizer=kernel_regularizer,
-        kernel_initializer=kernel_initializer)
+        kernel_initializer=tfgnn.keras.clone_initializer(kernel_initializer))
     self._add_self_loops = add_self_loops
-    self._normalize = normalize
     self._node_feature = node_feature
     self._receiver = receiver_tag
     self._sender = tfgnn.reverse_tag(receiver_tag)
     self._edge_weight_feature_name = edge_weight_feature_name
+    self._degree_normalization = degree_normalization
 
   def get_config(self):
     filter_config = self._filter.get_config()
     return dict(
         receiver_tag=self._receiver,
         node_feature=self._node_feature,
         add_self_loops=self._add_self_loops,
-        normalize=self._normalize,
         units=filter_config['units'],
         activation=filter_config['activation'],
         use_bias=filter_config['use_bias'],
         kernel_initializer=filter_config['kernel_initializer'],
         kernel_regularizer=filter_config['kernel_regularizer'],
         edge_weight_feature_name=self._edge_weight_feature_name,
-        **super().get_config())
+        degree_normalization=self._degree_normalization,
+        **super().get_config(),
+    )
 
   def call(
       self,
       graph: tfgnn.GraphTensor,
       *,
       edge_set_name: Optional[tfgnn.EdgeSetName],
   ):
@@ -146,78 +184,101 @@
     # the diagonal matrix
     edge_adj = graph.edge_sets[edge_set_name].adjacency
     sender_name = edge_adj.node_set_name(self._sender)
     if edge_adj.node_set_name(self._receiver) != sender_name:
       raise ValueError('source and target node sets must be the same '
                        f'for edge set {edge_set_name} ')
 
-    nnodes = tf.cast(graph.node_sets[sender_name].total_size, tf.int64)
-    float_type = graph.node_sets[sender_name][self._node_feature].dtype
-
-    if self._normalize:
-      edge_set = graph.edge_sets[edge_set_name]
-      if self._edge_weight_feature_name is not None:
-        try:
-          edge_weights = graph.edge_sets[edge_set_name][
-              self._edge_weight_feature_name]
-        except KeyError as e:
-          raise ValueError(f'{self._edge_weight_feature_name} is not given '
-                           f'for edge set {edge_set_name} ') from e
-        if edge_weights.shape.rank != 1:
-          # GraphTensor guarantees it is not None.
-          raise ValueError(
-              'Expecting vector for edge weights. Received rank '
-              f'{edge_weights.shape.rank}.'
-          )
-        edge_weights = tf.expand_dims(
-            edge_weights, axis=1)  # Align with state feature.
-      else:
-        edge_weights = tf.ones([edge_set.total_size, 1])
+    edge_set = graph.edge_sets[edge_set_name]
+    if self._edge_weight_feature_name is not None:
+      try:
+        edge_weights = graph.edge_sets[edge_set_name][
+            self._edge_weight_feature_name
+        ]
+      except KeyError as e:
+        raise ValueError(
+            f'{self._edge_weight_feature_name} is not given '
+            f'for edge set {edge_set_name} '
+        ) from e
+      if edge_weights.shape.rank != 1:
+        # GraphTensor guarantees it is not None.
+        raise ValueError(
+            'Expecting vector for edge weights. Received rank '
+            f'{edge_weights.shape.rank}.'
+        )
+      edge_weights = tf.expand_dims(
+          edge_weights, axis=1
+      )  # Align with state feature.
+    else:
+      edge_weights = tf.ones([edge_set.total_size, 1])
 
-      in_degree = tf.squeeze(
-          tfgnn.pool_edges_to_node(
-              graph,
-              edge_set_name,
-              self._receiver,
-              'sum',
-              feature_value=edge_weights), -1)
-      # Degree matrix is the sum of rows of adjacency
-      # Adding self-loops adds an identity matrix to the adjacency
+    def get_degree(node_tag: tfgnn.IncidentNodeTag):
+      # If node_tag is receiver, this function computes the in_degree of nodes
+      # and if node_tag is sender, it comptes the out_degree of nodes.
+      # Shape of node_degree is [nnodes, 1]
+      node_degree = tfgnn.pool_edges_to_node(
+          graph,
+          edge_set_name,
+          node_tag,
+          'sum',
+          feature_value=edge_weights,
+      )
+      # Adding self-loops connects each node to itself.
       # This adds 1 to each diagonal element of the degree matrix
       if self._add_self_loops:
-        in_degree += 1
-      invsqrt_deg = tf.math.rsqrt(in_degree)
+        node_degree += 1
+      else:
+        # Prevent division by zero.
+        node_degree = tf.maximum(node_degree, 1)
+      return node_degree
+
+    if self._degree_normalization == 'none':
+      sender_scale = receiver_scale = None
+    elif self._degree_normalization == 'in':
+      receiver_scale = 1 / get_degree(self._receiver)
+      sender_scale = None
+    elif self._degree_normalization == 'out':
+      sender_scale = 1 / get_degree(self._sender)
+      receiver_scale = None
+    elif self._degree_normalization == 'in_out':
+      sender_scale = tf.math.rsqrt(get_degree(self._sender))
+      receiver_scale = tf.math.rsqrt(get_degree(self._receiver))
+    elif self._degree_normalization == 'in_in':
+      sender_scale = receiver_scale = tf.math.rsqrt(get_degree(self._receiver))
     else:
-      invsqrt_deg = tf.ones(nnodes, dtype=float_type)
-
-    # Calculate \hat{D^{-1/2}}X first
-    normalized_values = (
-        invsqrt_deg[:, tf.newaxis] *
-        graph.node_sets[sender_name][self._node_feature])
+      raise ValueError(
+          'Expecting degree_normalization to be `none`, `in`, `out`,'
+          ' `in_out`, or `in_in`.'
+      )
+
+    if sender_scale is not None:
+      normalized_values = (
+          sender_scale * graph.node_sets[sender_name][self._node_feature]
+      )
+    else:
+      normalized_values = graph.node_sets[sender_name][self._node_feature]
 
-    # Calculate A\hat{D^{-1/2}}X by broadcasting then pooling
     source_bcast = tfgnn.broadcast_node_to_edges(
         graph,
         edge_set_name,
         self._sender,
         feature_value=normalized_values,
     )
     if self._edge_weight_feature_name is not None:
       source_bcast = source_bcast * edge_weights
     pooled = tfgnn.pool_edges_to_node(
         graph, edge_set_name, self._receiver, 'sum', feature_value=source_bcast)
+    if receiver_scale is not None:
+      pooled = receiver_scale * pooled
 
-    # left-multiply the result by \hat{D^{-1/2}}
-    pooled = invsqrt_deg[:, tf.newaxis] * pooled
-
-    # Add \hat{D^{-1/2}} I \hat{D^{-1/2}} X
-    # Since the right two factors are already computed,
-    # we can remove I and just multiply by the normalizing matrix again
     if self._add_self_loops:
-      pooled += invsqrt_deg[:, tf.newaxis] * normalized_values
+      if receiver_scale is not None:
+        pooled += receiver_scale * normalized_values
+      else:
+        pooled += normalized_values
 
     return self._filter(pooled)
 
 
 def GCNHomGraphUpdate(*,  # To be called like a class initializer.  pylint: disable=invalid-name
                       units: int,
                       receiver_tag: tfgnn.IncidentNodeTag = tfgnn.TARGET,
@@ -255,24 +316,23 @@
     **kwargs: Any optional arguments to GCNConv, see there.
   """
 
   # Build a GraphUpdate for the target node set of the given edge_set_name.
   # That needs to be deferred until we see a GraphTensorSpec that tells us
   # the node_set_name.
   def deferred_init_callback(spec: tfgnn.GraphTensorSpec):
-    tfgnn.check_homogeneous_graph_tensor(spec, 'GCNHomGraphUpdate')
-    edge_set_name, = spec.edge_sets_spec.keys()
-    node_set_name = spec.edge_sets_spec[
-        edge_set_name].adjacency_spec.node_set_name(receiver_tag)
+    node_set_name, edge_set_name = tfgnn.get_homogeneous_node_and_edge_set_name(
+        spec, 'GCNHomGraphUpdate')
     node_set_updates = {
         node_set_name: tfgnn.keras.layers.NodeSetUpdate(
             {edge_set_name: GCNConv(
                 units=units,
                 receiver_tag=receiver_tag,
                 add_self_loops=add_self_loops,
                 node_feature=feature_name,
-                **kwargs)},
+                **kwargs,  # Any kernel_initializer gets cloned by GCNConv.
+            )},
             next_state=tfgnn.keras.layers.SingleInputNextState(),
             node_input_feature=feature_name)}
     return dict(node_sets=node_set_updates)
   return tfgnn.keras.layers.GraphUpdate(
       deferred_init_callback=deferred_init_callback, name=name)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gcn/gcn_conv_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/gcn/gcn_conv_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -21,456 +21,892 @@
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.models.gcn import gcn_conv
 
 
 class ReloadModel(int, enum.Enum):
   """Controls how to reload a model for further testing after saving."""
+
   SKIP = 0
   SAVED_MODEL = 1
   KERAS = 2
 
 
 class GcnConvTest(tf.test.TestCase, parameterized.TestCase):
   """Tests for GCNConv layer."""
 
   @parameterized.named_parameters(
       dict(
           testcase_name='noSelfLoops',
           graph=tfgnn.GraphTensor.from_pieces(
               node_sets={
-                  tfgnn.NODES:
-                      tfgnn.NodeSet.from_fields(
-                          sizes=[2],
-                          features={
-                              tfgnn.HIDDEN_STATE:
-                                  tf.constant([[1., 0, 0], [0, 1, 0]])
-                          },
-                      )
+                  tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                      sizes=[2],
+                      features={
+                          tfgnn.HIDDEN_STATE: tf.constant(
+                              [[1.0, 0, 0], [0, 1, 0]]
+                          )
+                      },
+                  )
               },
               edge_sets={
-                  tfgnn.EDGES:
-                      tfgnn.EdgeSet.from_fields(
-                          sizes=[2],
-                          adjacency=tfgnn.Adjacency.from_indices(
-                              source=(tfgnn.NODES,
-                                      tf.constant([0, 1], dtype=tf.int64)),
-                              target=(tfgnn.NODES,
-                                      tf.constant([1, 0], dtype=tf.int64)),
-                          ))
-              }),
+                  tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                      sizes=[2],
+                      adjacency=tfgnn.Adjacency.from_indices(
+                          source=(
+                              tfgnn.NODES,
+                              tf.constant([0, 1], dtype=tf.int64),
+                          ),
+                          target=(
+                              tfgnn.NODES,
+                              tf.constant([1, 0], dtype=tf.int64),
+                          ),
+                      ),
+                  )
+              },
+          ),
           add_self_loops=False,
-          expected_result=tf.constant([[0, 1, 0], [1., 0, 0]])),
+          expected_result=tf.constant([[0, 1, 0],
+                                       [1.0, 0, 0]]),
+      ),
       dict(
           testcase_name='selfLoops',
           graph=tfgnn.GraphTensor.from_pieces(
               node_sets={
-                  tfgnn.NODES:
-                      tfgnn.NodeSet.from_fields(
-                          sizes=[2],
-                          features={
-                              tfgnn.HIDDEN_STATE:
-                                  tf.constant([[1., 0, 0], [0, 1, 0]])
-                          },
-                      )
+                  tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                      sizes=[2],
+                      features={
+                          tfgnn.HIDDEN_STATE: tf.constant(
+                              [[1.0, 0, 0],
+                               [0, 1, 0]]
+                          )
+                      },
+                  )
               },
               edge_sets={
-                  tfgnn.EDGES:
-                      tfgnn.EdgeSet.from_fields(
-                          sizes=[2],
-                          adjacency=tfgnn.Adjacency.from_indices(
-                              source=(tfgnn.NODES,
-                                      tf.constant([0, 1], dtype=tf.int64)),
-                              target=(tfgnn.NODES,
-                                      tf.constant([1, 0], dtype=tf.int64)),
-                          ))
-              }),
+                  tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                      sizes=[2],
+                      adjacency=tfgnn.Adjacency.from_indices(
+                          source=(
+                              tfgnn.NODES,
+                              tf.constant([0, 1], dtype=tf.int64),
+                          ),
+                          target=(
+                              tfgnn.NODES,
+                              tf.constant([1, 0], dtype=tf.int64),
+                          ),
+                      ),
+                  )
+              },
+          ),
           add_self_loops=True,
-          expected_result=tf.constant([[0.5, 0.5, 0], [0.5, 0.5, 0]]),
+          expected_result=tf.constant([[0.5, 0.5, 0],
+                                       [0.5, 0.5, 0]]),
       ),
       dict(
           testcase_name='discreteComponents',
           graph=tfgnn.GraphTensor.from_pieces(
               node_sets={
-                  tfgnn.NODES:
-                      tfgnn.NodeSet.from_fields(
-                          sizes=[2, 2],
-                          features={
-                              tfgnn.HIDDEN_STATE:
-                                  tf.constant([[1., 0, 0], [0, 1, 0]] * 2)
-                          },
-                      )
+                  tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                      sizes=[2, 2],
+                      features={
+                          tfgnn.HIDDEN_STATE: tf.constant(
+                              [[1.0, 0, 0], [0, 1, 0]] * 2
+                          )
+                      },
+                  )
               },
               edge_sets={
-                  tfgnn.EDGES:
-                      tfgnn.EdgeSet.from_fields(
-                          sizes=[2, 2],
-                          adjacency=tfgnn.Adjacency.from_indices(
-                              source=(tfgnn.NODES,
-                                      tf.constant([0, 1, 2, 3],
-                                                  dtype=tf.int64)),
-                              target=(tfgnn.NODES,
-                                      tf.constant([1, 0, 3, 2],
-                                                  dtype=tf.int64)),
-                          ))
-              }),
+                  tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                      sizes=[2, 2],
+                      adjacency=tfgnn.Adjacency.from_indices(
+                          source=(
+                              tfgnn.NODES,
+                              tf.constant([0, 1, 2, 3], dtype=tf.int64),
+                          ),
+                          target=(
+                              tfgnn.NODES,
+                              tf.constant([1, 0, 3, 2], dtype=tf.int64),
+                          ),
+                      ),
+                  )
+              },
+          ),
           add_self_loops=False,
           expected_result=tf.constant([[0, 1.0, 0], [1, 0, 0]] * 2),
       ),
   )
   def test_gcnconv(self, graph, add_self_loops, expected_result):
     """Tests that gcn_conv returns the correct values."""
     conv = gcn_conv.GCNConv(
         units=3,
         activation=None,
         use_bias=False,
         add_self_loops=add_self_loops,
-        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)))
-    self.assertAllClose(expected_result,
-                        conv(graph, edge_set_name=tfgnn.EDGES),
-                        rtol=1e-06, atol=1e-06)
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)),
+    )
+    self.assertAllClose(
+        expected_result,
+        conv(graph, edge_set_name=tfgnn.EDGES),
+        rtol=1e-06,
+        atol=1e-06,
+    )
 
   def test_gcnconv_activation(self):
     """Tests that the activation function is correctly passed through."""
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE:
-                            tf.constant([[-1., 0, 0], [0, 1, 0]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=(tfgnn.NODES, tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[-1.0, 0, 0], [0, 1, 0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
     conv_relu = gcn_conv.GCNConv(
         units=3,
         use_bias=False,
         add_self_loops=True,
-        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)))
-    expected_result = tf.constant([[0., 0.5, 0], [0, 0.5, 0]])
-    self.assertAllClose(expected_result,
-                        conv_relu(graph, edge_set_name=tfgnn.EDGES),
-                        rtol=1e-06, atol=1e-06)
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)),
+    )
+    expected_result = tf.constant([[0.0, 0.5, 0], [0, 0.5, 0]])
+    self.assertAllClose(
+        expected_result,
+        conv_relu(graph, edge_set_name=tfgnn.EDGES),
+        rtol=1e-06,
+        atol=1e-06,
+    )
 
   def test_gcnconv_heterogeneous(self):
     """Tests that heterogeneous edges throw an error."""
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE:
-                            tf.constant([[1., 0, 0], [0, 1, 0]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=('antinodes', tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0, 0], [0, 1, 0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=('antinodes', tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
     conv = gcn_conv.GCNConv(units=3)
-    self.assertRaisesRegex(ValueError,
-                           ('source and target node sets must be the same '
-                            'for edge set edges '),
-                           lambda: conv(graph, edge_set_name=tfgnn.EDGES))
+    self.assertRaisesRegex(
+        ValueError,
+        'source and target node sets must be the same for edge set edges ',
+        lambda: conv(graph, edge_set_name=tfgnn.EDGES),
+    )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='noSelfLoops_noBias',
           use_bias=False,
           add_self_loops=False,
-      ),)
+      ),
+  )
   def test_gcnconv_with_edge_weights_ones(self, use_bias, add_self_loops):
     """Tests that gcn_conv returns the correct values with edge weights."""
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE: tf.constant([[1., 0.], [0., 1.]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        'weights': tf.constant([1.0, 1.0], dtype=tf.float32)
-                    },
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=(tfgnn.NODES, tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0.0], [0.0, 1.0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                features={'weights': tf.constant([1.0, 1.0], dtype=tf.float32)},
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
     conv_with_edge_weights = gcn_conv.GCNConv(
         units=2,
         use_bias=use_bias,
         add_self_loops=add_self_loops,
         kernel_initializer=tf.keras.initializers.Constant(tf.eye(2)),
-        edge_weight_feature_name='weights')
+        edge_weight_feature_name='weights',
+    )
     conv_without_edge_weights = gcn_conv.GCNConv(
         units=2,
         use_bias=use_bias,
         add_self_loops=add_self_loops,
-        kernel_initializer=tf.keras.initializers.Constant(tf.eye(2)))
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(2)),
+    )
     self.assertAllClose(
         conv_with_edge_weights(graph, edge_set_name=tfgnn.EDGES),
         conv_without_edge_weights(graph, edge_set_name=tfgnn.EDGES),
         rtol=1e-06,
-        atol=1e-06)
+        atol=1e-06,
+    )
 
   @parameterized.named_parameters(
       dict(
           testcase_name='noSelfLoops_noBias',
           use_bias=False,
           add_self_loops=False,
-          expected_result=tf.constant([[0., 4. / (2. * 3.)],
-                                       [9. / (2. * 3.), 0.]])),
+          expected_result=tf.constant(
+              [[0.0, 4.0 / (2.0 * 2.0)], [9.0 / (3.0 * 3.0), 0.0]]
+          ),
+      ),
       dict(
           testcase_name='selfLoops_noBias',
           use_bias=False,
           add_self_loops=True,
-          expected_result=tf.constant(
-              [[
-                  1. / (math.sqrt(5.) * math.sqrt(5.)),
-                  4. / (math.sqrt(10.) * math.sqrt(5.))
+          expected_result=tf.constant([
+              [
+                  1.0 / (math.sqrt(5.0) * math.sqrt(10.0)),
+                  4.0 / (math.sqrt(5.0) * math.sqrt(5.0)),
               ],
-               [
-                   9. / (math.sqrt(10.) * math.sqrt(5.)),
-                   1. / (math.sqrt(10.) * math.sqrt(10.))
-               ]])),
+              [
+                  9.0 / (math.sqrt(10.0) * math.sqrt(10.0)),
+                  1.0 / (math.sqrt(10.0) * math.sqrt(5.0)),
+              ],
+          ]),
+      ),
   )
-  def test_gcnconv_with_edge_weights(self, use_bias, add_self_loops,
-                                     expected_result):
+  def test_gcnconv_with_edge_weights(
+      self, use_bias, add_self_loops, expected_result
+  ):
     """Tests that gcn_conv returns the correct values with edge weights."""
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE: tf.constant([[1., 0.], [0., 1.]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        'weights': tf.constant([9.0, 4.0], dtype=tf.float32)
-                    },
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=(tfgnn.NODES, tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0.0], [0.0, 1.0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                features={'weights': tf.constant([9.0, 4.0], dtype=tf.float32)},
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
     conv = gcn_conv.GCNConv(
         units=2,
         use_bias=use_bias,
         add_self_loops=add_self_loops,
         kernel_initializer=tf.keras.initializers.Constant(tf.eye(2)),
-        edge_weight_feature_name='weights')
+        edge_weight_feature_name='weights',
+    )
 
     self.assertAllClose(
         expected_result,
         conv(graph, edge_set_name=tfgnn.EDGES),
         rtol=1e-06,
-        atol=1e-06)
+        atol=1e-06,
+    )
 
   def test_gcnconv_with_edge_weights_missing(self):
     """Tests that missing given edge weights feature name in the graph tensor throws an error."""
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE: tf.constant([[1., 0.], [0., 1.]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=(tfgnn.NODES, tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0.0], [0.0, 1.0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
 
     conv = gcn_conv.GCNConv(units=2, edge_weight_feature_name='weights')
-    self.assertRaisesRegex(ValueError,
-                           'weights is not given for edge set edges ',
-                           lambda: conv(graph, edge_set_name=tfgnn.EDGES))
+    self.assertRaisesRegex(
+        ValueError,
+        'weights is not given for edge set edges ',
+        lambda: conv(graph, edge_set_name=tfgnn.EDGES),
+    )
 
   def test_gcnconv_with_bad_shaped_edge_weights(self):
     """Tests that given edge weights feature with bad shape throws an error."""
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE: tf.constant([[1., 0.], [0., 1.]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        'weights': tf.constant([[9.0], [4.0]], dtype=tf.float32)
-                    },
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=(tfgnn.NODES, tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0.0], [0.0, 1.0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                features={
+                    'weights': tf.constant([[9.0], [4.0]], dtype=tf.float32)
+                },
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
 
     conv = gcn_conv.GCNConv(units=2, edge_weight_feature_name='weights')
     self.assertRaisesRegex(
-        ValueError, 'Expecting vector for edge weights. Received rank 2.',
-        lambda: conv(graph, edge_set_name=tfgnn.EDGES))
+        ValueError,
+        'Expecting vector for edge weights. Received rank 2.',
+        lambda: conv(graph, edge_set_name=tfgnn.EDGES),
+    )
+
+  def test_gcnconv_with_unknown_normalization(self):
+    """Tests that unknown degree normalization throws an error."""
+    graph = tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0.0], [0.0, 1.0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
+
+    conv = gcn_conv.GCNConv(units=2, degree_normalization='unknown')
+    self.assertRaisesRegex(
+        ValueError,
+        (
+            'Expecting degree_normalization to be `none`, `in`, `out`,'
+            ' `in_out`, or `in_in`'
+        ),
+        lambda: conv(graph, edge_set_name=tfgnn.EDGES),
+    )
+
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='noneDegreeNormalization',
+          degree_normalization='none',
+          expected_result=tf.constant(
+              [[1.0, 0.0, 3.0, 0.0], [2.0, 1.0, 0.0, 0.0], [0.0, 1.0, 1.0, 0.0]]
+          ),
+      ),
+      dict(
+          testcase_name='outDegreeNormalization',
+          degree_normalization='out',
+          expected_result=tf.constant([
+              [1.0 / 3.0, 0.0, 3.0 / 4.0, 0.0],
+              [2.0 / 3.0, 1.0 / 2.0, 0.0, 0.0],
+              [0.0, 1.0 / 2.0, 1.0 / 4.0, 0.0],
+          ]),
+      ),
+      dict(
+          testcase_name='inDegreeNormalization',
+          degree_normalization='in',
+          expected_result=tf.constant([
+              [1.0 / 4.0, 0.0, 3.0 / 4.0, 0.0],
+              [2.0 / 3.0, 1.0 / 3.0, 0.0, 0.0],
+              [0.0, 1.0 / 2.0, 1.0 / 2.0, 0.0],
+          ]),
+      ),
+      dict(
+          testcase_name='in_outDegreeNormalization',
+          degree_normalization='in_out',
+          expected_result=tf.constant([
+              [
+                  1.0 / (math.sqrt(4.0) * math.sqrt(3.0)),
+                  0.0,
+                  3.0 / (math.sqrt(4.0) * math.sqrt(4.0)),
+                  0.0,
+              ],
+              [
+                  2.0 / (math.sqrt(3.0) * math.sqrt(3.0)),
+                  1.0 / (math.sqrt(3.0) * math.sqrt(2.0)),
+                  0.0,
+                  0.0,
+              ],
+              [
+                  0.0,
+                  1.0 / (math.sqrt(2.0) * math.sqrt(2.0)),
+                  1.0 / (math.sqrt(2.0) * math.sqrt(4.0)),
+                  0.0,
+              ],
+          ]),
+      ),
+      dict(
+          testcase_name='in_inDegreeNormalization',
+          degree_normalization='in_in',
+          expected_result=tf.constant([
+              [
+                  1.0 / (math.sqrt(4.0) * math.sqrt(4.0)),
+                  0.0,
+                  3.0 / (math.sqrt(4.0) * math.sqrt(2.0)),
+                  0.0,
+              ],
+              [
+                  2.0 / (math.sqrt(3.0) * math.sqrt(4.0)),
+                  1.0 / (math.sqrt(3.0) * math.sqrt(3.0)),
+                  0.0,
+                  0.0,
+              ],
+              [
+                  0.0,
+                  1.0 / (math.sqrt(2.0) * math.sqrt(3.0)),
+                  1.0 / (math.sqrt(2.0) * math.sqrt(2.0)),
+                  0.0,
+              ],
+          ]),
+      ),
+  )
+  def test_gcnconv_degree_normalization(
+      self, degree_normalization, expected_result
+  ):
+    """Tests that gcn_conv returns the correct values with an asymmetric adjacency."""
+    graph = tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[4],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([
+                        [1.0, 0.0, 0.0, 0.0],
+                        [0.0, 1.0, 0.0, 0.0],
+                        [0.0, 0.0, 1.0, 0.0],
+                    ])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[3],
+                features={
+                    'weights': tf.constant([2.0, 1.0, 3.0], dtype=tf.float32)
+                },
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(
+                        tfgnn.NODES,
+                        tf.constant([0, 1, 2], dtype=tf.int64),
+                    ),
+                    target=(
+                        tfgnn.NODES,
+                        tf.constant([1, 2, 0], dtype=tf.int64),
+                    ),
+                ),
+            )
+        },
+    )
 
-  @parameterized.named_parameters(('', ReloadModel.SKIP),
-                                  ('Restored', ReloadModel.SAVED_MODEL),
-                                  ('RestoredKeras', ReloadModel.KERAS))
+    conv = gcn_conv.GCNConv(
+        units=4,
+        use_bias=False,
+        add_self_loops=True,
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(4)),
+        edge_weight_feature_name='weights',
+        degree_normalization=degree_normalization,
+    )
+
+    self.assertAllClose(
+        expected_result,
+        conv(graph, edge_set_name=tfgnn.EDGES),
+        rtol=1e-06,
+        atol=1e-06,
+    )
+
+  @parameterized.named_parameters(
+      dict(
+          testcase_name='inDegreeNormalization',
+          degree_normalization='in',
+          # Same as the expected result in the previous test.
+          expected_result=tf.constant([
+              [1.0 / 4.0, 0.0, 3.0 / 4.0],
+              [2.0 / 3.0, 1.0 / 3.0, 0.0],
+              [0.0, 1.0 / 2.0, 1.0 / 2.0],
+          ]),
+      ),
+      dict(
+          testcase_name='outDegreeNormalization',
+          degree_normalization='out',
+          # Same as the expected result in the previous test.
+          expected_result=tf.constant([
+              [1.0 / 3.0, 0.0, 3.0 / 4.0],
+              [2.0 / 3.0, 1.0 / 2.0, 0.0],
+              [0.0, 1.0 / 2.0, 1.0 / 4.0],
+          ]),
+      ),
+  )
+  def test_gcnconv_degree_normalization_reverse_edges(
+      self, degree_normalization, expected_result
+  ):
+    """Tests that gcn_conv returns the correct values with an asymmetric adjacency."""
+    graph = tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[3],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant(
+                        [[1.0, 0.0, 0.0],
+                         [0.0, 1.0, 0.0],
+                         [0.0, 0.0, 1.0],]
+                    )
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[3],
+                features={
+                    'weights': tf.constant([2.0, 1.0, 3.0], dtype=tf.float32)
+                },
+                adjacency=tfgnn.Adjacency.from_indices(
+                    # Swapping source and target compared to the previous test.
+                    target=(
+                        tfgnn.NODES,
+                        tf.constant([0, 1, 2], dtype=tf.int64),
+                    ),
+                    source=(
+                        tfgnn.NODES,
+                        tf.constant([1, 2, 0], dtype=tf.int64),
+                    ),
+                ),
+            )
+        },
+    )
+
+    conv = gcn_conv.GCNConv(
+        units=3,
+        # Changing the receiver to be the source node instead of the target node
+        receiver_tag=tfgnn.SOURCE,
+        use_bias=False,
+        add_self_loops=True,
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)),
+        edge_weight_feature_name='weights',
+        degree_normalization=degree_normalization,
+    )
+
+    self.assertAllClose(
+        expected_result,
+        conv(graph, edge_set_name=tfgnn.EDGES),
+        rtol=1e-06,
+        atol=1e-06,
+    )
+
+  def test_gcnconv_symmetric_adj(self):
+    """Tests that gcn_conv returns the same values for a symmetric adjacency with in_in and in_out normalizations."""
+    graph = tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[3],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant(
+                        [[1.0, 0.0, 0.0],
+                         [0.0, 1.0, 0.0],
+                         [0.0, 0.0, 1.0]]
+                    )
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[4],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(
+                        tfgnn.NODES,
+                        tf.constant([0, 0, 1, 2], dtype=tf.int64),
+                    ),
+                    target=(
+                        tfgnn.NODES,
+                        tf.constant([1, 2, 0, 0], dtype=tf.int64),
+                    ),
+                ),
+            )
+        },
+    )
+
+    conv_in_out = gcn_conv.GCNConv(
+        units=3,
+        use_bias=False,
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)),
+        degree_normalization='in_out',
+    )
+
+    conv_in_in = gcn_conv.GCNConv(
+        units=3,
+        use_bias=False,
+        kernel_initializer=tf.keras.initializers.Constant(tf.eye(3)),
+        degree_normalization='in_in',
+    )
+    self.assertAllEqual(
+        conv_in_in(graph, edge_set_name=tfgnn.EDGES),
+        conv_in_out(graph, edge_set_name=tfgnn.EDGES),
+    )
+
+  @parameterized.named_parameters(
+      ('', ReloadModel.SKIP),
+      ('Restored', ReloadModel.SAVED_MODEL),
+      ('RestoredKeras', ReloadModel.KERAS),
+  )
   def test_full_model(self, reload_model):
     """Tests GCNGraphUpdate in a full Model (incl. saving) with edge input."""
     gt_input = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            tfgnn.NODES:
-                tfgnn.NodeSet.from_fields(
-                    sizes=[2],
-                    features={
-                        tfgnn.HIDDEN_STATE:
-                            tf.constant([[1., 0, 0], [0, 1, 0]])
-                    },
-                )
-        },
-        edge_sets={
-            tfgnn.EDGES:
-                tfgnn.EdgeSet.from_fields(
-                    sizes=[2],
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        source=(tfgnn.NODES, tf.constant([0, 1],
-                                                         dtype=tf.int64)),
-                        target=(tfgnn.NODES, tf.constant([1, 0],
-                                                         dtype=tf.int64)),
-                    ))
-        })
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0, 0], [0, 1, 0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([1, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
     l2reg = 0.1  # Coefficient for L2 regularization.
     layer = gcn_conv.GCNHomGraphUpdate(
-        units=3, add_self_loops=True,
-        kernel_regularizer=tf.keras.regularizers.l2(l2reg))
+        units=3,
+        add_self_loops=True,
+        kernel_regularizer=tf.keras.regularizers.l2(l2reg),
+    )
     _ = layer(gt_input)  # Build weights.
     weights = {v.name: v for v in layer.trainable_weights}
     self.assertLen(weights, 2)
-    weights['gcn/node_set_update/gcn_conv/dense/bias:0'].assign(
-        [0., 0., 0.])
-    weights['gcn/node_set_update/gcn_conv/dense/kernel:0'].assign(
-        [[1., 0, 0,],
-         [0, 1, 0,],
-         [0, 0, 1,]])
+    weights['gcn/node_set_update/gcn_conv/dense/bias:0'].assign([0.0, 0.0, 0.0])
+    weights['gcn/node_set_update/gcn_conv/dense/kernel:0'].assign([
+        [1.0, 0, 0],
+        [0, 1, 0],
+        [0, 0, 1],
+    ])
 
     # Build a Model around the Layer, possibly saved and restored.
     inputs = tf.keras.layers.Input(type_spec=gt_input.spec)
     outputs = layer(inputs)
     model = tf.keras.Model(inputs, outputs)
     if reload_model:
       export_dir = os.path.join(self.get_temp_dir(), 'gcn')
       model.save(export_dir, include_optimizer=False)
       if reload_model == ReloadModel.KERAS:
         model = tf.keras.models.load_model(export_dir)
         # Check that from_config() worked, no fallback to a function trace, see
         # https://www.tensorflow.org/guide/keras/save_and_serialize#how_savedmodel_handles_custom_objects
-        self.assertIsInstance(model.get_layer(index=1),
-                              tfgnn.keras.layers.GraphUpdate)
+        self.assertIsInstance(
+            model.get_layer(index=1), tfgnn.keras.layers.GraphUpdate
+        )
       else:
         model = tf.saved_model.load(export_dir)
 
     if not reload_model or reload_model == ReloadModel.KERAS:
       # Model.losses only works on Keras models. tf.saved_model.load(), however,
       # does not return a Keras model. See:
       # https://www.tensorflow.org/api_docs/python/tf/saved_model/load
-      kernel_variables = [v for v in model.trainable_variables
-                          if '/kernel:0' in v.name]
+      kernel_variables = [
+          v for v in model.trainable_variables if '/kernel:0' in v.name
+      ]
       self.assertLen(kernel_variables, 1)  # 1 kernel variable per `weights[]`.
-      self.assertLen(model.losses, 1)      # One loss term per kernel variable.
+      self.assertLen(model.losses, 1)  # One loss term per kernel variable.
 
       expected_model_loss = tf.reduce_sum(kernel_variables[0] ** 2) * l2reg
       self.assertAllClose(model.losses[0], expected_model_loss)
 
     got_gt = model(gt_input)
     got = got_gt.node_sets['nodes'][tfgnn.HIDDEN_STATE]
 
     # The fourth column with values x.y from nodes is analogous to the
     # testBasic test above, with the contribution x from the favored
     # input before the decimal dot and the other contribution y after.
     # The fifth column with values (2x).(3y) is from edges, with the
     # multipliers 2 and 3 used above in setting up the edge features.
-    want = tf.constant([[0.5, 0.5, 0.],
-                        [0.5, 0.5, 0.]])
+    want = tf.constant([[0.5, 0.5, 0.0], [0.5, 0.5, 0.0]])
     self.assertAllEqual(got.shape, (2, 3))
-    self.assertAllClose(got, want, atol=.0001)
+    self.assertAllClose(got, want, atol=0.0001)
 
   def test_full_model_heterogeneous(self):
     graph = tfgnn.GraphTensor.from_pieces(
         node_sets={
-            'paper':
-                tfgnn.NodeSet.from_fields(
-                    features={'f': tf.constant([[1., 2., 3.], [2., 1., 3.]])},
-                    sizes=tf.constant([1, 1])),
-            'author':
-                tfgnn.NodeSet.from_fields(
-                    features={'f': tf.constant([[1., 0.], [0., 2.]] * 2)},
-                    sizes=tf.constant([2, 2])),
-        },
-        edge_sets={
-            'written':
-                tfgnn.EdgeSet.from_fields(
-                    features={},
-                    sizes=tf.constant([2, 1]),
-                    adjacency=tfgnn.Adjacency.from_indices(
-                        ('paper', tf.constant([0, 0, 1])),
-                        ('author', tf.constant([1, 0, 3])),
-                    )),
+            'paper': tfgnn.NodeSet.from_fields(
+                features={'f': tf.constant([[1.0, 2.0, 3.0],
+                                            [2.0, 1.0, 3.0]])},
+                sizes=tf.constant([1, 1]),
+            ),
+            'author': tfgnn.NodeSet.from_fields(
+                features={'f': tf.constant([[1.0, 0.0], [0.0, 2.0]] * 2)},
+                sizes=tf.constant([2, 2]),
+            ),
+        },
+        edge_sets={
+            'written': tfgnn.EdgeSet.from_fields(
+                features={},
+                sizes=tf.constant([2, 1]),
+                adjacency=tfgnn.Adjacency.from_indices(
+                    ('paper', tf.constant([0, 0, 1])),
+                    ('author', tf.constant([1, 0, 3])),
+                ),
+            ),
         },
     )
     layer = gcn_conv.GCNHomGraphUpdate(units=3)
     self.assertRaises(ValueError, lambda: layer(graph))
 
+  def test_no_nans(self):
+    gt_input = tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            tfgnn.NODES: tfgnn.NodeSet.from_fields(
+                sizes=[2],
+                features={
+                    tfgnn.HIDDEN_STATE: tf.constant([[1.0, 0, 0],
+                                                     [0, 1, 0]])
+                },
+            )
+        },
+        edge_sets={
+            tfgnn.EDGES: tfgnn.EdgeSet.from_fields(
+                sizes=[2],
+                adjacency=tfgnn.Adjacency.from_indices(
+                    source=(tfgnn.NODES, tf.constant([0, 1], dtype=tf.int64)),
+                    target=(tfgnn.NODES, tf.constant([0, 0], dtype=tf.int64)),
+                ),
+            )
+        },
+    )
+    l2reg = 0.1  # Coefficient for L2 regularization.
+    layer = gcn_conv.GCNHomGraphUpdate(
+        units=3,
+        add_self_loops=False,
+        kernel_regularizer=tf.keras.regularizers.l2(l2reg),
+    )
+    _ = layer(gt_input)  # Build weights.
+    weights = {v.name: v for v in layer.trainable_weights}
+    self.assertLen(weights, 2)
+    weights['gcn/node_set_update/gcn_conv/dense/bias:0'].assign([0.0, 0.0, 0.0])
+    weights['gcn/node_set_update/gcn_conv/dense/kernel:0'].assign([
+        [1.0, 0, 0],
+        [0, 1, 0],
+        [0, 0, 1],
+    ])
+
+    node_feats = layer(gt_input).node_sets['nodes'][tfgnn.HIDDEN_STATE]
+    second_row = node_feats[1]
+    # Although no leading connections, there should be 0's rather than NaNs.
+    self.assertAllClose(second_row, tf.zeros_like(second_row))
+
+
+class GCNTFLiteTest(tf.test.TestCase, parameterized.TestCase):
+
+  @parameterized.named_parameters(
+      ('Simplest', False, None),
+      ('OnlySelfLoops', True, None),
+      ('AllOps', True, 'edge_weights'),
+  )
+  def testBasic(self, add_self_loops, edge_weight_feature_name):
+    test_graph_1_dict = {
+        # We care that the TFLite interpreter gives the same output as the
+        # initialized weights that we keep here).
+        'source': tf.constant([0, 1, 2, 3]),
+        'target': tf.constant([1, 0, 3, 2]),
+        'node_features': tf.constant([[1.0, 0, 0], [0, 1, 0]] * 2),
+        'edge_weights': tf.constant([1.2, 0.8, 0.9, 1.1])
+    }
+
+    layer = gcn_conv.GCNHomGraphUpdate(
+        units=4,
+        add_self_loops=add_self_loops,
+        edge_weight_feature_name=edge_weight_feature_name,
+    )
+
+    inputs = {
+        'node_features': tf.keras.Input([3], None, 'node_features', tf.float32),
+        'source': tf.keras.Input([], None, 'source', tf.int32),
+        'target': tf.keras.Input([], None, 'target', tf.int32),
+        'edge_weights': tf.keras.Input([], None, 'edge_weights', tf.float32),
+    }
+    graph_in = _MakeGraphTensor()(inputs)
+    graph_out = layer(graph_in)
+    outputs = tf.keras.layers.Layer(name='final_node_states')(
+        graph_out.node_sets['nodes'][tfgnn.HIDDEN_STATE]
+    )
+    model = tf.keras.Model(inputs, outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = model(test_graph_1_dict).numpy()
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith('2.10.'):
+      self.skipTest('GNN models are unsupported in TFLite until TF 2.11 but '
+                    f'got TF {tf.__version__}')
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner('serving_default')
+    obtained = signature_runner(**test_graph_1_dict)['final_node_states']
+    self.assertAllClose(expected, obtained)
+
+
+# TODO(b/274779989): Replace this layer with a more standard representation
+# of GraphTensor as a dict of plain Tensors.
+class _MakeGraphTensor(tf.keras.layers.Layer):
+  """Makes a homogeneous GraphTensor of rank 0 with a single component."""
+
+  def call(self, inputs):
+    node_sizes = tf.shape(inputs['node_features'])[0]
+    edge_sizes = tf.shape(inputs['edge_weights'])[0]
+    return tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            'nodes': tfgnn.NodeSet.from_fields(
+                sizes=tf.expand_dims(node_sizes, axis=0),
+                features={tfgnn.HIDDEN_STATE: inputs['node_features']},
+            )
+        },
+        edge_sets={
+            'edges': tfgnn.EdgeSet.from_fields(
+                sizes=tf.expand_dims(edge_sizes, axis=0),
+                adjacency=tfgnn.Adjacency.from_indices(
+                    ('nodes', inputs['source']), ('nodes', inputs['target'])
+                ),
+                features={'edge_weights': inputs['edge_weights']},
+            )
+        },
+    )
+
+
 if __name__ == '__main__':
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/gpt_gnn/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/examples.proto`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-# Copyright 2021 The TensorFlow GNN Authors. All Rights Reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-# ==============================================================================
-"""GPT-GNN.
+// Copyright 2021 The TensorFlow GNN Authors. All Rights Reserved.
+//
+// Licensed under the Apache License, Version 2.0 (the "License");
+// you may not use this file except in compliance with the License.
+// You may obtain a copy of the License at
+//
+//     http://www.apache.org/licenses/LICENSE-2.0
+//
+// Unless required by applicable law or agreed to in writing, software
+// distributed under the License is distributed on an "AS IS" BASIS,
+// WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+// See the License for the specific language governing permissions and
+// limitations under the License.
+// =============================================================================
+syntax = "proto2";
 
-Users of TF-GNN can use this model by importing it next to the core library as
+package tensorflow_gnn.testdata;
 
-```python
-import tensorflow_gnn as tfgnn
-from tensorflow_gnn.models import gpt_gnn
-```
-"""
-from tensorflow_gnn.models.gpt_gnn import tensor_utils
+import "tensorflow/core/example/example.proto";
 
-sample_unconnected_nodes = tensor_utils.sample_unconnected_nodes
+// Specifies one or more Examples. This is used to aid testing readability by
+// allowing us to specify multiple Examples in an ASCII proto file.
+message ExampleList {
+  repeated tensorflow.Example examples = 1;
+}
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contains GraphSAGE convolution layer implementations."""
 
-import collections
 import copy
 from typing import Any, Callable, Collection, Optional, Set, Union
 
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 
 
@@ -470,30 +469,30 @@
     if self._use_bias:
       result += self._bias_term
     result = self._activation(result)
     return {self._self_node_feature: result}
 
 
 @tf.keras.utils.register_keras_serializable(package="GraphSAGE")
-def GraphSAGEGraphUpdate(*,
-                         units: int,
-                         hidden_units: Optional[int] = None,
-                         receiver_tag: tfgnn.IncidentNodeTag,
-                         node_set_names: Optional[
-                             Collection[tfgnn.NodeSetName]] = None,
-                         reduce_type: str = "mean",
-                         use_pooling: bool = True,
-                         use_bias: bool = True,
-                         dropout_rate: float = 0.0,
-                         l2_normalize: bool = True,
-                         combine_type: str = "sum",
-                         activation: Union[str, Callable[..., Any]] = "relu",
-                         feature_name: str = tfgnn.HIDDEN_STATE,
-                         name: str = "graph_sage",
-                         **kwargs):
+def GraphSAGEGraphUpdate(  # To be called like a class initializer.  pylint: disable=invalid-name
+    *,
+    units: int,
+    hidden_units: Optional[int] = None,
+    receiver_tag: tfgnn.IncidentNodeTag,
+    node_set_names: Optional[Collection[tfgnn.NodeSetName]] = None,
+    reduce_type: str = "mean",
+    use_pooling: bool = True,
+    use_bias: bool = True,
+    dropout_rate: float = 0.0,
+    l2_normalize: bool = True,
+    combine_type: str = "sum",
+    activation: Union[str, Callable[..., Any]] = "relu",
+    feature_name: str = tfgnn.HIDDEN_STATE,
+    name: str = "graph_sage",
+    **kwargs) -> tf.keras.layers.Layer:
   """Returns a GraphSAGE GraphUpdater layer for nodes in node_set_names.
 
   For more information on GraphSAGE algorithm please refer to
   [Hamilton et al., 2017](https://arxiv.org/abs/1706.02216).
   Returned layer applies only one step of GraphSAGE convolution over the
   incident nodes of the edge_set_name_list for the specified node_set_name node.
 
@@ -502,19 +501,19 @@
       final aggregated sender node features as well as the self node feature.
     hidden_units: Number of output units to be configure for GraphSAGE pooling
       type convolution only.
     receiver_tag: Either one of `tfgnn.SOURCE` or `tfgnn.TARGET`. The results of
       GraphSAGE are aggregated for this graph piece. When set to `tfgnn.SOURCE`
       or `tfgnn.TARGET`, the layer is called for an edge set and will aggregate
       results at the specified endpoint of the edges.
-    node_set_names: A set (or convertible container) of node_set_names for which
-      the GraphSAGE graph update happens over each of their incident edges,
-      where node_set_name is configured as the receiver_tag end.
-      If unset, defaults to all node sets that receive from at least one edge
-      set.
+    node_set_names: By default, this layer updates all node sets that receive
+      from at least one edge set. Optionally, this argument can specify a subset
+      of those node sets. It is not allowed to include node sets that do not
+      receive messages from any edge set. It is also not allowed to include
+      auxiliary node sets.
     reduce_type: An aggregation operation name. Supported list of aggregation
       operators can be found at `tfgnn.get_registered_reduce_operation_names()`.
     use_pooling: If enabled, `graph_sage.GraphSAGEPoolingConv` will be used,
       otherwise `graph_sage.GraphSAGEAggregatorConv` will be executed for the
       provided edges.
     use_bias: If true a bias term will be added to the linear transformations
       for the incident node features as well as for the self node feature.
@@ -532,65 +531,65 @@
     feature_name: The feature name of node states; defaults to
       `tfgnn.HIDDEN_STATE`.
     name: Optionally, a name for the layer returned.
     **kwargs: Any optional arguments to `graph_sage.GraphSAGEPoolingConv`,
       `graph_sage.GraphSAGEAggregatorConv` or `graph_sage.GraphSAGENextState`,
       see there.
   """
-  if node_set_names is not None:
-    node_set_names = set(node_set_names)
-
-  # graph_update_callback is deferred until we get the graph spec.
-  def GraphUpdateCallback(spec: tfgnn.GraphTensorSpec):
-    if use_pooling != (hidden_units is not None):
-      raise ValueError(
-          "Either use_pooling or hidden_units has been configured without the "
-          "other, please configure them together or disable them both.")
-    node_set_update_dict = collections.defaultdict(dict)
-    for edge_set_name, edge_set_spec in spec.edge_sets_spec.items():
-      node_set_name = edge_set_spec.adjacency_spec.node_set_name(receiver_tag)
-      if node_set_names is None or node_set_name in node_set_names:
-        if use_pooling:
-          node_set_update_dict[node_set_name][
-              edge_set_name] = GraphSAGEPoolingConv(
-                  receiver_tag=receiver_tag,
-                  sender_node_feature=feature_name,
-                  reduce_type=reduce_type,
-                  units=units,
-                  hidden_units=hidden_units,
-                  use_bias=use_bias,
-                  dropout_rate=dropout_rate,
-                  **kwargs)
-        else:
-          node_set_update_dict[node_set_name][
-              edge_set_name] = GraphSAGEAggregatorConv(
-                  receiver_tag=receiver_tag,
-                  reduce_type=reduce_type,
-                  sender_node_feature=feature_name,
-                  units=units,
-                  dropout_rate=dropout_rate,
-                  **kwargs)
-    node_set_updates = dict()
-    for node_set_name, edge_set_update_dict in node_set_update_dict.items():
-      node_set_updates[node_set_name] = tfgnn.keras.layers.NodeSetUpdate(
-          edge_set_update_dict,
-          next_state=GraphSAGENextState(
-              units=units,
-              use_bias=use_bias,
-              dropout_rate=dropout_rate,
-              feature_name=feature_name,
-              l2_normalize=l2_normalize,
-              combine_type=combine_type,
-              activation=activation,
-              **kwargs),
-          node_input_feature=feature_name)
-    return dict(node_sets=node_set_updates)
+  if use_pooling != (hidden_units is not None):
+    raise ValueError(
+        "Either use_pooling or hidden_units has been configured without the "
+        "other, please configure them together or disable them both.")
+
+  def convolutions_factory(edge_set_name, receiver_tag):
+    del edge_set_name  # Unused.
+    if use_pooling:
+      return GraphSAGEPoolingConv(
+          receiver_tag=receiver_tag,
+          sender_node_feature=feature_name,
+          reduce_type=reduce_type,
+          units=units,
+          hidden_units=hidden_units,
+          use_bias=use_bias,
+          dropout_rate=dropout_rate,
+          **kwargs)
+    else:
+      return GraphSAGEAggregatorConv(
+          receiver_tag=receiver_tag,
+          reduce_type=reduce_type,
+          sender_node_feature=feature_name,
+          units=units,
+          dropout_rate=dropout_rate,
+          **kwargs)
+
+  def nodes_next_state_factory(node_set_name):
+    del node_set_name  # Unused.
+    return GraphSAGENextState(
+        units=units,
+        use_bias=use_bias,
+        dropout_rate=dropout_rate,
+        feature_name=feature_name,
+        l2_normalize=l2_normalize,
+        combine_type=combine_type,
+        activation=activation,
+        **kwargs)
 
-  return tfgnn.keras.layers.GraphUpdate(
-      deferred_init_callback=GraphUpdateCallback, name=name)
+  def node_set_update_factory(node_set_name, edge_set_inputs, next_state):
+    del node_set_name  # Unused.
+    return tfgnn.keras.layers.NodeSetUpdate(
+        edge_set_inputs=edge_set_inputs,
+        next_state=next_state,
+        node_input_feature=feature_name)
+
+  gnn_builder = tfgnn.keras.ConvGNNBuilder(
+      convolutions_factory,
+      nodes_next_state_factory,
+      node_set_update_factory=node_set_update_factory,
+      receiver_tag=receiver_tag)
+  return gnn_builder.Convolve(node_set_names, name=name)
 
 
 @tf.keras.utils.register_keras_serializable(package="GraphSAGE")
 class GraphSAGENextState(tf.keras.layers.Layer):
   r"""GraphSAGENextState: compute new node states with GraphSAGE algorithm.
 
   This layer lets you compute a GraphSAGE update of node states from the
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/graph_sage/layers_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/graph_sage/layers_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -183,19 +183,19 @@
         units=out_units,
         feature_name=_FEATURE_NAME)
     _ = layer(graph)
     weights = {v.name: v for v in layer.trainable_weights}
     self.assertLen(weights, 3)
     node_dims = 30
     weights[
-        "graph_sage/node_set_update/graph_sage_aggregator_conv/dense/kernel:0"].assign(
-            tf.eye(node_dims))
+        "graph_sage/node_set_update/graph_sage_aggregator_conv/dense/kernel:0"
+    ].assign(tf.eye(node_dims))
     weights[
-        "graph_sage/node_set_update/graph_sage_next_state/dense_1/kernel:0"].assign(
-            tf.eye(node_dims))
+        "graph_sage/node_set_update/graph_sage_next_state/dense_1/kernel:0"
+    ].assign(tf.eye(node_dims))
     bias_shape = out_units
     weights["graph_sage/node_set_update/graph_sage_next_state/bias:0"].assign(
         [0.] * bias_shape)
     inputs = tf.keras.layers.Input(type_spec=graph.spec)
     outputs = layer(inputs)
     model = tf.keras.Model(inputs, outputs)
     if reload_model:
@@ -282,44 +282,44 @@
     else:
       self.assertLen(weights, 4)
     paper_node_dims = 3
     institution_node_dims = 4
     target_node_dims = 2
     if use_pooling:
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/kernel:0"].assign(
-              [[1.]] * paper_node_dims)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/kernel:0"
+      ].assign([[1.0]] * paper_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/bias:0"].assign(
-              [0.])
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/bias:0"
+      ].assign([0.0])
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_1/kernel:0"].assign(
-              [[1.]] * out_units)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_1/kernel:0"
+      ].assign([[1.0]] * out_units)
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/kernel:0"].assign(
-              [[1.]] * institution_node_dims)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/kernel:0"
+      ].assign([[1.0]] * institution_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/bias:0"].assign(
-              [0.])
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/bias:0"
+      ].assign([0.0])
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_3/kernel:0"].assign(
-              [[1.]] * out_units)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_3/kernel:0"
+      ].assign([[1.0]] * out_units)
       weights[
-          "graph_sage/node_set_update/graph_sage_next_state/dense_4/kernel:0"].assign(
-              [[1.]] * target_node_dims)
+          "graph_sage/node_set_update/graph_sage_next_state/dense_4/kernel:0"
+      ].assign([[1.0]] * target_node_dims)
     else:
       weights[
-          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense/kernel:0"].assign(
-              [[1.]] * paper_node_dims)
+          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense/kernel:0"
+      ].assign([[1.0]] * paper_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense_1/kernel:0"].assign(
-              [[1.]] * institution_node_dims)
+          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense_1/kernel:0"
+      ].assign([[1.0]] * institution_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_next_state/dense_2/kernel:0"].assign(
-              [[1.]] * target_node_dims)
+          "graph_sage/node_set_update/graph_sage_next_state/dense_2/kernel:0"
+      ].assign([[1.0]] * target_node_dims)
     num_edge_type = 2
     bias_shape = out_units if combine_type == "sum" else out_units * (
         num_edge_type + 1)
     weights["graph_sage/node_set_update/graph_sage_next_state/bias:0"].assign(
         [0.] * bias_shape)
     inputs = tf.keras.layers.Input(type_spec=graph.spec)
     outputs = layer(inputs)
@@ -371,14 +371,27 @@
                              [2., 6., 6.]]),
             "sum":
                 tf.constant([[13.], [14.], [7.], [14.]])
         }
     }
     self.assertAllClose(actual, expected_outputs[normalize][combine_type])
 
+  def testReceivingRequired(self):
+    graph = _get_test_graph()
+    assert not any(edge_set.adjacency.target_name == "paper"
+                   for edge_set in graph.edge_sets.values())
+    layer = graph_sage.GraphSAGEGraphUpdate(
+        node_set_names={"author", "paper"},
+        receiver_tag=tfgnn.TARGET,
+        units=1,
+        hidden_units=1,
+        feature_name=_FEATURE_NAME)
+    with self.assertRaisesRegex(ValueError, r"not .* from any edge set.*paper"):
+      _ = layer(graph)
+
   @parameterized.named_parameters(
       ("E2ELoadKerasMeanPool", "mean", True, ReloadModel.KERAS),
       ("E2ELoadKerasMeanAgg", "mean", False, ReloadModel.KERAS),
       ("E2ELoadKerasMaxPool", "max", True, ReloadModel.KERAS),
       ("E2ELoadKerasMaxAgg", "max", False, ReloadModel.KERAS),
       ("E2ELoadKerasMaxNoInfPool", "max_no_inf", True, ReloadModel.KERAS),
       ("E2ELoadKerasMaxNoInfAgg", "max_no_inf", False, ReloadModel.KERAS),
@@ -389,15 +402,15 @@
                                   False, ReloadModel.SAVED_MODEL),
       ("E2ELoadSavedModelMeanPool", "mean", True, ReloadModel.SAVED_MODEL),
       ("E2ELoadSavedModelMeanAgg", "mean", False, ReloadModel.SAVED_MODEL))
   def testModelLoad(self, reduce_operation, use_pooling, reload_model):
     graph = _get_test_graph()
     out_units = 1
     layer = graph_sage.GraphSAGEGraphUpdate(
-        node_set_names={"author", "paper"},
+        node_set_names={"author"},
         receiver_tag=tfgnn.TARGET,
         reduce_type=reduce_operation,
         combine_type="concat",
         use_pooling=use_pooling,
         units=out_units,
         hidden_units=out_units if use_pooling else None,
         feature_name=_FEATURE_NAME)
@@ -408,44 +421,44 @@
     else:
       self.assertLen(weights, 4)
     paper_node_dims = 3
     institution_node_dims = 4
     target_node_dims = 2
     if use_pooling:
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/kernel:0"].assign(
-              [[1.]] * paper_node_dims)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/kernel:0"
+      ].assign([[1.0]] * paper_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/bias:0"].assign(
-              [0.])
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense/bias:0"
+      ].assign([0.0])
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_1/kernel:0"].assign(
-              [[1.]] * out_units)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_1/kernel:0"
+      ].assign([[1.0]] * out_units)
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/kernel:0"].assign(
-              [[1.]] * institution_node_dims)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/kernel:0"
+      ].assign([[1.0]] * institution_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/bias:0"].assign(
-              [0.])
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_2/bias:0"
+      ].assign([0.0])
       weights[
-          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_3/kernel:0"].assign(
-              [[1.]] * out_units)
+          "graph_sage/node_set_update/graph_sage_pooling_conv/dense_3/kernel:0"
+      ].assign([[1.0]] * out_units)
       weights[
-          "graph_sage/node_set_update/graph_sage_next_state/dense_4/kernel:0"].assign(
-              [[1.]] * target_node_dims)
+          "graph_sage/node_set_update/graph_sage_next_state/dense_4/kernel:0"
+      ].assign([[1.0]] * target_node_dims)
     else:
       weights[
-          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense/kernel:0"].assign(
-              [[1.]] * paper_node_dims)
+          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense/kernel:0"
+      ].assign([[1.0]] * paper_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense_1/kernel:0"].assign(
-              [[1.]] * institution_node_dims)
+          "graph_sage/node_set_update/graph_sage_aggregator_conv/dense_1/kernel:0"
+      ].assign([[1.0]] * institution_node_dims)
       weights[
-          "graph_sage/node_set_update/graph_sage_next_state/dense_2/kernel:0"].assign(
-              [[1.]] * target_node_dims)
+          "graph_sage/node_set_update/graph_sage_next_state/dense_2/kernel:0"
+      ].assign([[1.0]] * target_node_dims)
     num_edge_type = 2
     bias_shape = out_units * (num_edge_type + 1)
     weights["graph_sage/node_set_update/graph_sage_next_state/bias:0"].assign(
         [0.] * bias_shape)
     inputs = tf.keras.layers.Input(type_spec=graph.spec)
     outputs = layer(inputs)
     model = tf.keras.Model(inputs, outputs)
@@ -573,9 +586,101 @@
         use_bias=True,
         reduce_type="max_no_inf")
     self.assertRaisesRegex(ValueError,
                            r".* isn't supported, please instead use any of .*",
                            lambda: conv(graph, node_set_name="author"))
 
 
+class GraphSAGETFLiteTest(tf.test.TestCase, parameterized.TestCase):
+
+  @parameterized.named_parameters(
+      ("WithPooling", True, 4, "sum"),
+      ("SumAggregation", False, None, "sum"),
+      ("ConcatAggregation", False, None, "concat"))
+  def testBasic(self, use_pooling, hidden_units, combine_type):
+    test_graph_1_dict = {
+        # We care that the TFLite interpreter gives the same output as the
+        # model, which was tested separately.
+        "source": tf.constant([0, 1, 2, 0, 2, 1]),
+        "target": tf.constant([1, 2, 0, 2, 1, 0]),
+        "node_features": tf.constant([
+            [1.0, 0.0, 0.0, 1.0],
+            [0.0, 1.0, 0.0, 2.0],
+            [0.0, 0.0, 1.0, 3.0],
+        ]),
+        "edge_features": tf.constant([
+            [3.0],
+            [6.0],
+            [9.0],
+            [2.0],
+            [6.0],
+            [4.0],
+        ]),
+    }
+
+    layer = graph_sage.GraphSAGEGraphUpdate(
+        units=4,
+        receiver_tag=tfgnn.TARGET,
+        use_bias=True,
+        use_pooling=use_pooling,
+        hidden_units=hidden_units,
+        combine_type=combine_type,
+        feature_name=tfgnn.HIDDEN_STATE,
+    )
+
+    inputs = {
+        "node_features": tf.keras.Input([4], None, "node_features", tf.float32),
+        "source": tf.keras.Input([], None, "source", tf.int32),
+        "target": tf.keras.Input([], None, "target", tf.int32),
+        "edge_features": tf.keras.Input([1], None, "edge_features", tf.float32),
+    }
+    graph_in = _MakeGraphTensor()(inputs)
+    graph_out = layer(graph_in)
+    outputs = tf.keras.layers.Layer(name="final_node_states")(
+        graph_out.node_sets["nodes"][tfgnn.HIDDEN_STATE]
+    )
+    model = tf.keras.Model(inputs, outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = model(test_graph_1_dict).numpy()
+
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith("2.10."):
+      self.skipTest("GNN models are unsupported in TFLite until TF 2.11 but "
+                    f"got TF {tf.__version__}")
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner("serving_default")
+    obtained = signature_runner(**test_graph_1_dict)["final_node_states"]
+    self.assertAllClose(expected, obtained)
+
+
+# TODO(b/274779989): Replace this layer with a more standard representation
+# of GraphTensor as a dict of plain Tensors.
+class _MakeGraphTensor(tf.keras.layers.Layer):
+  """Makes a homogeneous GraphTensor of rank 0 with a single component."""
+
+  def call(self, inputs):
+    node_sizes = tf.shape(inputs["node_features"])[0]
+    edge_sizes = tf.shape(inputs["edge_features"])[0]
+    return tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            "nodes": tfgnn.NodeSet.from_fields(
+                sizes=tf.expand_dims(node_sizes, axis=0),
+                features={tfgnn.HIDDEN_STATE: inputs["node_features"]},
+            )
+        },
+        edge_sets={
+            "edges": tfgnn.EdgeSet.from_fields(
+                sizes=tf.expand_dims(edge_sizes, axis=0),
+                adjacency=tfgnn.Adjacency.from_indices(
+                    ("nodes", inputs["source"]), ("nodes", inputs["target"])
+                ),
+                features={tfgnn.HIDDEN_STATE: inputs["edge_features"]},
+            )
+        },
+    )
+
+
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/BUILD`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
+package(default_visibility = ["//visibility:public"])
 
-licenses(["notice"])
+licenses(["notice"])  # Apache 2.0
 
-package(
-    default_visibility = [":__subpackages__"],
-)
-
-package_group(name = "users")
+load("@com_google_protobuf//:protobuf.bzl", "py_proto_library")
 
-pytype_strict_library(
-    name = "hgt",
-    srcs = ["__init__.py"],
+py_proto_library(
+    name = "graph_schema_py_proto",
+    srcs = ["graph_schema.proto"],
+    default_runtime = "@com_google_protobuf//:protobuf_python",
+    protoc = "@com_google_protobuf//:protoc",
     srcs_version = "PY3",
-    visibility = [
-        ":__subpackages__",
-        ":users",
+    deps = [
+        "@com_google_protobuf//:protobuf_python",
+        "@org_tensorflow//tensorflow/core:protos_all_py",
     ],
-    deps = [],
 )
 
-pytype_strict_library(
-    name = "softmax",
-    srcs = ["softmax.py"],
+py_library(
+    name = "graph_schema",
+    srcs = ["graph_schema.py"],
     srcs_version = "PY3",
     deps = [
-        "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
+        ":graph_schema_py_proto",
     ],
 )
 
-tf_py_test(
-    name = "softmax_test",
-    srcs = ["softmax_test.py"],
+py_proto_library(
+    name = "examples_py_proto",
+    srcs = ["examples.proto"],
+    default_runtime = "@com_google_protobuf//:protobuf_python",
+    protoc = "@com_google_protobuf//:protoc",
     srcs_version = "PY3",
     deps = [
-        ":softmax",
-        "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
+        "@com_google_protobuf//:protobuf_python",
+        "@org_tensorflow//tensorflow/core:protos_all_py",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/hgt/softmax.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/label_fns.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,72 @@
-# Copyright 2022 The TensorFlow GNN Authors. All Rights Reserved.
+# Copyright 2023 The TensorFlow GNN Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Contains the softmax implementation for Heterogeneous Graph Transformer.
-"""
+"""Label readout helpers."""
 from __future__ import annotations
 
-from typing import Mapping
-
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 
 
-def _correct_node_set_at_tag(
-    gt, edge_set_name, node_set_name, node_tag):
-
-  return gt.edge_sets[edge_set_name].adjacency.node_set_name(
-      node_tag) == node_set_name
-
-
-def global_segmented_softmax_edges_per_node(
-    graph: tfgnn.GraphTensor,
-    node_tag: tfgnn.IncidentNodeTag,
-    feature_values: Mapping[tfgnn.EdgeSetName, tfgnn.Field],
-) -> tfgnn.Fields:
-  """softmax() over edges where `node_set_name` is the `node_tag` node."""
-
-  # Ensure that all the edge sets have the same node_set at the desired node_tag
-  if len(
-      set(graph.edge_sets[edge_set_name].adjacency.node_set_name(node_tag)
-          for edge_set_name in feature_values)) != 1:
-    msg_tag = "target" if node_tag == 1 else "source"
-    raise ValueError(
-        f"all edge sets in feature_values need the same {msg_tag} node set")
-
-  maxes = []
-  exps_by_edge = {}
-  sumexps = []
-  softmax_segments = {}
-  # First get the maxes to subtract out
-  for edge_set_name, value in feature_values.items():
-    maxes.append(
-        tfgnn.pool_edges_to_node(
-            graph,
-            edge_set_name,
-            node_tag,
-            reduce_type="max",
-            feature_value=value))
-
-  max_by_node = tf.keras.layers.maximum(maxes)
-
-  # Next get all the offset exp sums, saving the per-edge exp sums
-  for edge_set_name, value in feature_values.items():
-    max_cast = tfgnn.broadcast_node_to_edges(
-        graph,
-        edge_set_name,
-        node_tag,
-        feature_value=max_by_node,
-    )
-    exps_by_edge[edge_set_name] = tf.exp(value - max_cast)
-    sumexps.append(
-        tfgnn.pool_edges_to_node(
-            graph,
-            edge_set_name,
-            node_tag,
-            reduce_type="sum",
-            feature_value=exps_by_edge[edge_set_name],
-        ))
-  sum_by_node = tf.math.add_n(sumexps)
-
-  # Finally compute the softmax segments per edge set
-  for edge_set_name, exps in exps_by_edge.items():
-    softmax_segments[edge_set_name] = (
-        exps / tfgnn.broadcast_node_to_edges(
-            graph, edge_set_name, node_tag, feature_value=sum_by_node))
-  return softmax_segments
+@tf.keras.utils.register_keras_serializable(package="GNN")
+class ContextLabelFn(tf.keras.layers.Layer):
+  """Reads out a context `tfgnn.Field`."""
+
+  def __init__(self, feature_name: str, **kwargs):
+    super().__init__(**kwargs)
+    self._feature_name = feature_name
+
+  def call(
+      self,
+      inputs: tfgnn.GraphTensor) -> tuple[tfgnn.GraphTensor, tfgnn.Field]:
+    if not tfgnn.is_graph_tensor(inputs):
+      raise ValueError(f"Expected `GraphTensor` inputs (got {inputs})")
+    y = inputs.context[self._feature_name]
+    x = inputs.remove_features(context=(self._feature_name,))
+    return x, y
+
+  def  get_config(self):
+    return dict(feature_name=self._feature_name, **super().get_config())
+
+
+@tf.keras.utils.register_keras_serializable(package="GNN")
+class RootNodeLabelFn(tf.keras.layers.Layer):
+  """Reads out a root node `tfgnn.Field`."""
+
+  def __init__(
+      self,
+      node_set_name: tfgnn.NodeSetName,
+      *,
+      feature_name: tfgnn.FieldName = tfgnn.HIDDEN_STATE,
+      **kwargs):
+    super().__init__(**kwargs)
+    self._node_set_name = node_set_name
+    self._feature_name = feature_name
+
+  def call(
+      self,
+      inputs: tfgnn.GraphTensor) -> tuple[tfgnn.GraphTensor, tfgnn.Field]:
+    y = tfgnn.gather_first_node(
+        inputs,
+        self._node_set_name,
+        feature_name=self._feature_name)
+    node_sets = {self._node_set_name: (self._feature_name,)}
+    x = inputs.remove_features(node_sets=node_sets)
+    return x, y
+
+  def  get_config(self):
+    return dict(
+        node_set_name=self._node_set_name,
+        feature_name=self._feature_name,
+        **super().get_config())
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 from ml_collections import config_dict
 import tensorflow as tf
 from tensorflow_gnn.models.multi_head_attention import layers
 
 
 def graph_update_get_config_dict() -> config_dict.ConfigDict:
   """Returns ConfigDict for graph_update_from_config_dict() with defaults."""
-  # Keep in sync with default args of
-  # MultiHeadAttentionMPNNGraphUpdate.__init__.
+  # LINT.IfChange(graph_update_get_config_dict)
   cfg = config_dict.ConfigDict()
   cfg.units = config_dict.placeholder(int)  # Sets type to Optional[int].
   cfg.message_dim = config_dict.placeholder(int)
   cfg.num_heads = config_dict.placeholder(int)
   cfg.receiver_tag = config_dict.placeholder(int)
   cfg.l2_regularization = 0.0
   cfg.edge_dropout_rate = 0.0
   cfg.state_dropout_rate = 0.0
   cfg.conv_activation = "relu"
   cfg.activation = "relu"
   cfg.lock()
+  # LINT.ThenChange(./layers.py:MultiHeadAttentionMPNNGraphUpdate_args)
   return cfg
 
 
 def graph_update_from_config_dict(
     cfg: config_dict.ConfigDict) -> tf.keras.layers.Layer:
   """Returns a MultiHeadAttentionMPNNGraphUpdate initialized from `cfg`.
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/config_dict_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/config_dict_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,19 +43,20 @@
         message_dim=message_dim,
         num_heads=num_heads,
         receiver_tag=receiver_tag)
 
     self.assertEqual(to_model_config(actual), to_model_config(expected))
 
 
+# TODO(b/265776928): De-duplicate the multiple copies of this test helper.
 def to_model_config(layer: tf.keras.layers.Layer):
   """Returns a parsed model config for `layer`, without `"name"` fields."""
   # Need a full model to serialize *recursively*.
   model = tf.keras.Sequential([layer])
-  # Subobjects are only build in the first call.
+  # Subobjects are only built in the first call.
   _ = model(_make_test_graph_loop())
   model_config = json.loads(model.to_json())
   # The names of layers are uniquified and impede the hparam comparison.
   return _remove_names(model_config)
 
 
 def _remove_names(obj):
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,37 +127,41 @@
       node set.
       If left unset for init, the tag must be passed at call time.
     receiver_feature: Can be set to override `tfgnn.HIDDEN_STATE`
       for use as the receiver's input feature to attention. (The attention key
       is derived from this input.)
     sender_node_feature: Can be set to override `tfgnn.HIDDEN_STATE`
       for use as the input feature from sender nodes to attention.
-      IMPORANT: Must be set to `None` for use with `receiver_tag=tfgnn.CONTEXT`
+      IMPORTANT: Must be set to `None` for use with `receiver_tag=tfgnn.CONTEXT`
       on an edge set, or for pooling from edges without sender node states.
     sender_edge_feature: Can be set to a feature name of the edge set to select
       it as an input feature. By default, this set to `None`, which disables
       this input.
       IMPORTANT: Must be set for use with `receiver_tag=tfgnn.CONTEXT`
       on an edge set.
     use_bias: If true, bias terms are added to the transformations of query,
       key and value inputs.
     edge_dropout: Can be set to a dropout rate for edge dropout. (When pooling
       nodes to context, it's the node's membership in a graph component that
       is dropped out.)
+    inputs_dropout: Dropout rate for random dropout on the inputs to this
+      convolution layer, i.e. the receiver, sender node, and sender edge inputs.
     attention_activation: The nonlinearity used on the transformed inputs
       (query, and keys if `transform_keys` is `True`) before computing the
       attention scores. This can be specified as a Keras layer, a
       tf.keras.activations.* function, or a string understood by
-      tf.keras.layers.Activation(). Defaults to None.
+      `tf.keras.layers.Activation`. Defaults to None.
     activation: The nonlinearity applied to the final result of attention,
       specified in the same ways as attention_activation.
     kernel_initializer: Can be set to a `kernel_initializer` as understood
-      by tf.keras.layers.Dense etc.
-    kernel_regularizer: Can be set to a `kernel_regularizer` as understood
-      by tf.keras.layers.Dense etc.
+      by `tf.keras.layers.Dense` etc.
+      An `Initializer` object gets cloned before use to ensure a fresh seed,
+      if not set explicitly. For more, see `tfgnn.keras.clone_initializer()`.
+    kernel_regularizer: Can be set to a `kernel_regularized` as understood
+      by `tf.keras.layers.Dense` etc.
     transform_keys: If true, transform both queries and keys inputs. Otherwise,
       only queries are transformed since the two transformations on queries and
       keys are equivalent to one. (The presence of transformations on values is
       independent of this arg.)
     score_scaling: One of either `"none"`, `"rsqrt_dim"`, or
       `"trainable_sigmoid"`. If set to `"rsqrt_dim"`, the attention scores are
       divided by the square root of the dimension of keys (i.e.,
@@ -169,35 +173,32 @@
       layer converge. Defaults to `"rsqrt_dim"`.
     transform_values_after_pooling: By default, each attention head applies
       the value transformation, then pools with attention coefficients.
       Setting this option pools inputs with attention coefficients, then applies
       the transformation. This is mathematically equivalent but can be faster
       or slower to compute, depending on the platform and the dataset.
       IMPORTANT: Toggling this option breaks checkpoint compatibility.
-      IMPORTANT: Setting this option requires TensorFlow 2.10 or greater,
-      because it uses `tf.keras.layers.EinsumDense`.
   """
 
   def __init__(
       self,
       *,
       num_heads: int,
       per_head_channels: int,
       receiver_tag: Optional[tfgnn.IncidentNodeOrContextTag] = None,
       receiver_feature: tfgnn.FieldName = tfgnn.HIDDEN_STATE,
       sender_node_feature: Optional[tfgnn.FieldName] = tfgnn.HIDDEN_STATE,
       sender_edge_feature: Optional[tfgnn.FieldName] = None,
       use_bias: bool = True,
       edge_dropout: float = 0.,
+      inputs_dropout: float = 0.,
       attention_activation: Optional[Union[str, Callable[..., Any]]] = None,
       activation: Union[str, Callable[..., Any]] = "relu",
-      kernel_initializer: Union[None, str,
-                                tf.keras.initializers.Initializer] = None,
-      kernel_regularizer: Union[None, str,
-                                tf.keras.regularizers.Regularizer] = None,
+      kernel_initializer: Any = None,
+      kernel_regularizer: Any = None,
       transform_keys: bool = True,
       score_scaling: Literal["none", "rsqrt_dim",
                              "trainable_sigmoid"] = "rsqrt_dim",
       transform_values_after_pooling: bool = False,
       **kwargs):
     kwargs.setdefault("name", "multi_head_attention_conv")
     super().__init__(
@@ -219,21 +220,18 @@
     if per_head_channels <= 0:
       raise ValueError(
           f"Per-head channels {per_head_channels} must be greater than 0.")
     self._per_head_channels = per_head_channels
 
     self._use_bias = use_bias
 
-    if not 0 <= edge_dropout < 1:
-      raise ValueError(f"Edge dropout {edge_dropout} must be in [0, 1).")
-    self._edge_dropout = edge_dropout
-    if self._edge_dropout > 0:
-      self._edge_dropout_layer = tf.keras.layers.Dropout(self._edge_dropout)
-    else:
-      self._edge_dropout_layer = None
+    # Create dropout layers. Note that if the dropout rate is zero, then the
+    # layer will just be a pass-through.
+    self._edge_dropout_layer = tf.keras.layers.Dropout(edge_dropout)
+    self._inputs_dropout_layer = tf.keras.layers.Dropout(inputs_dropout)
 
     # Check for conflicting options.
     if attention_activation is not None and score_scaling != "none":
       warnings.warn(
           "using both an activation on transformed inputs and score scaling "
           "may lead to degraded accuracy if the activation function restricts "
           "the range of the values, e.g. 'tanh' which restricts the values to "
@@ -241,14 +239,15 @@
 
     # Check for valid inputs.
     if (not self.takes_sender_node_input and not self.takes_sender_edge_input):
       raise ValueError("MultiHeadAttentionConv initialized with no inputs.")
 
     self._attention_activation = tf.keras.activations.get(attention_activation)
     self._activation = tf.keras.activations.get(activation)
+    # IMPORTANT: Use with tfgnn.keras.clone_initializer(), b/268648226.
     self._kernel_initializer = tf.keras.initializers.get(kernel_initializer)
     self._kernel_regularizer = tf.keras.regularizers.get(kernel_regularizer)
     self._transform_keys = transform_keys
     self._score_scaling = score_scaling
     self._transform_values_after_pooling = transform_values_after_pooling
 
     # The creation of queries transfomations is deferred to the first call of
@@ -260,78 +259,75 @@
     if not self._transform_keys:
       self._w_sender_node_to_key = None
       self._w_sender_edge_to_key = None
     else:
       if self.takes_sender_node_input:
         self._w_sender_node_to_key = tf.keras.layers.Dense(
             per_head_channels * num_heads,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                self._kernel_initializer),
             kernel_regularizer=kernel_regularizer,
             use_bias=use_bias,
             name="key_node")
       else:
         self._w_sender_node_to_key = None
       if self.takes_sender_edge_input:
         self._w_sender_edge_to_key = tf.keras.layers.Dense(
             per_head_channels * num_heads,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                self._kernel_initializer),
             kernel_regularizer=kernel_regularizer,
             # This bias would be redundant with self._w_sender_node_to_key.
             use_bias=use_bias and self._w_sender_node_to_key is None,
             name="key_edge")
       else:
         self._w_sender_edge_to_key = None
 
     if not self._transform_values_after_pooling:
       if self.takes_sender_node_input:
         self._w_sender_node_to_value = tf.keras.layers.Dense(
             per_head_channels * num_heads,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                self._kernel_initializer),
             kernel_regularizer=kernel_regularizer,
             use_bias=use_bias,
             name="value_node")
       else:
         self._w_sender_node_to_value = None
       if self.takes_sender_edge_input:
         self._w_sender_edge_to_value = tf.keras.layers.Dense(
             per_head_channels * num_heads,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                self._kernel_initializer),
             kernel_regularizer=kernel_regularizer,
             # This bias would be redundant with self._w_sender_node_to_value.
             use_bias=use_bias and self._w_sender_node_to_value is None,
             name="value_edge")
       else:
         self._w_sender_edge_to_value = None
     else:
-      # TODO(b/266868417): Remove when TF2.10+ is required by all of TF-GNN.
-      try:
-        _ = tf.keras.layers.EinsumDense
-      except AttributeError as e:
-        raise ValueError(
-            "MultiHeadAttentionConv(transform_values_after_pooling=True) "
-            "requires tf.keras.layers.EinsumDense from "
-            f"TensorFlow 2.10 or newer, got TensorFlow {tf.__version__}"
-        ) from e
       self._w_sender_pooled_to_value = tf.keras.layers.EinsumDense(
           equation="...hv,hvc->...hc",
           output_shape=(num_heads, per_head_channels),
           bias_axes="hc" if use_bias else None,
-          kernel_initializer=kernel_initializer,
+          kernel_initializer=tfgnn.keras.clone_initializer(
+              self._kernel_initializer),
           kernel_regularizer=kernel_regularizer,
           name="value_pooled")
 
     if self._score_scaling == "trainable_sigmoid":
       self._score_scaling_weight = None
 
   def get_config(self):
     return dict(
         num_heads=self._num_heads,
         per_head_channels=self._per_head_channels,
         use_bias=self._use_bias,
-        edge_dropout=self._edge_dropout,
+        edge_dropout=self._edge_dropout_layer.rate,
+        inputs_dropout=self._inputs_dropout_layer.rate,
         # All forms of activation functions can be returned as-is:
         # - A Keras Layer is serialized and deserialized recursively through
         #   its own get_config/from config methods. It's best to not try and
         #   simulate that recursive process here.
         # - A str with a name may be passed to __init__, but __init__ anyways
         #   calls .get() to turn it into a function from tf.keras.activations.*.
         # - A function from tf.keras.activations.* is automatically serialized
@@ -359,36 +355,45 @@
                broadcast_from_sender_node: Callable[[tf.Tensor], tf.Tensor],
                broadcast_from_receiver: Callable[[tf.Tensor], tf.Tensor],
                pool_to_receiver: Callable[..., tf.Tensor],
                extra_receiver_ops: Optional[Mapping[str, Callable[...,
                                                                   Any]]] = None,
                **kwargs) -> tf.Tensor:
 
+    # Apply dropout on the inputs.
+    receiver_input = self._inputs_dropout_layer(receiver_input)
+    if sender_node_input is not None:
+      sender_node_input = self._inputs_dropout_layer(sender_node_input)
+    if sender_edge_input is not None:
+      sender_edge_input = self._inputs_dropout_layer(sender_edge_input)
+
     # Determine the width of transformed queries and create transfomations.
     # If transform_keys is true, queries will be transformed to
     # self._per_head_channels. Otherwise, transform the queries to match
     # the width of raw sender inputs (keys).
     if self._w_query is None:
       with tf.init_scope():
         if not self._transform_keys:
           keys_width = 0
           if sender_node_input is not None:
             keys_width += sender_node_input.shape[-1]
           if sender_edge_input is not None:
             keys_width += sender_edge_input.shape[-1]
           self._w_query = tf.keras.layers.Dense(
               keys_width * self._num_heads,
-              kernel_initializer=self._kernel_initializer,
+              kernel_initializer=tfgnn.keras.clone_initializer(
+                  self._kernel_initializer),
               kernel_regularizer=self._kernel_regularizer,
               use_bias=self._use_bias,
               name="query")
         else:
           self._w_query = tf.keras.layers.Dense(
               self._per_head_channels * self._num_heads,
-              kernel_initializer=self._kernel_initializer,
+              kernel_initializer=tfgnn.keras.clone_initializer(
+                  self._kernel_initializer),
               kernel_regularizer=self._kernel_regularizer,
               use_bias=self._use_bias,
               name="query")
     assert self._w_query is not None
 
     # Form the attention query for each head.
     # If transform_keys is true, it has the shape:
@@ -396,15 +401,15 @@
     # Otherwise, the shape is: [num_items, *extra_dims, num_heads, keys_width].
     assert receiver_input is not None, "__init__() should have checked this."
     queries = self._w_query(receiver_input)
     queries = self._attention_activation(queries)
     queries = broadcast_from_receiver(self._split_heads(queries))
 
     # Form the attention key for each head.
-    # If transform_keys is ture, the pieces of keys inputs are transformed to
+    # If transform_keys is true, the pieces of keys inputs are transformed to
     # [num_items, *extra_dims, num_heads, channels_per_head] and the results
     # are added, which allows transformation for the piece from the nodes before
     # broadcasting it and equals to first concatenating the pieces and
     # then transforming them to channels_per_head.
     # If transform_keys is false, the pieces of keys inputs are concatenated on
     # last axis with a shape [num_items, *extra_dims, num_heads, keys_width].
     keys = []
@@ -462,25 +467,24 @@
     else:
       raise ValueError("Unknown value MultiHeadAttentionConv("
                        f"score_scaling='{self._score_scaling}')")
 
     attention_coefficients = extra_receiver_ops["softmax"](
         attention_coefficients)
 
-    if self._edge_dropout_layer is not None:
-      # If requested, add layer with dropout to the normalized attention
-      # coefficients. This should have the same effect as edge dropout.
-      # Also, note that `keras.layers.Dropout` upscales the remaining values,
-      # which should maintain the sum-up-to-1 per node in expectation.
-      attention_coefficients = self._edge_dropout_layer(attention_coefficients,
-                                                        **kwargs)
+    # Add layer with dropout to the normalized attention coefficients. This
+    # should have the same effect as edge dropout. Also, note that
+    # `keras.layers.Dropout` upscales the remaining values, which should
+    # maintain the sum-up-to-1 per node in expectation.
+    attention_coefficients = self._edge_dropout_layer(attention_coefficients,
+                                                      **kwargs)
 
     # Compute the pooled values by
     #   * transforming the inputs and
-    #   * computing their weighted sum according to the attention coefficents.
+    #   * computing their weighted sum according to the attention coefficients.
     # These two operations are linear, so, mathematically, they can be applied
     # in either order. It depends on input/output dimensions, the ratio of
     # num_items to num_receivers and the platform which one is faster.
     if not self._transform_values_after_pooling:
       # Option 1: First transform the inputs, then pool the values.
       # The transformation is split into the terms for node inputs and edge
       # inputs, so that each node input is transformed once before broadcasting.
@@ -610,15 +614,15 @@
       receiver_tag=receiver_tag,
       receiver_feature=receiver_feature,
       sender_edge_feature=sender_feature,
       sender_node_feature=None,
       **kwargs)
 
 
-# TODO(b/236941740): a systematic solution for adding loops.
+# TODO(b/286015280): a systematic solution for adding loops.
 def MultiHeadAttentionHomGraphUpdate(
     *,  # To be called like a class initializer.  pylint: disable=invalid-name
     num_heads: int,
     per_head_channels: int,
     receiver_tag: tfgnn.IncidentNodeTag,
     feature_name: str = tfgnn.HIDDEN_STATE,
     name: str = "multi_head_attention",
@@ -649,57 +653,55 @@
     **kwargs: Any optional arguments to MultiHeadAttentionConv, see there.
   """
 
   # Build a GraphUpdate for the target node set of the given edge_set_name.
   # That needs to be deferred until we see a GraphTensorSpec that tells us
   # the node_set_name.
   def deferred_init_callback(spec: tfgnn.GraphTensorSpec):
-    tfgnn.check_homogeneous_graph_tensor(spec,
-                                         "MultiHeadAttentionHomGraphUpdate")
-    edge_set_name, = spec.edge_sets_spec.keys()
-    node_set_name = spec.edge_sets_spec[
-        edge_set_name].adjacency_spec.node_set_name(receiver_tag)
+    node_set_name, edge_set_name = tfgnn.get_homogeneous_node_and_edge_set_name(
+        spec, "MultiHeadAttentionHomGraphUpdate")
     node_set_updates = {
         node_set_name:
             tfgnn.keras.layers.NodeSetUpdate(
                 {
                     edge_set_name:
                         MultiHeadAttentionConv(
                             num_heads=num_heads,
                             per_head_channels=per_head_channels,
                             receiver_tag=receiver_tag,
                             sender_node_feature=feature_name,
                             receiver_feature=feature_name,
-                            **kwargs)
+                            **kwargs)  # kernel_initializer cloned by layer.
                 },
                 next_state=tfgnn.keras.layers.SingleInputNextState(),
                 node_input_feature=feature_name)
     }
     return dict(node_sets=node_set_updates)
 
   return tfgnn.keras.layers.GraphUpdate(
       deferred_init_callback=deferred_init_callback, name=name)
 
 
 def MultiHeadAttentionMPNNGraphUpdate(  # To be called like a class initializer.  pylint: disable=invalid-name
+    # LINT.IfChange(MultiHeadAttentionMPNNGraphUpdate_args)
     *,
     units: int,
     message_dim: int,
     num_heads: int,
     receiver_tag: tfgnn.IncidentNodeTag,
     node_set_names: Optional[Collection[tfgnn.NodeSetName]] = None,
     edge_feature: Optional[tfgnn.FieldName] = None,
     l2_regularization: float = 0.0,
     edge_dropout_rate: float = 0.0,
     state_dropout_rate: float = 0.0,
     attention_activation: Optional[Union[str, Callable[..., Any]]] = None,
     conv_activation: Union[str, Callable[..., Any]] = "relu",
     activation: Union[str, Callable[..., Any]] = "relu",
-    kernel_initializer: Union[
-        None, str, tf.keras.initializers.Initializer] = "glorot_uniform",
+    kernel_initializer: Any = "glorot_uniform",
+    # LINT.ThenChange(./config_dict.py:graph_update_get_config_dict)
 ) -> tf.keras.layers.Layer:
   """Returns a GraphUpdate layer for message passing with MultiHeadAttention pooling.
 
   The returned layer performs one round of message passing between the nodes
   of a heterogeneous GraphTensor, using
   `multi_head_attention.MultiHeadAttentionConv` to compute the messages and
   their pooling with attention, followed by a dense layer to compute the new
@@ -724,21 +726,23 @@
       biases.
     edge_dropout_rate: The edge dropout rate applied during attention pooling of
       edges.
     state_dropout_rate: The dropout rate applied to the resulting node states.
     attention_activation: The nonlinearity used on the transformed inputs before
       multiplying with the trained weights of the attention layer. This can be
       specified as a Keras layer, a tf.keras.activations.* function, or a string
-      understood by tf.keras.layers.Activation(). Defaults to None.
+      understood by `tf.keras.layers.Activation`. Defaults to None.
     conv_activation: The nonlinearity applied to the result of attention on one
       edge set, specified in the same ways as attention_activation.
     activation: The nonlinearity applied to the new node states computed by this
       graph update.
-    kernel_initializer: Can be set to a `kerner_initializer` as understood by
-      `tf.keras.layers.Dense` etc.
+    kernel_initializer: Can be set to a `kernel_initializer` as understood
+      by `tf.keras.layers.Dense` etc.
+      An `Initializer` object gets cloned before use to ensure a fresh seed,
+      if not set explicitly. For more, see `tfgnn.keras.clone_initializer()`.
 
   Returns:
     A GraphUpdate layer for use on a scalar GraphTensor with
     `tfgnn.HIDDEN_STATE` features on the node sets.
   """
   if message_dim % num_heads:
     raise ValueError("message_dim must be divisible by num_heads, "
@@ -748,15 +752,16 @@
   def dense(units):  # pylint: disable=invalid-name
     regularizer = tf.keras.regularizers.l2(l2_regularization)
     return tf.keras.Sequential([
         tf.keras.layers.Dense(
             units,
             activation=activation,
             use_bias=True,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                kernel_initializer),
             bias_initializer="zeros",
             kernel_regularizer=regularizer,
             bias_regularizer=regularizer),
         tf.keras.layers.Dropout(state_dropout_rate)
     ])
 
   # pylint: disable=g-long-lambda
@@ -765,12 +770,12 @@
           num_heads=num_heads,
           per_head_channels=per_head_channels,
           edge_dropout=edge_dropout_rate,
           receiver_tag=receiver_tag,
           sender_edge_feature=edge_feature,
           attention_activation=attention_activation,
           activation=conv_activation,
-          kernel_initializer=kernel_initializer),
+          kernel_initializer=kernel_initializer),  # Cloned by the layer.
       lambda node_set_name: tfgnn.keras.layers.NextStateFromConcat(
           dense(units)),
       receiver_tag=receiver_tag)
   return gnn_builder.Convolve(node_set_names)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/multi_head_attention/layers_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/multi_head_attention/layers_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,28 +30,17 @@
   SKIP = 0
   SAVED_MODEL = 1
   KERAS = 2
 
 
 class MultiHeadAttentionTest(tf.test.TestCase, parameterized.TestCase):
 
-  # TODO(b/266868417): Remove when TF2.10+ is required by all of TF-GNN.
-  def _skip_if_unsupported(self, transform_values_after_pooling=None):
-    """Skips test if TF is tool old for a requested option."""
-    if transform_values_after_pooling:
-      if tf.__version__.startswith("2.8.") or tf.__version__.startswith("2.9."):
-        self.skipTest(
-            "MultiHeadAttentionConv(transform_values_after_pooling=True) "
-            f"requires TF 2.10+, got {tf.__version__}")
-
   @parameterized.named_parameters(("", False), ("TransformAfter", True))
   def testBasic(self, transform_values_after_pooling):
     """Tests that a single-headed MHA is correct given predefined weights."""
-    self._skip_if_unsupported(
-        transform_values_after_pooling=transform_values_after_pooling)
     # NOTE: Many following tests use minor variations of the explicit
     # construction of weights and results introduced here.
 
     # Construct a graph with three nodes 0, 1, 2, and six edges:
     # a cycle 0->1->2->0 (let's call it clockwise)
     # and the reverse cycle 0->2->1->0 (counterclockwise).
     gt_input = _get_test_bidi_cycle_graph(
@@ -510,16 +499,14 @@
     ])
     self.assertAllEqual(got_2.shape, (3, 2, 3))
     self.assertAllClose(got_2, want_2, atol=.0001)
 
   @parameterized.named_parameters(("", False), ("TransformAfter", True))
   def testMultihead(self, transform_values_after_pooling):
     """Extends testBasic with multiple attention heads."""
-    self._skip_if_unsupported(
-        transform_values_after_pooling=transform_values_after_pooling)
     # The same test graph as in the testBasic above.
     gt_input = _get_test_bidi_cycle_graph(
         tf.constant([
             [1., 0., 0., 1.],
             [0., 1., 0., 2.],
             [0., 0., 1., 3.],
         ]))
@@ -604,16 +591,14 @@
       ("", ReloadModel.SKIP, False), ("TransformAfter", ReloadModel.SKIP, True),
       ("Restored", ReloadModel.SAVED_MODEL, False),
       ("RestoredTransformAfter", ReloadModel.SAVED_MODEL, True),
       ("RestoredKeras", ReloadModel.KERAS, False),
       ("RestoredKerasTransformAfter", ReloadModel.KERAS, True))
   def testFullModel(self, reload_model, transform_values_after_pooling):
     """Tests MultiHeadAttentionHomGraphUpdate in a Model with edge input."""
-    self._skip_if_unsupported(
-        transform_values_after_pooling=transform_values_after_pooling)
     # The same example as in the testBasic above, but with extra inputs
     # from edges.
     gt_input = _get_test_bidi_cycle_graph(
         # Node i has value i+1 in the last component, which will be mapped
         # into the fourth component of the value.
         tf.constant([
             [1., 0., 0., 1.],  # Node 0.
@@ -1075,14 +1060,112 @@
       got = got_gt.node_sets["nodes"][tfgnn.HIDDEN_STATE][target_node_id]
       return [tf.reduce_min(got), tf.reduce_max(got)]
 
     self.assertAllEqual(min_max(), [1., 1.])  # Inference is the default.
     self.assertAllEqual(min_max(training=False), [1., 1.])
     self.assertAllClose(min_max(training=True), [0., 1.5])
 
+  def testInputsDropout(self):
+    """Tests dropout, esp. the switch between training and inference modes."""
+    # Avoid flakiness.
+    tf.random.set_seed(42)
+
+    # This test graph has many source nodes feeding into one target node.
+    # The node features are all ones, the edge features are one-hot encodings of
+    # the source node IDs.
+    num_nodes = 32
+    target_node_id = 7
+    gt_input = tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            "nodes":
+                tfgnn.NodeSet.from_fields(
+                    sizes=[num_nodes],
+                    features={
+                        tfgnn.HIDDEN_STATE:
+                            tf.ones(
+                                shape=(num_nodes, num_nodes), dtype=tf.float32)
+                    }),
+        },
+        edge_sets={
+            "edges":
+                tfgnn.EdgeSet.from_fields(
+                    sizes=[num_nodes],
+                    adjacency=tfgnn.Adjacency.from_indices(
+                        ("nodes", tf.constant(list(range(num_nodes)))),
+                        ("nodes", tf.constant([target_node_id] * num_nodes))),
+                    features={tfgnn.HIDDEN_STATE: tf.eye(num_nodes)})
+        })
+
+    # On purpose, this test is not for MultiHeadAttentionConv directly,
+    # but for its common usage in a GraphUpdate, to make sure the
+    # training/inference mode is propagated correctly.
+    inputs_dropout_rate = 0.25
+    layer = multi_head_attention.MultiHeadAttentionHomGraphUpdate(
+        num_heads=1,
+        per_head_channels=num_nodes,
+        receiver_tag=tfgnn.TARGET,
+        sender_edge_feature=tfgnn.HIDDEN_STATE,
+        inputs_dropout=inputs_dropout_rate,  # Note here.
+        activation="linear",
+        attention_activation="linear",
+        use_bias=False)
+
+    _ = layer(gt_input)  # Build weights.
+    weights = {v.name: v for v in layer.trainable_weights}
+    self.assertLen(weights, 5)
+    # Do not transform the queries.
+    weights["multi_head_attention/node_set_update/" +
+            "multi_head_attention_conv/query/kernel:0"].assign(
+                tf.eye(num_nodes))
+    # Filter out the key edge features, keep only the node features.
+    weights["multi_head_attention/node_set_update/" +
+            "multi_head_attention_conv/key_node/kernel:0"].assign(
+                tf.eye(num_nodes))
+    weights["multi_head_attention/node_set_update/" +
+            "multi_head_attention_conv/key_edge/kernel:0"].assign(
+                tf.zeros(shape=(num_nodes, num_nodes), dtype=tf.float32))
+    # Filter out the value node features, keep only the one-hot edge features.
+    weights["multi_head_attention/node_set_update/" +
+            "multi_head_attention_conv/value_node/kernel:0"].assign(
+                tf.zeros(shape=(num_nodes, num_nodes), dtype=tf.float32))
+    weights["multi_head_attention/node_set_update/" +
+            "multi_head_attention_conv/value_edge/kernel:0"].assign(
+                tf.eye(num_nodes))
+
+    # Build a Model around the Layer, possibly saved and restored.
+    inputs = tf.keras.layers.Input(type_spec=gt_input.spec)
+    outputs = layer(inputs)
+    model = tf.keras.Model(inputs, outputs)
+
+    # Without dropout, i.e. during inference, The transformed queries and keys
+    # should be all ones, so the softmaxe'd scores should be all equal. Since
+    # the transformed values are one-hots, their scaled sum should be a vector
+    # with the normalized scores.
+    self.assertAllEqual(
+        model(gt_input).node_sets["nodes"][tfgnn.HIDDEN_STATE][target_node_id],
+        [1 / num_nodes] * num_nodes)
+
+    # With dropout, i.e. during training, the scores will be binomially
+    # distributed with n=32 and p=0.5625 (probability of neither the query nor
+    # the key value to have been dropped out). Additionally, ~25% of the
+    # resulting values will be zero if the one-hot encoded value was dropped
+    # out.
+    outputs = model(
+        gt_input,
+        training=True).node_sets["nodes"][tfgnn.HIDDEN_STATE][target_node_id]
+    outputs = tf.boolean_mask(outputs, mask=outputs > 0)
+    num_zero_outputs = num_nodes - tf.size(outputs)
+
+    # Check that some values were dropped out completely.
+    self.assertGreater(num_zero_outputs, 0)
+
+    # Check that the stdv of the remaining values is not zero, i.e. the
+    # remaining scores are not all identical.
+    self.assertGreater(tf.math.reduce_std(outputs), 0.0)
+
 
 def _get_test_bidi_cycle_graph(node_state, edge_state=None):
   return tfgnn.GraphTensor.from_pieces(
       node_sets={
           "nodes":
               tfgnn.NodeSet.from_fields(
                   sizes=[3], features={tfgnn.HIDDEN_STATE: node_state}),
@@ -1128,14 +1211,116 @@
   def testMessageUnitsNotDivisible(self):
     with self.assertRaisesRegex(ValueError,
                                 r"must be divisible by num_heads, got 5 and 2"):
       _ = multi_head_attention.MultiHeadAttentionMPNNGraphUpdate(
           message_dim=5, num_heads=2, units=12, receiver_tag=tfgnn.TARGET)
 
 
+class MultiHeadAttentionMPNNTFLiteTest(tf.test.TestCase,
+                                       parameterized.TestCase):
+
+  @parameterized.named_parameters(
+      ("Simplest", "none", False, False),
+      ("TransformedKeys", "rsqrt_dim", True, False),
+      ("AllOps", "trainable_sigmoid", True, True))
+  def testBasic(
+      self,
+      score_scaling,
+      transform_keys,
+      transform_values_after_pooling,
+  ):
+    test_graph_1_dict = {
+        # We care that the TFLite interpreter gives the same output as the
+        # model, which was tested separately (although not for the randomly
+        # initialized weights that we keep here).
+        "source":
+            tf.constant([0, 1, 2, 0, 2, 1]),
+        "target":
+            tf.constant([1, 2, 0, 2, 1, 0]),
+        "node_features":
+            tf.constant([
+                [1., 0., 0., 1.],
+                [0., 1., 0., 2.],
+                [0., 0., 1., 3.],
+            ]),
+        "edge_features":
+            tf.constant([
+                [3.],
+                [6.],
+                [9.],
+                [2.],
+                [6.],
+                [4.]]),
+    }
+    # TODO(b/276291104): Remove when TF 2.11+ is required by all of TFGNN
+    if tf.__version__.startswith("2.10."):
+      self.skipTest("GNN models are unsupported in TFLite until TF 2.11 but "
+                    f"got TF {tf.__version__}")
+    layer = multi_head_attention.MultiHeadAttentionHomGraphUpdate(
+        num_heads=2,
+        per_head_channels=2,
+        receiver_tag=tfgnn.TARGET,
+        sender_edge_feature=tfgnn.HIDDEN_STATE,  # Activate edge input.
+        attention_activation="relu",
+        kernel_initializer="zeros",
+        kernel_regularizer=tf.keras.regularizers.L2(0.05),  # Add a regularizer.
+        score_scaling=score_scaling,
+        transform_keys=transform_keys,
+        transform_values_after_pooling=transform_values_after_pooling,
+    )
+
+    inputs = {
+        "node_features": tf.keras.Input([4], None, "node_features", tf.float32),
+        "source": tf.keras.Input([], None, "source", tf.int32),
+        "target": tf.keras.Input([], None, "target", tf.int32),
+        "edge_features": tf.keras.Input([1], None, "edge_features", tf.float32),
+    }
+    graph_in = _MakeGraphTensor()(inputs)
+    graph_out = layer(graph_in)
+    outputs = tf.keras.layers.Layer(name="final_node_states")(
+        graph_out.node_sets["nodes"][tfgnn.HIDDEN_STATE])
+    model = tf.keras.Model(inputs, outputs)
+
+    # The other unit tests should verify that this is correct
+    expected = model(test_graph_1_dict).numpy()
+
+    converter = tf.lite.TFLiteConverter.from_keras_model(model)
+    model_content = converter.convert()
+    interpreter = tf.lite.Interpreter(model_content=model_content)
+    signature_runner = interpreter.get_signature_runner("serving_default")
+    obtained = signature_runner(**test_graph_1_dict)["final_node_states"]
+    self.assertAllClose(expected, obtained)
+
+
+# TODO(b/274779989): Replace this layer with a more standard representation
+# of GraphTensor as a dict of plain Tensors.
+class _MakeGraphTensor(tf.keras.layers.Layer):
+  """Makes a homogeneous GraphTensor of rank 0 with a single component."""
+
+  def call(self, inputs):
+    node_sizes = tf.shape(inputs["node_features"])[0]
+    edge_sizes = tf.shape(inputs["edge_features"])[0]
+    return tfgnn.GraphTensor.from_pieces(
+        node_sets={
+            "nodes":
+                tfgnn.NodeSet.from_fields(
+                    sizes=tf.expand_dims(node_sizes, axis=0),
+                    features={tfgnn.HIDDEN_STATE: inputs["node_features"]})
+        },
+        edge_sets={
+            "edges":
+                tfgnn.EdgeSet.from_fields(
+                    sizes=tf.expand_dims(edge_sizes, axis=0),
+                    adjacency=tfgnn.Adjacency.from_indices(
+                        ("nodes", inputs["source"]),
+                        ("nodes", inputs["target"])),
+                    features={tfgnn.HIDDEN_STATE: inputs["edge_features"]})
+        })
+
+
 def _make_test_graph_abc():
   return tfgnn.GraphTensor.from_pieces(
       node_sets={
           "a":
               tfgnn.NodeSet.from_fields(
                   sizes=tf.constant([1]),
                   features={tfgnn.HIDDEN_STATE: tf.constant([[1.]])}),
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,24 +17,25 @@
 from ml_collections import config_dict
 import tensorflow as tf
 from tensorflow_gnn.models.vanilla_mpnn import layers
 
 
 def graph_update_get_config_dict() -> config_dict.ConfigDict:
   """Returns ConfigDict for graph_update_from_config_dict() with defaults."""
-  # Keep in sync with default args of VanillaMPNNGraphUpdate.__init__.
+  # LINT.IfChange(graph_update_get_config_dict)
   cfg = config_dict.ConfigDict()
   cfg.units = config_dict.placeholder(int)  # Sets type to Optional[int].
   cfg.message_dim = config_dict.placeholder(int)
   cfg.receiver_tag = config_dict.placeholder(int)
   cfg.reduce_type = "sum"
   cfg.l2_regularization = 0.0
   cfg.dropout_rate = 0.0
   cfg.use_layer_normalization = False
   cfg.lock()
+  # LINT.ThenChange(./layers.py:VanillaMPNNGraphUpdate_args)
   return cfg
 
 
 def graph_update_from_config_dict(
     cfg: config_dict.ConfigDict) -> tf.keras.layers.Layer:
   """Returns a VanillaMPNNGraphUpdate initialized from `cfg`.
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/config_dict_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -38,19 +38,20 @@
 
     expected = layers.VanillaMPNNGraphUpdate(
         units=units, message_dim=message_dim, receiver_tag=receiver_tag)
 
     self.assertEqual(to_model_config(actual), to_model_config(expected))
 
 
+# TODO(b/265776928): De-duplicate the multiple copies of this test helper.
 def to_model_config(layer: tf.keras.layers.Layer):
   """Returns a parsed model config for `layer`, without `"name"` fields."""
   # Need a full model to serialize *recursively*.
   model = tf.keras.Sequential([layer])
-  # Subobjects are only build in the first call.
+  # Subobjects are only built in the first call.
   _ = model(_make_test_graph_loop())
   model_config = json.loads(model.to_json())
   # The names of layers are uniquified and impede the hparam comparison.
   return _remove_names(model_config)
 
 
 def _remove_names(obj):
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/hparams_vizier_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/vanilla_mpnn/layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contains the Vanilla MPNN layers."""
-from typing import Collection, Optional, Union
+from typing import Any, Collection, Optional
 
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 
 
 def VanillaMPNNGraphUpdate(  # To be called like a class initializer.  pylint: disable=invalid-name
+    # LINT.IfChange(VanillaMPNNGraphUpdate_args)
     *,
     units: int,
     message_dim: int,
     receiver_tag: tfgnn.IncidentNodeTag,
     node_set_names: Optional[Collection[tfgnn.NodeSetName]] = None,
     edge_feature: Optional[tfgnn.FieldName] = None,
     reduce_type: str = "sum",
     l2_regularization: float = 0.0,
     dropout_rate: float = 0.0,
-    kernel_initializer: Union[
-        None, str, tf.keras.initializers.Initializer] = "glorot_uniform",
+    kernel_initializer: Any = "glorot_uniform",
     use_layer_normalization: bool = False,
+    # LINT.ThenChange(./config_dict.py:graph_update_get_config_dict)
 ) -> tf.keras.layers.Layer:
   r"""Returns a GraphUpdate layer for a Vanilla MPNN.
 
   The returned layer performs one round of node state updates with a
   Message Passing Neural Network that uses a single dense layer to
   compute messages and update node states.
 
@@ -55,47 +56,50 @@
   state and the pooled messages from all incident node sets E_1, E_2, ...:
 
   $$h_v := \text{ReLU}(
       W_{\text{state}} (h_v || m_{E_1} || m_{E_2} || \ldots)).$$
 
   Args:
     units: The dimension of output hidden states for each node.
-    message_dim: The dimension of messages (attention values) computed on
-      each edge.  Must be divisible by `num_heads`.
+    message_dim: The dimension of messages computed on each edge.
     receiver_tag: one of `tfgnn.TARGET` or `tfgnn.SOURCE`, to select the
       incident node of each edge that receives the message.
     node_set_names: The names of node sets to update. If unset, updates all
       that are on the receiving end of any edge set.
     edge_feature: Can be set to a feature name of the edge set to select
       it as an input feature. By default, this set to `None`, which disables
       this input.
-    reduce_type: How to pool the messages from edges to receiver nodes.
-      Can be any name from `tfgnn.get_registered_reduce_operation_names()`,
-      defaults to "sum".
+    reduce_type: How to pool the messages from edges to receiver nodes; defaults
+      to `"sum"`. Can be any reduce_type understood by `tfgnn.pool()`, including
+      concatenations like `"sum|max"` (but mind the increased dimension of the
+      result and the growing number of model weights in the next-state layer).
     l2_regularization: The coefficient of L2 regularization for weights and
       biases.
     dropout_rate: The dropout rate applied to messages on each edge and to the
       new node state.
-    kernel_initializer: Can be set to a `kerner_initializer` as understood
+    kernel_initializer: Can be set to a `kernel_initializer` as understood
       by `tf.keras.layers.Dense` etc.
+      An `Initializer` object gets cloned before use to ensure a fresh seed,
+      if not set explicitly. For more, see `tfgnn.keras.clone_initializer()`.
     use_layer_normalization: Flag to determine whether to apply layer
       normalization to the new node state.
 
   Returns:
     A GraphUpdate layer for use on a scalar GraphTensor with
     `tfgnn.HIDDEN_STATE` features on the node sets.
   """
   def dense(units, *, use_layer_normalization=False):  # pylint: disable=invalid-name
     regularizer = tf.keras.regularizers.l2(l2_regularization)
     result = tf.keras.Sequential([
         tf.keras.layers.Dense(
             units,
             activation="relu",
             use_bias=True,
-            kernel_initializer=kernel_initializer,
+            kernel_initializer=tfgnn.keras.clone_initializer(
+                kernel_initializer),
             bias_initializer="zeros",
             kernel_regularizer=regularizer,
             bias_regularizer=regularizer),
         tf.keras.layers.Dropout(dropout_rate)])
     if use_layer_normalization:
       result.add(tf.keras.layers.LayerNormalization())
     return result
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/models/vanilla_mpnn/layers_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,96 +8,150 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Tests for VanillaMPNN."""
+"""Tests for parsing."""
+import functools
+
 from absl.testing import parameterized
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
-from tensorflow_gnn.models import vanilla_mpnn
-
-
-# The components of VanillaMPNNGraphUpdate have been tested elsewhere.
-class VanillaMPNNTest(tf.test.TestCase, parameterized.TestCase):
-
-  def testVanillaMPNNGraphUpdate(self):
-    input_graph = _make_test_graph_abc()
-    units = 2
-    layer = vanilla_mpnn.VanillaMPNNGraphUpdate(
-        units=units,
-        message_dim=1,
-        receiver_tag=tfgnn.TARGET,
-        node_set_names=["b"],
-        edge_feature="fab",
-        kernel_initializer="ones")
-    graph = layer(input_graph)
-    # Nodes "a" and "c" are unchanged.
-    self.assertAllEqual([[1.]], graph.node_sets["a"][tfgnn.HIDDEN_STATE])
-    self.assertAllEqual([[8.]], graph.node_sets["c"][tfgnn.HIDDEN_STATE])
-    # Node "b" receives message 1+2+16 = 19 and combines it with old state 2.
-    self.assertAllEqual([[21.]*units], graph.node_sets["b"][tfgnn.HIDDEN_STATE])
-
-  @parameterized.named_parameters(("WithoutLayerNorm", False),
-                                  ("WithLayerNorm", True))
-  def testVanillaMPNNGraphUpdateWithCustomKernelInitializer(
-      self, use_layer_normalization):
-    input_graph = _make_test_graph_abc()
-    # To ensure that the updated node-state has non-identical entries
-    kernel_initializer = tf.constant_initializer([[1., 1.],
-                                                  [2., 0.],
-                                                  [1., 1.]])
-    units = 2
-    layer = vanilla_mpnn.VanillaMPNNGraphUpdate(
-        units=units,
-        message_dim=2,
-        receiver_tag=tfgnn.TARGET,
-        node_set_names=["b"],
-        edge_feature="fab",
-        kernel_initializer=kernel_initializer,
-        use_layer_normalization=use_layer_normalization)
-    graph = layer(input_graph)
-
-    # Nodes "a" and "c" are unchanged.
-    self.assertAllEqual([[1.]], graph.node_sets["a"][tfgnn.HIDDEN_STATE])
-    self.assertAllEqual([[8.]], graph.node_sets["c"][tfgnn.HIDDEN_STATE])
-    # Node "b" receives message [b, a, fab] * Kw = [20., 18.]
-    # Message is combined with "b" old state [b, 20., 18.] * Kw = [60, 20]
-    # If use_layer_normalization flag is set, layer normalization is applied on
-    # the updated node state
-    if use_layer_normalization:
-      want = [[1., -1.]]
-    else:
-      want = [[60., 20.]]
-    self.assertAllClose(want, graph.node_sets["b"][tfgnn.HIDDEN_STATE])
-
-
-def _make_test_graph_abc():
-  return tfgnn.GraphTensor.from_pieces(
-      node_sets={
-          "a": tfgnn.NodeSet.from_fields(
-              sizes=tf.constant([1]),
-              features={tfgnn.HIDDEN_STATE: tf.constant([[1.]])}),
-          "b": tfgnn.NodeSet.from_fields(
-              sizes=tf.constant([1]),
-              features={tfgnn.HIDDEN_STATE: tf.constant([[2.]])}),
-          "c": tfgnn.NodeSet.from_fields(
-              sizes=tf.constant([1]),
-              features={tfgnn.HIDDEN_STATE: tf.constant([[8.]])})},
-      edge_sets={
-          "a->b": tfgnn.EdgeSet.from_fields(
-              sizes=tf.constant([1]),
-              adjacency=tfgnn.Adjacency.from_indices(
-                  ("a", tf.constant([0])),
-                  ("b", tf.constant([0]))),
-              features={"fab": tf.constant([[16.]])}),
-          "c->c": tfgnn.EdgeSet.from_fields(
-              sizes=tf.constant([1]),
-              adjacency=tfgnn.Adjacency.from_indices(
-                  ("c", tf.constant([0])),
-                  ("c", tf.constant([0]))))})
+from tensorflow_gnn.runner.utils import parsing as parsing_utils
 
+SCHEMA = """
+  node_sets {
+    key: "node"
+    value {
+      features {
+        key: "features"
+        value {
+          dtype: DT_FLOAT
+          shape { dim { size: 4 } }
+        }
+      }
+    }
+  }
+  edge_sets {
+    key: "edge"
+    value {
+      source: "node"
+      target: "node"
+    }
+  }
+"""
+
+Fields = tfgnn.Fields
+GraphTensor = tfgnn.GraphTensor
+
+ds_from_tensor = tf.data.Dataset.from_tensors
+
+
+def gtspec() -> tfgnn.GraphTensorSpec:
+  return tfgnn.create_graph_spec_from_schema_pb(tfgnn.parse_schema(SCHEMA))
+
+
+@functools.lru_cache(None)
+def random_graph_tensor() -> tfgnn.GraphTensor:
+  return tfgnn.random_graph_tensor(gtspec())
+
+
+@functools.lru_cache(None)
+def random_serialized_graph_tensor() -> str:
+  return tfgnn.write_example(random_graph_tensor()).SerializeToString()
+
+
+class ParsingTest(tf.test.TestCase, parameterized.TestCase):
+
+  def _assert_fields_equal(self, a: Fields, b: Fields):
+    self.assertCountEqual(a.keys(), b.keys())
+    for k, v in a.items():
+      self.assertAllEqual(v, b[k])
+
+  def _assert_graph_tensors_equal(self, a: GraphTensor, b: GraphTensor):
+    self.assertCountEqual(a.node_sets.keys(), b.node_sets.keys())
+    self.assertCountEqual(a.edge_sets.keys(), b.edge_sets.keys())
+
+    self._assert_fields_equal(a.context.features, b.context.features)
+
+    for k, v in a.node_sets.items():
+      self._assert_fields_equal(v.features, b.node_sets[k].features)
+
+    for k, v in a.edge_sets.items():
+      self._assert_fields_equal(v.features, b.edge_sets[k].features)
+
+  @parameterized.named_parameters([
+      dict(
+          testcase_name="SerializedGraphTensorElement",
+          ds=ds_from_tensor(random_serialized_graph_tensor()),
+          spec=random_graph_tensor().spec,
+          expected=random_graph_tensor(),
+      ),
+      dict(
+          testcase_name="GraphTensorElement",
+          ds=ds_from_tensor(random_graph_tensor()),
+          spec=random_graph_tensor().spec,
+          expected=random_graph_tensor(),
+      ),
+      dict(
+          testcase_name="SerializedGraphTensorElements",
+          ds=ds_from_tensor(random_serialized_graph_tensor()).repeat().batch(4),
+          spec=random_graph_tensor().spec,
+          expected=next(
+              iter(
+                  ds_from_tensor(random_graph_tensor()).repeat().batch(4)
+                  )
+              ),
+      ),
+      dict(
+          testcase_name="GraphTensorElements",
+          ds=ds_from_tensor(random_graph_tensor()).repeat().batch(4),
+          spec=random_graph_tensor().spec,
+          expected=next(
+              iter(
+                  ds_from_tensor(random_graph_tensor()).repeat().batch(4)
+                  )
+              ),
+      ),
+  ])
+  def test_maybe_parse_graph_tensor_dataset(
+      self,
+      ds: tf.data.Dataset,
+      spec: tfgnn.GraphTensorSpec,
+      expected: tfgnn.GraphTensor):
+    ds = parsing_utils.maybe_parse_graph_tensor_dataset(ds, spec)
+    self._assert_graph_tensors_equal(
+        expected,
+        next(iter(ds)))
+
+  @parameterized.named_parameters([
+      dict(
+          testcase_name="FloatElement",
+          ds=ds_from_tensor(tf.constant(8191.)),
+          spec=random_graph_tensor().spec,
+          expected_failure=r"Expected `GraphTensorSpec` \(got .*\)",
+      ),
+      dict(
+          testcase_name="IncompatibleGraphTensorElement",
+          ds=ds_from_tensor(
+              tfgnn.homogeneous(
+                  source=tf.constant((0, 3)),
+                  target=tf.constant((1, 2)),
+                  node_set_sizes=tf.constant((4,))
+                  ),
+              ),
+          spec=random_graph_tensor().spec,
+          expected_failure=r"Graph is not compatible with the graph schema.*",
+      ),
+  ])
+  def test_maybe_parse_graph_tensor_dataset_fails(
+      self,
+      ds: tf.data.Dataset,
+      spec: tfgnn.GraphTensorSpec,
+      expected_failure: str):
+    with self.assertRaisesRegex(ValueError, expected_failure):
+      _ = parsing_utils.maybe_parse_graph_tensor_dataset(ds, spec)
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/examples.proto` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/hgt/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,32 @@
-// Copyright 2021 The TensorFlow GNN Authors. All Rights Reserved.
-//
-// Licensed under the Apache License, Version 2.0 (the "License");
-// you may not use this file except in compliance with the License.
-// You may obtain a copy of the License at
-//
-//     http://www.apache.org/licenses/LICENSE-2.0
-//
-// Unless required by applicable law or agreed to in writing, software
-// distributed under the License is distributed on an "AS IS" BASIS,
-// WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-// See the License for the specific language governing permissions and
-// limitations under the License.
-// =============================================================================
-syntax = "proto2";
+# Copyright 2022 The TensorFlow GNN Authors. All Rights Reserved.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+# ==============================================================================
+"""Heterogeneous Graph Transformers.
 
-package tensorflow_gnn.testdata;
+Users of TF-GNN can use this model by importing it next to the core library as
 
-import "tensorflow/core/example/example.proto";
+```python
+import tensorflow_gnn as tfgnn
+from tensorflow_gnn.models import hgt
+```
+"""
+from tensorflow_gnn.models.hgt import config_dict
+from tensorflow_gnn.models.hgt import layers
 
-// Specifies one or more Examples. This is used to aid testing readability by
-// allowing us to specify multiple Examples in an ASCII proto file.
-message ExampleList {
-  repeated tensorflow.Example examples = 1;
-}
+HGTGraphUpdate = layers.HGTGraphUpdate
+graph_update_get_config_dict = config_dict.graph_update_get_config_dict
+graph_update_from_config_dict = config_dict.graph_update_from_config_dict
+
+del config_dict
+del layers
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.proto` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.proto`

 * *Files 4% similar despite different names*

```diff
@@ -47,17 +47,28 @@
 // The top-level container for graph schemas.
 message GraphSchema {
   // A set of global context tensors. These are referenced by name from the
   // 'context' fields of the node sets and edge sets below.
   optional Context context = 1;
 
   // A list of available node sets. The keys are the NodeSet names.
+  //
+  // A name starting with `_` (preferred) or any of `#`, `!`, `%`, `.`, `^`, `~`
+  // (reserved for future use) marks an **auxiliary node set**, for use by
+  // certain TF-GNN helper functions; see `tfgnn.get_aux_type_prefix(name)` for
+  // more. These node sets are stored in the graph and do appear in the schema
+  // as usual, but modeling code ignores them when looking for the graph data
+  // from the application domain.
   map<string, NodeSet> node_sets = 2;
 
   // A list of available edge sets. The keys are the EdgeSet names.
+  //
+  // A name starting with `_` (preferred) or any of `#`, `!`, `%`, `.`, `^`, `~`
+  // (reserved for future use) marks an **auxiliary edge set**, analogous to the
+  // auxiliary node sets explained above; see `tfgnn.get_aux_type_prefix(name)`.
   map<string, EdgeSet> edge_sets = 3;
 
   // Optional metadata about the origin of the graph. Tools that produce graph
   // tensors should provide this detail.
   optional OriginInfo info = 4;
 }
 
@@ -107,15 +118,15 @@
 
   // THIS FIELD IS DEPRECATED.  TODO(b/266790186): Remove it.
   // Example feature data. This can be used both to document what the data looks
   // like in the schema proto, and also to sample from when generating bogus
   // example data. When generating random graph tensor= data, values are sampled
   // from any array you provided here. This allows us to generate random tensors
   // with more realistic values (that look more like the real thing).
-  optional tensorflow.Feature sample_values = 6;
+  optional tensorflow.Feature sample_values = 6 [deprecated = true];
 
   // Extension to attach domain-specific metadata about the feature.
   repeated tensorflow.Feature example_values = 5 [deprecated = true];
   extensions 65536 to max;
 }
 
 // Message describing a BigQuery table or SQL statement at a source for node
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/proto/graph_schema.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/proto/graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/BUILD`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "py_strict_test")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "distribute_py_test")
 
 licenses(["notice"])
 
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = ["//visibility:public"],
+)
+
 pytype_strict_library(
     name = "runner",
     srcs = ["__init__.py"],
     visibility = ["//visibility:public"],
     deps = [
         ":interfaces",
         ":orchestration",
         "//tensorflow_gnn/runner/input:datasets",
         "//tensorflow_gnn/runner/tasks:classification",
+        "//tensorflow_gnn/runner/tasks:link_prediction",
         "//tensorflow_gnn/runner/tasks:regression",
         "//tensorflow_gnn/runner/trainers:keras_fit",
         "//tensorflow_gnn/runner/utils:attribution",
-        "//tensorflow_gnn/runner/utils:model",
+        "//tensorflow_gnn/runner/utils:label_fns",
         "//tensorflow_gnn/runner/utils:model_dir",
         "//tensorflow_gnn/runner/utils:model_export",
-        "//tensorflow_gnn/runner/utils:model_templates",
         "//tensorflow_gnn/runner/utils:padding",
         "//tensorflow_gnn/runner/utils:strategies",
     ],
 )
 
 pytype_strict_library(
     name = "interfaces",
@@ -40,15 +45,14 @@
     name = "orchestration",
     srcs = ["orchestration.py"],
     srcs_version = "PY3",
     deps = [
         ":interfaces",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
-        "//tensorflow_gnn/runner/utils:model",
         "//tensorflow_gnn/runner/utils:model_export",
         "//tensorflow_gnn/runner/utils:parsing",
     ],
 )
 
 distribute_py_test(
     name = "distribute_test",
@@ -65,27 +69,27 @@
         "//third_party/py/immutabledict",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
         "//tensorflow_gnn/models/vanilla_mpnn",
         "//tensorflow_gnn/runner/tasks:classification",
         "//tensorflow_gnn/runner/tasks:regression",
         "//tensorflow_gnn/runner/trainers:keras_fit",
-        "//tensorflow_gnn/runner/utils:model_templates",
+        "//tensorflow_gnn/runner/utils:label_fns",
         "//tensorflow_gnn/runner/utils:padding",
     ],
 )
 
 py_strict_test(
     name = "orchestration_test",
     srcs = ["orchestration_test.py"],
     deps = [
+        ":interfaces",
         ":orchestration",
         "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
         "//tensorflow_gnn/models/vanilla_mpnn",
         "//tensorflow_gnn/runner/tasks:classification",
         "//tensorflow_gnn/runner/trainers:keras_fit",
-        "//tensorflow_gnn/runner/utils:model_templates",
-        "//tensorflow_gnn/runner/utils:padding",
+        "//tensorflow_gnn/runner/utils:label_fns",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/__init__.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,27 @@
 # limitations under the License.
 # ==============================================================================
 """A general purpose runner for TF-GNN."""
 from tensorflow_gnn.runner import interfaces
 from tensorflow_gnn.runner import orchestration
 from tensorflow_gnn.runner.input import datasets
 from tensorflow_gnn.runner.tasks import classification
+from tensorflow_gnn.runner.tasks import link_prediction
 from tensorflow_gnn.runner.tasks import regression
 from tensorflow_gnn.runner.trainers import keras_fit
 from tensorflow_gnn.runner.utils import attribution
-from tensorflow_gnn.runner.utils import model as model_utils
+from tensorflow_gnn.runner.utils import label_fns
 from tensorflow_gnn.runner.utils import model_dir
 from tensorflow_gnn.runner.utils import model_export
-from tensorflow_gnn.runner.utils import model_templates
 from tensorflow_gnn.runner.utils import padding as padding_utils
 from tensorflow_gnn.runner.utils import strategies
 
+# Attribution
+integrated_gradients = attribution.integrated_gradients
+
 # Input
 PassthruDatasetProvider = datasets.PassthruDatasetProvider
 PassthruSampleDatasetsProvider = datasets.PassthruSampleDatasetsProvider
 SimpleDatasetProvider = datasets.SimpleDatasetProvider
 SimpleSampleDatasetsProvider = datasets.SimpleSampleDatasetsProvider
 SampleTFRecordDatasetsProvider = datasets.SampleTFRecordDatasetsProvider
 TFRecordDatasetProvider = datasets.TFRecordDatasetProvider
@@ -38,26 +41,28 @@
 # Interfaces
 DatasetProvider = interfaces.DatasetProvider
 GraphTensorPadding = interfaces.GraphTensorPadding
 GraphTensorProcessorFn = interfaces.GraphTensorProcessorFn
 ModelExporter = interfaces.ModelExporter
 Trainer = interfaces.Trainer
 Task = interfaces.Task
+RunResult = interfaces.RunResult
+
+# Label fns
+ContextLabelFn = label_fns.ContextLabelFn
+RootNodeLabelFn = label_fns.RootNodeLabelFn
 
 # Model directory
 incrementing_model_dir = model_dir.incrementing_model_dir
 
 # Model export
 IntegratedGradientsExporter = attribution.IntegratedGradientsExporter
 KerasModelExporter = model_export.KerasModelExporter
 SubmoduleExporter = model_export.SubmoduleExporter
 
-# Model helpers
-chain_first_output = model_utils.chain_first_output
-
 # Orchestration
 run = orchestration.run
 TFDataServiceConfig = orchestration.TFDataServiceConfig
 
 # Padding
 one_node_per_component = padding_utils.one_node_per_component
 FitOrSkipPadding = padding_utils.FitOrSkipPadding
@@ -73,39 +78,43 @@
 # in `distribute_test.py`.)
 #
 # Tasks (Classification)
 RootNodeBinaryClassification = classification.RootNodeBinaryClassification
 RootNodeMulticlassClassification = classification.RootNodeMulticlassClassification
 GraphBinaryClassification = classification.GraphMulticlassClassification
 GraphMulticlassClassification = classification.GraphMulticlassClassification
+# Tasks (Link Prediction)
+DotProductLinkPrediction = link_prediction.DotProductLinkPrediction
+HadamardProductLinkPrediction = link_prediction.HadamardProductLinkPrediction
 # Tasks (Regression)
 GraphMeanAbsoluteError = regression.GraphMeanAbsoluteError
 GraphMeanAbsolutePercentageError = regression.GraphMeanAbsolutePercentageError
 GraphMeanSquaredError = regression.GraphMeanSquaredError
 GraphMeanSquaredLogarithmicError = regression.GraphMeanSquaredLogarithmicError
 GraphMeanSquaredLogScaledError = regression.GraphMeanSquaredLogScaledError
 RootNodeMeanAbsoluteError = regression.RootNodeMeanAbsoluteError
 RootNodeMeanAbsolutePercentageError = regression.RootNodeMeanAbsolutePercentageError
 RootNodeMeanSquaredError = regression.RootNodeMeanSquaredError
 RootNodeMeanSquaredLogarithmicError = regression.RootNodeMeanSquaredLogarithmicError
 RootNodeMeanSquaredLogScaledError = regression.RootNodeMeanSquaredLogScaledError
+RootNodeMeanAbsoluteLogarithmicError = (
+    regression.RootNodeMeanAbsoluteLogarithmicError
+)
 
 # Training
 KerasTrainer = keras_fit.KerasTrainer
 KerasTrainerOptions = keras_fit.KerasTrainerOptions
 KerasTrainerCheckpointOptions = keras_fit.KerasTrainerCheckpointOptions
 
-# Model templates
-ModelFromInitAndUpdates = model_templates.ModelFromInitAndUpdates
-
+del interfaces
 del orchestration
 del datasets
 del classification
+del link_prediction
 del regression
 del keras_fit
 del attribution
-del model_utils
+del label_fns
 del model_dir
 del model_export
-del model_templates
 del padding_utils
 del strategies
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/distribute_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/distribute_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,19 +24,21 @@
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.models import vanilla_mpnn
 from tensorflow_gnn.runner import interfaces
 from tensorflow_gnn.runner import orchestration
 from tensorflow_gnn.runner.tasks import classification
 from tensorflow_gnn.runner.tasks import regression
 from tensorflow_gnn.runner.trainers import keras_fit
-from tensorflow_gnn.runner.utils import model_templates
+from tensorflow_gnn.runner.utils import label_fns
 from tensorflow_gnn.runner.utils import padding
 
 _LABELS = tuple(range(32))
+
 _SAMPLE_DICT = immutabledict({(tfgnn.CONTEXT, None, "label"): _LABELS})
+
 _SCHEMA = """
   context {
     features {
       key: "label"
       value {
         dtype: DT_INT32
       }
@@ -59,16 +61,14 @@
     value {
       source: "node"
       target: "node"
     }
   }
 """
 
-TaskAndProcessor = tuple[interfaces.Task, interfaces.GraphTensorProcessorFn]
-
 
 def _all_eager_strategy_combinations():
   strategies = [
       # default
       tfdistribute.combinations.default_strategy,
       # MirroredStrategy
       tfdistribute.combinations.mirrored_strategy_with_gpu_and_cpu,
@@ -86,63 +86,78 @@
       tfdistribute.combinations.parameter_server_strategy_3worker_2ps_1gpu,
       tfdistribute.combinations.parameter_server_strategy_1worker_2ps_cpu,
       tfdistribute.combinations.parameter_server_strategy_1worker_2ps_1gpu,
   ]
   return tftest.combinations.combine(distribution=strategies)
 
 
-def _all_task_and_processors_combinations():
+def _all_task_combinations():
 
-  def extract_binary_labels(gt):
-    return gt, gt.context["label"] % 2
+  def extract_binary_labels(inputs):
+    x, y = label_fns.ContextLabelFn("label")(inputs)
+    return x, y % 2
 
-  def extract_multiclass_labels(gt):
-    return gt, gt.context["label"]
+  def extract_multiclass_labels(inputs):
+    return label_fns.ContextLabelFn("label")(inputs)
 
-  def extract_regression_labels(gt):
-    return gt, tf.ones_like(gt.context["label"], dtype=tf.float32)
+  def extract_regression_labels(inputs):
+    x, y = label_fns.ContextLabelFn("label")(inputs)
+    return x, tf.ones_like(y, dtype=tf.float32)
 
-  task_and_processor = {
+  tasks = [
       # Root node classification
-      classification.RootNodeBinaryClassification(node_set_name="node"):
-          extract_binary_labels,
+      classification.RootNodeBinaryClassification(
+          "node",
+          label_fn=extract_binary_labels),
       classification.RootNodeMulticlassClassification(
-          node_set_name="node",
-          num_classes=len(_LABELS)): extract_multiclass_labels,
+          "node",
+          num_classes=len(_LABELS),
+          label_fn=extract_multiclass_labels),
       # Graph classification
-      classification.GraphBinaryClassification(node_set_name="node"):
-          extract_binary_labels,
+      classification.GraphBinaryClassification(
+          "node",
+          label_fn=extract_binary_labels),
       classification.GraphMulticlassClassification(
-          node_set_name="node",
-          num_classes=len(_LABELS)): extract_multiclass_labels,
+          "node",
+          num_classes=len(_LABELS),
+          label_fn=extract_multiclass_labels),
       # Root node regression
-      regression.RootNodeMeanAbsoluteError(node_set_name="node"):
-          extract_regression_labels,
-      regression.RootNodeMeanAbsolutePercentageError(node_set_name="node"):
-          extract_regression_labels,
-      regression.RootNodeMeanSquaredError(node_set_name="node"):
-          extract_regression_labels,
-      regression.RootNodeMeanSquaredLogarithmicError(node_set_name="node"):
-          extract_regression_labels,
-      regression.RootNodeMeanSquaredLogScaledError(node_set_name="node"):
-          extract_regression_labels,
+      regression.RootNodeMeanAbsoluteError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.RootNodeMeanAbsolutePercentageError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.RootNodeMeanSquaredError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.RootNodeMeanSquaredLogarithmicError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.RootNodeMeanSquaredLogScaledError(
+          "node",
+          label_fn=extract_regression_labels),
       # Graph regression
-      regression.GraphMeanAbsoluteError(node_set_name="node"):
-          extract_regression_labels,
-      regression.GraphMeanAbsolutePercentageError(node_set_name="node"):
-          extract_regression_labels,
-      regression.GraphMeanSquaredError(node_set_name="node"):
-          extract_regression_labels,
-      regression.GraphMeanSquaredLogarithmicError(node_set_name="node"):
-          extract_regression_labels,
-      regression.GraphMeanSquaredLogScaledError(node_set_name="node"):
-          extract_regression_labels,
-  }
-  items = list(task_and_processor.items())
-  return tftest.combinations.combine(task_and_processor=items)
+      regression.GraphMeanAbsoluteError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.GraphMeanAbsolutePercentageError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.GraphMeanSquaredError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.GraphMeanSquaredLogarithmicError(
+          "node",
+          label_fn=extract_regression_labels),
+      regression.GraphMeanSquaredLogScaledError(
+          "node",
+          label_fn=extract_regression_labels),
+  ]
+  return tftest.combinations.combine(task=tasks)
 
 
 class DatasetProvider(interfaces.DatasetProvider):
 
   def __init__(self, examples: Sequence[bytes]):
     self._examples = list(examples)
 
@@ -151,37 +166,40 @@
 
 
 class OrchestrationTests(tf.test.TestCase, parameterized.TestCase):
 
   @tfdistribute.combinations.generate(
       tftest.combinations.times(
           _all_eager_strategy_combinations(),
-          _all_task_and_processors_combinations()
+          _all_task_combinations()
       )
   )
   def test_run(
       self,
       distribution: tf.distribute.Strategy,
-      task_and_processor: TaskAndProcessor):
+      task: interfaces.Task):
     schema = tfgnn.parse_schema(_SCHEMA)
     gtspec = tfgnn.create_graph_spec_from_schema_pb(schema)
     gt = tfgnn.write_example(tfgnn.random_graph_tensor(
         gtspec,
         sample_dict=_SAMPLE_DICT))
     ds_provider = DatasetProvider((gt.SerializeToString(),) * 4)
 
-    node_sets_fn = lambda node_set, node_set_name: node_set["features"]
-    model_fn = model_templates.ModelFromInitAndUpdates(
-        init=tfgnn.keras.layers.MapFeatures(node_sets_fn=node_sets_fn),
-        updates=[vanilla_mpnn.VanillaMPNNGraphUpdate(
-            units=1,
-            message_dim=2,
-            receiver_tag=tfgnn.SOURCE,
-            l2_regularization=5e-4,
-            dropout_rate=0.1)])
+    def model_fn(graph_tensor_spec):
+      graph = inputs = tf.keras.layers.Input(type_spec=graph_tensor_spec)
+      graph = tfgnn.keras.layers.MapFeatures(
+          node_sets_fn=lambda node_set, node_set_name: node_set["features"]
+      )(graph)
+      graph = vanilla_mpnn.VanillaMPNNGraphUpdate(
+          units=1,
+          message_dim=2,
+          receiver_tag=tfgnn.SOURCE,
+          l2_regularization=5e-4,
+          dropout_rate=0.1)(graph)
+      return tf.keras.Model(inputs, graph)
 
     model_dir = self.create_tempdir()
 
     trainer = keras_fit.KerasTrainer(
         strategy=distribution,
         model_dir=model_dir,
         steps_per_epoch=1,
@@ -195,27 +213,24 @@
           fit_or_skip_sample_sample_size=5,
           fit_or_skip_success_ratio=0.7)
       valid_padding = padding.TightPadding(gtspec, ds_provider)
     else:
       train_padding = None
       valid_padding = None
 
-    task, processor = task_and_processor
-
     orchestration.run(
         train_ds_provider=ds_provider,
         train_padding=train_padding,
         model_fn=model_fn,
         optimizer_fn=tf.keras.optimizers.Adam,
         epochs=1,
         trainer=trainer,
         task=task,
         gtspec=gtspec,
         global_batch_size=2,
-        feature_processors=(processor,),
         valid_ds_provider=ds_provider,
         valid_padding=valid_padding)
 
     dataset = ds_provider.get_dataset(tf.distribute.InputContext())
     kwargs = {"examples": next(iter(dataset.batch(2)))}
 
     saved_model = tf.saved_model.load(os.path.join(model_dir, "export"))
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/examples/ogbn/mag/train.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/examples/ogbn/mag/train.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """An e2e training example for OGBN-MAG."""
+
 import functools
 from typing import Any, Callable, Mapping, Optional, Sequence
 
 from absl import app
 from absl import flags
 from absl import logging
 from ml_collections import config_dict
 from ml_collections import config_flags
-
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
-
 from tensorflow_gnn import runner
+from tensorflow_gnn.models import gat_v2
+from tensorflow_gnn.models import hgt
+from tensorflow_gnn.models import mt_albis
 from tensorflow_gnn.models import multi_head_attention
 from tensorflow_gnn.models import vanilla_mpnn
+from tensorflow_gnn.runner.examples.ogbn.mag import utils
+
 
 FLAGS = flags.FLAGS
 
 _SAMPLES_FORMAT = flags.DEFINE_string(
     "samples_format",
     "tfrecord",
     "Indicates the file format for --samples.")
@@ -49,21 +53,34 @@
     None,
     "A filepath for the GraphSchema of the --samples.",
     required=True)
 
 _BASE_DIR = flags.DEFINE_string(
     "base_dir",
     None,
-    "The training and export base directory "
-    "(`runner.incrementing_model_dir(...)` is used to generate the model "
-    "directory).",
-    required=True)
+    (
+        "The training base directory ("
+        "`runner.incrementing_model_dir(...)` is used to generate the model "
+        "directory)."
+    ),
+    required=True,
+)
 
-_TPU_ADDRESS = flags.DEFINE_string(
-    "tpu_address",
+_EXPORT_DIR = flags.DEFINE_string(
+    "export_dir",
+    None,
+    (
+        "Directory where the model will be exported to. If not specified, a "
+        "default is chosen by the TF-GNN runner. See `runner.run()` for "
+        "details."
+    ),
+)
+
+_TPU = flags.DEFINE_string(
+    "tpu",
     None,
     "An optional TPU address "
     "(see: `tf.distribute.cluster_resolver.TPUClusterResolver`), if empty "
     "string: TensorFlow will try to automatically resolve the Cloud TPU; if "
     "`None`: `MirroredStrategy` is used.")
 
 _EPOCHS = flags.DEFINE_integer(
@@ -85,59 +102,113 @@
     "The initial learning rate of the learning rate schedule.")
 
 _PAPER_DIM = flags.DEFINE_integer(
     "paper_dim", 512,
     "Dimensionality of dense layer applied to paper features. "
     "Set to '0' for no dense transform.")
 
+_READOUT_USE_SKIP_CONNECTION = flags.DEFINE_boolean(
+    "readout_use_skip_connection", False,
+    "If set, readout of GNN states for prediction extends the final state "
+    "by concatenation with the initial state.")
+
+_MASKED_LABELS = flags.DEFINE_enum(
+    "masked_labels",
+    None,
+    ["standard", "causal"],
+    "If set to None, does not utilize training labels as features. If set to "
+    "standard, masks the seed node as well as the validation and test nodes "
+    "following https://ogb.stanford.edu/docs/leader_rules/. If set to causal, "
+    "additionally masks the neighbour nodes published in the same year or "
+    "after the seed node.")
+
 
 # The GNN model used by this script is configured by a ConfigDict
 # (see https://github.com/google/ml_collections).
 # The following function defines the available configuration options
 # and their default values. The subsequent config_flags definition
 # allows users to override them from the command line, for example,
 # --config.gnn.vanilla_mpnn.dropout_rate = 0.1
+# TODO(b/290314181): The model choice should also be able to influence
+# non-model hparams.
 def get_config_dict() -> config_dict.ConfigDict:
   """The default config that users can override with --config.foo=bar."""
   cfg = config_dict.ConfigDict()
   cfg.gnn = config_dict.ConfigDict()
-  cfg.gnn.type = "vanilla_mpnn"
   # For each supported gnn.type="foo", there is a config gnn.foo for that type's
   # GraphUpdate class, overridden with the defaults for this training.
-  cfg.gnn.vanilla_mpnn = vanilla_mpnn.graph_update_get_config_dict()
-  cfg.gnn.vanilla_mpnn.units = 128
-  cfg.gnn.vanilla_mpnn.message_dim = 128
-  cfg.gnn.vanilla_mpnn.receiver_tag = tfgnn.SOURCE
-  cfg.gnn.vanilla_mpnn.dropout_rate = 0.2
-  cfg.gnn.vanilla_mpnn.l2_regularization = 6e-6
-  cfg.gnn.vanilla_mpnn.use_layer_normalization = True
-  # Config for multi head attention
+  cfg.gnn.type = "vanilla_mpnn"
+  # For gnn.type="gat_v2":
+  cfg.gnn.gat_v2 = gat_v2.graph_update_get_config_dict()
+  cfg.gnn.gat_v2.units = 128
+  cfg.gnn.gat_v2.message_dim = 128
+  cfg.gnn.gat_v2.num_heads = 4
+  cfg.gnn.gat_v2.receiver_tag = tfgnn.SOURCE
+  cfg.gnn.gat_v2.state_dropout_rate = 0.1
+  cfg.gnn.gat_v2.l2_regularization = 5e-6
+  cfg.gnn.gat_v2.edge_dropout_rate = 0.1
+  # For gnn.type="hgt":
+  cfg.gnn.hgt = hgt.graph_update_get_config_dict()
+  cfg.gnn.hgt.per_head_channels = 64
+  cfg.gnn.hgt.num_heads = 8
+  cfg.gnn.hgt.receiver_tag = tfgnn.SOURCE
+  cfg.use_weighted_skip = True
+  cfg.dropout_rate = 0.2
+  cfg.use_layer_norm = True
+  cfg.use_bias = True
+  cfg.activation = "gelu"
+  # For gnn.type="mt_albis":
+  cfg.gnn.mt_albis = mt_albis.graph_update_get_config_dict()
+  cfg.gnn.mt_albis.units = 256
+  cfg.gnn.mt_albis.message_dim = 256
+  cfg.gnn.mt_albis.receiver_tag = tfgnn.SOURCE
+  cfg.gnn.mt_albis.simple_conv_reduce_type = "mean|sum"
+  cfg.gnn.mt_albis.state_dropout_rate = 0.1
+  cfg.gnn.mt_albis.edge_dropout_rate = 0.2
+  cfg.gnn.mt_albis.l2_regularization = 1e-5
+  cfg.gnn.mt_albis.normalization_type = "layer"
+  cfg.gnn.mt_albis.next_state_type = "residual"
+  # For gnn.type="multi head attention":
   cfg.gnn.multi_head_attention = (
       multi_head_attention.graph_update_get_config_dict())
   cfg.gnn.multi_head_attention.units = 128
   cfg.gnn.multi_head_attention.message_dim = 128
   cfg.gnn.multi_head_attention.num_heads = 4
   cfg.gnn.multi_head_attention.receiver_tag = tfgnn.SOURCE
   cfg.gnn.multi_head_attention.state_dropout_rate = 0.2
   cfg.gnn.multi_head_attention.l2_regularization = 6e-6
   cfg.gnn.multi_head_attention.edge_dropout_rate = 0.2
+  # For gnn.type="vanilla_mpnn":
+  cfg.gnn.vanilla_mpnn = vanilla_mpnn.graph_update_get_config_dict()
+  cfg.gnn.vanilla_mpnn.units = 256
+  cfg.gnn.vanilla_mpnn.message_dim = 256
+  cfg.gnn.vanilla_mpnn.receiver_tag = tfgnn.SOURCE
+  cfg.gnn.vanilla_mpnn.dropout_rate = 0.2
+  cfg.gnn.vanilla_mpnn.l2_regularization = 2e-6
+  cfg.gnn.vanilla_mpnn.use_layer_normalization = True
   cfg.lock()
   return cfg
 
 _CONFIG = config_flags.DEFINE_config_dict("config", get_config_dict())
 
 
 def _graph_update_from_config(
     cfg: config_dict.ConfigDict) -> tf.keras.layers.Layer:
   """Returns one instance of the configured GraphUpdate layer."""
-  if cfg.gnn.type == "vanilla_mpnn":
-    return vanilla_mpnn.graph_update_from_config_dict(cfg.gnn.vanilla_mpnn)
+  if cfg.gnn.type == "gat_v2":
+    return gat_v2.graph_update_from_config_dict(cfg.gnn.gat_v2)
+  elif cfg.gnn.type == "hgt":
+    return hgt.graph_update_from_config_dict(cfg.gnn.hgt)
+  elif cfg.gnn.type == "mt_albis":
+    return mt_albis.graph_update_from_config_dict(cfg.gnn.mt_albis)
   elif cfg.gnn.type == "multi_head_attention":
     return multi_head_attention.graph_update_from_config_dict(
         cfg.gnn.multi_head_attention)
+  elif cfg.gnn.type == "vanilla_mpnn":
+    return vanilla_mpnn.graph_update_from_config_dict(cfg.gnn.vanilla_mpnn)
   else:
     raise ValueError(f"Unknown gnn.type: {cfg.gnn.type}")
 
 
 # The following helper lets us filter a single input dataset by OGBN-MAG's
 # specific rule for the test/validation/train split before parsing the full
 # GraphTensor. (Models for production systems should probably use separate
@@ -173,14 +244,17 @@
     self._delegate = delegate
     self._split_name = split_name
 
   def get_dataset(self, context: tf.distribute.InputContext) -> tf.data.Dataset:
     dataset = self._delegate.get_dataset(context)
     return dataset.filter(_is_in_split(self._split_name))
 
+_NUM_CLASSES = 349
+_FIELD_OF_STUDY_BINS = 50_000
+_INSTITUTION_BINS = 6_500
 _DEFAULT_DATASET_FORMATS = {
     "tfrecord": runner.TFRecordDatasetProvider,
 }
 
 
 def main(
     args,
@@ -198,69 +272,122 @@
   ds_provider = dataset_formats[_SAMPLES_FORMAT.value](_SAMPLES.value)
   train_ds_provider = _SplitDatasetProvider(ds_provider, "train")
   valid_ds_provider = _SplitDatasetProvider(ds_provider, "validation")
 
   graph_schema = tfgnn.read_schema(_GRAPH_SCHEMA.value)
   gtspec = tfgnn.create_graph_spec_from_schema_pb(graph_schema)
 
-  def extract_labels(graphtensor: tfgnn.GraphTensor):
-    labels = tfgnn.keras.layers.ReadoutFirstNode(
-        node_set_name="paper",
-        feature_name="labels")(graphtensor)
-    graphtensor = graphtensor.remove_features(node_sets={"paper": ["labels"]})
-    return graphtensor, labels
-
   def drop_all_features(_, **unused_kwargs):
     return {}
 
+  def process_paper_node_features(node_set: tfgnn.NodeSet):
+    if _MASKED_LABELS.value:
+      logging.info("Utilizing training labels as features for training.")
+      # Mask for validation and test node labels.
+      year_feature = node_set["year"]
+      extra_label_mask = year_feature >= 2018
+      if _MASKED_LABELS.value == "causal":
+        logging.info(
+            "Masking neighbours published after or in the same year as seed"
+            " node"
+        )
+        extra_label_mask = tf.math.logical_or(
+            extra_label_mask, utils.make_causal_mask(node_set)
+        )
+      masked_labels = utils.mask_paper_labels(
+          node_set, label_feature_name="labels", mask_value=_NUM_CLASSES,
+          extra_label_mask=extra_label_mask)
+      return {
+          "feat": node_set["feat"],
+          "labels": node_set["labels"],
+          "masked_labels": masked_labels,
+      }
+    return {"feat": node_set["feat"], "labels": node_set["labels"]}
+
   def  process_node_features(node_set: tfgnn.NodeSet, node_set_name: str):
     if node_set_name == "field_of_study":
-      return {"hashed_id": tf.keras.layers.Hashing(50_000)(node_set["#id"])}
+      return {
+          "hashed_id": tf.keras.layers.Hashing(_FIELD_OF_STUDY_BINS)(
+              node_set["#id"]
+          )
+      }
     if node_set_name == "institution":
-      return {"hashed_id": tf.keras.layers.Hashing(6_500)(node_set["#id"])}
+      return {
+          "hashed_id": tf.keras.layers.Hashing(_INSTITUTION_BINS)(
+              node_set["#id"]
+          )
+      }
     if node_set_name == "paper":
-      return {"feat": node_set["feat"]}
+      return process_paper_node_features(node_set)
     if node_set_name == "author":
       return {"empty_state": tfgnn.keras.layers.MakeEmptyFeature()(node_set)}
     raise KeyError(f"Unexpected node_set_name='{node_set_name}'")
 
+  def set_paper_node_state(node_set: tfgnn.NodeSet):
+    embedding_list = []
+    # Paper title features
+    if not _PAPER_DIM.value:
+      logging.info("Skipping dense layer for paper.")
+      embedding_list.append(node_set["feat"])
+    else:
+      logging.info("Applying dense layer %d to paper.", _PAPER_DIM.value)
+      embedding_list.append(
+          tf.keras.layers.Dense(_PAPER_DIM.value)(node_set["feat"])
+      )
+    # Masked label
+    if _MASKED_LABELS.value:
+      embedding_list.append(
+          tf.keras.layers.Embedding(_NUM_CLASSES + 1, 64)(
+              node_set["masked_labels"]
+          )
+      )
+    return tf.keras.layers.Concatenate()(embedding_list)
+
   def set_initial_node_states(node_set: tfgnn.NodeSet, node_set_name: str):
     if node_set_name == "field_of_study":
-      return tf.keras.layers.Embedding(50_000, 32)(node_set["hashed_id"])
+      return tf.keras.layers.Embedding(_FIELD_OF_STUDY_BINS, 32)(
+          node_set["hashed_id"]
+      )
     if node_set_name == "institution":
-      return tf.keras.layers.Embedding(6_500, 16)(node_set["hashed_id"])
+      return tf.keras.layers.Embedding(_INSTITUTION_BINS, 16)(
+          node_set["hashed_id"]
+      )
     if node_set_name == "paper":
-      if not _PAPER_DIM.value:
-        logging.info("Skipping dense layer for paper.")
-        return node_set["feat"]
-      logging.info("Applying dense layer %d to paper.", _PAPER_DIM.value)
-      return tf.keras.layers.Dense(_PAPER_DIM.value)(node_set["feat"])
+      return set_paper_node_state(node_set)
     if node_set_name == "author":
       return node_set["empty_state"]
     raise KeyError(f"Unexpected node_set_name='{node_set_name}'")
 
+  task_node_set_name = "paper"
+  task = runner.RootNodeMulticlassClassification(
+      node_set_name=task_node_set_name,
+      num_classes=_NUM_CLASSES,
+      label_fn=runner.RootNodeLabelFn("paper", feature_name="labels"))
+
   def model_fn(gtspec: tfgnn.GraphTensorSpec):
-    graph = inputs = tf.keras.layers.Input(type_spec=gtspec)
-    graph = tfgnn.keras.layers.MapFeatures(
-        node_sets_fn=set_initial_node_states)(graph)
+    model_inputs = tf.keras.layers.Input(type_spec=gtspec)
+    graph = gnn_inputs = tfgnn.keras.layers.MapFeatures(
+        node_sets_fn=set_initial_node_states)(model_inputs)
     for _ in range(4):
       graph_update = _graph_update_from_config(_CONFIG.value)
       graph = graph_update(graph)
-    return tf.keras.Model(inputs, graph)
-
-  task = runner.RootNodeMulticlassClassification(
-      node_set_name="paper",
-      num_classes=349)
+    if _READOUT_USE_SKIP_CONNECTION.value:
+      # TODO(b/234563300): Allow `graph = MapFeatures(...)(graph, gnn_inputs)`.
+      initial_features = gnn_inputs.node_sets[task_node_set_name].features
+      features = graph.node_sets[task_node_set_name].get_features_dict()
+      features[tfgnn.HIDDEN_STATE] = tf.keras.layers.Concatenate()(
+          [features[tfgnn.HIDDEN_STATE], initial_features[tfgnn.HIDDEN_STATE]])
+      graph = graph.replace_features(node_sets={task_node_set_name: features})
+    return tf.keras.Model(model_inputs, graph)
 
   global_batch_size = 128
-  validation_batch_size = 32
   steps_per_epoch = 629_571 // global_batch_size  # len(train) == 629,571
 
   # len(validation) == 64,879
-  validation_steps = 64_879 // validation_batch_size
+  validation_steps = 64_879 // global_batch_size
 
   # Determine learning rate schedule
   if _LEARNING_RATE_SCHEDULE.value == "cosine_decay":
     learning_rate = tf.keras.optimizers.schedules.CosineDecay(
         _LEARNING_RATE.value, steps_per_epoch*_EPOCHS.value)
   elif _LEARNING_RATE_SCHEDULE.value == "constant":
     learning_rate = _LEARNING_RATE.value
@@ -268,16 +395,16 @@
     raise ValueError(
         f"Learning rate schedule '{_LEARNING_RATE_SCHEDULE.value}' not defined")
 
   # Optimizer Function
   optimizer_fn = functools.partial(tf.keras.optimizers.Adam,
                                    learning_rate=learning_rate)
 
-  if _TPU_ADDRESS.value is not None:
-    strategy = runner.TPUStrategy(_TPU_ADDRESS.value)
+  if _TPU.value is not None:
+    strategy = runner.TPUStrategy(_TPU.value)
     # Update `min_nodes_per_component.` Default requirement of at least one node
     # from each node set in input is sufficient but more than necessary.
     # The condition that each graph component must contain at least one "paper"
     # node is sufficient.
     min_nodes_per_component = {"paper": 1}
     train_padding = runner.FitOrSkipPadding(gtspec, train_ds_provider,
                                             min_nodes_per_component)
@@ -295,30 +422,33 @@
       steps_per_epoch=steps_per_epoch,
       validation_steps=validation_steps,
       restore_best_weights=_RESTORE_BEST_WEIGHTS.value,
       checkpoint_every_n_steps=("epoch" if _RESTORE_BEST_WEIGHTS.value
                                 else "never"),
   )
 
+  export_dirs = [_EXPORT_DIR.value] if _EXPORT_DIR.value is not None else None
   runner.run(
       train_ds_provider=train_ds_provider,
       train_padding=train_padding,
       model_fn=model_fn,
       optimizer_fn=optimizer_fn,
       epochs=_EPOCHS.value,
       trainer=trainer,
       task=task,
       gtspec=gtspec,
       global_batch_size=global_batch_size,
+      export_dirs=export_dirs,
       feature_processors=[
-          extract_labels,  # Extract any labels first!
           tfgnn.keras.layers.MapFeatures(
               context_fn=drop_all_features,
               node_sets_fn=process_node_features,
-              edge_sets_fn=drop_all_features)
+              edge_sets_fn=drop_all_features,
+          ),
       ],
       valid_ds_provider=valid_ds_provider,
-      valid_padding=valid_padding)
+      valid_padding=valid_padding,
+  )
 
 
 if __name__ == "__main__":
   app.run(main)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,15 @@
       required iff `extra_weights` are also provided.
 
     The choice of `principal_dataset` is important and should, in most
     cases, be chosen as the largest underlying dataset as compared to
     `extra_datasets.` `positives` and `negatives` where `len(negatives)` >>
     `len(positives)` and with `positives` corresponding to `principal_dataset,`
     the desired behavior of epochs determined by the exhaustion of `positives`
-    and the contined mixing of unique elements from `negatives` may not occur:
+    and the continued mixing of unique elements from `negatives` may not occur:
     On sampled dataset reiteration `positives` will again be exhausted but
     elements from `negatives` may be those same seen in the previous epoch
     (as they occur at the beginning of the same, reiterated underlying
     `negatives` dataset). In this case, the recommendations are to:
 
     1) Reformulate the sampling in terms of the larger dataset (`negatives`),
        where, with `fixed_cardinality=False`, if the exhaustion of `negatives`
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/input/datasets_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/input/datasets_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/interfaces.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/interfaces.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,35 +9,66 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Interfaces for the runner entry point."""
+from __future__ import annotations
+
 import abc
+import dataclasses
 import sys
-from typing import Callable, Optional, Sequence, Tuple, Union
+from typing import Callable, Optional, Sequence, TypeVar, Union
 
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 
 # pylint:disable=g-import-not-at-top
 if sys.version_info >= (3, 8):
   from typing import Protocol
   from typing import runtime_checkable
 else:
   from typing_extensions import Protocol
   from typing_extensions import runtime_checkable
 # pylint:enable=g-import-not-at-top
 
+T = TypeVar("T")
+OneOrSequenceOf = Union[T, Sequence[T]]
+
+Field = tfgnn.Field
 GraphTensor = tfgnn.GraphTensor
-GraphTensorAndField = Tuple[GraphTensor, tfgnn.Field]
 SizeConstraints = tfgnn.SizeConstraints
 
 
+@dataclasses.dataclass
+class RunResult:
+  """Holds the return values of `run(...)`.
+
+  Attributes:
+    preprocess_model: Keras model containing only the computation for
+      preprocessing inputs. It is not trained. The model takes serialized
+      `GraphTensor`s as its inputs and returns preprocessed `GraphTensor`s.
+      `None` when no preprocess model exists.
+    base_model: Keras base GNN (as returned by the user provided `model_fn`).
+      The model both takes and returns `GraphTensor`s. The model contains
+      any--but not all--trained weights. The `trained_model` contains all
+      `base_model` trained weights in addition to any prediction trained
+      weights.
+    trained_model: Keras model for the e2e GNN. (Base GNN plus any prediction
+      head(s).) The model takes `preprocess_model` output as its inputs and
+      returns `Task` predictions as its output. Output matches the structure of
+      the `Task`: an atom for single- or a mapping for multi- `Task` training.
+      The model contains all trained weights.
+  """
+  preprocess_model: Optional[tf.keras.Model]
+  base_model: tf.keras.Model
+  trained_model: tf.keras.Model
+
+
 class DatasetProvider(abc.ABC):
 
   @abc.abstractmethod
   def get_dataset(self, context: tf.distribute.InputContext) -> tf.data.Dataset:
     """Get a `tf.data.Dataset` by `context` per replica."""
     raise NotImplementedError()
 
@@ -56,103 +87,125 @@
     raise NotImplementedError()
 
 
 @runtime_checkable
 class GraphTensorProcessorFn(Protocol):
   """A class for `GraphTensor` processing."""
 
-  def __call__(
-      self,
-      gt: GraphTensor) -> Union[GraphTensor, GraphTensorAndField]:
-    """Processes a `GraphTensor` with optional `Field` extraction.
-
-    Args:
-      gt: A `GraphTensor` for processing.
-
-    Returns:
-      A processed `GraphTensor` or a processed `GraphTensor` and `Field.`
-    """
+  def __call__(self, inputs: GraphTensor) -> GraphTensor:
+    """Processes a `GraphTensor`."""
     raise NotImplementedError()
 
 
 class ModelExporter(abc.ABC):
   """Saves a Keras model."""
 
   @abc.abstractmethod
-  def save(
-      self,
-      preprocess_model: Optional[tf.keras.Model],
-      model: tf.keras.Model,
-      export_dir: str):
+  def save(self, run_result: RunResult, export_dir: str):
     """Saves a Keras model.
 
     All persistence decisions are left to the implementation: e.g., a Keras
     model with full API or a simple `tf.train.Checkpoint` may be saved.
 
     Args:
-      preprocess_model: An optional `tf.keras.Model` for preprocessing.
-      model: A `tf.keras.Model` to save.
-      export_dir: A destination directory for the model.
+      run_result: A `RunResult` from training.
+      export_dir: A destination directory.
     """
     raise NotImplementedError()
 
 
 class Task(abc.ABC):
-  """Collects the ancillary, supporting pieces to train a Keras model.
+  """Defines a learning objective for a GNN.
 
-  `Task`s are applied and used to compile a `tf.keras.Model` in the scope
-  of a training invocation: they are subject to the executing context
-  of the `Trainer` and should, when needed, override it (e.g., a global
-  policy, like `tf.keras.mixed_precision.global_policy()` and its implications
-  over logit and activation layers).
-
-  A `Task` is expected to coordinate all of its methods and their return values
-  to define a graph learning objective. Precisely:
-
-  1) `preprocess` is expected to return a `GraphTensor` or
-     (`GraphTensor`, `Field`) where the `GraphTensor` matches the input of the
-     model returned by `adapt` and the `Field` is a training label
-  2) `adapt` is expected to return a `tf.keras.Model` that accepts a
-     `GraphTensor` matching the output of `preprocess`
+  A `Task` represents a learning objective for a GNN model and defines all the
+  non-GNN pieces around the base GNN. Specifically:
+
+  1) `preprocess` is expected to return a `GraphTensor` (or `GraphTensor`s) and
+     a `Field` where (a) the base GNN's output for each `GraphTensor` is passed
+     to `predict` and (b) the `Field` is used as the training label (for
+     supervised tasks);
+  2) `predict` is expected to (a) take the base GNN's output for each
+     `GraphTensor` returned by `preprocess` and (b) return a tensor with the
+     model's prediction for this task;
   3) `losses` is expected to return callables (`tf.Tensor`, `tf.Tensor`) ->
      `tf.Tensor` that accept (`y_true`, `y_pred`) where `y_true` is produced
-     by some dataset and `y_pred` is output of the adapted model (see (2))
+     by some dataset and `y_pred` is the model's prediction from (2);
   4) `metrics` is expected to return callables (`tf.Tensor`, `tf.Tensor`) ->
      `tf.Tensor` that accept (`y_true`, `y_pred`) where `y_true` is produced
-     by some dataset and `y_pred` is output of the adapted model (see (2)).
+     by some dataset and `y_pred` is the model's prediction from (2).
 
-  No constraints are made on the `adapt` method; e.g.: it may adapt its input by
-  appending a head, it may add losses to its input, it may add metrics to its
-  input or it may do any combination of the aforementioned modifications. The
-  `adapt` method is expected to adapt an arbitrary `tf.keras.Model` to the graph
-  learning objective. (The entire `Tasks` coordinates what that means with
-  respect to input—via `preprocess`—, modeling—via `adapt`— and optimization—via
-  `losses.`)
+  No constraints are made on the `predict` method; e.g.: it may append a head
+  with learnable weights or it may perform tensor computations only. (The entire
+  `Task` coordinates what that means with respect to dataset—via `preprocess`—,
+  modeling—via `predict`— and optimization—via `losses`.)
+
+  `Task`s are applied in the scope of a training invocation: they are subject to
+  the executing context of the `Trainer` and should, when needed, override it
+  (e.g., a global policy, like `tf.keras.mixed_precision.global_policy()` and
+  its implications over logit and activation layers).
   """
 
   @abc.abstractmethod
-  def adapt(self, model: tf.keras.Model) -> tf.keras.Model:
-    """Adapt a model to a task by appending arbitrary head(s)."""
+  def preprocess(
+      self,
+      inputs: GraphTensor) -> tuple[OneOrSequenceOf[GraphTensor], Field]:
+    """Preprocesses a scalar (after `merge_batch_to_components`) `GraphTensor`.
+
+    This function uses the Keras functional API to define non-trainable
+    transformations of the symbolic input `GraphTensor`, which get executed
+    during dataset preprocessing in a `tf.data.Dataset.map(...)` operation.
+    It has two responsibilities:
+
+     1. Splitting the training label out of the input for training. It must be
+        returned as a separate tensor.
+     2. Optionally, transforming input features. Some advanced modeling
+        techniques require running the same base GNN on multiple different
+        transformations, so this function may return a single `GraphTensor`
+        or a non-empty sequence of `GraphTensors`. The corresponding base GNN
+        output for each `GraphTensor` is provided to the `predict(...)` method.
+
+    Args:
+      inputs: A symbolic Keras `GraphTensor` for processing.
+
+    Returns:
+      A tuple of processed `GraphTensor`(s) and a `Field` to be used as labels.
+    """
     raise NotImplementedError()
 
   @abc.abstractmethod
-  def preprocess(
-      self,
-      gt: GraphTensor) -> Union[GraphTensor, GraphTensorAndField]:
-    """Preprocess a scalar (after `merge_batch_to_components`) `GraphTensor`."""
+  def predict(self, *args: GraphTensor) -> Field:
+    """Produces prediction outputs for the learning objective.
+
+    Overall model composition* makes use of the Keras Functional API
+    (https://www.tensorflow.org/guide/keras/functional) to map symbolic Keras
+    `GraphTensor` inputs to symbolic Keras `Field` outputs.
+
+    *) `outputs = predict(GNN(inputs))` where `inputs` are those `GraphTensor`
+       returned by `preprocess(...)`, `GNN` is the base GNN, `predict` is this
+       method and `outputs` are the prediction outputs for the learning
+       objective.
+
+    Args:
+      *args: The symbolic Keras `GraphTensor` inputs(s). These inputs correspond
+        (in sequence) to the base GNN output of each `GraphTensor` returned by
+        `preprocess(...)`.
+
+    Returns:
+      The model's prediction output for this task.
+    """
     raise NotImplementedError()
 
   @abc.abstractmethod
   def losses(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
-    """Arbitrary losses matching any head(s)."""
+    """Returns arbitrary task specific losses."""
     raise NotImplementedError()
 
   @abc.abstractmethod
   def metrics(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
-    """Arbitrary task specific metrics."""
+    """Returns arbitrary task specific metrics."""
     raise NotImplementedError()
 
 
 class Trainer(abc.ABC):
   """A class for training and validation."""
 
   @property
@@ -184,10 +237,10 @@
       epochs: The epochs to train.
       valid_ds_provider: A `DatasetProvider` for validation. The items of the
         `tf.data.Dataset` are pairs `(graph_tensor, label)` that represent one
         batch of per-replica training inputs after
         `GraphTensor.merge_batch_to_components()` has been applied.
 
     Returns:
-      A trained `tf.keras.Model.`
+      A trained `tf.keras.Model`.
     """
     raise NotImplementedError()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/orchestration_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/experimental/in_memory/networkx_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,186 +1,143 @@
-# Copyright 2021 The TensorFlow GNN Authors. All Rights Reserved.
+# Copyright 2023 The TensorFlow GNN Authors. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Tests for orchestration."""
-import os
-from typing import Any, Sequence, Union
+"""Wraps a homogeneous (simple) NetworkX graph for use with GraphTensor."""
 
-from absl.testing import parameterized
+import collections
+from typing import Dict, Mapping, MutableMapping, Optional, Tuple
+
+import numpy as np
+import scipy.sparse as sp
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
-from tensorflow_gnn.models import vanilla_mpnn
-from tensorflow_gnn.runner import orchestration
-from tensorflow_gnn.runner.tasks import classification
-from tensorflow_gnn.runner.trainers import keras_fit
-from tensorflow_gnn.runner.utils import model_templates
-
-_LABELS = tuple(range(32))
-
-_SCHEMA_A = """
-  context {
-    features {
-      key: "label"
-      value {
-        dtype: DT_INT32
-      }
-    }
-  }
-  node_sets {
-    key: "node"
-    value {
-      features {
-        key: "features"
-        value {
-          dtype: DT_FLOAT
-          shape { dim { size: 4 } }
-        }
-      }
-    }
-  }
-  edge_sets {
-    key: "edge"
-    value {
-      source: "node"
-      target: "node"
-    }
-  }
-"""
-
-_SCHEMA_B = """
-  context {
-    features {
-      key: "label"
-      value {
-        dtype: DT_INT32
-      }
-    }
-  }
-  node_sets {
-    key: "node"
-    value {
-      features {
-        key: "features"
-        value {
-          dtype: DT_FLOAT
-          shape { dim { size: 12 } }
-        }
-      }
-    }
-  }
-"""
+from tensorflow_gnn.experimental.in_memory import datasets
 
+Example = tf.train.Example
 
-def graph_spec(txt: str = _SCHEMA_A) -> tfgnn.GraphTensorSpec:
-  schema = tfgnn.parse_schema(txt)
-  return tfgnn.create_graph_spec_from_schema_pb(schema)
 
+class NetworkXDiGraphData(datasets.InMemoryGraphData):
+  """Implementation of in-memory dataset loader for networkx format.
 
-def random_graph_tensor(txt: str = _SCHEMA_A) -> tfgnn.GraphTensor:
-  sample_dict = {(tfgnn.CONTEXT, None, "label"): _LABELS}
-  return tfgnn.random_graph_tensor(graph_spec(txt), sample_dict=sample_dict)
+  This class only wraps a homogeneous (simple) NetworkX graph (networkx.Graph
+  or networkx.DiGraph) for use with GraphTensor.
 
+  The schema used for this graph has one node set ("nodes") and two edge sets
+  {"edges", "rev_edges"} containing the forward and reverse directed edges
+  respectively.
 
-def random_serialized_graph_tensor(txt: str = _SCHEMA_A) -> tfgnn.GraphTensor:
-  return tfgnn.write_example(random_graph_tensor(txt)).SerializeToString()
+  Note: This converter currently ignores node and edge features.
+  """
 
+  def __init__(
+      self,
+      nx_graph,
+      graph_schema: Optional[tfgnn.GraphSchema] = None,
+  ):
+    """Constructor to represent a NetworkX graph in memory.
+
+    Args:
+      nx_graph: A networkx DiGraph.
+      graph_schema: A tfgnn.GraphSchema protobuf message.
+    """
+    super().__init__()
+    self._graph_schema = graph_schema
+
+    # Make "compression map":
+    #   String Node ID ->  auto-incrementing int node id
+    self.graph = nx_graph
+    self.compression_map = {}
+    self.reverse_compression_map = {}
+    for idx, node_id in enumerate(sorted(nx_graph.nodes())):
+      self.compression_map[node_id] = idx
+      self.reverse_compression_map[idx] = node_id
+
+    # We'll also create a version of the graph with compressed ids.
+    src = []
+    dst = []
+    weight = []
+    for _, node_id in enumerate(sorted(nx_graph.nodes())):
+      for dst_id in nx_graph[node_id]:
+        src.append(self.compression_map[node_id])
+        dst.append(self.compression_map[dst_id])
+        if "weight" in nx_graph[node_id][dst_id]:
+          weight.append(nx_graph[node_id][dst_id]["weight"])
+        else:
+          weight.append(1.0)
+
+    self.flat_adjacency = sp.coo_array(
+        (weight, (src, dst)),
+        shape=(len(self.compression_map), len(self.compression_map)),
+        dtype="float",
+    )
+
+    # Add node feature support (this constructor would take a list of
+    # node features to copy from the networkx graph)
+    self.node_features = {}
+
+  def get_adjacency_list(self) -> Dict[tfgnn.EdgeSetName, Dict[str, Example]]:
+    """Returns weighted edges as an adjacency list of nested dictionaries.
+
+    This function is useful for testing for fast access to edge features based
+    on (source, target) IDs. Beware, this function will create an object that
+    may increase memory usage.
+    """
+    adjacency_sets = collections.defaultdict(dict)
+    adjacency_sets["edges"] = collections.defaultdict(dict)
+    for source, target, weight in zip(
+        self.flat_adjacency.row,
+        self.flat_adjacency.col,
+        self.flat_adjacency.data,
+    ):
+      e = tf.train.Example(
+          features=tf.train.Features(
+              feature={
+                  "weight": tf.train.Feature(
+                      float_list=tf.train.FloatList(value=[weight])
+                  )
+              }
+          )
+      )
+      adjacency_sets["edges"][source][target] = e
 
-class DatasetProvider(orchestration.DatasetProvider):
+    return adjacency_sets
 
-  def __init__(
+  def node_features_dicts(
       self,
-      element: Union[tfgnn.GraphTensor, bytes, Any],
-      cardinality: int = 8):
-    self._ds = tf.data.Dataset.from_tensors(element).repeat(cardinality)
-
-  def get_dataset(self, _: tf.distribute.InputContext) -> tf.data.Dataset:
-    return self._ds
-
-
-class OrchestrationTests(tf.test.TestCase, parameterized.TestCase):
-
-  @parameterized.named_parameters([
-      dict(
-          testcase_name="GraphTensors",
-          gtspec=graph_spec(),
-          ds_provider=DatasetProvider(random_graph_tensor()),
-          examples=tf.constant((random_serialized_graph_tensor(),) * 2),
-      ),
-      dict(
-          testcase_name="SerializedGraphTensors",
-          gtspec=graph_spec(),
-          ds_provider=DatasetProvider(random_serialized_graph_tensor()),
-          examples=tf.constant((random_serialized_graph_tensor(),) * 2),
-      ),
-  ])
-  def test_run(
+  ) -> Mapping[tfgnn.NodeSetName, MutableMapping[tfgnn.FieldName, tf.Tensor]]:
+    ret = {}
+    ret["nodes"] = self.node_features
+    return ret
+
+  def node_counts(self) -> Mapping[tfgnn.NodeSetName, int]:
+    """Returns total number of graph nodes per node set."""
+    return {"nodes": len(self.compression_map)}
+
+  def edge_lists(
       self,
-      gtspec: tfgnn.GraphTensorSpec,
-      ds_provider: orchestration.DatasetProvider,
-      examples: Sequence[str]):
-    def extract_labels(gt):
-      return gt, gt.context["label"]
-
-    def node_sets_fn(node_set, node_set_name):
-      del node_set_name
-      return node_set["features"]
-
-    model_fn = model_templates.ModelFromInitAndUpdates(
-        init=tfgnn.keras.layers.MapFeatures(node_sets_fn=node_sets_fn),
-        updates=[vanilla_mpnn.VanillaMPNNGraphUpdate(
-            units=1,
-            message_dim=2,
-            receiver_tag=tfgnn.SOURCE,
-            l2_regularization=5e-4,
-            dropout_rate=0.1)])
-
-    task = classification.RootNodeMulticlassClassification(
-        node_set_name="node",
-        num_classes=len(_LABELS))
-
-    model_dir = self.create_tempdir()
-
-    trainer = keras_fit.KerasTrainer(
-        strategy=tf.distribute.get_strategy(),
-        model_dir=model_dir,
-        steps_per_epoch=1,
-        validation_steps=1,
-        restore_best_weights=False)
-
-    orchestration.run(
-        train_ds_provider=ds_provider,
-        model_fn=model_fn,
-        optimizer_fn=tf.keras.optimizers.Adam,
-        epochs=1,
-        trainer=trainer,
-        task=task,
-        gtspec=gtspec,
-        drop_remainder=False,
-        global_batch_size=4,
-        feature_processors=(extract_labels,),
-        valid_ds_provider=ds_provider)
-
-    saved_model = tf.saved_model.load(os.path.join(model_dir, "export"))
-    output = saved_model.signatures["serving_default"](examples=examples)
-    actual = next(iter(output.values()))
-
-    # The model has one output
-    self.assertLen(output, 1)
-
-    # The expected shape is (batch size, num classes) or
-    # (len(examples), len(_LABELS))
-    self.assertAllEqual(actual.shape, (examples.shape[0], len(_LABELS)))
+  ) -> Mapping[
+      Tuple[tfgnn.NodeSetName, tfgnn.EdgeSetName, tfgnn.NodeSetName], tf.Tensor
+  ]:
+    """Returns dict from "edge type tuple" to int array of shape (2, num_edges).
+
+    "edge type tuple" string-tuple: (src_node_set, edge_set, target_node_set).
+    """
+    return {
+        ("nodes", "edges", "nodes"): np.vstack(
+            [self.flat_adjacency.row, self.flat_adjacency.col],
+        )
+    }
 
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/BUILD`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,124 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "py_strict_test")
 
 licenses(["notice"])
 
+package(
+    default_applicable_licenses = ["//tensorflow_gnn:license"],
+    default_visibility = ["//visibility:public"],
+)
+
 pytype_strict_library(
-    name = "classification",
-    srcs = ["classification.py"],
+    name = "attribution",
+    srcs = ["attribution.py"],
     srcs_version = "PY3",
     visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
+        "//:expect_numpy_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
         "//tensorflow_gnn/runner:interfaces",
     ],
 )
 
-py_strict_test(
-    name = "classification_test",
-    srcs = ["classification_test.py"],
+pytype_strict_library(
+    name = "label_fns",
+    srcs = ["label_fns.py"],
     srcs_version = "PY3",
-    tags = ["tf_at_least_2_10"],
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
-        ":classification",
-        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
     ],
 )
 
 pytype_strict_library(
-    name = "regression",
-    srcs = ["regression.py"],
+    name = "model_dir",
+    srcs = ["model_dir.py"],
     srcs_version = "PY3",
     visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
         "//:expect_tensorflow_installed",
+    ],
+)
+
+pytype_strict_library(
+    name = "model_export",
+    srcs = ["model_export.py"],
+    srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    deps = [
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn/runner:interfaces",
+    ],
+)
+
+pytype_strict_library(
+    name = "padding",
+    srcs = ["padding.py"],
+    srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    deps = [
+        ":parsing",
+        "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
         "//tensorflow_gnn/runner:interfaces",
     ],
 )
 
+pytype_strict_library(
+    name = "parsing",
+    srcs = ["parsing.py"],
+    srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    deps = [
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+    ],
+)
+
+pytype_strict_library(
+    name = "strategies",
+    srcs = ["strategies.py"],
+    srcs_version = "PY3",
+    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    deps = [
+        "//:expect_tensorflow_installed",
+    ],
+)
+
+py_strict_test(
+    name = "attribution_test",
+    srcs = ["attribution_test.py"],
+    srcs_version = "PY3",
+    deps = [
+        ":attribution",
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+        "//tensorflow_gnn/runner:interfaces",
+    ],
+)
+
+py_strict_test(
+    name = "model_export_test",
+    srcs = ["model_export_test.py"],
+    python_version = "PY3",
+    deps = [
+        ":model_export",
+        "//:expect_absl_installed",
+        "//:expect_tensorflow_installed",
+        "//tensorflow_gnn/runner:interfaces",
+    ],
+)
+
 py_strict_test(
-    name = "regression_test",
-    srcs = ["regression_test.py"],
+    name = "parsing_test",
+    srcs = ["parsing_test.py"],
     srcs_version = "PY3",
-    tags = ["tf_at_least_2_10"],
     deps = [
-        ":regression",
+        ":parsing",
         "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/tasks/classification.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/tasks/classification.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,28 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Classification tasks."""
+from __future__ import annotations
+
 import abc
-from typing import Any, Callable, Mapping, Optional, Sequence, Union
+from typing import Any, Callable, Mapping, Optional, Sequence, Tuple
 
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.runner import interfaces
 
-Tensor = Union[tf.Tensor, tf.RaggedTensor]
+Field = tfgnn.Field
+GraphTensor = tfgnn.GraphTensor
+# TODO(b/274672364): make this tuple[...] in Python 3.9 style
+# when we drop py38 support.
+LabelFn = Callable[[GraphTensor], Tuple[GraphTensor, Field]]
 
 
 class _FromLogitsMixIn(tf.keras.metrics.Metric):
   """Mixin for `tf.keras.metrics.Metric` with a from_logits option."""
 
   def __init__(self, from_logits: bool, *args, **kwargs) -> None:
     super().__init__(*args, **kwargs)
@@ -90,60 +96,88 @@
 class _Classification(interfaces.Task):
   """Abstract classification class.
 
   Any subclass must implement all of `gather_activations`, `losses` and
   `metrics`, usually by inheriting from the classes below.
   """
 
-  def __init__(self, units: int):
+  def __init__(
+      self,
+      units: int,
+      *,
+      name: str = "classification_logits",
+      label_fn: Optional[LabelFn] = None,
+      label_feature_name: Optional[str] = None):
+    """Sets `Task` parameters.
+
+    Args:
+      units: The units for the classification head. (Typically `1` for binary
+        classification and `num_classes` for multiclass classification.)
+      name: The classification head's layer name. This name typically appears
+        in the exported model's SignatureDef.
+      label_fn: A label extraction function. This function mutates the input
+        `GraphTensor`. Mutually exclusive with `label_feature_name`.
+      label_feature_name: A label feature name for readout from the auxiliary
+        '_readout' node set. Readout does not mutate the input `GraphTensor`.
+        Mutually exclusive with `label_fn`.
+    """
+    if (label_fn is None) == (label_feature_name is None):
+      raise ValueError(
+          "Exactly one of `label_fn` or `label_feature_name` may be specified"
+          f" (got label_fn={label_fn} and"
+          f" label_feature_name={label_feature_name})"
+      )
     self._units = units
+    self._name = name
+    self._label_fn = label_fn
+    self._label_feature_name = label_feature_name
 
   @abc.abstractmethod
-  def gather_activations(self, gt: tfgnn.GraphTensor) ->  Tensor:
+  def gather_activations(self, inputs: GraphTensor) -> Field:
     raise NotImplementedError()
 
-  def adapt(self, model: tf.keras.Model) -> tf.keras.Model:
-    """Append a linear head with `units` output units.
-
-    Multiple `tf.keras.Model` outputs are not supported.
+  def predict(self, inputs: tfgnn.GraphTensor) -> Field:
+    """Apply a linear head for classification.
 
     Args:
-      model: A `tf.keras.Model` to adapt.
+      inputs: A `tfgnn.GraphTensor` for classification.
 
     Returns:
-      An adapted `tf.keras.Model.`
+      The classification logits.
     """
-    tfgnn.check_scalar_graph_tensor(model.output, name="Classification")
-    activations = self.gather_activations(model.output)
+    tfgnn.check_scalar_graph_tensor(inputs, name="Classification")
+    activations = self.gather_activations(inputs)
     logits = tf.keras.layers.Dense(
         self._units,
-        name="logits")(activations)  # Name seen in SignatureDef.
-    return tf.keras.Model(model.input, logits)
+        name=self._name)(activations)  # Name seen in SignatureDef.
+    return logits
 
-  @abc.abstractmethod
-  def preprocess(self, gt: tfgnn.GraphTensor) -> tfgnn.GraphTensor:
-    raise NotImplementedError()
+  def preprocess(self, inputs: GraphTensor) -> tuple[GraphTensor, Field]:
+    if self._label_fn is not None:
+      return self._label_fn(inputs)
+    x = inputs
+    y = tfgnn.keras.layers.Readout(
+        feature_name=self._label_feature_name,
+        node_set_name="_readout")(inputs)
+    return x, y
 
   @abc.abstractmethod
   def losses(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
     raise NotImplementedError()
 
   @abc.abstractmethod
   def metrics(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
     raise NotImplementedError()
 
 
 class _BinaryClassification(_Classification):
   """Binary classification."""
 
-  def __init__(self, *args, units: int = 1, **kwargs):
-    super().__init__(units, *args, **kwargs)
-
-  def preprocess(self, gt: tfgnn.GraphTensor) -> tfgnn.GraphTensor:
-    return gt
+  def __init__(self, units: int = 1, **kwargs):
+    super().__init__(units, **kwargs)
 
   def losses(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
     return (tf.keras.losses.BinaryCrossentropy(from_logits=True),)
 
   def metrics(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
     return (FromLogitsPrecision(from_logits=True),
             FromLogitsRecall(from_logits=True),
@@ -153,34 +187,31 @@
             tf.keras.losses.BinaryCrossentropy(from_logits=True))
 
 
 class _MulticlassClassification(_Classification):
   """Multiclass classification."""
 
   def __init__(self,
-               *args,
+               *,
                num_classes: Optional[int] = None,
                class_names: Optional[Sequence[str]] = None,
                per_class_statistics: bool = False,
-               **kwargs):  # pylint: disable=useless-super-delegation
+               **kwargs):
     if (num_classes is None) == (class_names is None):
       raise ValueError(
           "Exactly one of `num_classes` or `class_names` must be specified")
     if num_classes is None:
       num_classes = len(class_names)
-    super().__init__(num_classes, *args, **kwargs)
+    super().__init__(num_classes, **kwargs)
     if class_names is None:
       self._class_names = [f"class_{i}" for i in range(num_classes)]
     else:
       self._class_names = class_names
     self._per_class_statistics = per_class_statistics
 
-  def preprocess(self, gt: tfgnn.GraphTensor) -> tfgnn.GraphTensor:
-    return gt
-
   def losses(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
     """Sparse categorical crossentropy loss."""
     return (tf.keras.losses.SparseCategoricalCrossentropy(from_logits=True),)
 
   def metrics(self) -> Sequence[Callable[[tf.Tensor, tf.Tensor], tf.Tensor]]:
     """Sparse categorical metrics."""
     metric_objs = [
@@ -200,84 +231,83 @@
     return metric_objs
 
 
 class _GraphClassification(_Classification):
   """Classification by the label provided in the graph context."""
 
   def __init__(self,
-               *args,
                node_set_name: str,
+               *,
                state_name: str = tfgnn.HIDDEN_STATE,
                reduce_type: str = "mean",
                **kwargs):
     """Classification by the label provided in the graph context.
 
     This task defines classification of a graph by a label found in its unique
     context. The representations are mean-pooled from a single set of nodes.
 
     Labels are expected to be sparse, i.e.: scalars.
 
     Args:
-      *args: Additional positional arguments.
       node_set_name: Node set to pool representations from.
       state_name: The feature name for node activations
         (typically: tfgnn.HIDDEN_STATE).
       reduce_type: The context pooling reduction type.
       **kwargs: Additional keyword arguments.
     """
-    super().__init__(*args, **kwargs)
+    super().__init__(**kwargs)
     self._node_set_name = node_set_name
     self._state_name = state_name
     self._reduce_type = reduce_type
 
-  def gather_activations(self, gt: tfgnn.GraphTensor) ->  Tensor:
+  def gather_activations(self, inputs: GraphTensor) -> Field:
     return tfgnn.keras.layers.Pool(
         tfgnn.CONTEXT,
         self._reduce_type,
         node_set_name=self._node_set_name,
-        feature_name=self._state_name)(gt)
+        feature_name=self._state_name)(inputs)
 
 
 class _RootNodeClassification(_Classification):
   """Classification by root node label."""
 
   def __init__(self,
-               *args,
                node_set_name: str,
+               *,
                state_name: str = tfgnn.HIDDEN_STATE,
                **kwargs):
     """Classification by root node label.
 
     This task defines classification of a rooted graph by a label found
     on its unique root node. By convention, root nodes are stored as the
     first node of each graph component in the respective node set.
     Typically, such graphs are created by go/graph-sampler by sampling the
     neighborhoods of root nodes (or "seed nodes") in large graphs to
     aggregate information relevant to the root node's classification.
 
     Any labels are expected to be sparse, i.e.: scalars.
 
     Args:
-      *args: Additional positional arguments.
       node_set_name: The node set containing the root node.
       state_name: The feature name for activations
         (typically: tfgnn.HIDDEN_STATE).
       **kwargs: Additional keyword arguments.
     """
-    super().__init__(*args, **kwargs)
+    super().__init__(**kwargs)
     self._node_set_name = node_set_name
     self._state_name = state_name
 
-  def gather_activations(self, gt: tfgnn.GraphTensor) ->  Tensor:
+  def gather_activations(self, inputs: GraphTensor) -> Field:
     """Gather activations from root nodes."""
     return tfgnn.keras.layers.ReadoutFirstNode(
         node_set_name=self._node_set_name,
-        feature_name=self._state_name)(gt)
+        feature_name=self._state_name)(inputs)
 
 
+# TODO(dzelle): Add an `__init__` with parameters and doc for all of the below.
 class GraphBinaryClassification(_GraphClassification, _BinaryClassification):
   pass
 
 
 class GraphMulticlassClassification(_GraphClassification,
                                     _MulticlassClassification):
   pass
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/trainers/keras_fit.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/trainers/keras_fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,38 +61,49 @@
       self,
       strategy: tf.distribute.Strategy,
       *,
       model_dir: str,
       checkpoint_options: Optional[KerasTrainerCheckpointOptions] = None,
       backup_dir: Optional[str] = None,
       steps_per_epoch: Optional[int] = None,
+      verbose: Union[int, str] = "auto",
       validation_steps: Optional[int] = None,
       validation_per_epoch: Optional[int] = None,
+      validation_freq: Optional[int] = None,
       summarize_every_n_steps: Union[int, str] = 500,
       checkpoint_every_n_steps: Union[int, str] = "epoch",
       backup_and_restore: bool = True,
       callbacks: Optional[Sequence[tf.keras.callbacks.Callback]] = None,
-      restore_best_weights: bool = True,
+      restore_best_weights: Optional[bool] = None,
       options: Optional[KerasTrainerOptions] = None):
     """Sets training parameters.
 
     Args:
       strategy: A `tf.distribute.Strategy.`
       model_dir: A model directory for summaries.
       checkpoint_options: An optional configuration for checkpointing related
         configs. If checkpoint_options.checkpoint_dir is unset;
         `os.path.join(model_dir, "ckpnt")` is used.
       backup_dir: An optional directory for backup, if unset;
         `(os.path.join(model_dir, "backup"),)` is used.
-      steps_per_epoch: An optional steps per epoch, if unspecified: epochs are
-        at `tf.data.Dataset` end.
-      validation_steps: An optional numer of validation steps, if unspecified:
-        the entire validation `tf.data.Dataset` is evaluated.
-      validation_per_epoch: An optional validations per epoch, if unspecified:
-        one evaluation per training epoch is performed.
+      steps_per_epoch: The number of training steps per epoch. Optional,
+        if unspecified: epochs are at `tf.data.Dataset` end.
+      verbose: Forwarded to `tf.keras.Model.fit()`. Possible values are
+        0 (silent), 1 (print progress bar), 2 (one line per epoch), and
+        "auto" (default) defers to keras to select verbosity.
+      validation_steps: The number of steps used during validation. Optional,
+        if unspecified: the entire validation `tf.data.Dataset` is evaluated.
+      validation_per_epoch: The number of validations done per training epoch.
+        Optional, if unspecified: Perform one validation per training epoch.
+        Only one of `validation_per_epoch` and `validation_freq` can be
+        specified.
+      validation_freq: Specifies how many training epochs to run before a new
+        validation run is performed. Optional, if unspecified: Performs
+        validation after every training epoch. Only one of
+        `validation_per_epoch` and `validation_freq` can be specified.
       summarize_every_n_steps: The frequency for writing TensorBoard summaries,
         as an integer number of steps, or "epoch" for once per epoch, or
         "never".
       checkpoint_every_n_steps: The frequency for writing latest models, as an
         integer number of steps, or "epoch" for once per epoch, or "never".
         The best model will always be saved after each validation epoch except
         when this parameter is set to "never", because the validation metric is
@@ -100,15 +111,17 @@
       backup_and_restore: Whether to backup and restore (According to
         `tf.keras.callbacks.BackupAndRestore`). The backup
         directory is determined by `backup_dir`.
       callbacks: Optional additional `tf.keras.callbacks.Callback` for
         `tf.keras.Model.fit.`
       restore_best_weights: Requires a `checkpoint_every_n_steps` other than
         "never." Whether to restore the best model weights as determined by
-        `tf.keras.callbacks.ModelCheckpoint` after training.
+        `tf.keras.callbacks.ModelCheckpoint` after training. If unspecified,
+        its value is determined at `train(...)` invocation: `True if
+        valid_ds_provider is not None else False`.
       options: A `KerasTrainerOptions.`
     """
     if restore_best_weights and checkpoint_every_n_steps == "never":
       raise ValueError("`restore_best_weights` requires a "
                        "`checkpoint_every_n_steps` other than \"never\"")
 
     if checkpoint_options is None:
@@ -116,21 +129,28 @@
 
     if checkpoint_options.checkpoint_dir is None:
       checkpoint_options.checkpoint_dir = os.path.join(model_dir, "ckpnt")
 
     if backup_dir is None:
       backup_dir = os.path.join(model_dir, "backup")
 
+    if (validation_freq is not None and validation_per_epoch is not None):
+      raise ValueError(
+          "`validation_freq` and `validation_per_epoch` are mutually exclusive."
+      )
+
     self._strategy = strategy
     self._model_dir = model_dir
     self._checkpoint_options = checkpoint_options
     self._backup_dir = backup_dir
     self._steps_per_epoch = steps_per_epoch
+    self._verbose = verbose
     self._validation_steps = validation_steps
     self._validation_per_epoch = validation_per_epoch
+    self._validation_freq = validation_freq
     self._summarize_every_n_steps = summarize_every_n_steps
     self._checkpoint_every_n_steps = checkpoint_every_n_steps
     self._backup_and_restore = backup_and_restore
     self._callbacks = callbacks
     self._restore_best_weights = restore_best_weights
     self._options = options
 
@@ -194,16 +214,27 @@
       checkpoint_every_n_steps = self._checkpoint_every_n_steps
       steps_per_epoch = self._steps_per_epoch
       validation_steps = self._validation_steps
 
     if validation_steps is not None and valid_ds_provider is None:
       raise ValueError("`validation_steps` requires a `valid_ds_fn`")
 
-    if self._restore_best_weights and valid_ds_provider is None:
+    if self._validation_freq is not None and valid_ds_provider is None:
+      raise ValueError("`validation_freq` requires a `valid_ds_fn`")
+
+    validation_freq = (
+        self._validation_freq if self._validation_freq is not None else 1
+    )
+
+    # Adjust `restore_best_weights` given `valid_ds_provider`:
+    restore_best_weights = self._restore_best_weights
+    if restore_best_weights and valid_ds_provider is None:
       raise ValueError("`restore_best_weights` requires a validation dataset")
+    elif restore_best_weights is None:
+      restore_best_weights = valid_ds_provider is not None
 
     if self._options and self._options.soft_device_placement:
       tf.config.set_soft_device_placement(True)
 
     if self._options and self._options.enable_check_numerics:
       tf.debugging.enable_check_numerics()
 
@@ -279,13 +310,15 @@
 
     model.fit(
         train_ds,
         epochs=epochs,
         steps_per_epoch=steps_per_epoch,
         validation_data=valid_ds,
         validation_steps=validation_steps,
+        validation_freq=validation_freq,
+        verbose=self._verbose,
         callbacks=callbacks)
 
-    if self._restore_best_weights:
+    if restore_best_weights:
       model.load_weights(self._checkpoint_options.best_checkpoint_filepath())
 
     return model
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/models/contrastive_losses/BUILD`

 * *Files 12% similar despite different names*

```diff
@@ -1,141 +1,135 @@
 load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "pytype_strict_library")
-load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "py_strict_test")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "tf_py_test")
+load("@tensorflow_gnn//tensorflow_gnn:tensorflow_gnn.bzl", "distribute_py_test")
 
 licenses(["notice"])
 
-pytype_strict_library(
-    name = "attribution",
-    srcs = ["attribution.py"],
-    srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
-    deps = [
-        ":model",
-        "//:expect_numpy_installed",
-        "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
-        "//tensorflow_gnn/runner:interfaces",
-    ],
-)
+package_group(name = "users")
 
 pytype_strict_library(
-    name = "model",
-    srcs = ["model.py"],
+    name = "contrastive_losses",
+    srcs = ["__init__.py"],
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    visibility = [
+        ":users",
+    ],
     deps = [
-        "//:expect_tensorflow_installed",
+        ":layers",
+        ":tasks",
     ],
 )
 
 pytype_strict_library(
-    name = "model_dir",
-    srcs = ["model_dir.py"],
+    name = "layers",
+    srcs = ["layers.py"],
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
+    visibility = [
+        ":__subpackages__",
+    ],
     deps = [
         "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
     ],
 )
 
-pytype_strict_library(
-    name = "model_export",
-    srcs = ["model_export.py"],
+tf_py_test(
+    name = "layers_test",
+    srcs = ["layers_test.py"],
+    python_version = "PY3",
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
-        ":model",
+        ":layers",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn/runner:interfaces",
+        "//tensorflow_gnn",
     ],
 )
 
 pytype_strict_library(
-    name = "model_templates",
-    srcs = ["model_templates.py"],
+    name = "losses",
+    srcs = ["losses.py"],
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
     ],
 )
 
-pytype_strict_library(
-    name = "padding",
-    srcs = ["padding.py"],
+tf_py_test(
+    name = "losses_test",
+    srcs = ["losses_test.py"],
+    python_version = "PY3",
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
-        ":parsing",
+        ":tasks",
+        "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
-        "//tensorflow_gnn/runner:interfaces",
     ],
 )
 
 pytype_strict_library(
-    name = "parsing",
-    srcs = ["parsing.py"],
+    name = "metrics",
+    srcs = ["metrics.py"],
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
         "//:expect_tensorflow_installed",
-        "//tensorflow_gnn",
     ],
 )
 
-pytype_strict_library(
-    name = "strategies",
-    srcs = ["strategies.py"],
+tf_py_test(
+    name = "metrics_test",
+    srcs = ["metrics_test.py"],
+    python_version = "PY3",
     srcs_version = "PY3",
-    visibility = ["//tensorflow_gnn/runner:__pkg__"],
     deps = [
+        ":metrics",
         "//:expect_tensorflow_installed",
     ],
 )
 
-py_strict_test(
-    name = "attribution_test",
-    srcs = ["attribution_test.py"],
+pytype_strict_library(
+    name = "tasks",
+    srcs = ["tasks.py"],
     srcs_version = "PY3",
-    tags = ["tf_at_least_2_10"],
     deps = [
-        ":attribution",
+        ":layers",
+        ":losses",
+        ":metrics",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
+        "//tensorflow_gnn/runner",
     ],
 )
 
-py_strict_test(
-    name = "model_test",
-    srcs = ["model_test.py"],
+tf_py_test(
+    name = "tasks_test",
+    srcs = ["tasks_test.py"],
     python_version = "PY3",
+    srcs_version = "PY3",
     deps = [
-        ":model",
+        ":tasks",
         "//:expect_absl_installed",
         "//:expect_tensorflow_installed",
+        "//tensorflow_gnn",
+        "//tensorflow_gnn/models/vanilla_mpnn",
     ],
 )
 
-py_strict_test(
-    name = "model_export_test",
-    srcs = ["model_export_test.py"],
-    python_version = "PY3",
-    deps = [
-        ":model_export",
-        "//:expect_absl_installed",
-        "//:expect_tensorflow_installed",
+distribute_py_test(
+    name = "distribute_test",
+    size = "large",
+    srcs = ["distribute_test.py"],
+    shard_count = 8,
+    tags = [
+        "no_oss",  # TODO(b/238827505)
+        "nomultivm",  # TODO(b/170502145)
     ],
-)
-
-py_strict_test(
-    name = "parsing_test",
-    srcs = ["parsing_test.py"],
-    srcs_version = "PY3",
+    xla_enable_strict_auto_jit = False,
     deps = [
-        ":parsing",
-        "//:expect_absl_installed",
+        ":tasks",
         "//:expect_tensorflow_installed",
         "//tensorflow_gnn",
+        "//tensorflow_gnn/models/vanilla_mpnn",
+        "//tensorflow_gnn/runner",
     ],
 )
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import os
 from typing import Callable, Optional, Sequence, Union
 
 import numpy as np
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.runner import interfaces
-from tensorflow_gnn.runner.utils import model as model_utils
 
 
 def reduce_graph_sequence(
     graphs: Sequence[tfgnn.GraphTensor],
     initializer: Optional[tfgnn.GraphTensor] = None,
     *,
     context_fn: Callable[[Sequence[tfgnn.Field]], tfgnn.Field],
@@ -107,20 +106,25 @@
     random: Whether to produce a random uniform counterfactual.
     seed: An optional random seed.
 
   Returns:
     A counterfactual `tfgnn.GraphTensor.`
   """
   if random:
-    fn = lambda inputs: tf.random.uniform(  # pylint: disable=g-long-lambda
-        tf.shape(*inputs),
-        minval=tf.math.reduce_min(*inputs),
-        maxval=tf.math.reduce_max(*inputs),
-        dtype=inputs[0].dtype,
-        seed=seed)
+    def fn(inputs):
+      dtype = inputs[0].dtype
+      minval = tf.math.reduce_min(*inputs)
+      maxval = tf.math.reduce_max(*inputs)
+      # The `maxval` boundary is exclusive for `tf.random.uniform`:
+      # For integers, add one to obtain a closed range.
+      # For floats, the half-open range is ok. (The special case
+      # minval = maxval is accepted by TF and uses that single value.)
+      if dtype.is_integer:
+        maxval = maxval + 1
+      return tf.random.uniform(tf.shape(*inputs), minval, maxval, dtype, seed)
   else:
     fn = lambda inputs: tf.zeros_like(*inputs)
   return reduce_graph_sequence(
       (graph,),
       context_fn=fn,
       edge_set_fn=fn,
       node_set_fn=fn)
@@ -234,29 +238,33 @@
   """Integrated gradients.
 
   This `tf.function` computes integrated gradients over a `tfgnn.GraphTensor.`
   The `tf.function` will be persisted in the ultimate saved model for
   subsequent attribution.
 
   Args:
-    preprocess_model: A `tf.keras.Model` for preprocessing.
+    preprocess_model: A `tf.keras.Model` for preprocessing. This model is
+      expected to return a tuple (`GraphTensor`, `Tensor`) where the
+      `GraphTensor` is used to invoke the below `model` and the tensor is used
+      used for any loss computation. (Via `model.compiled_loss`.)
     model: A `tf.keras.Model` for integrated gradients.
     output_name: The output `Tensor` name. If unset, the tensor will be named
       by Keras defaults.
     random_counterfactual: Whether to use a random uniform counterfactual.
     steps: The number of interpolations of the Riemann sum approximation.
     seed: An option random seed.
 
   Returns:
-    A `tfgnn.GraphTensor` with the integrated gradients.
+    A `tf.function` with the integrated gradients as output.
   """
   @tf.function(input_signature=_input_signature(preprocess_model))
   def fn(inputs):
     try:
       graph, labels = preprocess_model(inputs)
+      if isinstance(graph, Sequence): graph, *_ = graph
     except ValueError as error:
       msg = "Integrated gradients requires both examples and labels"
       raise ValueError(msg) from error
     else:
       tfgnn.check_scalar_graph_tensor(graph, name="integrated_gradients")
 
     baseline = counterfactual(graph, random=random_counterfactual, seed=seed)
@@ -268,26 +276,26 @@
         tape.watch(interpolation)
         logits = model(interpolation)
         loss = model.compiled_loss(
             labels,
             logits,
             regularization_losses=model.losses)
 
-      def fn(inputs):
+      def gradient_fn(inputs):
         return tape.gradient(  # pylint: disable=cell-var-from-loop
             loss,  # pylint: disable=cell-var-from-loop
             *inputs,
             unconnected_gradients=tf.UnconnectedGradients.ZERO)
 
       gradients += [
           reduce_graph_sequence(
               (interpolation,),
-              context_fn=fn,
-              edge_set_fn=fn,
-              node_set_fn=fn)
+              context_fn=gradient_fn,
+              edge_set_fn=gradient_fn,
+              node_set_fn=gradient_fn)
       ]
 
     gradients = sum_graph_features(gradients)
     return {output_name: gradients} if output_name is not None else gradients
 
   return fn
 
@@ -301,14 +309,26 @@
                subdirectory: Optional[str] = None,
                random_counterfactual: bool = True,
                steps: int = 32,
                seed: Optional[int] = None,
                options: Optional[tf.saved_model.SaveOptions] = None):
     """Captures the args shared across `save(...)` calls.
 
+    Random counterfactuals (see `random_counterfactual` below) sample from, per
+    graph piece and feature, a uniform distribution bounded by the minimum
+    (inclusive) and maximum (exclusive) of that graph piece instance's features.
+    For integer features, the maximum is adjust to maximum += 1. Uses of
+    integrated gradients on inputs* with many uniform (e.g.: a default value)
+    or near uniform (e.g.: a categorical value with few states) features should
+    consider i) not use a random counterfactual or ii) omitting transformations
+    like one-hot encoding in any preprocessing.
+
+    *) Where inputs are: the inputs of the `trained_model` (which correspond to
+       the outputs of the `preprocess_model`).
+
     Args:
       integrated_gradients_output_name: The name for the integrated gradients
         output tensor. If unset, the tensor will be named by Keras defaults.
       subdirectory: An optional subdirectory, if set: models are exported to
         `os.path.join(export_dir, subdirectory).`
       random_counterfactual: Whether to use a random uniform counterfactual.
       steps: The number of interpolations of the Riemann sum approximation.
@@ -318,41 +338,47 @@
     self._integrated_gradients_output_name = integrated_gradients_output_name
     self._subdirectory = subdirectory
     self._random_counterfactual = random_counterfactual
     self._steps = steps
     self._seed = seed
     self._options = options
 
-  def save(self,
-           preprocess_model: Optional[tf.keras.Model],
-           model: tf.keras.Model,
-           export_dir: str):
+  def save(self, run_result: interfaces.RunResult, export_dir: str):
     """Exports a Keras model with an additional integrated gradients signature.
 
-    Importantly: the `preprocess_model` is required and is concatenated with
-    `model` before any export. Concatenation involves the chaining of the
-    first output of `preprocess_model` to the only input of `model.` The result
-    is a model with the input of `preprocess_model` and the output of `model.`
+    Importantly: the `run_result.preprocess_model`, if provided, and
+    `run_result.trained_model` are stacked before any export. Stacking involves
+    the chaining of the first output of `run_result.preprocess_model` to the
+    only input of `run_result.trained_model.` The result is a model with the
+    input of `run_result.preprocess_model` and the output of
+    `run_result.trained_model.`
 
     Two serving signatures are exported:
 
     'serving_default') The default serving signature (i.e., the
       `preprocess_model` input signature),
     'integrated_gradients') The integrated gradients signature (i.e., the
       `preprocess_model` input signature).
 
     Args:
-      preprocess_model: A `tf.keras.Model` for preprocessing.
-      model: A `tf.keras.Model` to save.
-      export_dir: A destination directory for the model.
+      run_result: A `RunResult` from training.
+      export_dir: A destination directory.
     """
+    preprocess_model = run_result.preprocess_model
+    model = run_result.trained_model
+
     if preprocess_model is None:
       raise ValueError("Integrated gradients requires a `preprocess_model.`")
+    elif not preprocess_model.built:
+      raise ValueError("`preprocess_model` is expected to have been built")
+    elif not model.built:
+      raise ValueError("`model` is expected to have been built")
 
-    model_for_export = model_utils.chain_first_output(preprocess_model, model)
+    xs, *_ = preprocess_model.output
+    model_for_export = tf.keras.Model(preprocess_model.input, model(xs))
 
     ig = integrated_gradients(
         preprocess_model,
         model,
         output_name=self._integrated_gradients_output_name,
         random_counterfactual=self._random_counterfactual,
         steps=self._steps,
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/attribution_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/attribution_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,188 +12,201 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for attribution."""
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 
+from tensorflow_gnn.runner import interfaces
 from tensorflow_gnn.runner.utils import attribution
 
 IntegratedGradientsExporter = attribution.IntegratedGradientsExporter
 
-as_tensor = lambda sequence: tf.constant(sequence, dtype=tf.float32)
-
 
 class AttributionTest(tf.test.TestCase):
 
   gt = tfgnn.GraphTensor.from_pieces(
       context=tfgnn.Context.from_fields(features={
-          "h": as_tensor((.514, .433)),
+          "h": tf.convert_to_tensor((.514, .433)),
+          # An integer feature with uniform values.
+          "labels": tf.convert_to_tensor((0,)),
       }),
       node_sets={
           "node":
               tfgnn.NodeSet.from_fields(
                   features={
-                      "h": as_tensor((.8191, .9474, .1634)),
+                      "h": tf.convert_to_tensor((.8191, .9474, .1634)),
                   },
-                  sizes=tf.constant((3,), dtype=tf.int32),
+                  sizes=tf.constant((3,)),
               ),
       },
       edge_sets={
           "edge":
               tfgnn.EdgeSet.from_fields(
-                  features={"weight": as_tensor((.153, .9))},
-                  sizes=tf.constant((2,), dtype=tf.int32),
+                  features={"weight": tf.convert_to_tensor((.153, .9))},
+                  sizes=tf.constant((2,)),
                   adjacency=tfgnn.Adjacency.from_indices(
                       source=("node", (0, 1)), target=("node", (1, 2))),
               ),
       },
   )
 
   def test_counterfactual_random(self):
     counterfactual = attribution.counterfactual(self.gt, random=True, seed=8191)
 
     self.assertAllEqual(
         counterfactual.context.features["h"],
-        as_tensor((0.49280962, 0.466383)))
+        tf.convert_to_tensor((0.49280962, 0.466383)))
+    self.assertAllEqual(
+        counterfactual.context.features["labels"],
+        tf.convert_to_tensor((0,)))
 
     self.assertAllEqual(
         counterfactual.edge_sets["edge"].features["weight"],
-        as_tensor((0.8038801, 0.45028666)))
+        tf.convert_to_tensor((0.8038801, 0.45028666)))
 
     self.assertAllEqual(
         counterfactual.node_sets["node"].features["h"],
-        as_tensor((0.6295455, 0.37102205, 0.51270497)))
+        tf.convert_to_tensor((0.6295455, 0.37102205, 0.51270497)))
 
   def test_counterfactual_zeros(self):
     counterfactual = attribution.counterfactual(self.gt, random=False)
 
     self.assertAllEqual(
         counterfactual.context.features["h"],
-        as_tensor((0, 0)))
+        tf.convert_to_tensor((0, 0)))
+    self.assertAllEqual(
+        counterfactual.context.features["labels"],
+        tf.convert_to_tensor((0,)))
 
     self.assertAllEqual(
         counterfactual.edge_sets["edge"].features["weight"],
-        as_tensor((0, 0)))
+        tf.convert_to_tensor((0, 0)))
 
     self.assertAllEqual(
         counterfactual.node_sets["node"].features["h"],
-        as_tensor((0, 0, 0)))
+        tf.convert_to_tensor((0, 0, 0)))
 
   def test_subtract_graph_features(self):
     deltas = attribution.subtract_graph_features(
         self.gt,
         self.gt.replace_features(
-            context={"h": as_tensor((.4, .8))},
+            context={
+                "h": tf.convert_to_tensor((.4, .8)),
+                "labels": tf.convert_to_tensor((1,))
+            },
             node_sets={
                 "node": {
-                    "h": as_tensor((.1, .2, .3))
+                    "h": tf.convert_to_tensor((.1, .2, .3))
                 }
             },
             edge_sets={
                 "edge": {
-                    "weight": as_tensor((.2, .1))
+                    "weight": tf.convert_to_tensor((.2, .1))
                 }
             }))
 
     self.assertAllClose(
         deltas.context.features["h"],
-        as_tensor((.514 - .4, .433 - .8)))
+        tf.convert_to_tensor((.514 - .4, .433 - .8)))
+    self.assertAllClose(
+        deltas.context.features["labels"],
+        tf.convert_to_tensor((0 - 1,)))
 
     self.assertAllClose(
         deltas.edge_sets["edge"].features["weight"],
-        as_tensor((.153 - .2, .9 - .1)))
+        tf.convert_to_tensor((.153 - .2, .9 - .1)))
 
     self.assertAllClose(
         deltas.node_sets["node"].features["h"],
-        as_tensor((.8191 - .1, .9474 - .2, .1634 - .3),))
+        tf.convert_to_tensor((.8191 - .1, .9474 - .2, .1634 - .3),))
 
   def test_interpolate(self):
     counterfactual = attribution.counterfactual(self.gt, random=True, seed=8191)
     interpolations = attribution.interpolate_graph_features(
         self.gt,
         counterfactual,
         steps=4)
 
     self.assertLen(interpolations, 4)
 
     # Interpolation 0
     self.assertAllEqual(
         interpolations[0].context.features["h"],
-        as_tensor((0.49280962, 0.466383)))
+        tf.convert_to_tensor((0.49280962, 0.466383)))
 
     self.assertAllEqual(
         interpolations[0].edge_sets["edge"].features["weight"],
-        as_tensor((0.8038801, 0.45028666)))
+        tf.convert_to_tensor((0.8038801, 0.45028666)))
 
     self.assertAllClose(
         interpolations[0].node_sets["node"].features["h"],
-        as_tensor((0.6295455, 0.37102205, 0.51270497)))
+        tf.convert_to_tensor((0.6295455, 0.37102205, 0.51270497)))
 
     # Interpolation 1
     self.assertAllEqual(
         interpolations[1].context.features["h"],
-        as_tensor((0.49280962 + (.514 - 0.49280962) * 1 / 3,
-                   0.466383 + (.433 - 0.466383) * 1 / 3)))
+        tf.convert_to_tensor((0.49280962 + (.514 - 0.49280962) * 1 / 3,
+                              0.466383 + (.433 - 0.466383) * 1 / 3)))
 
     self.assertAllClose(
         interpolations[1].edge_sets["edge"].features["weight"],
-        as_tensor((0.8038801 + (.153 - 0.8038801) * 1 / 3,
-                   0.45028666 + (.9 - 0.45028666) * 1 / 3)))
+        tf.convert_to_tensor((0.8038801 + (.153 - 0.8038801) * 1 / 3,
+                              0.45028666 + (.9 - 0.45028666) * 1 / 3)))
 
     self.assertAllClose(
         interpolations[1].node_sets["node"].features["h"],
-        as_tensor((0.6295455 + (.8191 - 0.6295455) * 1 / 3,
-                   0.37102205 + (.9474 - 0.37102205) * 1 / 3,
-                   0.51270497 + (.1634 - 0.51270497) * 1 / 3)))
+        tf.convert_to_tensor((0.6295455 + (.8191 - 0.6295455) * 1 / 3,
+                              0.37102205 + (.9474 - 0.37102205) * 1 / 3,
+                              0.51270497 + (.1634 - 0.51270497) * 1 / 3)))
 
     # Interpolation 2
     self.assertAllEqual(
         interpolations[2].context.features["h"],
-        as_tensor((0.49280962 + (.514 - 0.49280962) * 2 / 3,
-                   0.466383 + (.433 - 0.466383) * 2 / 3)))
+        tf.convert_to_tensor((0.49280962 + (.514 - 0.49280962) * 2 / 3,
+                              0.466383 + (.433 - 0.466383) * 2 / 3)))
 
     self.assertAllClose(
         interpolations[2].edge_sets["edge"].features["weight"],
-        as_tensor((0.8038801 + (.153 - 0.8038801) * 2 / 3,
-                   0.45028666 + (.9 - 0.45028666) * 2 / 3)))
+        tf.convert_to_tensor((0.8038801 + (.153 - 0.8038801) * 2 / 3,
+                              0.45028666 + (.9 - 0.45028666) * 2 / 3)))
 
     self.assertAllClose(
         interpolations[2].node_sets["node"].features["h"],
-        as_tensor((0.6295455 + (.8191 - 0.6295455) * 2 / 3,
-                   0.37102205 + (.9474 - 0.37102205) * 2 / 3,
-                   0.51270497 + (.1634 - 0.51270497) * 2 / 3)))
+        tf.convert_to_tensor((0.6295455 + (.8191 - 0.6295455) * 2 / 3,
+                              0.37102205 + (.9474 - 0.37102205) * 2 / 3,
+                              0.51270497 + (.1634 - 0.51270497) * 2 / 3)))
 
     # Interpolation 3
     self.assertAllEqual(
         interpolations[3].context.features["h"],
-        as_tensor((.514, .433)))
+        tf.convert_to_tensor((.514, .433)))
 
     self.assertAllEqual(
         interpolations[3].edge_sets["edge"].features["weight"],
-        as_tensor((.153, .9)))
+        tf.convert_to_tensor((.153, .9)))
 
     self.assertAllEqual(
         interpolations[3].node_sets["node"].features["h"],
-        as_tensor((.8191, .9474, .1634)))
+        tf.convert_to_tensor((.8191, .9474, .1634)))
 
   def test_sum_graph_features(self):
     summation = attribution.sum_graph_features((self.gt,) * 4)
 
     self.assertAllEqual(
         summation.context.features["h"],
-        as_tensor((.514 * 4, .433 * 4)))
+        tf.convert_to_tensor((.514 * 4, .433 * 4)))
 
     self.assertAllEqual(
         summation.edge_sets["edge"].features["weight"],
-        as_tensor((.153 * 4, .9 * 4)))
+        tf.convert_to_tensor((.153 * 4, .9 * 4)))
 
     self.assertAllEqual(
         summation.node_sets["node"].features["h"],
-        as_tensor((.8191 * 4, .9474 * 4, .1634 * 4)))
+        tf.convert_to_tensor((.8191 * 4, .9474 * 4, .1634 * 4)))
 
   def test_integrated_gradients_exporter(self):
     # Preprocess model
     examples = tf.keras.Input(shape=(), dtype=tf.string, name="examples")
     parsed = tfgnn.keras.layers.ParseExample(self.gt.spec)(examples)
     parsed = parsed.merge_batch_to_components()
     label = tfgnn.keras.layers.ReadoutFirstNode(
@@ -201,15 +214,15 @@
         feature_name="h")(parsed)
     label = tf.random.uniform(
         tf.shape(label),
         minval=0,
         maxval=9,
         dtype=tf.int32)  # 10 classes
 
-    preprocess_model = tf.keras.Model(examples, (parsed, label))
+    preprocess_model = tf.keras.Model(examples, ((parsed,), label))
 
     # Model
     inputs = graph = tf.keras.Input(type_spec=parsed.spec)
     values = tfgnn.broadcast_node_to_edges(
         graph,
         "edge",
         tfgnn.TARGET,
@@ -243,15 +256,17 @@
     # Compile and fit
     model.compile("adam", "sparse_categorical_crossentropy")
     model.fit(ds.map(preprocess_model), epochs=16)
 
     # Export
     export_dir = self.create_tempdir()
     exporter = attribution.IntegratedGradientsExporter("output", steps=3)
-    exporter.save(preprocess_model, model, export_dir)
+
+    run_result = interfaces.RunResult(preprocess_model, None, model)
+    exporter.save(run_result, export_dir)
 
     saved_model = tf.saved_model.load(export_dir)
 
     # Integrated gradients
     kwargs = {
         "examples": next(iter(ds)),
     }
@@ -262,16 +277,16 @@
     # collecting a seed node for activations. The above graph is a line:
     # seed --weight 0--> node 1 --weight 1--> node 2.
     #
     # Information from weight 1 and node 2 never reaches the activations: they
     # should see no integrated gradients.
     self.assertAllClose(
         gt.node_sets["node"].features["h"],
-        as_tensor((2.3298206, -0.9860805, 0.)), 1e-04, 1e-04)
+        tf.convert_to_tensor((2.1929948, -1.0116194, 0.)), 1e-04, 1e-04)
 
     self.assertAllClose(
         gt.edge_sets["edge"].features["weight"],
-        as_tensor((4.725009, 0.)), 1e-04, 1e-04)
+        tf.convert_to_tensor((3.4002826, 0.)), 1e-04, 1e-04)
 
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_dir.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_dir.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,40 +14,31 @@
 # ==============================================================================
 """Model export helpers."""
 import os
 from typing import Any, Optional, Union
 
 import tensorflow as tf
 from tensorflow_gnn.runner import interfaces
-from tensorflow_gnn.runner.utils import model as model_utils
 
 Field = Union[tf.Tensor, tf.RaggedTensor]
 
 
 # TODO(b/196880966) Move to `model.py` and add unit tests.
 def _rename_output(output: Any, names: Any) -> Any:
   """Renames atoms of `output` with `names` for two matching structures."""
   tf.nest.assert_same_structure(output, names, check_types=False)
-
-  if not tf.nest.is_nested(output):
-    if names is not None:
-      return tf.keras.layers.Layer(name=names)(output)
-    else:
-      return output
-
   renamed_output = [
       tf.keras.layers.Layer(name=atom2)(atom1) if atom2 is not None else atom1
       for atom1, atom2 in zip(tf.nest.flatten(output), tf.nest.flatten(names))
   ]
-
   return tf.nest.pack_sequence_as(names, renamed_output)
 
 
 class KerasModelExporter(interfaces.ModelExporter):
-  """Exports a Keras model (with Keras API) via tf.keras.models.save_model."""
+  """Exports a Keras model (with Keras API) via `tf.keras.models.save_model`."""
 
   def __init__(self,
                *,
                output_names: Optional[Any] = None,
                subdirectory: Optional[str] = None,
                include_preprocessing: bool = True,
                options: Optional[tf.saved_model.SaveOptions] = None):
@@ -56,109 +47,146 @@
     Args:
       output_names: The name(s) for any output Tensor(s). Can be a single `str`
         name or a nested structure of `str` names. If a nested structure is
         given, it must match the structure of the exported model's output
         (as asserted by `tf.nest.assert_same_structure`): model output is
         renamed by flattening (`tf.nest.flatten`) and zipping the two
         structures. Any `None` values in `output_names` are ignored (leaving
-        that corresponding atom with its original name). Renamed atoms are
-        packed into the structure of `output_names`: in this way, `dict(...)`
-        keys of a model output can also be renamed.
+        that corresponding atom with its original name).
       subdirectory: An optional subdirectory, if set: models are exported to
         `os.path.join(export_dir, subdirectory).`
       include_preprocessing: Whether to include any `preprocess_model.`
-      options: Options for saving to SavedModel.
+      options: Options for saving to a TensorFlow `SavedModel`.
     """
     self._output_names = output_names
     self._subdirectory = subdirectory
     self._include_preprocessing = include_preprocessing
     self._options = options
 
-  def save(self,
-           preprocess_model: Optional[tf.keras.Model],
-           model: tf.keras.Model,
-           export_dir: str):
+  def save(self, run_result: interfaces.RunResult, export_dir: str):
     """Exports a Keras model (with Keras API) via tf.keras.models.save_model.
 
-    Importantly: the `preprocess_model`, if provided, and `model` are
-    concatenated before any export. Concatenation involves the chaining of the
-    first output of `preprocess_model` to the only input of `model.` The result
-    is a model with the input of `preprocess_model` and the output of `model.`
+    Importantly: the `run_result.preprocess_model`, if provided, and
+    `run_result.trained_model` are stacked before any export. Stacking involves
+    the chaining of the first output of `run_result.preprocess_model` to the
+    only input of `run_result.trained_model.` The result is a model with the
+    input of `run_result.preprocess_model` and the output of
+    `run_result.trained_model.`
 
     Args:
-      preprocess_model: An optional `tf.keras.Model` for preprocessing.
-      model: A `tf.keras.Model` to save.
-      export_dir: A destination directory for the model.
+      run_result: A `RunResult` from training.
+      export_dir: A destination directory.
     """
-    if preprocess_model is not None and self._include_preprocessing:
-      model = model_utils.chain_first_output(preprocess_model, model)
-    if self._output_names is not None:
-      output = _rename_output(model.output, self._output_names)
-      model = tf.keras.Model(model.input, output)
-    if self._subdirectory:
-      export_dir = os.path.join(export_dir, self._subdirectory)
-    tf.keras.models.save_model(model, export_dir, options=self._options)
+    preprocess_model = run_result.preprocess_model
+    model = run_result.trained_model
+
+    if preprocess_model and not preprocess_model.built:
+      raise ValueError("`preprocess_model` is expected to have been built")
+    elif not model.built:
+      raise ValueError("`model` is expected to have been built")
+
+    _save_model(export_dir,
+                preprocess_model,
+                model,
+                self._include_preprocessing,
+                self._output_names,
+                self._subdirectory,
+                self._options)
 
 
 class SubmoduleExporter(interfaces.ModelExporter):
-  """Exports a Keras model submodule (`getarr(model, 'submodules')`) by name."""
+  """Exports a Keras submodule.
+
+  Given a `RunResult`, this exporter creates and exports a submodule with
+  inputs identical to the trained model and outputs from some intermediate layer
+  (named `sublayer_name`). For example, with pseudocode:
+
+  `trained_model = tf.keras.Sequential([layer1, layer2, layer3, layer4])`
+  and
+  `SubmoduleExporter(sublayer_name='layer2')`
+
+  The exported submodule is:
+
+  `submodule = tf.keras.Sequential([layer1, layer2])`
+  """
 
   def __init__(self,
-               submodule_name: str,
+               sublayer_name: str,
                *,
                output_names: Optional[Any] = None,
                subdirectory: Optional[str] = None,
                include_preprocessing: bool = False,
                options: Optional[tf.saved_model.SaveOptions] = None):
     """Captures the args shared across `save(...)` calls.
 
     Args:
-      submodule_name: The name of the submodule to export.
-      output_names: The names for output Tensor(s), see: `KerasModelExporter.`
+      sublayer_name: The name of the submodule's final layer.
+      output_names: The names for output Tensor(s), see: `KerasModelExporter`.
       subdirectory: An optional subdirectory, if set: submodules are exported
-        to `os.path.join(export_dir, subdirectory).`
-      include_preprocessing: Whether to include any `preprocess_model.`
-      options: Options for saving to SavedModel.
+        to `os.path.join(export_dir, subdirectory)`.
+      include_preprocessing: Whether to include any `preprocess_model`.
+      options: Options for saving to a TensorFlow `SavedModel`.
     """
+    self._sublayer_name = sublayer_name
     self._output_names = output_names
     self._subdirectory = subdirectory
-    self._submodule_name = submodule_name
     self._include_preprocessing = include_preprocessing
     self._options = options
 
-  def save(self,
-           preprocess_model: Optional[tf.keras.Model],
-           model: tf.keras.Model,
-           export_dir: str):
+  def save(self, run_result: interfaces.RunResult, export_dir: str):
     """Saves a Keras model submodule.
 
-    Importantly: the `preprocess_model`, if provided, and `model` are
-    concatenated before any export.
+    Importantly: the `run_result.preprocess_model`, if provided, and
+    `run_result.trained_model` are stacked before any export. Stacking involves
+    the chaining of the first output of `run_result.preprocess_model` to the
+    only input of `run_result.trained_model.` The result is a model with the
+    input of `run_result.preprocess_model` and the output of
+    `run_result.trained_model.`
 
     Args:
-      preprocess_model: An optional `tf.keras.Model` for preprocessing.
-      model: A `tf.keras.Model` to save.
-      export_dir: A destination directory for the model.
+      run_result: A `RunResult` from training.
+      export_dir: A destination directory.
     """
-    submodules = [m for m in model.submodules if self._submodule_name == m.name]
-
-    if not submodules:
-      raise ValueError(f"No submodule `{self._submodule_name}` found")
-    elif len(submodules) > 1:
-      raise ValueError(f"More than one submodule found ({submodules})")
-    elif isinstance(submodules[0], tf.keras.Model):
-      [submodel] = submodules
-    elif isinstance(submodules[0], tf.keras.layers.Layer):
-      [sublayer] = submodules
-      submodel = tf.keras.Model(sublayer.input, sublayer.output)
-    else:
-      [submodel] = submodules
-      raise ValueError(
-          f"Submodule ({submodel}) is neither a Keras Model nor Layer`")
-
-    exporter = KerasModelExporter(
-        output_names=self._output_names,
-        subdirectory=self._subdirectory,
-        include_preprocessing=self._include_preprocessing,
-        options=self._options)
+    preprocess_model = run_result.preprocess_model
+    model = run_result.trained_model
 
-    exporter.save(preprocess_model, submodel, export_dir)
+    if preprocess_model and not preprocess_model.built:
+      raise ValueError("`preprocess_model` is expected to have been built")
+    elif not model.built:
+      raise ValueError("`model` is expected to have been built")
+
+    layers = [l for l in model.layers if self._sublayer_name == l.name]
+
+    if not layers:
+      raise ValueError(f"No intermediate layer `{self._sublayer_name}` found")
+    elif len(layers) > 1:
+      raise ValueError(f"More than one intermediate layer found ({layers})")
+
+    [layer] = layers
+    submodule = tf.keras.Model(model.input, layer.output)
+
+    _save_model(export_dir,
+                preprocess_model,
+                submodule,
+                self._include_preprocessing,
+                self._output_names,
+                self._subdirectory,
+                self._options)
+
+
+def _save_model(export_dir: str,
+                preprocess_model: tf.keras.Model,
+                model: tf.keras.Model,
+                include_preprocessing: bool,
+                output_names: Optional[Any] = None,
+                subdirectory: Optional[str] = None,
+                options: Optional[tf.saved_model.SaveOptions] = None):
+  """Saves a Keras model."""
+  if preprocess_model and include_preprocessing:
+    xs, *_ = preprocess_model.output
+    model = tf.keras.Model(preprocess_model.input, model(xs))
+  if output_names:
+    output = _rename_output(model.output, output_names)
+    model = tf.keras.Model(model.input, output)
+  if subdirectory:
+    export_dir = os.path.join(export_dir, subdirectory)
+  tf.keras.models.save_model(model, export_dir, options=options)
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/model_export_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/model_export_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Tests for model_export."""
+import itertools
 import os
 from typing import Any
 
 from absl.testing import parameterized
 import tensorflow as tf
+
+from tensorflow_gnn.runner import interfaces
 from tensorflow_gnn.runner.utils import model_export
 
 
 def _duplicate_submodules(name: str) -> tf.keras.Model:
   inputs = tf.keras.Input(shape=(4,))
   outputs = tf.keras.layers.Dense(2)(inputs)
   model = tf.keras.Model(inputs, outputs)
@@ -54,23 +57,32 @@
     output = submodel(submodel.input) + 8191
   model = tf.keras.Model(submodel.input, output)
   return model
 
 
 def _no_submodule(ninputs: int, noutputs: int, name: str) -> tf.keras.Model:
   inputs = [tf.keras.Input(shape=(4,)) for _ in range(ninputs)]
-  x = tf.math.add_n(inputs)
-  outputs = [tf.keras.layers.Dense(2)(x) for _ in range(noutputs)]
+  x = tf.add_n(tf.nest.flatten(inputs))
+  delta = itertools.count(1)
+  outputs = [next(delta) + x for _ in range(noutputs)]
   if len(inputs) == 1:
     [inputs] = inputs
   if len(outputs) == 1:
     [outputs] = outputs
   return tf.keras.Model(inputs, outputs, name=name)
 
 
+def _structure_like(inputs: Any, outputs: Any) -> tf.keras.Model:
+  inputs = tf.nest.map_structure(lambda _: tf.keras.Input(shape=(4,)), inputs)
+  x = tf.add_n(tf.nest.flatten(inputs))
+  delta = itertools.count(1)
+  outputs = tf.nest.map_structure(lambda _: next(delta) + x, outputs)
+  return tf.keras.Model(inputs, outputs)
+
+
 def _tf_module_as_submodule(name: str) -> tf.keras.Model:
   inputs = tf.keras.Input(shape=(4,))
   outputs = tf.keras.layers.Dense(2)(inputs)
   submodule = tf.Module(name=name)
   model = tf.keras.Model(inputs, outputs)
   model.submodule = submodule
   return model
@@ -78,57 +90,58 @@
 
 class ModelExportTests(tf.test.TestCase, parameterized.TestCase):
 
   @parameterized.named_parameters([
       dict(
           testcase_name="SingleInputOutput",
           model=_no_submodule(1, 1, "abc123"),
-          output_names="output",
+          output_names="output_a",
       ),
       dict(
           testcase_name="SingleInputMultipleOutput",
           model=_no_submodule(1, 2, "abc123"),
-          output_names=["output_0", "output_1"],
+          output_names=["output_b", "output_a"],
       ),
       dict(
           testcase_name="MultipleInputSingleOutput",
           model=_no_submodule(2, 1, "abc123"),
-          output_names="output",
+          output_names="output_b",
       ),
       dict(
           testcase_name="MultipleInputOutput",
           model=_no_submodule(2, 2, "abc123"),
-          output_names=["output_0", "output_1"],
+          output_names=["output_a", "output_b"],
+      ),
+      dict(
+          testcase_name="MappingOutput",
+          model=_structure_like(None, {"x": None, "y": None}),
+          output_names={"y": "output_b", "x": "output_a"},
       ),
   ])
   def test_keras_model_exporter(
       self,
       model: tf.keras.Model,
       output_names: Any):
     export_dir = self.create_tempdir()
     exporter = model_export.KerasModelExporter(output_names=output_names)
-    exporter.save(None, model, export_dir)
+    exporter.save(interfaces.RunResult(None, None, model), export_dir)
 
     for load_fn in (tf.keras.models.load_model, tf.saved_model.load):
       saved_model = load_fn(export_dir)
 
-      if tf.nest.is_nested(model.input):
-        args = [tf.random.uniform([1, *i.shape[1:]]) for i in model.input]
-        kwargs = {i.name: v for i, v in zip(model.input, args)}
-      else:  # Single input
-        args = tf.random.uniform([1, *model.input.shape[1:]])
-        kwargs = {model.input.name: args}
+      names = [i.name for i in tf.nest.flatten(model.input)]
+      func = lambda i: tf.random.uniform((1, *i.shape[1:]))
+      args = [func(i) for i in tf.nest.flatten(model.input)]
+      kwargs = dict(zip(names, args))
 
       model_output = model(args)
       saved_model_outputs = saved_model.signatures["serving_default"](**kwargs)
 
-      if tf.nest.is_nested(model_output):
-        zipped = zip(model_output, output_names)
-      else:  # Single output
-        zipped = zip([model_output], [output_names])
+      tf.nest.assert_same_structure(model_output, output_names)
+      zipped = zip(tf.nest.flatten(model_output), tf.nest.flatten(output_names))
 
       for output, name in zipped:
         self.assertAllClose(
             output,
             saved_model_outputs[name],
             msg=f"Testing {load_fn.__name__} with output {name}")
 
@@ -204,15 +217,15 @@
       subdirectory: str,
       output_names: Any):
     export_dir = self.create_tempdir()
     exporter = model_export.SubmoduleExporter(
         submodule_name,
         output_names=output_names,
         subdirectory=subdirectory)
-    exporter.save(None, model, export_dir)
+    exporter.save(interfaces.RunResult(None, None, model), export_dir)
 
     submodule = next(m for m in model.submodules if submodule_name == m.name)
 
     if subdirectory:
       saved_model = tf.saved_model.load(os.path.join(export_dir, subdirectory))
     else:  # `export_dir` only
       saved_model = tf.saved_model.load(export_dir)
@@ -239,34 +252,35 @@
           saved_model_outputs[name], msg=f"Testing {name}...")
 
   @parameterized.named_parameters([
       dict(
           testcase_name="DuplicateSubmodules",
           model=_duplicate_submodules("abc123"),
           submodule_name="abc123",
-          expected_error=r"More than one submodule found \(\[.*\]\)",
+          expected_error=r"More than one intermediate layer found \(\[.*\]\)",
       ),
       dict(
           testcase_name="NoSubmodule",
           model=_no_submodule(1, 1, "abc123"),
           submodule_name="abc123",
-          expected_error="No submodule `abc123` found",
+          expected_error="No intermediate layer `.*` found",
       ),
       dict(
           testcase_name="TFModuleAsSubmodule",
           model=_tf_module_as_submodule("abc123"),
           submodule_name="abc123",
-          expected_error=r"Submodule \(.*\) is neither a Keras Model nor Layer",
+          expected_error="No intermediate layer `.*` found",
       ),
   ])
   def test_submodule_exporter_fails(
       self,
       model: tf.keras.Model,
       submodule_name: str,
       expected_error: str):
     exporter = model_export.SubmoduleExporter(submodule_name)
     with self.assertRaisesRegex(ValueError, expected_error):
-      exporter.save(None, model, self.create_tempdir())
+      run_result = interfaces.RunResult(None, None, model)
+      exporter.save(run_result, self.create_tempdir())
 
 
 if __name__ == "__main__":
   tf.test.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/padding.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/padding.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/parsing.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/runner/utils/strategies.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/runner/utils/strategies.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/BUILD` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/BUILD`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.data import unigraph
 from tensorflow_gnn.sampler import sampling_lib
 from tensorflow_gnn.sampler import sampling_spec_pb2
 from tensorflow_gnn.sampler import subgraph
 
 from google.protobuf import text_format
-# Placeholder for Google-internal runner import
 
 _DIRECT_RUNNER = "DirectRunner"
 _DATAFLOW_RUNNER = "DataflowRunner"
 
 PCollection = beam.pvalue.PCollection
 Example = tf.train.Example
 Features = tf.train.Features
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/graph_sampler_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/graph_sampler_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_lib_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_lib_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec.proto` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Provides builder pattern that eases creation of `tfgnn.SamplingSpec`.
 
 Output `SamplingSpec` will contain topologically-sorted `SamplingOp`s.
 
-# Usage examples.
 
-## Homogeneous Graphs.
+
+Example: Homogeneous Graphs.
 
 If your graph is *homogeneous* and your node set is named "nodes" and edge set
 is named "edges", then you can create the sampling spec proto as:
 
 
-```
+```python
 # Assume homogeneous schema with edge-set name "edges" connecting "nodes".
-schema = tfgnn.GraphSchema()
+schema = schema_pb2.GraphSchema()
 schema.edge_sets['edges'].source = s.edge_sets['edges'].target = 'nodes'
 
 proto = (SamplingSpecBuilder(schema).seed('nodes').sample(10, 'edges')
          .sample(5, 'edges').build())
 
 # Since graph homogeneous (i.e., only one edge type and node type), then you may
 # skip the edge-set and node-set names, and call as:
@@ -48,34 +48,34 @@
 The above spec is instructing to start at:
   - Nodes of type set name "nodes", then,
   - for each seed node, sample (up to) 10 of its neighbors (from edge set
     "edges").
   - for each of those neighbors, sample (up to) 5 neighbors (from same edgeset).
 
 
-## Heterogeneous Graphs.
+Example: Heterogeneous Graphs.
 
 E.g., if you consider citation datasets, you can make a SamplingSpec proto as:
 
-```
+```python
 proto = (SamplingSpecBuilder(schema)
           .seed('author').sample('writes', 10).sample('cited_by', 5)
           .build())
 ```
 
 This samples, starting from author node, 10 papers written by author, and for
 each paper, 10 papers citing it.
 
 
-## DAG Sampling.
+Example: DAG Sampling.
 
 Finally, your sampling might consist of a DAG. For this, you need to cache
 some returns of `.sample()` calls. For example:
 
-```
+```python
 # Store builder at level of "author written papers":
 builder = tfgnn.SamplingSpecBuilder(schema).seed('author').sample('writes', 10)
 path1 = builder.sample('cited_by', 5)
 path2 = builder.sample('written_by', 3).sample('writes')
 
 proto = (tfgnn.SamplingSpecBuilder.Join([path1, path2]).sample('cited_by', 10)
          .build())
@@ -84,20 +84,27 @@
 proto = path1.Join([path2]).sample('cited_by', 10).build()
 ```
 
 This merges together the papers written by author, and written by co-authors,
 and for each of those papers, sample 10 papers citing it.
 """
 import collections
-from typing import Optional, Iterable, Union, List
-
-import tensorflow_gnn as tfgnn
+from typing import Optional, Iterable, Union, List, Any, Mapping
 
+from tensorflow_gnn.graph import graph_constants
+from tensorflow_gnn.graph import graph_tensor
+from tensorflow_gnn.graph import graph_tensor_ops
+import tensorflow_gnn.proto.graph_schema_pb2 as schema_pb2
 from tensorflow_gnn.sampler import sampling_spec_pb2
 
+
+NodeSetName = graph_constants.NodeSetName
+EdgeSetName = graph_constants.EdgeSetName
+GraphTensor = graph_tensor.GraphTensor
+
 SamplingStrategy = sampling_spec_pb2.SamplingStrategy
 
 
 def _topological_sort(all_steps):
   """Uses `children` & `parents` to topologically-sort `all_steps`."""
   sorted_steps = []
   all_steps_set = set(all_steps)
@@ -129,53 +136,115 @@
 def _op_name_from_parents(parents):
   if len(parents) == 1:
     return parents[0].node_set_name
 
   return '(%s)' % '|'.join([s.op_name for s in parents])
 
 
+def make_sampling_spec_tree(
+    graph_schema: schema_pb2.GraphSchema,
+    seed_nodeset: NodeSetName,
+    *,
+    sample_sizes: List[int],
+    sampling_strategy=SamplingStrategy.RANDOM_UNIFORM
+) -> sampling_spec_pb2.SamplingSpec:
+  """Automatically creates `SamplingSpec` by starting from seed node set.
+
+  From seed node set, `sample_sizes[0]` are sampled from *every* edge set `E`
+  that originates from seed node set. Subsequently, from sampled edge `e` in `E`
+  the created `SamplingSpec` instructs sampling up to `sample_sizes[1]` edges
+  for `e`'s target node, and so on, until depth of `len(sample_sizes)`.
+
+  Args:
+    graph_schema: contains node-sets & edge-sets.
+    seed_nodeset: name of node-set that the sampler will be instructed to use as
+      seed nodes.
+    sample_sizes: list of number of nodes to sample. E.g. if `sample_sizes` are
+      `[5, 2, 2]`, then for every sampled node, up-to `5` of its neighbors will
+      be sampled, and for each, up to `2` of its neighbors will be sampled, etc,
+      totalling sampled nodes up to `5 * 2 * 2 = 20` for each seed node.
+    sampling_strategy: one of the supported sampling strategies, the same for
+      each depth.
+
+  Returns:
+    `SamplingSpec` that instructs the sampler to sample according to the
+    `sampling_strategy` and `sample_sizes`.
+  """
+  edge_sets_by_src_node_set = _edge_set_names_by_source(graph_schema)
+  spec_builder = SamplingSpecBuilder(
+      graph_schema,
+      default_strategy=sampling_strategy)
+  spec_builder = spec_builder.seed(seed_nodeset)
+
+  def _recursively_sample_all_edge_sets(
+      cur_node_set_name, sampling_step, remaining_sample_sizes):
+    if not remaining_sample_sizes:
+      return
+    for edge_set_name in sorted(edge_sets_by_src_node_set[cur_node_set_name]):
+      if graph_tensor.get_aux_type_prefix(edge_set_name):
+        continue  # Skip private edges (e.g., _readout).
+
+      edge_set_schema = graph_schema.edge_sets[edge_set_name]
+      _recursively_sample_all_edge_sets(
+          edge_set_schema.target,
+          sampling_step.sample(remaining_sample_sizes[0], edge_set_name),
+          remaining_sample_sizes[1:])
+
+  _recursively_sample_all_edge_sets(seed_nodeset, spec_builder, sample_sizes)
+
+  return spec_builder.build()
+
+
 class SamplingSpecBuilder(object):
   """Mimics builder pattern that eases creation of `tfgnn.SamplingSpec`.
 
-  # Usage examples.
-  ## Homogeneous Graphs.
+
+  Example: Homogeneous Graphs.
+
   If your graph is *homogeneous* and your node set is named "nodes" and edge set
   is named "edges", then you can create the sampling spec proto as:
 
-  ### NOTE: This should come from the outside, e.g., `graph_tensor.schema`.
-  ```
-  schema = tfgnn.GraphSchema()
+  NOTE: This should come from the outside, e.g., `graph_tensor.schema`.
+  
+  ```python
+  schema = schema_pb2.GraphSchema()
   schema.edge_sets['edges'].source = s.edge_sets['edges'].target = 'nodes'
 
   proto = (SamplingSpecBuilder(schema)
            .seed('nodes').sample('edges', 10).sample('edges', 5)
            .build())
   ```
+
   The above spec is instructing to start at:
     - Nodes of type set name "nodes", then,
     - for each seed node, sample 10 of its neighbors (from edge set "edges").
     - for each of those neighbors, sample 5 neighbors (from same edge set).
 
-  ## Heterogeneous Graphs.
+  Example: Heterogeneous Graphs.
+
   E.g., if you consider citation datasets, you can make a SamplingSpec proto as:
-  ```
+
+  ```python
   proto = (SamplingSpecBuilder(schema)
            .seed('author').sample('writes', 10).sample('cited_by', 5)
            .build())
   ```
+
   This samples, starting from author node, 10 papers written by author, and for
   each paper, 10 papers citing it.
 
-  ## DAG Sampling.
+
+  Example: DAG Sampling.
+
   Finally, your sampling might consist of a DAG. For this, you need to cache
   some returns of `.sample()` calls.
   """
 
   def __init__(
-      self, graph_schema: tfgnn.GraphSchema,
+      self, graph_schema: schema_pb2.GraphSchema,
       default_strategy: SamplingStrategy = SamplingStrategy.TOP_K):
     self.graph_schema = graph_schema
     self.seeds = []
     self.default_strategy = default_strategy
 
   @staticmethod
   def join(steps):
@@ -387,7 +456,23 @@
     if not steps:
       raise ValueError('Expecting at least one step.')
     self._steps = steps
 
   def sample(self, *sample_args, **sample_kwargs) -> '_SamplingStep':
     return self._steps[0].merge_then_sample(
         self._steps[1:], *sample_args, **sample_kwargs)
+
+
+def _edge_set_names_by_source(
+    graph: Union[schema_pb2.GraphSchema, GraphTensor, Any]
+    ) -> Mapping[NodeSetName, List[EdgeSetName]]:
+  """Returns map: node set name -> list of edge names outgoing from node set."""
+  results = collections.defaultdict(list)
+  if isinstance(graph, schema_pb2.GraphSchema):
+    for edge_set_name, edge_set_schema in graph.edge_sets.items():
+      results[edge_set_schema.source].append(edge_set_name)
+  elif graph_tensor_ops.is_graph_tensor(graph):
+    for edge_set_name, edge_set_tensor in graph.edge_sets.items():
+      results[edge_set_tensor.adjacency.source_name].append(edge_set_name)
+  else:
+    raise TypeError('Not yet supported type %s' % str(graph.__class__))
+  return results
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_spec_builder_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_spec_builder_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,33 +13,43 @@
 # limitations under the License.
 # ==============================================================================
 """Tests for sampling_spec_builder."""
 
 from absl.testing import absltest
 from absl.testing import parameterized
 
-import tensorflow_gnn as tfgnn
+import tensorflow_gnn.proto.graph_schema_pb2 as schema_pb2
 from tensorflow_gnn.sampler import sampling_spec_builder
 from tensorflow_gnn.sampler import sampling_spec_pb2
 
 from google.protobuf import text_format
 
 
-def get_schema(edge_sets=('AA', 'AB', 'AC', 'BC', 'CD')) -> tfgnn.GraphSchema:
-  schema = tfgnn.GraphSchema()
+def get_schema(edge_sets=('AA', 'AB', 'AC', 'BC', 'CD'),
+               add_readout_artifacts=False) -> schema_pb2.GraphSchema:
+  schema = schema_pb2.GraphSchema()
+
   # Schema has DAG like:
   # A -> B
   #  \    \
   #   +--> C -> D
   for edge_set_name in edge_sets:
     schema.edge_sets[edge_set_name].source = edge_set_name[0]
     schema.edge_sets[edge_set_name].target = edge_set_name[1]
     unused_node_set = schema.node_sets[edge_set_name[0]]  # To initalize.
     unused_node_set = schema.node_sets[edge_set_name[1]]
 
+  if add_readout_artifacts:
+    # Auxilary (_readout) node and edge sets should not appear output.
+    unused_node_set = schema.node_sets['_readout']  # Initialize
+    schema.edge_sets['_readout/source'].source = 'A'
+    schema.edge_sets['_readout/source'].target = '_readout'
+    schema.edge_sets['_readout/target'].source = 'B'
+    schema.edge_sets['_readout/target'].target = '_readout'
+
   return schema
 
 
 class SamplingSpecBuilderTest(parameterized.TestCase):
 
   def test_line_to_sampling_spec(self):
     schema = get_schema()
@@ -197,9 +207,135 @@
           sample_size: 1
           strategy: TOP_K
         }
         """, sampling_spec_pb2.SamplingSpec())
     self.assertEqual(expected_proto, proto)
 
 
+class MakeSamplingSpecTreeTest(parameterized.TestCase):
+
+  def test_1_hop(self):
+    sampling_spec_1hop = sampling_spec_builder.make_sampling_spec_tree(
+        get_schema(), 'A', sample_sizes=[3])
+
+    expected_spec_1hop = text_format.Parse(
+        """
+        seed_op {
+          op_name: "SEED->A"
+          node_set_name: "A"
+        }
+        sampling_ops {
+          op_name: "A->C"
+          input_op_names: "SEED->A"
+          edge_set_name: "AC"
+          sample_size: 3
+          strategy: RANDOM_UNIFORM
+        }
+        sampling_ops {
+          op_name: "A->B"
+          input_op_names: "SEED->A"
+          edge_set_name: "AB"
+          sample_size: 3
+          strategy: RANDOM_UNIFORM
+        }
+        sampling_ops {
+          op_name: "A->A"
+          input_op_names: "SEED->A"
+          edge_set_name: "AA"
+          sample_size: 3
+          strategy: RANDOM_UNIFORM
+        }
+        """, sampling_spec_pb2.SamplingSpec())
+    self.assertEqual(sampling_spec_1hop, expected_spec_1hop)
+
+  @parameterized.parameters(
+      [sampling_spec_pb2.RANDOM_UNIFORM, sampling_spec_pb2.TOP_K]
+  )
+  def test_2_hops(self, sampling_strategy: sampling_spec_pb2.SamplingStrategy):
+    sampling_spec_2hops = sampling_spec_builder.make_sampling_spec_tree(
+        get_schema(add_readout_artifacts=True),
+        'A',
+        sample_sizes=[3, 2],
+        sampling_strategy=sampling_strategy,
+    )
+    expected_spec_2hops = text_format.Parse(
+        """
+        seed_op {{
+          op_name: "SEED->A"
+          node_set_name: "A"
+        }}
+        sampling_ops {{
+          op_name: "A->C"
+          input_op_names: "SEED->A"
+          edge_set_name: "AC"
+          sample_size: 3
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "C->D"
+          input_op_names: "A->C"
+          edge_set_name: "CD"
+          sample_size: 2
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "A->B"
+          input_op_names: "SEED->A"
+          edge_set_name: "AB"
+          sample_size: 3
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "B->C"
+          input_op_names: "A->B"
+          edge_set_name: "BC"
+          sample_size: 2
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "A->A"
+          input_op_names: "SEED->A"
+          edge_set_name: "AA"
+          sample_size: 3
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "A->C.2"
+          input_op_names: "A->A"
+          edge_set_name: "AC"
+          sample_size: 2
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "A->B.2"
+          input_op_names: "A->A"
+          edge_set_name: "AB"
+          sample_size: 2
+          strategy: {sampling_strategy}
+        }}
+        sampling_ops {{
+          op_name: "A->A.2"
+          input_op_names: "A->A"
+          edge_set_name: "AA"
+          sample_size: 2
+          strategy: {sampling_strategy}
+        }}
+        """.format(sampling_strategy=sampling_strategy),
+        sampling_spec_pb2.SamplingSpec(),
+    )
+    self.assertEqual(sampling_spec_2hops, expected_spec_2hops)
+
+  def test_0_hops(self):
+    sampling_spec_0hops = sampling_spec_builder.make_sampling_spec_tree(
+        get_schema(), 'A', sample_sizes=[])
+    expected_spec_0hops = text_format.Parse(
+        """
+        seed_op {
+          op_name: "SEED->A"
+          node_set_name: "A"
+        }
+        """, sampling_spec_pb2.SamplingSpec())
+    self.assertEqual(sampling_spec_0hops, expected_spec_0hops)
+
+
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/sampling_utils_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/sampling_utils_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.proto` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/sampler/subgraph_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/sampler/subgraph_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tensorflow_gnn.bzl` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tensorflow_gnn.bzl`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 def pytype_strict_binary(name, **kwargs):
     native.py_binary(name = name, **kwargs)
 
 # Placeholder to use until bazel supports pytype_strict_library.
 def pytype_strict_library(name, **kwargs):
     native.py_library(name = name, **kwargs)
 
+# Placeholder to use until bazel supports pytype_library.
+def pytype_library(name, **kwargs):
+    native.py_library(name = name, **kwargs)
+
 # Deletes deps with a no_tfgnn_py_deps flag so that tests
 # can run from the pip wheel instead of bazel runfiles
 def py_test(name, deps = [], **kwargs):
     native.py_test(
         name = name,
         deps = select({
             "//conditions:default": deps,
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/generate_training_data_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/generate_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/print_training_data_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/print_training_data_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.proto` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.proto`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,17 +25,14 @@
 from absl import logging
 import apache_beam as beam
 from apache_beam.runners.direct import direct_runner
 import tensorflow as tf
 import tensorflow_gnn as tfgnn
 from tensorflow_gnn.tools import sampled_stats_pb2 as sspb
 
-# Placeholder for Google-internal runner import
-# Placeholder for Google-internal sorted string file format pipeline import
-
 
 def define_flags():
   """Define commandline flags."""
 
   flags.DEFINE_string(
       "graph_schema", None,
       ("Path to a text-formatted GraphSchema proto file describing the "
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/sampled_stats_test.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/sampled_stats_test.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/tools/validate_graph_schema.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/tools/validate_graph_schema.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/utils/test_utils.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn/version.py` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,8 +37,8 @@
 #
 # Patch releases X.Y.Z, Z > 0, incl. their release candidates, can be done for
 # patches on branch rX.Y as needed.
 #
 # IMPORANT: Right after branching rX.Y, bump the main branch to X.(Y+1).0.dev1.
 # (Submit a change to the Source of Truth, get it out on the main branch asap.)
 
-__version__ = "0.5.1"
+__version__ = "0.6.0rc0"
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/PKG-INFO` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorflow-gnn
-Version: 0.5.1
+Version: 0.6.0rc0
 Summary: A library for building scalable graph neural networks in TensorFlow.
 Home-page: https://github.com/tensorflow/gnn
 Download-URL: https://github.com/tensorflow/gnn.git
 Author: Google LLC
 Author-email: tensorflow-gnn@googlegroups.com
 License: Apache 2.0
 Keywords: tensorflow gnn graph
@@ -30,18 +30,14 @@
 License-File: AUTHORS
 
 # TensorFlow GNN
 
 **This is an early (alpha) release to get community feedback.** It's under
 active development and **we may break API compatibility in the future**.
 
-> **NOTE**:
-> 2023/01/11: Release 0.4.1 was yanked due to a broken merge that passed through
-> our tests. Release 0.4.0 still works, and we are working on a new release,
-> stay tuned.
 
 TensorFlow GNN is a library to build Graph Neural Networks on the TensorFlow
 platform. It contains the following components:
 
 * A high-level Keras-style API to create GNN models that can easily be composed
   with other types of models. GNNs are often used in combination with ranking,
   deep-retrieval (dual-encoders) or mixed with other types of models
```

### Comparing `tensorflow-gnn-0.5.1/tensorflow_gnn.egg-info/SOURCES.txt` & `tensorflow-gnn-0.6.0rc0/tensorflow_gnn.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -21,34 +21,70 @@
 tensorflow_gnn.egg-info/requires.txt
 tensorflow_gnn.egg-info/top_level.txt
 tensorflow_gnn/converters/__init__.py
 tensorflow_gnn/converters/triples.py
 tensorflow_gnn/converters/triples_test.py
 tensorflow_gnn/converters/ogb/__init__.py
 tensorflow_gnn/converters/ogb/convert_ogb_dataset.py
+tensorflow_gnn/converters/ogb/convert_ogb_to_npz.py
 tensorflow_gnn/converters/ogb/ogb_lib.py
 tensorflow_gnn/data/BUILD
 tensorflow_gnn/data/__init__.py
 tensorflow_gnn/data/unigraph.py
 tensorflow_gnn/data/unigraph_test.py
 tensorflow_gnn/experimental/__init__.py
 tensorflow_gnn/experimental/in_memory/__init__.py
 tensorflow_gnn/experimental/in_memory/datasets.py
+tensorflow_gnn/experimental/in_memory/datasets_test.py
 tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler.py
 tensorflow_gnn/experimental/in_memory/int_arithmetic_sampler_test.py
 tensorflow_gnn/experimental/in_memory/models.py
+tensorflow_gnn/experimental/in_memory/networkx_data.py
+tensorflow_gnn/experimental/in_memory/networkx_data_test.py
 tensorflow_gnn/experimental/in_memory/reader_utils.py
 tensorflow_gnn/experimental/in_memory/unigraph_data.py
 tensorflow_gnn/experimental/in_memory/unigraph_data_test.py
+tensorflow_gnn/experimental/sampler/BUILD
+tensorflow_gnn/experimental/sampler/__init__.py
+tensorflow_gnn/experimental/sampler/core.py
+tensorflow_gnn/experimental/sampler/core_test.py
+tensorflow_gnn/experimental/sampler/custom_ops_test.py
+tensorflow_gnn/experimental/sampler/eval_dag.proto
+tensorflow_gnn/experimental/sampler/eval_dag.py
+tensorflow_gnn/experimental/sampler/eval_dag_test.py
+tensorflow_gnn/experimental/sampler/ext_ops.py
+tensorflow_gnn/experimental/sampler/ext_ops_parallel.py
+tensorflow_gnn/experimental/sampler/ext_ops_test.py
+tensorflow_gnn/experimental/sampler/ext_ops_vectorized.py
+tensorflow_gnn/experimental/sampler/interfaces.py
+tensorflow_gnn/experimental/sampler/link_samplers.py
+tensorflow_gnn/experimental/sampler/link_samplers_test.py
+tensorflow_gnn/experimental/sampler/subgraph_pipeline.py
+tensorflow_gnn/experimental/sampler/subgraph_pipeline_test.py
+tensorflow_gnn/experimental/sampler/beam/BUILD
+tensorflow_gnn/experimental/sampler/beam/accessors.py
+tensorflow_gnn/experimental/sampler/beam/accessors_test.py
+tensorflow_gnn/experimental/sampler/beam/edge_samplers.py
+tensorflow_gnn/experimental/sampler/beam/edge_samplers_test.py
+tensorflow_gnn/experimental/sampler/beam/executor_lib.py
+tensorflow_gnn/experimental/sampler/beam/executor_lib_test.py
+tensorflow_gnn/experimental/sampler/beam/sampler.py
+tensorflow_gnn/experimental/sampler/beam/sampler_test.py
+tensorflow_gnn/experimental/sampler/beam/unigraph_utils.py
+tensorflow_gnn/experimental/sampler/beam/unigraph_utils_test.py
+tensorflow_gnn/experimental/sampler/beam/utils.py
+tensorflow_gnn/experimental/sampler/beam/utils_test.py
 tensorflow_gnn/graph/BUILD
 tensorflow_gnn/graph/__init__.py
 tensorflow_gnn/graph/adjacency.py
 tensorflow_gnn/graph/adjacency_test.py
 tensorflow_gnn/graph/batching_utils.py
 tensorflow_gnn/graph/batching_utils_test.py
+tensorflow_gnn/graph/broadcast_ops.py
+tensorflow_gnn/graph/broadcast_ops_test.py
 tensorflow_gnn/graph/dict_utils.py
 tensorflow_gnn/graph/dict_utils_test.py
 tensorflow_gnn/graph/graph_constants.py
 tensorflow_gnn/graph/graph_piece.py
 tensorflow_gnn/graph/graph_piece_test.py
 tensorflow_gnn/graph/graph_tensor.py
 tensorflow_gnn/graph/graph_tensor_encode.py
@@ -63,28 +99,35 @@
 tensorflow_gnn/graph/graph_tensor_random_test.py
 tensorflow_gnn/graph/graph_tensor_test.py
 tensorflow_gnn/graph/graph_tensor_test_utils.py
 tensorflow_gnn/graph/normalization_ops.py
 tensorflow_gnn/graph/normalization_ops_test.py
 tensorflow_gnn/graph/padding_ops.py
 tensorflow_gnn/graph/padding_ops_test.py
+tensorflow_gnn/graph/pool_ops.py
+tensorflow_gnn/graph/pool_ops_test.py
 tensorflow_gnn/graph/preprocessing_common.py
 tensorflow_gnn/graph/preprocessing_common_test.py
+tensorflow_gnn/graph/readout.py
+tensorflow_gnn/graph/readout_test.py
 tensorflow_gnn/graph/schema_utils.py
 tensorflow_gnn/graph/schema_utils_test.py
 tensorflow_gnn/graph/schema_validation.py
 tensorflow_gnn/graph/schema_validation_test.py
 tensorflow_gnn/graph/tag_utils.py
 tensorflow_gnn/graph/tag_utils_test.py
 tensorflow_gnn/graph/tensor_utils.py
 tensorflow_gnn/graph/tensor_utils_test.py
+tensorflow_gnn/graph/tf_internal.py
 tensorflow_gnn/keras/BUILD
 tensorflow_gnn/keras/__init__.py
 tensorflow_gnn/keras/builders.py
 tensorflow_gnn/keras/builders_test.py
+tensorflow_gnn/keras/initializers.py
+tensorflow_gnn/keras/initializers_test.py
 tensorflow_gnn/keras/keras_e2e_test.py
 tensorflow_gnn/keras/keras_tensors.py
 tensorflow_gnn/keras/keras_tensors_test.py
 tensorflow_gnn/keras/layers/BUILD
 tensorflow_gnn/keras/layers/__init__.py
 tensorflow_gnn/keras/layers/convolution_base.py
 tensorflow_gnn/keras/layers/convolution_base_test.py
@@ -102,41 +145,55 @@
 tensorflow_gnn/keras/layers/next_state_test.py
 tensorflow_gnn/keras/layers/padding_ops.py
 tensorflow_gnn/keras/layers/padding_ops_test.py
 tensorflow_gnn/keras/layers/parse_example.py
 tensorflow_gnn/keras/layers/parse_example_test.py
 tensorflow_gnn/models/contrastive_losses/BUILD
 tensorflow_gnn/models/contrastive_losses/__init__.py
+tensorflow_gnn/models/contrastive_losses/distribute_test.py
 tensorflow_gnn/models/contrastive_losses/layers.py
-tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/BUILD
-tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/distribute_test.py
-tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers.py
-tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/layers_test.py
-tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks.py
-tensorflow_gnn/models/contrastive_losses/deep_graph_infomax/tasks_test.py
+tensorflow_gnn/models/contrastive_losses/layers_test.py
+tensorflow_gnn/models/contrastive_losses/losses.py
+tensorflow_gnn/models/contrastive_losses/losses_test.py
+tensorflow_gnn/models/contrastive_losses/metrics.py
+tensorflow_gnn/models/contrastive_losses/metrics_test.py
+tensorflow_gnn/models/contrastive_losses/tasks.py
+tensorflow_gnn/models/contrastive_losses/tasks_test.py
 tensorflow_gnn/models/gat_v2/BUILD
 tensorflow_gnn/models/gat_v2/__init__.py
+tensorflow_gnn/models/gat_v2/config_dict.py
+tensorflow_gnn/models/gat_v2/config_dict_test.py
+tensorflow_gnn/models/gat_v2/hparams_vizier.py
+tensorflow_gnn/models/gat_v2/hparams_vizier_test.py
 tensorflow_gnn/models/gat_v2/layers.py
 tensorflow_gnn/models/gat_v2/layers_test.py
 tensorflow_gnn/models/gcn/BUILD
 tensorflow_gnn/models/gcn/__init__.py
 tensorflow_gnn/models/gcn/gcn_conv.py
 tensorflow_gnn/models/gcn/gcn_conv_test.py
-tensorflow_gnn/models/gpt_gnn/BUILD
-tensorflow_gnn/models/gpt_gnn/__init__.py
-tensorflow_gnn/models/gpt_gnn/tensor_utils.py
-tensorflow_gnn/models/gpt_gnn/tensor_utils_test.py
 tensorflow_gnn/models/graph_sage/BUILD
 tensorflow_gnn/models/graph_sage/__init__.py
 tensorflow_gnn/models/graph_sage/layers.py
 tensorflow_gnn/models/graph_sage/layers_test.py
 tensorflow_gnn/models/hgt/BUILD
 tensorflow_gnn/models/hgt/__init__.py
-tensorflow_gnn/models/hgt/softmax.py
-tensorflow_gnn/models/hgt/softmax_test.py
+tensorflow_gnn/models/hgt/config_dict.py
+tensorflow_gnn/models/hgt/config_dict_test.py
+tensorflow_gnn/models/hgt/hparams_vizier.py
+tensorflow_gnn/models/hgt/hparams_vizier_test.py
+tensorflow_gnn/models/hgt/layers.py
+tensorflow_gnn/models/hgt/layers_test.py
+tensorflow_gnn/models/mt_albis/BUILD
+tensorflow_gnn/models/mt_albis/__init__.py
+tensorflow_gnn/models/mt_albis/config_dict.py
+tensorflow_gnn/models/mt_albis/config_dict_test.py
+tensorflow_gnn/models/mt_albis/hparams_vizier.py
+tensorflow_gnn/models/mt_albis/hparams_vizier_test.py
+tensorflow_gnn/models/mt_albis/layers.py
+tensorflow_gnn/models/mt_albis/layers_test.py
 tensorflow_gnn/models/multi_head_attention/BUILD
 tensorflow_gnn/models/multi_head_attention/__init__.py
 tensorflow_gnn/models/multi_head_attention/config_dict.py
 tensorflow_gnn/models/multi_head_attention/config_dict_test.py
 tensorflow_gnn/models/multi_head_attention/hparams_vizier.py
 tensorflow_gnn/models/multi_head_attention/hparams_vizier_test.py
 tensorflow_gnn/models/multi_head_attention/layers.py
@@ -158,33 +215,35 @@
 tensorflow_gnn/runner/__init__.py
 tensorflow_gnn/runner/distribute_test.py
 tensorflow_gnn/runner/interfaces.py
 tensorflow_gnn/runner/orchestration.py
 tensorflow_gnn/runner/orchestration_test.py
 tensorflow_gnn/runner/examples/ogbn/mag/BUILD
 tensorflow_gnn/runner/examples/ogbn/mag/train.py
+tensorflow_gnn/runner/examples/ogbn/mag/utils.py
+tensorflow_gnn/runner/examples/ogbn/mag/utils_test.py
 tensorflow_gnn/runner/input/BUILD
 tensorflow_gnn/runner/input/datasets.py
 tensorflow_gnn/runner/input/datasets_test.py
 tensorflow_gnn/runner/tasks/BUILD
 tensorflow_gnn/runner/tasks/classification.py
 tensorflow_gnn/runner/tasks/classification_test.py
+tensorflow_gnn/runner/tasks/link_prediction.py
+tensorflow_gnn/runner/tasks/link_prediction_test.py
 tensorflow_gnn/runner/tasks/regression.py
 tensorflow_gnn/runner/tasks/regression_test.py
 tensorflow_gnn/runner/trainers/BUILD
 tensorflow_gnn/runner/trainers/keras_fit.py
 tensorflow_gnn/runner/utils/BUILD
 tensorflow_gnn/runner/utils/attribution.py
 tensorflow_gnn/runner/utils/attribution_test.py
-tensorflow_gnn/runner/utils/model.py
+tensorflow_gnn/runner/utils/label_fns.py
 tensorflow_gnn/runner/utils/model_dir.py
 tensorflow_gnn/runner/utils/model_export.py
 tensorflow_gnn/runner/utils/model_export_test.py
-tensorflow_gnn/runner/utils/model_templates.py
-tensorflow_gnn/runner/utils/model_test.py
 tensorflow_gnn/runner/utils/padding.py
 tensorflow_gnn/runner/utils/parsing.py
 tensorflow_gnn/runner/utils/parsing_test.py
 tensorflow_gnn/runner/utils/strategies.py
 tensorflow_gnn/sampler/BUILD
 tensorflow_gnn/sampler/__init__.py
 tensorflow_gnn/sampler/graph_sampler.py
```

