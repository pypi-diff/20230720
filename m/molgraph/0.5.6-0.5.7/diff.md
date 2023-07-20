# Comparing `tmp/molgraph-0.5.6.tar.gz` & `tmp/molgraph-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.6.tar", last modified: Wed Jul 19 15:00:44 2023, max compression
+gzip compressed data, was "molgraph-0.5.7.tar", last modified: Thu Jul 20 11:49:52 2023, max compression
```

## Comparing `molgraph-0.5.6.tar` & `molgraph-0.5.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.6/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-19 15:00:44.027500 molgraph-0.5.6/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5998 2023-07-17 15:20:50.000000 molgraph-0.5.6/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.019500 molgraph-0.5.6/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.019500 molgraph-0.5.6/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       81 2023-07-18 13:59:25.000000 molgraph-0.5.6/molgraph/applications/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10465 2023-07-19 14:41:48.000000 molgraph-0.5.6/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.6/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.6/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21162 2023-07-19 14:31:44.000000 molgraph-0.5.6/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.6/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.6/molgraph/chemistry/vis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      923 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/internal.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.6/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12927 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11735 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9923 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11863 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10845 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17229 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.6/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10192 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11264 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10555 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.6/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9981 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10871 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    26149 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.6/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16323 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14494 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.6/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10772 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.6/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3829 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3031 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.6/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11065 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4593 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9633 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4258 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11887 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6688 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20500 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.6/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6405 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4687 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3332 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6274 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5369 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.023500 molgraph-0.5.6/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.6/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2382 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.6/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      984 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6987 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7101 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.6/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10961 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6905 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.6/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    27436 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20236 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.027500 molgraph-0.5.6/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.6/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.6/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1877 2023-07-17 15:20:50.000000 molgraph-0.5.6/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    51982 2023-07-19 15:00:26.000000 molgraph-0.5.6/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-19 15:00:44.019500 molgraph-0.5.6/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6718 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-19 15:00:43.000000 molgraph-0.5.6/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-19 15:00:44.027500 molgraph-0.5.6/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1418 2023-07-17 15:20:50.000000 molgraph-0.5.6/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.331200 molgraph-0.5.7/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.7/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6797 2023-07-20 11:49:52.331200 molgraph-0.5.7/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6077 2023-07-20 11:49:31.000000 molgraph-0.5.7/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.283200 molgraph-0.5.7/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1341 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-20 11:49:31.000000 molgraph-0.5.7/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.287200 molgraph-0.5.7/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       81 2023-07-18 13:59:25.000000 molgraph-0.5.7/molgraph/applications/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.299200 molgraph-0.5.7/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.299200 molgraph-0.5.7/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.7/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.7/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.7/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.7/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13260 2023-07-20 11:49:31.000000 molgraph-0.5.7/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.7/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.7/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21138 2023-07-20 11:49:31.000000 molgraph-0.5.7/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.7/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.7/molgraph/chemistry/vis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      923 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/internal.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.299200 molgraph-0.5.7/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.307200 molgraph-0.5.7/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.7/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12927 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11735 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9923 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11863 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10845 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17229 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.307200 molgraph-0.5.7/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.7/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10241 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10192 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11264 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10555 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.311200 molgraph-0.5.7/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.7/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9981 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10871 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1633 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    26149 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.311200 molgraph-0.5.7/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.7/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16323 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14494 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.315200 molgraph-0.5.7/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.7/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10760 2023-07-20 11:49:31.000000 molgraph-0.5.7/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.315200 molgraph-0.5.7/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.7/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3829 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2061 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3031 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.315200 molgraph-0.5.7/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.7/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11065 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4593 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9633 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4258 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11887 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6688 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20500 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.327200 molgraph-0.5.7/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.7/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6405 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4687 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3332 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6274 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5369 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.327200 molgraph-0.5.7/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.7/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2382 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5383 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.327200 molgraph-0.5.7/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.7/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2083 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      566 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.327200 molgraph-0.5.7/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      984 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6987 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7101 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.331200 molgraph-0.5.7/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.7/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10961 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6905 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.331200 molgraph-0.5.7/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.7/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    27436 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20236 2023-07-19 15:00:26.000000 molgraph-0.5.7/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.331200 molgraph-0.5.7/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.7/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.7/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1877 2023-07-17 15:20:50.000000 molgraph-0.5.7/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    52934 2023-07-20 11:49:31.000000 molgraph-0.5.7/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-20 11:49:52.287200 molgraph-0.5.7/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6797 2023-07-20 11:49:52.000000 molgraph-0.5.7/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-20 11:49:52.000000 molgraph-0.5.7/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-20 11:49:52.000000 molgraph-0.5.7/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       65 2023-07-20 11:49:52.000000 molgraph-0.5.7/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-20 11:49:52.000000 molgraph-0.5.7/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-20 11:49:52.331200 molgraph-0.5.7/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1418 2023-07-17 15:20:50.000000 molgraph-0.5.7/setup.py
```

### Comparing `molgraph-0.5.6/LICENSE` & `molgraph-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/PKG-INFO` & `molgraph-0.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.6
+Version: 0.5.7
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MolGraph: Graph Neural Networks for Molecular Machine Learning
 
 *This is an early release; things are still being updated, added and experimented with. Hence, API compatibility may break in the future.*
 
-*Any feedback is welcomed!*
+*Any feedback is welcomed! If there are any issues/suggestions/questions, do not hesitate to bring it up!*
 
 ## Manuscript
 See [pre-print](https://arxiv.org/abs/2208.09944)
 
 ## Documentation
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
```

### Comparing `molgraph-0.5.6/README.md` & `molgraph-0.5.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # MolGraph: Graph Neural Networks for Molecular Machine Learning
 
 *This is an early release; things are still being updated, added and experimented with. Hence, API compatibility may break in the future.*
 
-*Any feedback is welcomed!*
+*Any feedback is welcomed! If there are any issues/suggestions/questions, do not hesitate to bring it up!*
 
 ## Manuscript
 See [pre-print](https://arxiv.org/abs/2208.09944)
 
 ## Documentation
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
```

### Comparing `molgraph-0.5.6/molgraph/_filter_warnings.py` & `molgraph-0.5.7/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/__init__.py` & `molgraph-0.5.7/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.7/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.7/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.7/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.7/molgraph/chemistry/benchmark/tf_records.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-import math
+import tensorflow as tf
+import numpy as np
+
 import os
-import multiprocessing
-from functools import partial
+import math
 import json
+import multiprocessing
+
 from glob import glob
-import tensorflow as tf
-import numpy as np
+from time import sleep
+from warnings import warn
 
-from rdkit import Chem
 from typing import Optional
 from typing import Union
 from typing import Dict
 from typing import List
 from typing import Tuple
-from typing import Sequence
 from typing import Any
 
 from molgraph.tensors.graph_tensor import GraphTensor
 from molgraph.tensors.graph_tensor import GraphTensorSpec
 from molgraph.chemistry.molecular_encoders import MolecularGraphEncoder
 from molgraph.chemistry.molecular_encoders import MolecularGraphEncoder3D
 from molgraph.chemistry.benchmark.datasets import Dataset
 
 
+# TODO: Clean up code.
 
 def write(
     path: str,
-    inputs: dict,
-    encoder: Union[MolecularGraphEncoder, MolecularGraphEncoder3D],
+    data: dict,
+    encoder: Union[MolecularGraphEncoder, MolecularGraphEncoder3D, None],
     num_files: Optional[int] = None,
-    processes: Optional[int] = None,
-    device: str = '/cpu:0'
+    num_processes: Optional[int] = None,
+    device: str = '/cpu:0',
+    **kwargs
 ) -> None:
 
     '''Writes TF records.
 
     **Example:**
 
     >>> x = ['CC', 'CCC', 'CCCC']
@@ -43,100 +46,135 @@
     ...     atom_encoder=molgraph.chemistry.Featurizer([
     ...         molgraph.chemistry.features.Symbol(),
     ...         molgraph.chemistry.features.Hybridization(),
     ...     ])
     ... )
     >>> molgraph.chemistry.tf_records.write( # doctest: +SKIP
     ...     path='/tmp/dummy_records/',
-    ...     inputs={'x': x, 'y': y},
+    ...     data={'x': x, 'y': y},
     ...     encoder=encoder
     ... )
 
     Args:
         path (str):
             The path to write TF records to (save path). Should not include
             file name. File names are automatically determined.
-        inputs (dict):
-            The data to be written as TF records. The keys of the inputs (dict),
+        data (dict):
+            The data to be written as TF records. The keys of the data (dict),
             are the name of the data fields, while the values are the actual
-            values (of the fields). E.g., ``{'x': ['CC', 'CCO'], 'y': [4.1, 2.4]}``.
-            The ``encoder`` will be applied to the mandatory ``inputs['x']`` field.
-        encoder (MolecularGraphEncoder, MolecularGraphEncoder3D):
-            The encoder to be applied to ``inputs['x']``. The encoder transforms
+            values (of the fields). E.g., 
+            ``{'x': ['CC', 'CCO'], 'y': [4.1, 2.4]}``. The ``encoder`` will be 
+            applied to the mandatory ``data['x']`` field.
+        encoder (MolecularGraphEncoder, MolecularGraphEncoder3D, None):
+            The encoder to be applied to ``data['x']``. The encoder transforms
             the string (or rdkit.Chem.Mol) representations of molecules into
-            a ``GraphTensor``.
+            a ``GraphTensor``. If None, it is assumed that ``data['x']`` already
+            contains GraphTensor instances in a list: [gt_1, gt_2, ..., gt_n]. 
+            Default to None.
         num_files (int, None):
             The number of TF record files to write to. If None, num_files will
-            be set to ``processes``. Default to None.
-        processes (int, None):
-            The number of worker processes to use. If None, ``multiprocessing.cpu_count()``
-            will be used. Using multiple worker processes significantly speeds up
-            writing of TF records. If ``num_files`` < ``processes``, only ``num_files``
-            processes will be used. Default to None.
+            be set to ``num_processes``. Default to None.
+        num_processes (int, None):
+            The number of worker processes to use. If None, 
+            ``multiprocessing.cpu_count()`` will be used. Using multiple worker 
+            processes significantly speeds up writing of TF records. If 
+            ``num_files`` < ``num_processes``, only ``num_files`` processes 
+            will be used. Default to None.
         device (str):
             The device to use. Default to `/cpu:0`.
 
     Returns:
         ``None``
     '''
-    if processes is None:
-        processes = multiprocessing.cpu_count()
+
+    inputs = kwargs.pop('inputs', None)
+    if inputs is not None:
+        warn(
+            (
+                '`inputs` argument will be depracated in the near future, '
+                ' please use `data` instead.'
+            ),
+            DeprecationWarning,
+            stacklevel=2
+        )
+    
+    assert 'x' in data, ('`data` requires field `x`.')
+
+    os.makedirs(path, exist_ok=True)
+
+    if num_processes is None:
+        num_processes = multiprocessing.cpu_count()
 
     if num_files is None:
-        num_files = processes
+        num_files = num_processes
 
-    chunk_size = math.ceil(len(inputs['x']) / num_files)
+    chunk_size = math.ceil(len(data['x']) / num_files)
 
     spec = {}
-    for key, value in inputs.items():
+    # Obtain spec for each data component, and also chunk the data components.
+    for key, value in data.items():
+
         if key == 'x':
-            graph_tensor_spec = encoder(value[0]).unspecific_spec._data_spec
+            graph_tensor = (
+                value[0] if isinstance(value[0], GraphTensor) else 
+                encoder(value[0])
+            )
+            graph_tensor_spec = graph_tensor.unspecific_spec._data_spec
             graph_tensor_spec.pop('graph_indicator')
             spec[key] = GraphTensorSpec(graph_tensor_spec)
         else:
             spec[key] = tf.type_spec_from_value(value[0])
 
-        inputs[key] = [
+        data[key] = [
             value[i * chunk_size: (i + 1) * chunk_size]
             for i in range(num_files)
         ]
 
-    input_keys = list(inputs.keys())
-    input_chunks = list(inputs.values())
-
-    os.makedirs(path, exist_ok=True)
-
+    # Save specs to json file, in the same folder as the tf records.
     _specs_to_json(spec, os.path.join(path, 'spec.json'))
-
+    
+    # Create different paths for associated with each chunk of data.
     paths = [
         os.path.join(path, f'tfrecord-{i:04d}.tfrecord')
         for i in range(num_files)
     ]
+    
+    # data contain nested chunks: 
+    # {'x': [x_chunk_1, x_chunk_2, ...], 'y': [y_chunk_1, y_chunk_2, ...]}
+    data_keys = data.keys()
+    data_values = data.values()
+    
+    processes = []
+    # Loop chunk-wise:
+    # [path_1, x_chunk_1, y_chunk_1], ..., [path_n, x_chunk_n, y_chunk_n]
+    for path, *values in zip(paths, *data_values):
+
+        # Do not start new processes if 'num_processes' are still alive
+        while len(processes) >= num_processes:
+            for process in processes:
+                if not process.is_alive():
+                    processes.remove(process)
+            else:
+                sleep(0.1)
+                continue
 
-    input_chunks.insert(0, paths)
-    input_chunks = zip(*input_chunks)
-
-    write_tfrecords_to_file_fn = partial(
-        _write_tfrecords_to_file,
-        input_keys=input_keys,
-        encoder=encoder,
-        device=device
-    )
-
-    pool = multiprocessing.Pool(processes)
-
-    for input_chunk in input_chunks:
-
-        #write_tfrecords_to_file_fn(input_chunk)
-
-        _ = pool.apply(write_tfrecords_to_file_fn, (input_chunk,))
-
-    pool.close()
-    pool.join()
+        # Create dictionary to keep track of the different data components:
+        # {'x': x_chunk_i, 'y': y_chunk_i}
+        data_chunk = dict(zip(data_keys, values))
+
+        # Start process. Will write (nested) data chunk to tf records
+        process = multiprocessing.Process(
+            target=_write_tfrecords_to_file,
+            args=(path, data_chunk, encoder, device)
+        )
+        processes.append(process)
+        process.start()
 
+    for process in processes:
+        process.join()
 
 def load(
     path: str,
     extract_tuple: Optional[Union[List[str], Tuple[str]]] = None,
     shuffle_tf_records: bool = False,
 ) -> tf.data.Dataset:
     '''Loads TF records.
@@ -161,44 +199,145 @@
             passed to ``write``). If not None, tuples will be produced.
             Default to None.
         shuffle_tf_records (bool):
             Whether tf record files should be shuffled. Default to False.
             Recommended to be set to True when loading training dataet.
 
     Returns:
-        ``tf.data.Dataset``: A TF dataset ready to be used for modeling (GNNs).
+        ``tf.data.Dataset``: A TF dataset ready to be passed to GNN models.
     '''
     specs = _specs_from_json(os.path.join(path, 'spec.json'))
     filenames = glob(os.path.join(path, '*.tfrecord'))
     filenames = sorted(filenames)
     num_files = len(filenames)
     dataset = tf.data.Dataset.from_tensor_slices(filenames)
     if shuffle_tf_records:
         dataset = dataset.shuffle(num_files)
     dataset = dataset.interleave(
         tf.data.TFRecordDataset, num_parallel_calls=1)
     dataset = dataset.map(
-        partial(_parse_features, specs=specs, extract_tuple=extract_tuple),
-        num_parallel_calls=tf.data.AUTOTUNE)
+        lambda data: _parse_features(
+            data, 
+            specs=specs, 
+            extract_tuple=extract_tuple
+        ),
+        num_parallel_calls=tf.data.AUTOTUNE
+    )
     return dataset
 
 def write_from_dataset(
     path: str,
     dataset: Dataset,
     encoder: MolecularGraphEncoder,
     num_files: Optional[int] = None,
     processes: Optional[int] = None,
     device: str = '/cpu:0'
 ) -> None:
     for key, value in dataset.items():
         path_subset = os.path.join(path, key, '')
         write(path_subset, value, encoder, num_files, processes, device)
 
+def _write_tfrecords_to_file(
+    path: str,
+    data_chunk: Dict[str, Any],
+    encoder: Union[
+        MolecularGraphEncoder, 
+        MolecularGraphEncoder3D, 
+        None
+    ] = None,
+    device: str = '/cpu:0',
+) -> None:
+    # Zip nested data chunks:
+    # {'x': ['C', 'CC', ...], 'y': [1, 2, ...]} -> [('C', 1), ('CC', 2), ...]
+    data_keys = data_chunk.keys()
+    data_values = list(zip(*data_chunk.values()))
+
+    # Write tf records using 'device'
+    with tf.device(device), tf.io.TFRecordWriter(path) as writer:
+
+        # Loop over each tuple in chunk (e.g. each (x, y) pair)
+        for value in data_values:
+            # Create dictionary to keep track of data component:
+            # ('C', 1) -> {'x': 'C', 'y': 1}
+            value = dict(zip(data_keys, value))
+            x = value.pop('x')
+            if not isinstance(x, GraphTensor):
+                graph_tensor = encoder(x)
+                if graph_tensor is None:
+                    # TODO: Raise warning?
+                    continue
+            else:
+                graph_tensor = x
+
+            # Extract graph tensor data components and convert to bytes feature
+            graph_tensor_data = graph_tensor._data.copy()
+            graph_tensor_data.pop('graph_indicator')
+            example = tf.nest.map_structure(
+                lambda x: _to_bytes_feature(x), graph_tensor_data)
+            
+            # Convert remaining data components (non-GraphTensor instances)
+            # to bytes features
+            for k, v in value.items():
+                example[k] = _to_bytes_feature(v)
+
+            # Serialize and write bytes features to tf records.
+            serialized = _serialize_example(example)
+            writer.write(serialized)
+
+def _parse_features(
+    example_proto: tf.Tensor,
+    specs: Dict[str, Union[GraphTensorSpec, tf.TensorSpec]],
+    extract_tuple: Optional[Union[List[str], Tuple[str]]] = None,
+) -> Dict[str, Union[GraphTensor, tf.Tensor]]:
+
+    graph_tensor_spec = specs.pop('x')
+    graph_tensor_spec_data = graph_tensor_spec._data_spec
+    graph_tensor_spec_data = tf.nest.map_structure(
+        lambda spec: tf.RaggedTensorSpec(
+            shape=spec.shape, 
+            dtype=spec.dtype, 
+            ragged_rank=0, 
+            row_splits_dtype=graph_tensor_spec_data['edge_src'].dtype
+        ),
+        graph_tensor_spec_data
+    )
+
+    feature_description = tf.nest.map_structure(
+        lambda _: tf.io.FixedLenFeature([], tf.string), 
+        graph_tensor_spec_data)
+    
+    example = tf.io.parse_single_example(
+        serialized=example_proto, 
+        features=feature_description)
+    
+    graph_tensor_data = tf.nest.map_structure(
+        lambda x, s: tf.io.parse_tensor(x, s.dtype), 
+        example, 
+        graph_tensor_spec_data)
+    
+    graph_tensor = GraphTensor(graph_tensor_data, graph_tensor_spec_data)
+
+    if specs:
+        feature_description = tf.nest.map_structure(
+            lambda _: tf.io.FixedLenFeature([], tf.string), specs)
+        example = tf.io.parse_single_example(example_proto, feature_description)
+        data = tf.nest.map_structure(
+            lambda x, s: tf.ensure_shape(
+                tf.io.parse_tensor(x, s.dtype), s.shape), example, specs)
+        data['x'] = graph_tensor
+    else:
+        data = {'x': graph_tensor}
+
+    if extract_tuple is not None:
+        data = tuple(data[key] for key in extract_tuple if key in data)
+
+    return data
+
 def _serialize_example(feature: Dict[str, tf.train.Feature]) -> bytes:
-    'Converts a dictionary of str:feature pairs to a bytes string.'
+    'Converts a dictionary of (str, feature) pairs to a bytes string.'
     example_proto = tf.train.Example(
         features=tf.train.Features(feature=feature))
     return example_proto.SerializeToString()
 
 def _to_bytes_feature(value: Union[tf.Tensor, np.ndarray]) -> tf.train.Feature:
     'Encodes array as a bytes feature.'
     value = tf.io.serialize_tensor(value)
@@ -234,72 +373,8 @@
         json.dump(specs, out_file)
 
 def _specs_from_json(
     path: str
 ) -> Dict[str, Union[GraphTensorSpec, tf.TensorSpec]]:
     with open(path) as in_file:
         specs = json.load(in_file)
-    return {k: _deserialize_spec(v) for (k, v) in specs.items()}
-
-def _write_tfrecords_to_file(
-    inputs: List[Any],
-    input_keys: List[str],
-    encoder: Union[MolecularGraphEncoder, MolecularGraphEncoder3D],
-    device: str = '/cpu:0',
-) -> None:
-    '''Writes data to a tf record file. This function is called from
-    `write_tfrecords`.
-    '''
-    path, *inps = inputs
-    inps = list(zip(*inps))
-    with tf.device(device), tf.io.TFRecordWriter(path) as writer:
-        for inp in inps:
-            inp = dict(zip(input_keys, inp))
-            x = inp.pop('x')
-            tensor = encoder(x)
-            if tensor is None:
-                continue
-            data = tensor._data.copy()
-            data.pop('graph_indicator')
-            example = tf.nest.map_structure(
-                lambda x: _to_bytes_feature(x), data)
-            for k, v in inp.items():
-                example[k] = _to_bytes_feature(v)
-            serialized = _serialize_example(example)
-            writer.write(serialized)
-    
-    del inputs, input_keys, encoder, device
-
-def _parse_features(
-    example_proto: tf.Tensor,
-    specs: Dict[str, Union[GraphTensorSpec, tf.TensorSpec]],
-    extract_tuple: Optional[Union[List[str], Tuple[str]]] = None,
-) -> Dict[str, Union[GraphTensor, tf.Tensor]]:
-
-    # parse graph tensor
-    x_spec = specs.pop('x')
-
-    feature_description = tf.nest.map_structure(
-        lambda _: tf.io.FixedLenFeature([], tf.string), x_spec._data_spec)
-
-    example = tf.io.parse_single_example(example_proto, feature_description)
-
-    x = tf.nest.map_structure(
-        lambda x, s: tf.io.parse_tensor(x, s.dtype), example, x_spec._data_spec)
-
-    feature_description = tf.nest.map_structure(
-        lambda _: tf.io.FixedLenFeature([], tf.string), specs)
-
-    example = tf.io.parse_single_example(example_proto, feature_description)
-
-    data = tf.nest.map_structure(
-        lambda x, s: tf.ensure_shape(
-            tf.io.parse_tensor(x, s.dtype), s.shape), example, specs)
-
-    x_spec = tf.nest.map_structure(
-        lambda spec: tf.RaggedTensorSpec(
-            spec.shape, spec.dtype, 0, x['edge_src'].dtype),
-        x_spec._data_spec)
-    data['x'] = GraphTensor(x, x_spec)
-    if extract_tuple is not None:
-        data = tuple(data[key] for key in extract_tuple if key in data)
-    return data
+    return {k: _deserialize_spec(v) for (k, v) in specs.items()}
```

### Comparing `molgraph-0.5.6/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.7/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.7/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/encoders.py` & `molgraph-0.5.7/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/features.py` & `molgraph-0.5.7/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.7/molgraph/chemistry/molecular_encoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
     >>> # Merge subgraphs into a single disjoint graph
     >>> graph_tensor.merge()
     GraphTensor(
       edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(6, 119), dtype=float32>,
       edge_feature=<tf.Tensor: shape=(8, 4), dtype=float32>,
-      positional_encoding=<tf.Tensor: shape=(6, 10), dtype=float32>,
+      node_position=<tf.Tensor: shape=(6, 10), dtype=float32>,
       graph_indicator=<tf.Tensor: shape=(6,), dtype=int32>)
 
     Generate a molecular graph with tokenizers:
 
     >>> # Define bond featurizer (to produce numerical encoding of atoms)
     >>> atom_tokenizer = molgraph.chemistry.Tokenizer([
     ...     molgraph.chemistry.features.Symbol(),
@@ -176,15 +176,15 @@
     >>> # Merge subgraphs into a single disjoint graph
     >>> graph_tensor.merge()
     GraphTensor(
       edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(6,), dtype=string>,
       edge_feature=<tf.Tensor: shape=(8,), dtype=string>,
-      positional_encoding=<tf.Tensor: shape=(6, 10), dtype=float32>,
+      node_position=<tf.Tensor: shape=(6, 10), dtype=float32>,
       graph_indicator=<tf.Tensor: shape=(6,), dtype=int32>)
 
 
     Obtain numerical encodings of atoms (``node_feature``) and bonds
     (``bond_feature``) with the EmbeddingLookup layer. This is only necessary
     when tokenizers are used to compute ``node_feature`` and ``edge_feature``:
 
@@ -226,15 +226,15 @@
     >>> graph_tensor = model(graph_tensor)
     >>> graph_tensor
     GraphTensor(
       edge_src=<tf.Tensor: shape=(8,), dtype=int32>,
       edge_dst=<tf.Tensor: shape=(8,), dtype=int32>,
       node_feature=<tf.Tensor: shape=(6, 16), dtype=float32>,
       edge_feature=<tf.Tensor: shape=(8, 8), dtype=float32>,
-      positional_encoding=<tf.Tensor: shape=(6, 10), dtype=float32>,
+      node_position=<tf.Tensor: shape=(6, 10), dtype=float32>,
       graph_indicator=<tf.Tensor: shape=(6,), dtype=int32>)
     '''
 
     bond_encoder: Optional[Union[
         Featurizer, Tokenizer, Callable]] = None
     molecule_from_string_fn: Callable[[str], Chem.Mol] = field(
         default_factory=lambda: partial(molecule_from_string, catch_errors=True),
@@ -283,15 +283,15 @@
         if self.bond_encoder is not None:
             bonds = _get_bonds(molecule, *sparse_adjacency)
             data['edge_feature'] = self.bond_encoder(
                 bonds, self_loops=self.self_loops)
 
         # Obtain positional encoding of nodes (atoms)
         if self.positional_encoding_dim:
-            data['positional_encoding'] = _compute_positional_encoding(
+            data['node_position'] = _compute_positional_encoding(
                 molecule=molecule,
                 dim=self.positional_encoding_dim,
                 dtype=getattr(self.atom_encoder, 'dtype', 'float32'))
 
         if self.auxiliary_encoders is not None:
             for field, encoder in self.auxiliary_encoders.items():
                 data[field] = encoder(molecule)
```

### Comparing `molgraph-0.5.6/molgraph/chemistry/ops.py` & `molgraph-0.5.7/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/chemistry/vis.py` & `molgraph-0.5.7/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/internal.py` & `molgraph-0.5.7/molgraph/internal.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/__init__.py` & `molgraph-0.5.7/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.7/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.7/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.7/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.7/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.7/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.7/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.7/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.7/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.7/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.7/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.7/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.7/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.7/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/gnn_layer.py` & `molgraph-0.5.7/molgraph/layers/gnn_layer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/gnn_ops.py` & `molgraph-0.5.7/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.7/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.7/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.7/molgraph/layers/positional_encoding/laplacian.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,27 +168,27 @@
         tensor_orig = tensor
         if isinstance(tensor.node_feature, tf.RaggedTensor):
             tensor = tensor.merge()
 
         if not self._built:
             self._build(
                 getattr(tensor, 'node_feature', None),
-                getattr(tensor, 'positional_encoding', None)
+                getattr(tensor, 'node_position', None)
             )
 
         def random_sign_flip(positional_encoding):
             random_vals = tf.random.uniform((self._target_dim,))
             return tf.where(
                 random_vals < 0.5, positional_encoding, -positional_encoding)
 
         if not self._positional_encoding_precomputed:
             positional_encoding = compute_positional_encoding(
                 tensor, self._target_dim)
         else:
-            positional_encoding = tensor.positional_encoding
+            positional_encoding = tensor.node_position
 
         if training:
             positional_encoding = random_sign_flip(positional_encoding)
         node_feature = tensor.node_feature + self.projection(positional_encoding)
         return tensor_orig.update({'node_feature': node_feature})
 
     @classmethod
```

### Comparing `molgraph-0.5.6/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.7/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.7/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.7/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.7/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.7/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.7/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.7/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.7/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.7/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/losses/link_losses.py` & `molgraph-0.5.7/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/losses/masked_losses.py` & `molgraph-0.5.7/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.7/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.7/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/__init__.py` & `molgraph-0.5.7/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/dgin.py` & `molgraph-0.5.7/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/dmpnn.py` & `molgraph-0.5.7/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.7/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.7/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/mpnn.py` & `molgraph-0.5.7/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.7/molgraph/models/pretraining/autoencoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.7/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.7/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.7/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.7/molgraph/tensors/graph_tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import tensorflow as tf
 
 from tensorflow.python.framework import composite_tensor
 from tensorflow.python.framework import type_spec
 
 import numpy as np
 
+from warnings import warn
+
 from typing import Optional
 from typing import Mapping
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Any
 from typing import Type
@@ -666,14 +668,19 @@
         return self._data.get('edge_weight', None) 
     
     @property
     def graph_indicator(self):
         'Obtain `graph_indicator` from graph tensor instance.'
         return self._data.get('graph_indicator', None) 
     
+    @property
+    def node_position(self):
+        'Obtain `node_position` from graph tensor instance.'
+        return self._data.get('node_position', None)
+    
     def __getattr__(self, name: str) -> Union[tf.Tensor, tf.RaggedTensor, Any]:
         '''Access nested data as attributes.
 
         Only called when attribute lookup has not found attribute `name` in
         the usual places. Hence convenient when new data has been added to
         the graph tensor and we want to access this data as an attribute.
 
@@ -684,14 +691,25 @@
         Returns:
             If ``name`` in nested data, data is returned. Otherwise,
             attribute ``name`` of the graph tensor instance is returned.
         
         Raises:
             AttributeError: if `name` does not exist in data.
         '''
+        if name == 'positional_encoding':
+            warn(
+                (
+                    '`positional_encoding` will be depracated in the '
+                    'near future, please use `node_position` instead.'
+                ),
+                DeprecationWarning,
+                stacklevel=2
+            )
+            name = 'node_position'
+
         if name in object.__getattribute__(self, '_data'):
             return self._data[name]
         
         _raise_attribute_error(self, name)
 
     def __getitem__(
         self,
@@ -711,14 +729,26 @@
         
         Raises:
             KeyError: if `index` (str) does not exist in data spec.
             tf.errors.InvalidArgumentError: if `index` (int, list[int]) is out 
             of range.
         '''
         if isinstance(index, str):
+
+            if index == 'positional_encoding':
+                warn(
+                    (
+                        '`positional_encoding` will be depracated in the '
+                        'near future, please use `node_position` instead.'
+                    ),
+                    DeprecationWarning,
+                    stacklevel=2
+                )
+                index = 'node_position'
+            
             return self._data[index]
         if isinstance(index, slice):
             index = _slice_to_tensor(index, self.num_subgraphs)
         return tf.gather(self, index)
 
     def __iter__(self):
         if not tf.executing_eagerly():
```

### Comparing `molgraph-0.5.6/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.7/molgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.6
+Version: 0.5.7
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MolGraph: Graph Neural Networks for Molecular Machine Learning
 
 *This is an early release; things are still being updated, added and experimented with. Hence, API compatibility may break in the future.*
 
-*Any feedback is welcomed!*
+*Any feedback is welcomed! If there are any issues/suggestions/questions, do not hesitate to bring it up!*
 
 ## Manuscript
 See [pre-print](https://arxiv.org/abs/2208.09944)
 
 ## Documentation
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
```

### Comparing `molgraph-0.5.6/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.7/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.6/setup.py` & `molgraph-0.5.7/setup.py`

 * *Files identical despite different names*

