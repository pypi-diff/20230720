# Comparing `tmp/datumaro-1.4.0rc3.tar.gz` & `tmp/datumaro-1.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.4.0rc3.tar", last modified: Tue Jul 18 06:06:24 2023, max compression
+gzip compressed data, was "datumaro-1.4.0rc4.tar", last modified: Thu Jul 20 08:13:36 2023, max compression
```

## Comparing `datumaro-1.4.0rc3.tar` & `datumaro-1.4.0rc4.tar`

### file list

```diff
@@ -1,367 +1,367 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.355518 datumaro-1.4.0rc3/
--rw-r--r--   0 runner    (1001) docker     (123)   391964 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-18 06:06:24.351518 datumaro-1.4.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:06:24.355518 datumaro-1.4.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.267516 datumaro-1.4.0rc3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.287517 datumaro-1.4.0rc3/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.287517 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.295517 datumaro-1.4.0rc3/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.299517 datumaro-1.4.0rc3/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.299517 datumaro-1.4.0rc3/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/config_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/contexts/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29629 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.307517 datumaro-1.4.0rc3/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.307517 datumaro-1.4.0rc3/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.307517 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.311517 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.315517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28679 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.327518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.327518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.327518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31336 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.343518 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.343518 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.343518 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.351518 datumaro-1.4.0rc3/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/
+-rw-r--r--   0 runner    (1001) docker     (123)   391964 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.632900 datumaro-1.4.0rc4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.636900 datumaro-1.4.0rc4/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.640900 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.644900 datumaro-1.4.0rc4/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.644900 datumaro-1.4.0rc4/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.644900 datumaro-1.4.0rc4/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29711 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25867 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14764 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.648900 datumaro-1.4.0rc4/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.652900 datumaro-1.4.0rc4/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.652900 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.652900 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.656900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17660 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.660900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31405 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.664900 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.668900 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.672900 datumaro-1.4.0rc4/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 08:13:26.000000 datumaro-1.4.0rc4/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 08:13:36.636900 datumaro-1.4.0rc4/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 08:13:36.000000 datumaro-1.4.0rc4/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.4.0rc3/3rd-party.txt` & `datumaro-1.4.0rc4/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/LICENSE` & `datumaro-1.4.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/PKG-INFO` & `datumaro-1.4.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc3/README.md` & `datumaro-1.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/pyproject.toml` & `datumaro-1.4.0rc4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/requirements-core.txt` & `datumaro-1.4.0rc4/requirements-core.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/setup.py` & `datumaro-1.4.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/capi/pybind.cpp` & `datumaro-1.4.0rc4/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/__main__.py` & `datumaro-1.4.0rc4/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/compare.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/convert.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/download.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/explain.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/explore.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/explore.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/filter.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/generate.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/info.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/merge.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/patch.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/prune.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/stats.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/transform.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/commands/validate.py` & `datumaro-1.4.0rc4/src/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/contexts/model.py` & `datumaro-1.4.0rc4/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/contexts/source.py` & `datumaro-1.4.0rc4/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/contexts/util.py` & `datumaro-1.4.0rc4/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/util/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/util/compare.py` & `datumaro-1.4.0rc4/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/cli/util/project.py` & `datumaro-1.4.0rc4/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/abstracts/merger.py` & `datumaro-1.4.0rc4/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.4.0rc4/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.4.0rc4/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.4.0rc4/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/algorithms/rise.py` & `datumaro-1.4.0rc4/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/annotation.py` & `datumaro-1.4.0rc4/src/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/annotations/matcher.py` & `datumaro-1.4.0rc4/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/annotations/merger.py` & `datumaro-1.4.0rc4/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/cli_plugin.py` & `datumaro-1.4.0rc4/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/comparator.py` & `datumaro-1.4.0rc4/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/config.py` & `datumaro-1.4.0rc4/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/config_model.py` & `datumaro-1.4.0rc4/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/contexts/importer.py` & `datumaro-1.4.0rc4/src/datumaro/components/contexts/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/crypter.py` & `datumaro-1.4.0rc4/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/dataset.py` & `datumaro-1.4.0rc4/src/datumaro/components/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -583,14 +583,15 @@
         has_ctx_args = progress_reporter is not None or error_policy is not None
 
         if not progress_reporter:
             progress_reporter = NullProgressReporter()
 
         assert "ctx" not in kwargs
         exporter_kwargs = copy(kwargs)
+        exporter_kwargs["stream"] = self._stream
         exporter_kwargs["ctx"] = ExportContext(
             progress_reporter=progress_reporter, error_policy=error_policy
         )
 
         try:
             if not inplace:
                 try:
@@ -628,15 +629,16 @@
                     exporter_kwargs.pop("ctx")
 
                     exporter.patch(self, self.get_patch(), save_dir=save_dir, **exporter_kwargs)
         except _ExportFail as e:
             raise e.__cause__
 
         self.bind(save_dir, format, options=copy(kwargs))
-        self.flush_changes()
+        if not self._stream:
+            self.flush_changes()
 
     def save(self, save_dir: Optional[str] = None, **kwargs) -> None:
         options = dict(self._options)
         options.update(kwargs)
 
         self.export(save_dir or self._source_path, format=self._format, **options)
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/dataset_base.py` & `datumaro-1.4.0rc4/src/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.4.0rc4/src/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/dataset_storage.py` & `datumaro-1.4.0rc4/src/datumaro/components/dataset_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,17 +608,17 @@
         source: IDataset,
         infos: Optional[DatasetInfo] = None,
         categories: Optional[CategoriesInfo] = None,
         media_type: Optional[Type[MediaElement]] = None,
     ):
         if not source.is_stream:
             raise ValueError("source should be a stream.")
-        super().__init__(source, infos, categories, media_type)
-        self._subset_names = None
+        self._subset_names = list(source.subsets().keys())
         self._transform_ids_for_latest_subset_names = []
+        super().__init__(source, infos, categories, media_type)
 
     def is_cache_initialized(self) -> bool:
         log.debug("This function has no effect on streaming.")
         return True
 
     def init_cache(self) -> None:
         log.debug("This function has no effect on streaming.")
@@ -656,20 +656,17 @@
         raise NotAvailableError("Drop-in removal is not allowed in streaming.")
 
     def get_subset(self, name: str) -> IDataset:
         return self.subsets()[name]
 
     @property
     def subset_names(self):
-        if self._subset_names is None:
-            self._subset_names = {item.subset for item in self}
-            self._transforms_for_latest_subset_names = [id(t) for t in self._transforms]
-        elif self._transforms_for_latest_subset_names != [id(t) for t in self._transforms]:
+        if self._transform_ids_for_latest_subset_names != [id(t) for t in self._transforms]:
             self._subset_names = {item.subset for item in self}
-            self._transforms_for_latest_subset_names = [id(t) for t in self._transforms]
+            self._transform_ids_for_latest_subset_names = [id(t) for t in self._transforms]
 
         return self._subset_names
 
     def subsets(self) -> Dict[str, IDataset]:
         return {subset: StreamSubset(self, subset) for subset in self.subset_names}
 
     def transform(self, method: Type[Transform], *args, **kwargs) -> None:
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/environment.py` & `datumaro-1.4.0rc4/src/datumaro/components/environment.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/errors.py` & `datumaro-1.4.0rc4/src/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/components/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,15 @@
         *,
         save_images=None,  # Deprecated
         save_media: Optional[bool] = None,
         image_ext: Optional[str] = None,
         default_image_ext: Optional[str] = None,
         save_dataset_meta: bool = False,
         save_hashkey_meta: bool = False,
+        stream: bool = False,
         ctx: Optional[ExportContext] = None,
     ):
         default_image_ext = default_image_ext or self.DEFAULT_IMAGE_EXT
         assert default_image_ext
         self._default_image_ext = default_image_ext
 
         if save_images is not None and save_media is not None:
@@ -218,14 +219,20 @@
         from datumaro.components.dataset import DatasetPatch
 
         if isinstance(extractor, DatasetPatch.DatasetPatchWrapper):
             self._patch = extractor.patch
         else:
             self._patch = None
 
+        if stream and not self.can_stream:
+            raise DatasetExportError(
+                f"{self.__class__.__name__} cannot export a dataset in a stream manner"
+            )
+        self._stream = stream
+
         self._ctx: ExportContext = ctx or NullExportContext()
 
     def _find_image_ext(self, item: Union[DatasetItem, Image]):
         src_ext = None
 
         if isinstance(item, DatasetItem) and isinstance(item.media, Image):
             src_ext = item.media.ext
@@ -295,14 +302,19 @@
         if self._save_hashkey_meta:
             return
         for annotation in item.annotations:
             if isinstance(annotation, HashKey):
                 self._save_hashkey_meta = True
                 return
 
+    @property
+    def can_stream(self) -> bool:
+        """Flag to indicate whether the exporter can export the dataset in a stream manner or not."""
+        return False
+
 
 # TODO: Currently, ExportContextComponent is introduced only for Datumaro and DatumaroBinary format
 # for multi-processing. We need to propagate this to everywhere in Datumaro 1.2.0
 
 
 class ExportContextComponent:
     def __init__(
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/extractor_tfds.py` & `datumaro-1.4.0rc4/src/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/filter.py` & `datumaro-1.4.0rc4/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/format_detection.py` & `datumaro-1.4.0rc4/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/generator.py` & `datumaro-1.4.0rc4/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/importer.py` & `datumaro-1.4.0rc4/src/datumaro/components/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/launcher.py` & `datumaro-1.4.0rc4/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/lazy_plugin.py` & `datumaro-1.4.0rc4/src/datumaro/components/lazy_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/media.py` & `datumaro-1.4.0rc4/src/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/media_manager.py` & `datumaro-1.4.0rc4/src/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/merge/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/merge/base.py` & `datumaro-1.4.0rc4/src/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.4.0rc4/src/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/merge/extractor_merger.py` & `datumaro-1.4.0rc4/src/datumaro/components/merge/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.4.0rc4/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/merge/union_merge.py` & `datumaro-1.4.0rc4/src/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/operations.py` & `datumaro-1.4.0rc4/src/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/progress_reporting.py` & `datumaro-1.4.0rc4/src/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/project.py` & `datumaro-1.4.0rc4/src/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/shift_analyzer.py` & `datumaro-1.4.0rc4/src/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/transformer.py` & `datumaro-1.4.0rc4/src/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/validator.py` & `datumaro-1.4.0rc4/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/components/visualizer.py` & `datumaro-1.4.0rc4/src/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,17 +54,21 @@
         export_context: ExportContextComponent,
         subset: str,
         ctx: ExportContext,
         max_chunk_size: int = 1000,
         num_shards: int = 1,
         max_shard_size: Optional[int] = None,
     ):
-        super().__init__(context, "", export_context)
+        super().__init__(
+            context=context,
+            subset=subset,
+            ann_file="",
+            export_context=export_context,
+        )
         self._schema = deepcopy(DatumaroArrow.SCHEMA)
-        self._subset = subset
         self._writers = []
         self._fnames = []
         self._max_chunk_size = max_chunk_size
         self._num_shards = num_shards
         self._max_shard_size = max_shard_size
         self._ctx = ctx
 
@@ -366,14 +370,15 @@
         default_image_ext: Optional[str] = None,
         save_dataset_meta: bool = False,
         ctx: Optional[ExportContext] = None,
         num_workers: int = 0,
         num_shards: int = 1,
         max_shard_size: Optional[int] = None,
         max_chunk_size: int = 1000,
+        **kwargs,
     ):
         super().__init__(
             extractor=extractor,
             save_dir=save_dir,
             save_images=save_images,
             save_media=save_media,
             image_ext=image_ext,
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # Copyright (C) 2020-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import json
 import logging as log
 import os
 import os.path as osp
+from dataclasses import dataclass
 from enum import Enum, auto
+from io import BufferedWriter
 from itertools import chain, groupby
-from typing import List, Union
+from typing import Dict, List, Optional, Type, Union
 
 import pycocotools.mask as mask_utils
+from json_stream.writer import streamable_dict, streamable_list
 
 import datumaro.util.annotation_util as anno_tools
 import datumaro.util.mask_tools as mask_tools
 from datumaro.components.annotation import (
     COORDINATE_ROUNDING_DIGITS,
     AnnotationType,
     Ellipse,
@@ -21,69 +25,190 @@
     Polygon,
 )
 from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
-from datumaro.util import cast, dump_json_file, find, str_to_bool
+from datumaro.util import cast, dump_json, dump_json_file, find, parse_json, str_to_bool
 from datumaro.util.image import save_image
 
 from .format import CocoPath, CocoTask
 
 
 class SegmentationMode(Enum):
     guess = auto()
     polygons = auto()
     mask = auto()
 
 
+@dataclass
+class _Writer:
+    fp: BufferedWriter
+    is_empty: bool
+
+
+class TemporaryWriters:
+    def __init__(self, subset: str, task: CocoTask, ann_dir: str):
+        self._subset = subset
+        self._task = task
+        self._ann_dir = ann_dir
+        self._writers = tuple()
+        self.reset()
+
+    def close(self):
+        for writer in self._writers:
+            if not writer.fp.closed:
+                writer.fp.close()
+
+    def remove(self):
+        self.close()
+
+        for writer in self._writers:
+            fpath = writer.fp.name
+            if osp.exists(fpath):
+                os.remove(fpath)
+
+    def reset(self):
+        self.remove()
+
+        self._writers = tuple(
+            _Writer(
+                fp=open(
+                    osp.join(self._ann_dir, f"__{self._task.name}_{self._subset}_{key}.tmp"), "wb"
+                ),
+                is_empty=True,
+            )
+            for key in ["imgs", "anns"]
+        )
+
+    def __del__(self):
+        self.remove()
+
+    @property
+    def imgs(self) -> _Writer:
+        return self._writers[0]
+
+    @property
+    def anns(self) -> _Writer:
+        return self._writers[1]
+
+    def add_item(self, data: Dict) -> None:
+        self.imgs.is_empty = False
+        writer = self.imgs.fp
+        writer.write(dump_json(data, append_newline=True))
+
+    def add_anns(self, data: Dict) -> None:
+        self.anns.is_empty = False
+        writer = self.anns.fp
+        writer.write(dump_json(data, append_newline=True))
+
+    def merge(self, path: str, header: Dict, min_ann_id: Optional[int]) -> None:
+        self.close()
+
+        @streamable_list
+        def _gen_images():
+            with open(self.imgs.fp.name, "rb") as fp:
+                for line in fp:
+                    yield parse_json(line)
+
+        @streamable_list
+        def _gen_anns():
+            with open(self.anns.fp.name, "rb") as fp:
+                next_id = min_ann_id
+                for line in fp:
+                    ann = parse_json(line)
+                    if min_ann_id is not None and not ann["id"]:
+                        ann["id"] = next_id
+                        next_id += 1
+                    yield ann
+
+        @streamable_dict
+        def _gen():
+            yield "licenses", header["licenses"]
+            yield "info", header["info"]
+            yield "categories", header["categories"]
+
+            if not self.imgs.is_empty:
+                yield "images", _gen_images()
+            else:
+                yield "images", []
+
+            if not self.anns.is_empty:
+                yield "annotations", _gen_anns()
+            else:
+                yield "annotations", []
+
+        with open(path, "w", encoding="utf-8") as fp:
+            json.dump(_gen(), fp)
+
+        self.remove()
+
+
 class _TaskExporter:
-    def __init__(self, context):
+    def __init__(
+        self, context: "CocoExporter", subset: str, task: CocoTask, ann_dir: str, stream: bool
+    ):
         self._min_ann_id = 1
         self._context = context
+        self._subset = subset
+        self._task = task
+        self._ann_dir = ann_dir
+        self._stream = stream
 
         data = {"licenses": [], "info": {}, "categories": [], "images": [], "annotations": []}
 
         data["licenses"].append({"name": "", "id": 0, "url": ""})
 
         data["info"] = {
             "contributor": "",
             "date_created": "",
             "description": "",
             "url": "",
             "version": "",
             "year": "",
         }
         self._data = data
+        self._temporary_writers = TemporaryWriters(
+            subset=subset,
+            task=task,
+            ann_dir=ann_dir,
+        )
 
     def is_empty(self):
-        return len(self._data["annotations"]) == 0
+        return (
+            len(self._data["annotations"]) == 0
+            if not self._stream
+            else self._temporary_writers.anns.is_empty
+        )
 
     def _get_image_id(self, item):
         return self._context._get_image_id(item)
 
     def save_image_info(self, item, filename):
         h = 0
         w = 0
         if item.media and item.media.size:
             h, w = item.media.size
 
-        self._data["images"].append(
-            {
-                "id": self._get_image_id(item),
-                "width": int(w),
-                "height": int(h),
-                "file_name": cast(filename, str, ""),
-                "license": 0,
-                "flickr_url": "",
-                "coco_url": "",
-                "date_captured": 0,
-            }
-        )
+        item_desc = {
+            "id": self._get_image_id(item),
+            "width": int(w),
+            "height": int(h),
+            "file_name": cast(filename, str, ""),
+            "license": 0,
+            "flickr_url": "",
+            "coco_url": "",
+            "date_captured": 0,
+        }
+
+        if not self._stream:
+            self._data["images"].append(item_desc)
+        else:
+            self._temporary_writers.add_item(item_desc)
 
     def save_categories(self, dataset):
         raise NotImplementedError()
 
     def save_annotations(self, item):
         raise NotImplementedError()
 
@@ -92,14 +217,17 @@
         for ann in self.annotations:
             if not ann["id"]:
                 ann["id"] = next_id
                 next_id += 1
 
         dump_json_file(path, self._data)
 
+        if self._stream:
+            self._temporary_writers.merge(path, self._data, self._min_ann_id)
+
     @property
     def annotations(self):
         return self._data["annotations"]
 
     @property
     def infos(self):
         return self._data["info"]
@@ -117,15 +245,19 @@
     @staticmethod
     def _convert_attributes(ann):
         return {k: v for k, v in ann.attributes.items() if k not in {"is_crowd", "score"}}
 
 
 class _ImageInfoExporter(_TaskExporter):
     def is_empty(self):
-        return len(self._data["images"]) == 0
+        return (
+            len(self._data["images"]) == 0
+            if not self._stream
+            else self._temporary_writers.imgs.is_empty
+        )
 
     def save_categories(self, dataset):
         pass
 
     def save_annotations(self, item):
         pass
 
@@ -154,15 +286,18 @@
                         "attribute 'score': %e" % (item.id, ann_idx, e)
                     )
             if self._context._allow_attributes:
                 attrs = self._convert_attributes(ann)
                 if attrs:
                     elem["attributes"] = attrs
 
-            self.annotations.append(elem)
+            if not self._stream:
+                self.annotations.append(elem)
+            else:
+                self._temporary_writers.add_anns(elem)
 
 
 class _InstancesExporter(_TaskExporter):
     _polygon_types = {AnnotationType.polygon, AnnotationType.ellipse}
     _allowed_types = {
         AnnotationType.bbox,
         AnnotationType.polygon,
@@ -288,18 +423,24 @@
         instances = [self.find_instance_parts(i, w, h) for i in instances]
 
         if self._context._crop_covered:
             instances = self.crop_segments(instances, w, h)
 
         for instance in instances:
             elem = self.convert_instance(instance, item)
-            if elem:
+
+            if elem is None:
+                continue
+
+            if not self._stream:
                 self.annotations.append(elem)
+            else:
+                self._temporary_writers.add_anns(elem)
 
-    def convert_instance(self, instance, item):
+    def convert_instance(self, instance, item) -> Optional[Dict]:
         ann, polygons, mask, bbox = instance
 
         is_crowd = mask is not None
         if is_crowd:
             segmentation = {
                 "counts": list(int(c) for c in mask["counts"]),
                 "size": list(int(c) for c in mask["size"]),
@@ -383,15 +524,18 @@
             return
 
         # Create annotations for solitary keypoints annotations
         for points in self.find_solitary_points(item.annotations):
             instance = [points, [], None, points.get_bbox()]
             elem = super().convert_instance(instance, item)
             elem.update(self.convert_points_object(points))
-            self.annotations.append(elem)
+            if not self._stream:
+                self.annotations.append(elem)
+            else:
+                self._temporary_writers.add_anns(elem)
 
         # Create annotations for complete instance + keypoints annotations
         super().save_annotations(item)
 
     @classmethod
     def find_solitary_points(cls, annotations):
         annotations = sorted(annotations, key=lambda a: a.group)
@@ -417,15 +561,15 @@
         num_annotated = len([v for v in visibility if v != Points.Visibility.absent])
 
         return {
             "keypoints": keypoints,
             "num_keypoints": num_annotated,
         }
 
-    def convert_instance(self, instance, item):
+    def convert_instance(self, instance, item) -> Optional[Dict]:
         points_ann = find(
             item.annotations,
             lambda x: x.type == AnnotationType.points
             and instance[0].group
             and x.group == instance[0].group,
         )
         if not points_ann:
@@ -470,25 +614,31 @@
                         "Item '%s': failed to convert attribute " "'score': %e" % (item.id, e)
                     )
             if self._context._allow_attributes:
                 attrs = self._convert_attributes(ann)
                 if attrs:
                     elem["attributes"] = attrs
 
-            self.annotations.append(elem)
+            if not self._stream:
+                self.annotations.append(elem)
+            else:
+                self._temporary_writers.add_anns(elem)
 
 
 class _StuffExporter(_InstancesExporter):
     pass
 
 
 class _PanopticExporter(_TaskExporter):
     def write(self, path):
         dump_json_file(path, self._data)
 
+        if self._stream:
+            self._temporary_writers.merge(path, self._data, None)
+
     def save_categories(self, dataset):
         label_categories = dataset.categories().get(AnnotationType.label)
         if label_categories is None:
             return
 
         for idx, cat in enumerate(label_categories.items):
             self.categories.append(
@@ -537,15 +687,19 @@
         )
 
         elem = {
             "image_id": self._get_image_id(item),
             "file_name": ann_filename,
             "segments_info": segments_info,
         }
-        self.annotations.append(elem)
+
+        if not self._stream:
+            self.annotations.append(elem)
+        else:
+            self._temporary_writers.add_anns(elem)
 
 
 class CocoExporter(Exporter):
     @staticmethod
     def _split_tasks_string(s):
         return [CocoTask[i.strip()] for i in s.split(",")]
 
@@ -617,15 +771,15 @@
             help="COCO task filter, comma-separated list of {%s} "
             "(default: all)" % ", ".join(t.name for t in CocoTask),
         )
         return parser
 
     DEFAULT_IMAGE_EXT = CocoPath.IMAGE_EXT
 
-    _TASK_CONVERTER = {
+    _TASK_CONVERTER: Dict[CocoTask, Type[_TaskExporter]] = {
         CocoTask.image_info: _ImageInfoExporter,
         CocoTask.instances: _InstancesExporter,
         CocoTask.person_keypoints: _KeypointsExporter,
         CocoTask.captions: _CaptionsExporter,
         CocoTask.labels: _LabelsExporter,
         CocoTask.panoptic: _PanopticExporter,
         CocoTask.stuff: _StuffExporter,
@@ -637,17 +791,18 @@
         save_dir,
         tasks=None,
         segmentation_mode=None,
         crop_covered=False,
         allow_attributes=True,
         reindex=False,
         merge_images=False,
+        stream: bool = False,
         **kwargs,
     ):
-        super().__init__(extractor, save_dir, **kwargs)
+        super().__init__(extractor, save_dir, stream=stream, **kwargs)
 
         assert tasks is None or isinstance(tasks, (CocoTask, list, str))
         if isinstance(tasks, CocoTask):
             tasks = [tasks]
         elif isinstance(tasks, str):
             tasks = [CocoTask[tasks]]
         elif tasks:
@@ -689,22 +844,29 @@
 
     def _make_segmentation_dir(self, subset_name):
         self._segmentation_dir = osp.join(
             self._save_dir, CocoPath.ANNOTATIONS_DIR, "panoptic_" + subset_name
         )
         os.makedirs(self._segmentation_dir, exist_ok=True)
 
-    def _make_task_converter(self, task):
+    def _make_task_converter(self, task: CocoTask, subset: str) -> _TaskExporter:
         if task not in self._TASK_CONVERTER:
             raise NotImplementedError()
-        return self._TASK_CONVERTER[task](self)
+        return self._TASK_CONVERTER[task](
+            context=self,
+            subset=subset,
+            task=task,
+            ann_dir=self._ann_dir,
+            stream=self._stream,
+        )
 
-    def _make_task_converters(self):
+    def _make_task_converters(self, subset: str):
         return {
-            task: self._make_task_converter(task) for task in (self._tasks or self._TASK_CONVERTER)
+            task: self._make_task_converter(task, subset)
+            for task in (self._tasks or self._TASK_CONVERTER)
         }
 
     def _get_image_id(self, item):
         image_id = self._image_ids.get(item.id)
         if image_id is None:
             if not self._reindex:
                 image_id = cast(item.attributes.get("id"), int, len(self._image_ids) + 1)
@@ -721,15 +883,15 @@
 
         if self._save_dataset_meta:
             self._save_meta_file(self._save_dir)
 
         subsets = self._extractor.subsets()
         pbars = self._ctx.progress_reporter.split(len(subsets))
         for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
-            task_converters = self._make_task_converters()
+            task_converters = self._make_task_converters(subset_name)
             for task_conv in task_converters.values():
                 task_conv.save_categories(subset)
             if CocoTask.panoptic in task_converters:
                 self._make_segmentation_dir(subset_name)
 
             for item in pbar.iter(subset, desc=f"Exporting '{subset_name}'"):
                 try:
@@ -791,14 +953,18 @@
             if osp.isfile(image_path):
                 os.unlink(image_path)
 
             image_path = osp.join(images_dir, subset, conv._make_image_filename(item))
             if osp.isfile(image_path):
                 os.unlink(image_path)
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
 
 class CocoInstancesExporter(CocoExporter):
     def __init__(self, *args, **kwargs):
         kwargs["tasks"] = CocoTask.instances
         super().__init__(*args, **kwargs)
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/extractor_merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/coco/page_mapper.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # pylint: disable=no-self-use
 
+import json
 import os
 import os.path as osp
 import shutil
 from contextlib import contextmanager
 from multiprocessing.pool import Pool
-from typing import Optional
+from typing import Dict, Optional
 
 import numpy as np
 import pycocotools.mask as mask_utils
+from json_stream.writer import streamable_dict, streamable_list
 
 from datumaro.components.annotation import (
     Annotation,
     Bbox,
     Caption,
     Cuboid3d,
     Ellipse,
@@ -39,16 +41,23 @@
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util import cast, dump_json_file
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 
 class _SubsetWriter:
-    def __init__(self, context: Exporter, ann_file: str, export_context: ExportContextComponent):
+    def __init__(
+        self,
+        context: Exporter,
+        subset: str,
+        ann_file: str,
+        export_context: ExportContextComponent,
+    ):
         self._context = context
+        self._subset = subset
 
         self._data = {
             "dm_format_version": DATUMARO_FORMAT_VERSION,
             "media_type": context._extractor.media_type()._type,
             "infos": {},
             "categories": {},
             "items": [],
@@ -118,15 +127,18 @@
                 item.media = PointCloud.from_file(path=pcd_fname, extra_images=extra_images)
 
             yield
             item.media = pcd
         else:
             raise NotImplementedError
 
-    def add_item(self, item: DatasetItem, *args, **kwargs):
+    def add_item(self, item: DatasetItem, *args, **kwargs) -> None:
+        self.items.append(self._gen_item_desc(item))
+
+    def _gen_item_desc(self, item: DatasetItem, *args, **kwargs) -> Dict:
         annotations = []
         item_desc = {
             "id": item.id,
             "annotations": annotations,
         }
 
         if item.attributes:
@@ -151,16 +163,14 @@
                 ]
 
                 if related_images:
                     item_desc["related_images"] = related_images
             elif isinstance(item.media, MediaElement):
                 item_desc["media"] = {"path": getattr(item.media, "path", None)}
 
-        self.items.append(item_desc)
-
         for ann in item.annotations:
             if isinstance(ann, Label):
                 converted_ann = self._convert_label_object(ann)
             elif isinstance(ann, Mask):
                 converted_ann = self._convert_mask_object(ann)
             elif isinstance(ann, Points):
                 converted_ann = self._convert_points_object(ann)
@@ -178,14 +188,16 @@
                 converted_ann = self._convert_ellipse_object(ann)
             elif isinstance(ann, HashKey):
                 continue
             else:
                 raise NotImplementedError()
             annotations.append(converted_ann)
 
+        return item_desc
+
     def add_infos(self, infos):
         self._data["infos"].update(infos)
 
     def add_categories(self, categories):
         for ann_type, desc in categories.items():
             if isinstance(desc, LabelCategories):
                 converted_desc = self._convert_label_categories(desc)
@@ -363,14 +375,48 @@
                     "labels": [cast(label, str) for label in item.labels],
                     "joints": [list(map(int, j)) for j in item.joints],
                 }
             )
         return converted
 
 
+class _StreamSubsetWriter(_SubsetWriter):
+    def __init__(
+        self,
+        context: Exporter,
+        subset: str,
+        ann_file: str,
+        export_context: ExportContextComponent,
+    ):
+        super().__init__(context, subset, ann_file, export_context)
+
+    def write(self, *args, **kwargs):
+        @streamable_list
+        def _item_list():
+            subset = self._context._extractor.get_subset(self._subset)
+            pbar = self._context._ctx.progress_reporter
+            for item in pbar.iter(subset, desc=f"Exporting '{self._subset}'"):
+                yield self._gen_item_desc(item)
+
+        @streamable_dict
+        def _data():
+            yield "dm_format_version", self._data["dm_format_version"]
+            yield "media_type", self._data["media_type"]
+            yield "infos", self._data["infos"]
+            yield "categories", self._data["categories"]
+            yield "items", _item_list()
+
+        with open(self.ann_file, "w", encoding="utf-8") as fp:
+            json.dump(_data(), fp)
+
+    def is_empty(self):
+        # TODO: Force empty to be False, but it should be fixed with refactoring `_SubsetWriter`.`
+        return False
+
+
 class DatumaroExporter(Exporter):
     DEFAULT_IMAGE_EXT = DatumaroPath.IMAGE_EXT
     PATH_CLS = DatumaroPath
 
     def create_writer(
         self,
         subset: str,
@@ -383,18 +429,28 @@
             images_dir=images_dir,
             pcd_dir=pcd_dir,
             crypter=NULL_CRYPTER,
             image_ext=self._image_ext,
             default_image_ext=self._default_image_ext,
         )
 
-        return _SubsetWriter(
-            context=self,
-            ann_file=osp.join(self._annotations_dir, subset + self.PATH_CLS.ANNOTATION_EXT),
-            export_context=export_context,
+        return (
+            _SubsetWriter(
+                context=self,
+                subset=subset,
+                ann_file=osp.join(self._annotations_dir, subset + self.PATH_CLS.ANNOTATION_EXT),
+                export_context=export_context,
+            )
+            if not self._stream
+            else _StreamSubsetWriter(
+                context=self,
+                subset=subset,
+                ann_file=osp.join(self._annotations_dir, subset + self.PATH_CLS.ANNOTATION_EXT),
+                export_context=export_context,
+            )
         )
 
     def _apply_impl(self, pool: Optional[Pool] = None, *args, **kwargs):
         os.makedirs(self._save_dir, exist_ok=True)
 
         images_dir = osp.join(self._save_dir, self.PATH_CLS.IMAGES_DIR)
         os.makedirs(images_dir, exist_ok=True)
@@ -417,18 +473,17 @@
 
         for writer in writers.values():
             writer.add_infos(self._extractor.infos())
             writer.add_categories(self._extractor.categories())
 
         pbar = self._ctx.progress_reporter
         for subset_name, subset in self._extractor.subsets().items():
-            for item in pbar.iter(subset, desc=f"Exporting '{subset_name}'"):
-                writers[subset_name].add_item(item, pool)
-
-                self._check_hash_key_existence(item)
+            if not self._stream:
+                for item in pbar.iter(subset, desc=f"Exporting '{subset_name}'"):
+                    writers[subset_name].add_item(item, pool)
 
         for subset, writer in writers.items():
             if self._patch and subset in self._patch.updated_subsets and writer.is_empty():
                 if osp.isfile(writer.ann_file):
                     # Remove subsets that became empty
                     os.remove(writer.ann_file)
                 continue
@@ -466,7 +521,11 @@
             )
             if osp.isfile(pcd_path):
                 os.unlink(pcd_path)
 
             related_images_path = osp.join(save_dir, cls.PATH_CLS.IMAGES_DIR, item.subset, item.id)
             if osp.isdir(related_images_path):
                 shutil.rmtree(related_images_path)
+
+    @property
+    def can_stream(self) -> bool:
+        return True
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,22 @@
 
 class _SubsetWriter(__SubsetWriter):
     """"""
 
     def __init__(
         self,
         context: Exporter,
+        subset: str,
         ann_file: str,
         export_context: ExportContextComponent,
         secret_key_file: str,
         no_media_encryption: bool = False,
         max_blob_size: int = DatumaroBinaryPath.MAX_BLOB_SIZE,
     ):
-        super().__init__(context, ann_file, export_context)
+        super().__init__(context, subset, ann_file, export_context)
         self._crypter = self.export_context.crypter
         self.secret_key_file = secret_key_file
 
         self._fp: Optional[BufferedWriter] = None
         self._data["items"]: List[Union[bytes, ApplyResult]] = []
         self._bytes: List[Union[bytes, ApplyResult]] = self._data["items"]
         self._item_cnt = 0
@@ -244,14 +245,15 @@
         save_dataset_meta: bool = False,
         ctx: Optional[ExportContext] = None,
         encryption_key: Optional[bytes] = None,
         no_media_encryption: bool = False,
         encryption: bool = False,
         num_workers: int = 0,
         max_blob_size: int = DatumaroBinaryPath.MAX_BLOB_SIZE,
+        **kwargs,
     ):
         """
         Parameters
         ----------
         encryption_key
             If provided, the dataset is encrypted with this key for export.
         no_media_encryption
@@ -304,14 +306,15 @@
             crypter=self._crypter,
             image_ext=self._image_ext,
             default_image_ext=self._default_image_ext,
         )
 
         return _SubsetWriter(
             context=self,
+            subset=subset,
             ann_file=osp.join(self._annotations_dir, subset + self.PATH_CLS.ANNOTATION_EXT),
             export_context=export_context,
             secret_key_file=osp.join(self._save_dir, self.PATH_CLS.SECRET_KEY_FILE),
             no_media_encryption=self._no_media_encryption,
             max_blob_size=self._max_blob_size,
         )
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -791,14 +791,18 @@
                 if osp.isfile(path):
                     os.unlink(path)
 
                 path = osp.join(save_dir, VocPath.INSTANCES_DIR, item.id + VocPath.SEGM_EXT)
                 if osp.isfile(path):
                     os.unlink(path)
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
 
 class VocClassificationExporter(VocExporter):
     def __init__(self, *args, **kwargs):
         kwargs["task"] = VocTask.voc_classification
         super().__init__(*args, **kwargs)
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,18 @@
             if osp.isfile(image_path):
                 os.remove(image_path)
 
             ann_path = osp.join(subset_dir, "%s.txt" % item.id)
             if osp.isfile(ann_path):
                 os.remove(ann_path)
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
 
 class YoloUltralyticsExporter(YoloExporter):
     allowed_subset_names = {"train", "val", "test"}
     must_subset_names = {"train", "val"}
 
     def __init__(self, extractor: IDataset, save_dir: str, **kwargs) -> None:
         super().__init__(extractor, save_dir, **kwargs)
```

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/explorer.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/ndr.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/specs.json` & `datumaro-1.4.0rc4/src/datumaro/plugins/specs.json`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/specs.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/splitter.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/tiling/util.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/transforms.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/plugins/validators.py` & `datumaro-1.4.0rc4/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/__init__.py` & `datumaro-1.4.0rc4/src/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/annotation_util.py` & `datumaro-1.4.0rc4/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/attrs_util.py` & `datumaro-1.4.0rc4/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/definitions.py` & `datumaro-1.4.0rc4/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/file_utils.py` & `datumaro-1.4.0rc4/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/image.py` & `datumaro-1.4.0rc4/src/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/image_cache.py` & `datumaro-1.4.0rc4/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/log_utils.py` & `datumaro-1.4.0rc4/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/mask_tools.py` & `datumaro-1.4.0rc4/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/meta_file_util.py` & `datumaro-1.4.0rc4/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/os_util.py` & `datumaro-1.4.0rc4/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/pickle_util.py` & `datumaro-1.4.0rc4/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/scope.py` & `datumaro-1.4.0rc4/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/telemetry_stub.py` & `datumaro-1.4.0rc4/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/telemetry_utils.py` & `datumaro-1.4.0rc4/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro/util/tf_util.py` & `datumaro-1.4.0rc4/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.4.0rc4/src/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc3
+Version: 1.4.0rc4
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc3/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.4.0rc4/src/datumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc3/src/datumaro.egg-info/requires.txt` & `datumaro-1.4.0rc4/src/datumaro.egg-info/requires.txt`

 * *Files identical despite different names*

