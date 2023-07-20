# Comparing `tmp/dstk_x250-3.8.8.tar.gz` & `tmp/dstk_x250-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dstk_x250-3.8.8.tar", last modified: Tue Nov  8 14:08:28 2022, max compression
+gzip compressed data, was "dstk_x250-3.8.9.tar", last modified: Tue Nov  8 14:52:59 2022, max compression
```

## Comparing `dstk_x250-3.8.8.tar` & `dstk_x250-3.8.9.tar`

### file list

```diff
@@ -1,545 +1,545 @@
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11349 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/LICENSE.txt
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       22 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/MANIFEST.in
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2276 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/PKG-INFO
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1910 2021-09-21 21:14:24.000000 dstk_x250-3.8.8/README.md
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/dstk/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       95 2022-11-08 14:06:13.000000 dstk_x250-3.8.8/dstk/__init__.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/dstk/data/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      259 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/data/__init__.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    13027 2022-06-16 09:32:59.000000 dstk_x250-3.8.8/dstk/data/_pandas_sql.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     5005 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/data/_sql.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/dstk/features/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      414 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/features/__init__.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    13878 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/features/_prepro.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     6300 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/features/_transformers.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/dstk/metrics/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      490 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/metrics/__init__.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     5618 2021-10-21 17:29:44.000000 dstk_x250-3.8.8/dstk/metrics/_aggregator.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    37526 2021-10-21 17:40:40.000000 dstk_x250-3.8.8/dstk/metrics/_handlers.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    15442 2021-10-21 17:38:13.000000 dstk_x250-3.8.8/dstk/metrics/_metrics.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)      564 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/metrics/push.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/dstk/ml/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      137 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/ml/__init__.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    10822 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/ml/_ml.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.051769 dstk_x250-3.8.8/dstk/pytorch/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2555 2022-11-04 12:30:57.000000 dstk_x250-3.8.8/dstk/pytorch/__init__.py
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    38171 2022-11-08 14:03:30.000000 dstk_x250-3.8.8/dstk/pytorch/_base.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    44986 2022-11-04 12:30:02.000000 dstk_x250-3.8.8/dstk/pytorch/_callback.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13592 2022-11-04 12:19:02.000000 dstk_x250-3.8.8/dstk/pytorch/_classifier.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    23175 2022-06-03 09:13:26.000000 dstk_x250-3.8.8/dstk/pytorch/_random_search.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9890 2022-11-04 12:18:25.000000 dstk_x250-3.8.8/dstk/pytorch/_regressor.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    30757 2021-10-17 11:15:04.000000 dstk_x250-3.8.8/dstk/pytorch/_swa.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    16475 2022-11-04 10:50:23.000000 dstk_x250-3.8.8/dstk/pytorch/_utils.py
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11593 2022-11-08 14:02:31.000000 dstk_x250-3.8.8/dstk/pytorch/_utils_distrib.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19254 2022-07-28 12:16:12.000000 dstk_x250-3.8.8/dstk/pytorch/metrics.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    16309 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/pytorch/networks.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11062 2022-10-23 13:04:55.000000 dstk_x250-3.8.8/dstk/pytorch/supervision.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.051769 dstk_x250-3.8.8/dstk/ssh/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      162 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/ssh/__init__.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19382 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/ssh/_ssh.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     2691 2021-09-20 08:41:05.000000 dstk_x250-3.8.8/dstk/ssh/_utils.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.051769 dstk_x250-3.8.8/dstk/utils/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      847 2022-05-30 13:03:05.000000 dstk_x250-3.8.8/dstk/utils/__init__.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     4573 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/_check.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     4500 2021-10-21 17:45:00.000000 dstk_x250-3.8.8/dstk/utils/_chunk.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     3630 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/_date.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     6364 2022-06-19 20:30:55.000000 dstk_x250-3.8.8/dstk/utils/_rolling.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1008 2022-06-08 07:27:32.000000 dstk_x250-3.8.8/dstk/utils/_seed.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     3149 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/_set_deep_params.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     2104 2021-10-22 05:57:44.000000 dstk_x250-3.8.8/dstk/utils/_statistique.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1472 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/_timeout.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     3076 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/_transpose.py
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8012 2022-02-14 09:21:43.000000 dstk_x250-3.8.8/dstk/utils/_trie.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1777 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/deprecated.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1319 2021-09-24 10:23:58.000000 dstk_x250-3.8.8/dstk/utils/errors.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)      793 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/utils/meta_interface.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.051769 dstk_x250-3.8.8/dstk/visualization/
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      181 2022-02-13 15:08:19.000000 dstk_x250-3.8.8/dstk/visualization/__init__.py
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2639 2022-02-13 21:35:23.000000 dstk_x250-3.8.8/dstk/visualization/_bias_analyzer.py
--rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    42032 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/visualization/_roc_analyser.py
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3217 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/dstk/visualization/statistique.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.051769 dstk_x250-3.8.8/dstk_x250.egg-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2276 2022-11-08 14:08:26.000000 dstk_x250-3.8.8/dstk_x250.egg-info/PKG-INFO
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    21640 2022-11-08 14:08:28.000000 dstk_x250-3.8.8/dstk_x250.egg-info/SOURCES.txt
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)        1 2022-11-08 14:08:26.000000 dstk_x250-3.8.8/dstk_x250.egg-info/dependency_links.txt
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)        1 2022-11-08 14:08:26.000000 dstk_x250-3.8.8/dstk_x250.egg-info/not-zip-safe
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       66 2022-11-08 14:08:26.000000 dstk_x250-3.8.8/dstk_x250.egg-info/requires.txt
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)        5 2022-11-08 14:08:26.000000 dstk_x250-3.8.8/dstk_x250.egg-info/top_level.txt
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       67 2021-09-18 08:57:47.000000 dstk_x250-3.8.8/pyproject.toml
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      295 2022-11-08 14:08:28.235778 dstk_x250-3.8.8/setup.cfg
--rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1367 2022-05-25 09:08:26.000000 dstk_x250-3.8.8/setup.py
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.187775 dstk_x250-3.8.8/venv/conda-meta/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1026 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/_libgcc_mutex-0.1-conda_forge.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1351 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/_openmp_mutex-4.5-2_kmp_llvm.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    23403 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/absl-py-1.3.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    52753 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/aiohttp-3.8.1-py38h7f8727e_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5786 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/aiosignal-1.2.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9578 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/alabaster-0.7.12-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8038 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/asttokens-2.0.5-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6240 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/async-timeout-4.0.2-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19793 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/attrs-21.4.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   325062 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/babel-2.9.1-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5702 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/backcall-0.2.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1377 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/blas-2.116-openblas.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2025 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/blas-devel-3.9.0-16_linux64_openblas.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6083 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/blinker-1.4-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    30513 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/bottleneck-1.3.5-py38h7deecbd_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2550 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/brotli-1.0.9-h5eee18b_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1506 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/brotli-bin-1.0.9-h5eee18b_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6631 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/brotlipy-0.7.0-py38h27cfd23_1003.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    29199 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/c-ares-1.18.1-h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1729 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/ca-certificates-2022.07.19-h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10906 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/cachetools-4.2.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7737 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/certifi-2022.9.24-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19830 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/cffi-1.15.1-py38h74dc2b5_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13107 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/charset-normalizer-2.0.4-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    18618 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/click-8.0.4-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6900 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/cloudpickle-2.0.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9407 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/colorama-0.4.5-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    84890 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/cryptography-37.0.1-py38h9ce1e76_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4924 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/cycler-0.11.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1170 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/dataclasses-0.8-pyh6d0b6a4_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    21766 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/dbus-1.13.18-hb2f20db_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   265333 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/debugpy-1.5.1-py38h295c915_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5389 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/decorator-5.1.1-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   139634 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/docutils-0.16-py38_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4874 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/entrypoints-0.4-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6214 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/executing-0.8.3-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6387 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/expat-2.4.9-h6a678d5_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    20367 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/fftw-3.3.9-h27cfd23_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    27963 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/fontconfig-2.13.1-h6c09931_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   168106 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/fonttools-4.25.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    24133 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/freetype-2.11.0-h70c0345_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7406 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/frozenlist-1.2.0-py38h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8494 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/giflib-5.2.1-h7b6447c_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   129725 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/glib-2.69.1-h4ff587b_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    38971 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/google-auth-2.6.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9220 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/google-auth-oauthlib-0.4.4-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    32139 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/greenlet-1.1.1-py38h295c915_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    51524 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/grpcio-1.42.0-py38hce63b2e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    95932 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/gst-plugins-base-1.14.0-h8213a91_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    58992 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/gstreamer-1.14.0-h28cd5cc_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    78588 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/icu-58.2-he6710b0_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10751 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/idna-3.4-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6155 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/imagesize-1.4.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12042 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/importlib-metadata-4.11.3-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6244 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/intel-openmp-2022.1.0-h9e868ea_3769.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    61417 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ipykernel-6.15.2-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   237142 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ipython-8.4.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   920954 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/jedi-0.18.1-py38h06a4308_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19787 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/jinja2-3.0.3-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    84932 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/joblib-0.17.0-py_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7424 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/jpeg-9e-h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    57757 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/jupyter_client-7.3.5-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    33274 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/jupyter_core-4.11.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6617 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/kiwisolver-1.4.2-py38h295c915_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    61078 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/krb5-1.19.2-hac12032_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6844 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/lcms2-2.12-h3be6417_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2310 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/ld_impl_linux-64-2.38-h1181459_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2121 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/lerc-3.0-h295c915_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1782 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libblas-3.9.0-16_linux64_openblas.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2657 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libbrotlicommon-1.0.9-h5eee18b_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2652 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libbrotlidec-1.0.9-h5eee18b_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2657 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libbrotlienc-1.0.9-h5eee18b_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1716 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libcblas-3.9.0-16_linux64_openblas.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1944 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libclang-10.0.1-default_hb85057a_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2690 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libdeflate-1.8-h7f8727e_5.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    14320 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libedit-3.1.20210910-h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    22391 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libevent-2.1.12-h8f2d780_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5225 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libffi-3.3-he6710b0_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5301 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libgcc-ng-12.2.0-h65d4601_18.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1179 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libgfortran-ng-11.2.0-h00389a5_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2734 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libgfortran5-11.2.0-h1234567_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1725 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/liblapack-3.9.0-16_linux64_openblas.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1734 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/liblapacke-3.9.0-16_linux64_openblas.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2226 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libllvm10-10.0.1-hbcb73fb_5.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1827 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libopenblas-0.3.21-pthreads_h78a6416_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7397 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libpng-1.6.37-hbc83047_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   537841 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libpq-12.9-h16c4e8d_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    54530 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libprotobuf-3.21.7-h6239696_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    25660 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libsodium-1.0.18-h7b6447c_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2304 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libstdcxx-ng-12.2.0-h46fd767_18.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11509 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libtiff-4.4.0-hecacb30_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3191 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libuuid-1.0.3-h7f8727e_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3504 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libwebp-1.2.4-h11a3e52_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10773 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libwebp-base-1.2.4-h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    54916 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libxcb-1.15-h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13492 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libxkbcommon-1.0.1-hfa300c1_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    22069 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libxml2-2.9.14-h74e7548_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    67170 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/libxslt-1.1.35-h4e12654_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1639 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/libzlib-1.2.12-h166bdaf_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5131 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/llvm-openmp-14.0.6-h9e868ea_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5900 2022-10-22 12:48:52.000000 dstk_x250-3.8.8/venv/conda-meta/lz4-c-1.9.3-h295c915_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    34485 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/markdown-3.3.4-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7855 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/markupsafe-2.1.1-py38h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1260 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/matplotlib-3.5.2-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   358096 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/matplotlib-base-3.5.2-py38hf590b9c_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7282 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/matplotlib-inline-0.1.6-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    17098 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/mkl-2022.1.0-hc2b9512_224.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9906 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/multidict-6.0.2-py38h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3359 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/munkres-1.1.4-py_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   944213 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ncurses-6.3-h5eee18b_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5368 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/nest-asyncio-1.5.5-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1149 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ninja-1.10.2-h06a4308_5.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1503 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ninja-base-1.10.2-hd09550d_5.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    29109 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/nspr-4.33-h295c915_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    95080 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/nss-3.74-h0370c37_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12094 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/numexpr-2.8.3-py38hd2a5715_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1308 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/numpy-1.23.3-py38hf838250_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   582593 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/numpy-base-1.23.3-py38h1e6e340_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19343 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/numpydoc-1.4.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    66874 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/oauthlib-3.2.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6430 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/openblas-0.3.21-pthreads_h320a7e8_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    44857 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/openssl-1.1.1q-h7f8727e_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12241 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/packaging-21.3-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  1263308 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/pandas-1.4.4-py38h6a678d5_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19918 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/parso-0.8.3-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9757 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pcre-8.45-h295c915_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13551 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pexpect-4.8.0-pyhd3eb1b0_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5017 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pickleshare-0.7.5-pyhd3eb1b0_1003.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    84455 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pillow-9.2.0-py38hace64e9_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   433596 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pip-22.2.2-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7505 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ply-3.11-py38_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    99816 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/prompt-toolkit-3.0.20-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    45762 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/protobuf-4.21.7-py38hfa26641_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    28788 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/psutil-5.9.0-py38h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6396 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/ptyprocess-0.7.0-pyhd3eb1b0_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7782 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pure_eval-0.2.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    26702 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyasn1-0.4.8-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    69586 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyasn1-modules-0.2.8-py_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    15016 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pycparser-2.21-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   173367 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pygments-2.11.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12420 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyjwt-2.4.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8536 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyopenssl-22.0.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13533 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyparsing-3.0.9-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   411416 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyqt-5.15.7-py38h6a678d5_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5280 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyqt5-sip-12.11.0-py38h6a678d5_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6035 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pysocks-1.7.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   774366 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/python-3.8.13-h12debd9_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    16259 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/python-dateutil-2.8.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1054 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/python_abi-3.8-2_cp38.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  5859523 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/pytorch-1.12.1-cpu_py38h23e632a_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   251324 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pytz-2022.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   115083 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/pyzmq-23.2.0-py38h6a678d5_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  4946273 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/qt-main-5.15.2-h327a75a_7.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   118404 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/qt-webengine-5.15.9-hd2b0992_4.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    43114 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/qtwebkit-5.212-h4eab89a_4.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9567 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/readline-8.1.2-h7f8727e_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19380 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/requests-2.28.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13906 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/requests-oauthlib-1.3.0-py_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13943 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/rsa-4.7.2-pyhd3eb1b0_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   522434 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/scikit-learn-0.24.2-py38ha9443f7_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   951290 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/scipy-1.9.1-py38h32ae08f_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   208221 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/setuptools-63.4.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    66896 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sip-6.6.2-py38h6a678d5_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4833 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/six-1.16.0-pyhd3eb1b0_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4787 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sleef-3.5.1-h9b69904_2.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    25314 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/snowballstemmer-2.2.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   249416 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/sphinx-3.3.1-pyhd8ed1ab_1.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    56141 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-applehelp-1.0.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    52899 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-devhelp-1.0.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    60376 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-htmlhelp-2.0.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6729 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-jsmath-1.0.1-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    53355 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-qthelp-1.0.3-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    63077 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-serializinghtml-1.1.5-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    24423 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/spyder-kernels-1.10.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   212718 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sqlalchemy-1.4.39-py38h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3977 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/sqlite-3.39.3-h5082296_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7481 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/stack_data-0.2.0-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   267113 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/tensorboard-2.9.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5701 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/tensorboard-data-server-0.6.0-py38hca6d32c_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    40548 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/tensorboard-plugin-wit-1.8.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4669 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/threadpoolctl-2.2.0-pyh0d69192_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   178666 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/tk-8.6.12-h1ccaba5_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7179 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/toml-0.10.2-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   136260 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/torchvision-0.13.0-cpu_py38h08bc92c_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    71945 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/tornado-6.2-py38h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    32144 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/tqdm-4.64.1-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    24103 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/traitlets-5.1.1-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5058 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/typing_extensions-4.3.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    36821 2022-10-22 12:48:54.000000 dstk_x250-3.8.8/venv/conda-meta/urllib3-1.26.12-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7730 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/wcwidth-0.2.5-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    37664 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/werkzeug-2.0.3-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13800 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5283 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/wurlitzer-3.0.2-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    43919 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/xz-5.2.6-h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9640 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/yarl-1.8.1-py38h5eee18b_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    28843 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/zeromq-4.3.4-h2531618_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5150 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/zipp-3.8.0-py38h06a4308_0.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3499 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/zlib-1.2.12-h5eee18b_3.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8530 2022-10-22 12:48:53.000000 dstk_x250-3.8.8/venv/conda-meta/zstd-1.5.2-ha4553b6_0.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.039768 dstk_x250-3.8.8/venv/lib/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.195776 dstk_x250-3.8.8/venv/lib/metatypes/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   354195 2022-08-10 09:29:06.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5core_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   248958 2022-08-10 09:32:59.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5gui_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   107605 2022-08-10 09:42:17.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5qml_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    72661 2022-08-10 09:42:29.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5qmlmodels_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4613 2022-08-10 09:42:43.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5qmlworkerscript_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  1241451 2022-08-10 09:46:05.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5quick_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   183364 2022-08-10 09:47:01.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5quickparticles_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    34253 2022-08-10 09:46:25.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5quickshapes_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    30480 2022-08-10 09:46:35.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5quicktest_metatypes.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   927527 2022-08-10 09:35:56.000000 dstk_x250-3.8.8/venv/lib/metatypes/qt5widgets_metatypes.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.199776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Babel-2.9.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2021-05-13 02:04:16.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Babel-2.9.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.199776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Bottleneck-1.3.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-07-07 06:33:49.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Bottleneck-1.3.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.199776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Jinja2-3.0.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-03-16 13:16:53.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Jinja2-3.0.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.199776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Markdown-3.3.4.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2021-02-26 18:19:21.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Markdown-3.3.4.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.199776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/MarkupSafe-2.1.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-06-07 10:37:30.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/MarkupSafe-2.1.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/PyJWT-2.4.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-07-11 13:04:41.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/PyJWT-2.4.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/PySocks-1.7.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2020-11-13 22:16:45.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/PySocks-1.7.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Pygments-2.11.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-02-07 15:52:27.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Pygments-2.11.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/SQLAlchemy-1.4.39.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      131 2022-07-15 06:52:18.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/SQLAlchemy-1.4.39.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Sphinx-3.3.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      102 2020-12-09 17:33:16.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Sphinx-3.3.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Werkzeug-2.0.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-02-23 14:59:02.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/Werkzeug-2.0.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/absl_py-1.3.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       67 2022-10-21 14:37:27.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/absl_py-1.3.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/aiohttp-3.8.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-03-09 06:13:33.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/aiohttp-3.8.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/aiosignal-1.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-25 12:24:50.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/aiosignal-1.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/alabaster-0.7.12.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-01-29 11:59:09.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/alabaster-0.7.12.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/asttokens-2.0.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-03-10 15:21:07.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/asttokens-2.0.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/async_timeout-4.0.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       87 2022-10-04 09:41:19.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/async_timeout-4.0.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/attrs-21.4.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-01-18 12:54:42.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/attrs-21.4.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/backcall-0.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2021-01-29 14:20:17.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/backcall-0.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cachetools-4.2.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2021-04-28 08:10:25.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cachetools-4.2.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/certifi-2022.9.24.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       75 2022-10-06 17:19:45.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/certifi-2022.9.24.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cffi-1.15.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2022-08-04 07:38:43.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cffi-1.15.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/charset_normalizer-2.0.4.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2021-08-26 18:40:58.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/charset_normalizer-2.0.4.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/click-8.0.4.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-02-28 08:54:51.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/click-8.0.4.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.203776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cloudpickle-2.0.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2021-09-24 18:27:35.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cloudpickle-2.0.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/colorama-0.4.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-07-05 08:19:07.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/colorama-0.4.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cryptography-37.0.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2022-05-09 08:11:56.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cryptography-37.0.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cycler-0.11.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2021-11-25 14:46:22.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/cycler-0.11.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   148950 2021-11-16 19:44:08.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocol.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10940 2021-11-16 19:44:08.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocolCustom.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/vendored/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/vendored/bytecode-0.13.0.dev0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-11-16 19:44:09.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/vendored/bytecode-0.13.0.dev0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy-1.5.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2021-11-16 19:44:09.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy-1.5.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/decorator-5.1.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-01-31 14:12:24.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/decorator-5.1.1.dist-info/direct_url.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       47 2022-01-31 14:12:24.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/decorator-5.1.1.dist-info/pbr.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/entrypoints-0.4.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-04-14 08:54:38.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/entrypoints-0.4.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/executing-0.8.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-03-10 15:11:58.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/executing-0.8.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/frozenlist-1.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2021-11-24 15:19:06.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/frozenlist-1.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/google_auth-2.6.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2022-03-08 10:40:20.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/google_auth-2.6.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/google_auth_oauthlib-0.4.4.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-03-30 16:10:02.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/google_auth_oauthlib-0.4.4.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/greenlet-1.1.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2021-08-13 20:49:28.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/greenlet-1.1.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/grpcio-1.42.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2021-11-22 14:22:18.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/grpcio-1.42.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/idna-3.4.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       64 2022-10-18 20:40:58.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/idna-3.4.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.207776 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/imagesize-1.4.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-07-07 07:39:00.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/imagesize-1.4.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/importlib_metadata-4.11.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2022-03-29 14:00:52.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/importlib_metadata-4.11.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/ipykernel-6.15.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-09-05 07:12:51.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/ipykernel-6.15.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/ipython-8.4.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2022-07-12 18:59:53.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/ipython-8.4.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/jedi-0.18.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       77 2022-02-08 10:14:23.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/jedi-0.18.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/joblib-0.17.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2020-10-05 15:48:53.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/joblib-0.17.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/jupyter_client-7.3.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       88 2022-09-06 22:46:43.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/jupyter_client-7.3.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/jupyter_core-4.11.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       86 2022-10-04 21:02:15.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/jupyter_core-4.11.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/kiwisolver-1.4.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-05-23 07:50:57.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/kiwisolver-1.4.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib/backends/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      545 2022-08-10 21:50:38.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/package.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib-3.5.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       90 2022-08-10 21:50:39.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib-3.5.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib_inline-0.1.6.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2022-09-01 06:44:00.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib_inline-0.1.6.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/multidict-6.0.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       69 2022-10-13 15:18:25.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/multidict-6.0.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/nest_asyncio-1.5.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2022-04-13 11:05:43.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/nest_asyncio-1.5.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/numexpr-2.8.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2022-07-04 13:16:18.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/numexpr-2.8.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/numpy-1.23.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-10-14 19:19:09.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/numpy-1.23.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.211777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/numpydoc-1.4.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-07-11 08:58:20.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/numpydoc-1.4.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/oauthlib-3.2.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       68 2022-10-11 12:22:04.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/oauthlib-3.2.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/packaging-21.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-19 09:32:07.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/packaging-21.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/parso-0.8.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-01-06 08:44:28.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/parso-0.8.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pexpect-4.8.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2020-11-16 21:47:14.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pexpect-4.8.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pickleshare-0.7.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2020-12-02 18:01:14.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pickleshare-0.7.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/prompt_toolkit-3.0.20.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       87 2021-10-05 13:23:13.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/prompt_toolkit-3.0.20.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/psutil-5.9.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-06-28 15:50:23.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/psutil-5.9.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/ptyprocess-0.7.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      130 2020-12-30 19:03:57.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/ptyprocess-0.7.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pure_eval-0.2.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-03-10 15:11:57.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pure_eval-0.2.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyOpenSSL-22.0.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-02-02 07:56:30.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyOpenSSL-22.0.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyasn1-0.4.8.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       92 2021-08-23 08:40:24.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyasn1-0.4.8.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pycparser-2.21.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-10 10:49:41.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pycparser-2.21.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyparsing-3.0.9.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-08-25 18:36:44.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyparsing-3.0.9.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/python_dateutil-2.8.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       88 2021-07-15 18:44:54.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/python_dateutil-2.8.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.215777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pytz-2022.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-06-09 08:18:53.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pytz-2022.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyzmq-23.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-07-13 14:59:35.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/pyzmq-23.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/requests-2.28.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-07-13 17:53:04.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/requests-2.28.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/rsa-4.7.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       76 2021-02-26 19:04:25.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/rsa-4.7.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scikit_learn-0.24.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2021-05-18 20:45:11.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scikit_learn-0.24.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scipy/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scipy/stats/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.043769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scipy/stats/tests/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scipy/stats/tests/data/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    29239 2022-08-26 19:12:35.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scipy/stats/tests/data/studentized_range_mpmath_ref.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sip-6.6.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       90 2022-07-28 12:50:12.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sip-6.6.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/six-1.16.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       76 2022-02-14 21:59:33.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/six-1.16.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/snowballstemmer-2.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       88 2021-11-26 14:31:46.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/snowballstemmer-2.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.219777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_applehelp-1.0.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       96 2021-01-29 11:47:26.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_applehelp-1.0.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_devhelp-1.0.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       94 2021-01-29 11:48:48.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_devhelp-1.0.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_htmlhelp-2.0.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       95 2021-06-17 16:01:12.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_htmlhelp-2.0.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-01-29 11:49:07.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_qthelp-1.0.3.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-01-29 11:51:00.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_qthelp-1.0.3.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_serializinghtml-1.1.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      102 2021-06-23 12:33:05.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/sphinxcontrib_serializinghtml-1.1.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/spyder_kernels-1.10.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       87 2020-12-02 17:15:36.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/spyder_kernels-1.10.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/stack_data-0.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-03-10 15:53:59.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/stack_data-0.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tensorboard-2.9.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      162 2022-08-25 17:18:20.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tensorboard-2.9.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tensorboard_data_server-0.6.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      164 2021-09-30 20:53:51.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tensorboard_data_server-0.6.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tensorboard_plugin_wit-1.8.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      166 2022-07-27 10:41:52.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tensorboard_plugin_wit-1.8.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/threadpoolctl-2.2.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       99 2021-08-24 10:51:21.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/threadpoolctl-2.2.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/toml-0.10.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       77 2021-03-19 15:10:42.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/toml-0.10.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.223777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/torch-1.12.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      110 2022-10-03 20:28:01.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/torch-1.12.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/torchvision-0.13.0a0+8069656.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      113 2022-07-24 12:16:58.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/torchvision-0.13.0a0+8069656.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tornado-6.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2022-09-01 19:50:05.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tornado-6.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tqdm-4.64.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-09-28 19:18:42.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/tqdm-4.64.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/traitlets-5.1.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-12 09:45:27.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/traitlets-5.1.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/typing_extensions-4.3.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      104 2022-08-04 18:48:42.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/typing_extensions-4.3.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/urllib3-1.26.12.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       67 2022-10-20 20:50:54.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/urllib3-1.26.12.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/wcwidth-0.2.5.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-08-19 07:13:28.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/wcwidth-0.2.5.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/wurlitzer-3.0.2.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-12-01 10:36:37.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/wurlitzer-3.0.2.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/yarl-1.8.1.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-08-25 14:19:47.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/yarl-1.8.1.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.227777 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/zipp-3.8.0.dist-info/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-05-12 07:49:54.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/zipp-3.8.0.dist-info/direct_url.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/zmq/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/zmq/utils/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      442 2022-10-22 12:48:41.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/zmq/utils/compiler.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      393 2022-10-22 12:48:41.000000 dstk_x250-3.8.8/venv/lib/python3.8/site-packages/zmq/utils/config.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/mkspecs/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/mkspecs/features/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/mkspecs/features/data/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      766 2020-10-27 08:02:11.000000 dstk_x250-3.8.8/venv/mkspecs/features/data/configure.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/jupyter/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/jupyter/kernels/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/share/jupyter/kernels/python3/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      257 2022-10-22 12:48:42.000000 dstk_x250-3.8.8/venv/share/jupyter/kernels/python3/kernel.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      846 2022-08-10 10:35:05.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/.eslintrc.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      161 2022-08-10 10:35:05.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/customFormatExample.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.047769 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/debug/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1152 2022-08-10 10:35:05.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/debug/package.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/nopt/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      522 2022-08-10 10:35:05.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/nopt/package.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4025 2022-08-10 10:35:05.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/package.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      434 2022-08-10 10:35:06.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/deprecated.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5291 2022-08-10 10:35:06.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/index.json
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      793 2022-08-10 10:35:06.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/package.json
-drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:08:28.231778 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/validate-npm-package-license/
--rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      747 2022-08-10 10:35:06.000000 dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/validate-npm-package-license/package.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11349 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/LICENSE.txt
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       22 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/MANIFEST.in
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2276 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/PKG-INFO
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1910 2021-09-21 21:14:24.000000 dstk_x250-3.8.9/README.md
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/dstk/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       95 2022-11-08 14:46:35.000000 dstk_x250-3.8.9/dstk/__init__.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/dstk/data/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      259 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/data/__init__.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    13027 2022-06-16 09:32:59.000000 dstk_x250-3.8.9/dstk/data/_pandas_sql.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     5005 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/data/_sql.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/dstk/features/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      414 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/features/__init__.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    13878 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/features/_prepro.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     6300 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/features/_transformers.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/dstk/metrics/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      490 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/metrics/__init__.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     5618 2021-10-21 17:29:44.000000 dstk_x250-3.8.9/dstk/metrics/_aggregator.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    37526 2021-10-21 17:40:40.000000 dstk_x250-3.8.9/dstk/metrics/_handlers.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    15442 2021-10-21 17:38:13.000000 dstk_x250-3.8.9/dstk/metrics/_metrics.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)      564 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/metrics/push.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/dstk/ml/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      137 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/ml/__init__.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    10822 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/ml/_ml.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.088197 dstk_x250-3.8.9/dstk/pytorch/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2555 2022-11-04 12:30:57.000000 dstk_x250-3.8.9/dstk/pytorch/__init__.py
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    37883 2022-11-08 14:46:10.000000 dstk_x250-3.8.9/dstk/pytorch/_base.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    44986 2022-11-04 12:30:02.000000 dstk_x250-3.8.9/dstk/pytorch/_callback.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13592 2022-11-04 12:19:02.000000 dstk_x250-3.8.9/dstk/pytorch/_classifier.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    23175 2022-06-03 09:13:26.000000 dstk_x250-3.8.9/dstk/pytorch/_random_search.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9890 2022-11-04 12:18:25.000000 dstk_x250-3.8.9/dstk/pytorch/_regressor.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    30757 2021-10-17 11:15:04.000000 dstk_x250-3.8.9/dstk/pytorch/_swa.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    16475 2022-11-04 10:50:23.000000 dstk_x250-3.8.9/dstk/pytorch/_utils.py
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8737 2022-11-08 14:50:07.000000 dstk_x250-3.8.9/dstk/pytorch/_utils_distrib.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19254 2022-07-28 12:16:12.000000 dstk_x250-3.8.9/dstk/pytorch/metrics.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    16309 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/pytorch/networks.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11062 2022-10-23 13:04:55.000000 dstk_x250-3.8.9/dstk/pytorch/supervision.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.088197 dstk_x250-3.8.9/dstk/ssh/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      162 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/ssh/__init__.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19382 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/ssh/_ssh.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     2691 2021-09-20 08:41:05.000000 dstk_x250-3.8.9/dstk/ssh/_utils.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.088197 dstk_x250-3.8.9/dstk/utils/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      847 2022-05-30 13:03:05.000000 dstk_x250-3.8.9/dstk/utils/__init__.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     4573 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/_check.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     4500 2021-10-21 17:45:00.000000 dstk_x250-3.8.9/dstk/utils/_chunk.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     3630 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/_date.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     6364 2022-06-19 20:30:55.000000 dstk_x250-3.8.9/dstk/utils/_rolling.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1008 2022-06-08 07:27:32.000000 dstk_x250-3.8.9/dstk/utils/_seed.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     3149 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/_set_deep_params.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     2104 2021-10-22 05:57:44.000000 dstk_x250-3.8.9/dstk/utils/_statistique.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1472 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/_timeout.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     3076 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/_transpose.py
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8012 2022-02-14 09:21:43.000000 dstk_x250-3.8.9/dstk/utils/_trie.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1777 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/deprecated.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)     1319 2021-09-24 10:23:58.000000 dstk_x250-3.8.9/dstk/utils/errors.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)      793 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/utils/meta_interface.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.088197 dstk_x250-3.8.9/dstk/visualization/
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      181 2022-02-13 15:08:19.000000 dstk_x250-3.8.9/dstk/visualization/__init__.py
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2639 2022-02-13 21:35:23.000000 dstk_x250-3.8.9/dstk/visualization/_bias_analyzer.py
+-rwxr-xr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)    42032 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/visualization/_roc_analyser.py
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3217 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/dstk/visualization/statistique.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.088197 dstk_x250-3.8.9/dstk_x250.egg-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2276 2022-11-08 14:52:57.000000 dstk_x250-3.8.9/dstk_x250.egg-info/PKG-INFO
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    21640 2022-11-08 14:52:59.000000 dstk_x250-3.8.9/dstk_x250.egg-info/SOURCES.txt
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)        1 2022-11-08 14:52:57.000000 dstk_x250-3.8.9/dstk_x250.egg-info/dependency_links.txt
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)        1 2022-11-08 14:52:57.000000 dstk_x250-3.8.9/dstk_x250.egg-info/not-zip-safe
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       66 2022-11-08 14:52:57.000000 dstk_x250-3.8.9/dstk_x250.egg-info/requires.txt
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)        5 2022-11-08 14:52:57.000000 dstk_x250-3.8.9/dstk_x250.egg-info/top_level.txt
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       67 2021-09-18 08:57:47.000000 dstk_x250-3.8.9/pyproject.toml
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      295 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/setup.cfg
+-rw-r--r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1367 2022-05-25 09:08:26.000000 dstk_x250-3.8.9/setup.py
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.120199 dstk_x250-3.8.9/venv/conda-meta/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1026 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/_libgcc_mutex-0.1-conda_forge.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1351 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/_openmp_mutex-4.5-2_kmp_llvm.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    23403 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/absl-py-1.3.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    52753 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/aiohttp-3.8.1-py38h7f8727e_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5786 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/aiosignal-1.2.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9578 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/alabaster-0.7.12-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8038 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/asttokens-2.0.5-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6240 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/async-timeout-4.0.2-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19793 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/attrs-21.4.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   325062 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/babel-2.9.1-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5702 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/backcall-0.2.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1377 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/blas-2.116-openblas.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2025 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/blas-devel-3.9.0-16_linux64_openblas.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6083 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/blinker-1.4-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    30513 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/bottleneck-1.3.5-py38h7deecbd_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2550 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/brotli-1.0.9-h5eee18b_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1506 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/brotli-bin-1.0.9-h5eee18b_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6631 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/brotlipy-0.7.0-py38h27cfd23_1003.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    29199 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/c-ares-1.18.1-h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1729 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/ca-certificates-2022.07.19-h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10906 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/cachetools-4.2.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7737 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/certifi-2022.9.24-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19830 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/cffi-1.15.1-py38h74dc2b5_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13107 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/charset-normalizer-2.0.4-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    18618 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/click-8.0.4-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6900 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/cloudpickle-2.0.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9407 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/colorama-0.4.5-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    84890 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/cryptography-37.0.1-py38h9ce1e76_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4924 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/cycler-0.11.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1170 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/dataclasses-0.8-pyh6d0b6a4_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    21766 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/dbus-1.13.18-hb2f20db_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   265333 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/debugpy-1.5.1-py38h295c915_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5389 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/decorator-5.1.1-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   139634 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/docutils-0.16-py38_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4874 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/entrypoints-0.4-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6214 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/executing-0.8.3-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6387 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/expat-2.4.9-h6a678d5_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    20367 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/fftw-3.3.9-h27cfd23_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    27963 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/fontconfig-2.13.1-h6c09931_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   168106 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/fonttools-4.25.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    24133 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/freetype-2.11.0-h70c0345_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7406 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/frozenlist-1.2.0-py38h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8494 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/giflib-5.2.1-h7b6447c_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   129725 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/glib-2.69.1-h4ff587b_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    38971 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/google-auth-2.6.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9220 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/google-auth-oauthlib-0.4.4-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    32139 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/greenlet-1.1.1-py38h295c915_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    51524 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/grpcio-1.42.0-py38hce63b2e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    95932 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/gst-plugins-base-1.14.0-h8213a91_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    58992 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/gstreamer-1.14.0-h28cd5cc_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    78588 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/icu-58.2-he6710b0_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10751 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/idna-3.4-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6155 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/imagesize-1.4.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12042 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/importlib-metadata-4.11.3-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6244 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/intel-openmp-2022.1.0-h9e868ea_3769.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    61417 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ipykernel-6.15.2-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   237142 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ipython-8.4.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   920954 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/jedi-0.18.1-py38h06a4308_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19787 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/jinja2-3.0.3-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    84932 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/joblib-0.17.0-py_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7424 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/jpeg-9e-h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    57757 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/jupyter_client-7.3.5-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    33274 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/jupyter_core-4.11.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6617 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/kiwisolver-1.4.2-py38h295c915_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    61078 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/krb5-1.19.2-hac12032_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6844 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/lcms2-2.12-h3be6417_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2310 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/ld_impl_linux-64-2.38-h1181459_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2121 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/lerc-3.0-h295c915_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1782 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libblas-3.9.0-16_linux64_openblas.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2657 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libbrotlicommon-1.0.9-h5eee18b_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2652 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libbrotlidec-1.0.9-h5eee18b_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2657 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libbrotlienc-1.0.9-h5eee18b_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1716 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libcblas-3.9.0-16_linux64_openblas.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1944 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libclang-10.0.1-default_hb85057a_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2690 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libdeflate-1.8-h7f8727e_5.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    14320 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libedit-3.1.20210910-h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    22391 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libevent-2.1.12-h8f2d780_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5225 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libffi-3.3-he6710b0_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5301 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libgcc-ng-12.2.0-h65d4601_18.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1179 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libgfortran-ng-11.2.0-h00389a5_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2734 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libgfortran5-11.2.0-h1234567_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1725 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/liblapack-3.9.0-16_linux64_openblas.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1734 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/liblapacke-3.9.0-16_linux64_openblas.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2226 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libllvm10-10.0.1-hbcb73fb_5.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1827 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libopenblas-0.3.21-pthreads_h78a6416_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7397 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libpng-1.6.37-hbc83047_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   537841 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libpq-12.9-h16c4e8d_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    54530 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libprotobuf-3.21.7-h6239696_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    25660 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libsodium-1.0.18-h7b6447c_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     2304 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libstdcxx-ng-12.2.0-h46fd767_18.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    11509 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libtiff-4.4.0-hecacb30_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3191 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libuuid-1.0.3-h7f8727e_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3504 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libwebp-1.2.4-h11a3e52_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10773 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libwebp-base-1.2.4-h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    54916 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libxcb-1.15-h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13492 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libxkbcommon-1.0.1-hfa300c1_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    22069 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libxml2-2.9.14-h74e7548_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    67170 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/libxslt-1.1.35-h4e12654_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1639 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/libzlib-1.2.12-h166bdaf_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5131 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/llvm-openmp-14.0.6-h9e868ea_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5900 2022-10-22 12:48:52.000000 dstk_x250-3.8.9/venv/conda-meta/lz4-c-1.9.3-h295c915_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    34485 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/markdown-3.3.4-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7855 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/markupsafe-2.1.1-py38h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1260 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/matplotlib-3.5.2-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   358096 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/matplotlib-base-3.5.2-py38hf590b9c_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7282 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/matplotlib-inline-0.1.6-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    17098 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/mkl-2022.1.0-hc2b9512_224.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9906 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/multidict-6.0.2-py38h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3359 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/munkres-1.1.4-py_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   944213 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ncurses-6.3-h5eee18b_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5368 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/nest-asyncio-1.5.5-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1149 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ninja-1.10.2-h06a4308_5.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1503 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ninja-base-1.10.2-hd09550d_5.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    29109 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/nspr-4.33-h295c915_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    95080 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/nss-3.74-h0370c37_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12094 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/numexpr-2.8.3-py38hd2a5715_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1308 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/numpy-1.23.3-py38hf838250_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   582593 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/numpy-base-1.23.3-py38h1e6e340_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19343 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/numpydoc-1.4.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    66874 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/oauthlib-3.2.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6430 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/openblas-0.3.21-pthreads_h320a7e8_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    44857 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/openssl-1.1.1q-h7f8727e_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12241 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/packaging-21.3-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  1263308 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/pandas-1.4.4-py38h6a678d5_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19918 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/parso-0.8.3-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9757 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pcre-8.45-h295c915_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13551 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pexpect-4.8.0-pyhd3eb1b0_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5017 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pickleshare-0.7.5-pyhd3eb1b0_1003.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    84455 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pillow-9.2.0-py38hace64e9_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   433596 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pip-22.2.2-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7505 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ply-3.11-py38_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    99816 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/prompt-toolkit-3.0.20-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    45762 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/protobuf-4.21.7-py38hfa26641_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    28788 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/psutil-5.9.0-py38h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6396 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/ptyprocess-0.7.0-pyhd3eb1b0_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7782 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pure_eval-0.2.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    26702 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyasn1-0.4.8-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    69586 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyasn1-modules-0.2.8-py_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    15016 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pycparser-2.21-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   173367 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pygments-2.11.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    12420 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyjwt-2.4.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8536 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyopenssl-22.0.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13533 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyparsing-3.0.9-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   411416 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyqt-5.15.7-py38h6a678d5_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5280 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyqt5-sip-12.11.0-py38h6a678d5_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6035 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pysocks-1.7.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   774366 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/python-3.8.13-h12debd9_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    16259 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/python-dateutil-2.8.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1054 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/python_abi-3.8-2_cp38.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  5859523 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/pytorch-1.12.1-cpu_py38h23e632a_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   251324 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pytz-2022.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   115083 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/pyzmq-23.2.0-py38h6a678d5_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  4946273 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/qt-main-5.15.2-h327a75a_7.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   118404 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/qt-webengine-5.15.9-hd2b0992_4.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    43114 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/qtwebkit-5.212-h4eab89a_4.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9567 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/readline-8.1.2-h7f8727e_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    19380 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/requests-2.28.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13906 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/requests-oauthlib-1.3.0-py_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13943 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/rsa-4.7.2-pyhd3eb1b0_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   522434 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/scikit-learn-0.24.2-py38ha9443f7_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   951290 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/scipy-1.9.1-py38h32ae08f_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   208221 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/setuptools-63.4.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    66896 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sip-6.6.2-py38h6a678d5_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4833 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/six-1.16.0-pyhd3eb1b0_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4787 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sleef-3.5.1-h9b69904_2.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    25314 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/snowballstemmer-2.2.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   249416 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/sphinx-3.3.1-pyhd8ed1ab_1.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    56141 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-applehelp-1.0.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    52899 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-devhelp-1.0.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    60376 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-htmlhelp-2.0.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     6729 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-jsmath-1.0.1-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    53355 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-qthelp-1.0.3-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    63077 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-serializinghtml-1.1.5-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    24423 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/spyder-kernels-1.10.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   212718 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sqlalchemy-1.4.39-py38h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3977 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/sqlite-3.39.3-h5082296_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7481 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/stack_data-0.2.0-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   267113 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/tensorboard-2.9.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5701 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/tensorboard-data-server-0.6.0-py38hca6d32c_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    40548 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/tensorboard-plugin-wit-1.8.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4669 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/threadpoolctl-2.2.0-pyh0d69192_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   178666 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/tk-8.6.12-h1ccaba5_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7179 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/toml-0.10.2-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   136260 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/torchvision-0.13.0-cpu_py38h08bc92c_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    71945 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/tornado-6.2-py38h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    32144 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/tqdm-4.64.1-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    24103 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/traitlets-5.1.1-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5058 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/typing_extensions-4.3.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    36821 2022-10-22 12:48:54.000000 dstk_x250-3.8.9/venv/conda-meta/urllib3-1.26.12-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     7730 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/wcwidth-0.2.5-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    37664 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/werkzeug-2.0.3-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    13800 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5283 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/wurlitzer-3.0.2-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    43919 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/xz-5.2.6-h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     9640 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/yarl-1.8.1-py38h5eee18b_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    28843 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/zeromq-4.3.4-h2531618_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5150 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/zipp-3.8.0-py38h06a4308_0.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     3499 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/zlib-1.2.12-h5eee18b_3.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     8530 2022-10-22 12:48:53.000000 dstk_x250-3.8.9/venv/conda-meta/zstd-1.5.2-ha4553b6_0.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/metatypes/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   354195 2022-08-10 09:29:06.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5core_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   248958 2022-08-10 09:32:59.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5gui_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   107605 2022-08-10 09:42:17.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5qml_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    72661 2022-08-10 09:42:29.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5qmlmodels_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4613 2022-08-10 09:42:43.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5qmlworkerscript_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)  1241451 2022-08-10 09:46:05.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5quick_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   183364 2022-08-10 09:47:01.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5quickparticles_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    34253 2022-08-10 09:46:25.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5quickshapes_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    30480 2022-08-10 09:46:35.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5quicktest_metatypes.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   927527 2022-08-10 09:35:56.000000 dstk_x250-3.8.9/venv/lib/metatypes/qt5widgets_metatypes.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Babel-2.9.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2021-05-13 02:04:16.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Babel-2.9.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Bottleneck-1.3.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-07-07 06:33:49.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Bottleneck-1.3.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Jinja2-3.0.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-03-16 13:16:53.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Jinja2-3.0.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Markdown-3.3.4.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2021-02-26 18:19:21.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Markdown-3.3.4.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/MarkupSafe-2.1.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-06-07 10:37:30.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/MarkupSafe-2.1.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/PyJWT-2.4.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-07-11 13:04:41.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/PyJWT-2.4.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/PySocks-1.7.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2020-11-13 22:16:45.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/PySocks-1.7.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Pygments-2.11.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-02-07 15:52:27.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Pygments-2.11.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/SQLAlchemy-1.4.39.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      131 2022-07-15 06:52:18.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/SQLAlchemy-1.4.39.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Sphinx-3.3.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      102 2020-12-09 17:33:16.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Sphinx-3.3.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Werkzeug-2.0.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-02-23 14:59:02.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/Werkzeug-2.0.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/absl_py-1.3.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       67 2022-10-21 14:37:27.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/absl_py-1.3.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/aiohttp-3.8.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-03-09 06:13:33.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/aiohttp-3.8.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/aiosignal-1.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-25 12:24:50.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/aiosignal-1.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/alabaster-0.7.12.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-01-29 11:59:09.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/alabaster-0.7.12.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/asttokens-2.0.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-03-10 15:21:07.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/asttokens-2.0.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/async_timeout-4.0.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       87 2022-10-04 09:41:19.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/async_timeout-4.0.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/attrs-21.4.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-01-18 12:54:42.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/attrs-21.4.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/backcall-0.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2021-01-29 14:20:17.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/backcall-0.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cachetools-4.2.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2021-04-28 08:10:25.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cachetools-4.2.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/certifi-2022.9.24.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       75 2022-10-06 17:19:45.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/certifi-2022.9.24.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cffi-1.15.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2022-08-04 07:38:43.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cffi-1.15.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/charset_normalizer-2.0.4.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2021-08-26 18:40:58.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/charset_normalizer-2.0.4.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/click-8.0.4.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-02-28 08:54:51.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/click-8.0.4.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cloudpickle-2.0.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2021-09-24 18:27:35.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cloudpickle-2.0.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/colorama-0.4.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-07-05 08:19:07.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/colorama-0.4.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cryptography-37.0.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2022-05-09 08:11:56.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cryptography-37.0.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cycler-0.11.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2021-11-25 14:46:22.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/cycler-0.11.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)   148950 2021-11-16 19:44:08.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocol.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    10940 2021-11-16 19:44:08.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocolCustom.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/vendored/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/vendored/bytecode-0.13.0.dev0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-11-16 19:44:09.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_frame_eval/vendored/bytecode-0.13.0.dev0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.124199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy-1.5.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2021-11-16 19:44:09.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy-1.5.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/decorator-5.1.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-01-31 14:12:24.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/decorator-5.1.1.dist-info/direct_url.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       47 2022-01-31 14:12:24.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/decorator-5.1.1.dist-info/pbr.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/entrypoints-0.4.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-04-14 08:54:38.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/entrypoints-0.4.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/executing-0.8.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-03-10 15:11:58.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/executing-0.8.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/frozenlist-1.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2021-11-24 15:19:06.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/frozenlist-1.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/google_auth-2.6.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2022-03-08 10:40:20.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/google_auth-2.6.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/google_auth_oauthlib-0.4.4.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-03-30 16:10:02.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/google_auth_oauthlib-0.4.4.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/greenlet-1.1.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2021-08-13 20:49:28.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/greenlet-1.1.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/grpcio-1.42.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2021-11-22 14:22:18.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/grpcio-1.42.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/idna-3.4.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       64 2022-10-18 20:40:58.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/idna-3.4.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/imagesize-1.4.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-07-07 07:39:00.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/imagesize-1.4.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/importlib_metadata-4.11.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2022-03-29 14:00:52.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/importlib_metadata-4.11.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/ipykernel-6.15.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-09-05 07:12:51.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/ipykernel-6.15.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/ipython-8.4.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2022-07-12 18:59:53.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/ipython-8.4.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/jedi-0.18.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       77 2022-02-08 10:14:23.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/jedi-0.18.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/joblib-0.17.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2020-10-05 15:48:53.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/joblib-0.17.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/jupyter_client-7.3.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       88 2022-09-06 22:46:43.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/jupyter_client-7.3.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/jupyter_core-4.11.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       86 2022-10-04 21:02:15.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/jupyter_core-4.11.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/kiwisolver-1.4.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-05-23 07:50:57.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/kiwisolver-1.4.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib/backends/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      545 2022-08-10 21:50:38.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/package.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib-3.5.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       90 2022-08-10 21:50:39.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib-3.5.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib_inline-0.1.6.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       91 2022-09-01 06:44:00.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib_inline-0.1.6.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/multidict-6.0.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       69 2022-10-13 15:18:25.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/multidict-6.0.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/nest_asyncio-1.5.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2022-04-13 11:05:43.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/nest_asyncio-1.5.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/numexpr-2.8.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2022-07-04 13:16:18.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/numexpr-2.8.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/numpy-1.23.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-10-14 19:19:09.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/numpy-1.23.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/numpydoc-1.4.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-07-11 08:58:20.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/numpydoc-1.4.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/oauthlib-3.2.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       68 2022-10-11 12:22:04.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/oauthlib-3.2.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/packaging-21.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-19 09:32:07.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/packaging-21.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/parso-0.8.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-01-06 08:44:28.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/parso-0.8.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pexpect-4.8.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2020-11-16 21:47:14.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pexpect-4.8.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pickleshare-0.7.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2020-12-02 18:01:14.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pickleshare-0.7.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/prompt_toolkit-3.0.20.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       87 2021-10-05 13:23:13.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/prompt_toolkit-3.0.20.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/psutil-5.9.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       80 2022-06-28 15:50:23.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/psutil-5.9.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/ptyprocess-0.7.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      130 2020-12-30 19:03:57.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/ptyprocess-0.7.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pure_eval-0.2.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-03-10 15:11:57.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pure_eval-0.2.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyOpenSSL-22.0.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-02-02 07:56:30.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyOpenSSL-22.0.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyasn1-0.4.8.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       92 2021-08-23 08:40:24.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyasn1-0.4.8.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pycparser-2.21.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-10 10:49:41.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pycparser-2.21.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyparsing-3.0.9.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       83 2022-08-25 18:36:44.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyparsing-3.0.9.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/python_dateutil-2.8.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       88 2021-07-15 18:44:54.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/python_dateutil-2.8.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pytz-2022.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-06-09 08:18:53.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pytz-2022.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyzmq-23.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       79 2022-07-13 14:59:35.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/pyzmq-23.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/requests-2.28.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2022-07-13 17:53:04.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/requests-2.28.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/rsa-4.7.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       76 2021-02-26 19:04:25.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/rsa-4.7.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scikit_learn-0.24.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       85 2021-05-18 20:45:11.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scikit_learn-0.24.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scipy/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scipy/stats/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.080197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scipy/stats/tests/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scipy/stats/tests/data/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)    29239 2022-08-26 19:12:35.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scipy/stats/tests/data/studentized_range_mpmath_ref.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sip-6.6.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       90 2022-07-28 12:50:12.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sip-6.6.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/six-1.16.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       76 2022-02-14 21:59:33.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/six-1.16.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/snowballstemmer-2.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       88 2021-11-26 14:31:46.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/snowballstemmer-2.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_applehelp-1.0.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       96 2021-01-29 11:47:26.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_applehelp-1.0.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_devhelp-1.0.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       94 2021-01-29 11:48:48.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_devhelp-1.0.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_htmlhelp-2.0.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       95 2021-06-17 16:01:12.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_htmlhelp-2.0.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-01-29 11:49:07.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_jsmath-1.0.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_qthelp-1.0.3.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-01-29 11:51:00.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_qthelp-1.0.3.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_serializinghtml-1.1.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      102 2021-06-23 12:33:05.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/sphinxcontrib_serializinghtml-1.1.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/spyder_kernels-1.10.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       87 2020-12-02 17:15:36.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/spyder_kernels-1.10.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/stack_data-0.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       84 2022-03-10 15:53:59.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/stack_data-0.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tensorboard-2.9.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      162 2022-08-25 17:18:20.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tensorboard-2.9.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tensorboard_data_server-0.6.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      164 2021-09-30 20:53:51.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tensorboard_data_server-0.6.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tensorboard_plugin_wit-1.8.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      166 2022-07-27 10:41:52.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tensorboard_plugin_wit-1.8.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/threadpoolctl-2.2.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       99 2021-08-24 10:51:21.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/threadpoolctl-2.2.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/toml-0.10.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       77 2021-03-19 15:10:42.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/toml-0.10.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/torch-1.12.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      110 2022-10-03 20:28:01.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/torch-1.12.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.128199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/torchvision-0.13.0a0+8069656.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      113 2022-07-24 12:16:58.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/torchvision-0.13.0a0+8069656.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tornado-6.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       81 2022-09-01 19:50:05.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tornado-6.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tqdm-4.64.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-09-28 19:18:42.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/tqdm-4.64.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/traitlets-5.1.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-11-12 09:45:27.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/traitlets-5.1.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/typing_extensions-4.3.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      104 2022-08-04 18:48:42.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/typing_extensions-4.3.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/urllib3-1.26.12.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       67 2022-10-20 20:50:54.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/urllib3-1.26.12.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/wcwidth-0.2.5.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       93 2021-08-19 07:13:28.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/wcwidth-0.2.5.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/wurlitzer-3.0.2.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       82 2021-12-01 10:36:37.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/wurlitzer-3.0.2.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/yarl-1.8.1.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-08-25 14:19:47.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/yarl-1.8.1.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/zipp-3.8.0.dist-info/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)       78 2022-05-12 07:49:54.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/zipp-3.8.0.dist-info/direct_url.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/zmq/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/zmq/utils/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      442 2022-10-22 12:48:41.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/zmq/utils/compiler.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      393 2022-10-22 12:48:41.000000 dstk_x250-3.8.9/venv/lib/python3.8/site-packages/zmq/utils/config.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/mkspecs/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/mkspecs/features/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/mkspecs/features/data/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      766 2020-10-27 08:02:11.000000 dstk_x250-3.8.9/venv/mkspecs/features/data/configure.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/jupyter/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/jupyter/kernels/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/share/jupyter/kernels/python3/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      257 2022-10-22 12:48:42.000000 dstk_x250-3.8.9/venv/share/jupyter/kernels/python3/kernel.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      846 2022-08-10 10:35:05.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/.eslintrc.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      161 2022-08-10 10:35:05.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/customFormatExample.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.084197 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/debug/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     1152 2022-08-10 10:35:05.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/debug/package.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/nopt/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      522 2022-08-10 10:35:05.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/nopt/package.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     4025 2022-08-10 10:35:05.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/package.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      434 2022-08-10 10:35:06.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/deprecated.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)     5291 2022-08-10 10:35:06.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/index.json
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      793 2022-08-10 10:35:06.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/package.json
+drwxrwxr-x   0 cyriledelestre  (1002) cyriledelestre  (1002)        0 2022-11-08 14:52:59.132199 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/validate-npm-package-license/
+-rw-rw-r--   0 cyriledelestre  (1002) cyriledelestre  (1002)      747 2022-08-10 10:35:06.000000 dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/validate-npm-package-license/package.json
```

### Comparing `dstk_x250-3.8.8/LICENSE.txt` & `dstk_x250-3.8.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/PKG-INFO` & `dstk_x250-3.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstk_x250
-Version: 3.8.8
+Version: 3.8.9
 Summary: Package d'utilitaires pour les projets de data science.
 Home-page: https://gitlab.com/Kirire/x250
 Author: Cyrile Delestre
 Author-email: cyrile.ufr.orsay@gmail.com
 License: Apache Software License 2.0
 Platform: any
 Requires-Python: >=3.5
```

### Comparing `dstk_x250-3.8.8/README.md` & `dstk_x250-3.8.9/README.md`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/data/_pandas_sql.py` & `dstk_x250-3.8.9/dstk/data/_pandas_sql.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/data/_sql.py` & `dstk_x250-3.8.9/dstk/data/_sql.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/features/_prepro.py` & `dstk_x250-3.8.9/dstk/features/_prepro.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/features/_transformers.py` & `dstk_x250-3.8.9/dstk/features/_transformers.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/metrics/_aggregator.py` & `dstk_x250-3.8.9/dstk/metrics/_aggregator.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/metrics/_handlers.py` & `dstk_x250-3.8.9/dstk/metrics/_handlers.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/metrics/_metrics.py` & `dstk_x250-3.8.9/dstk/metrics/_metrics.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/metrics/push.py` & `dstk_x250-3.8.9/dstk/metrics/push.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/ml/_ml.py` & `dstk_x250-3.8.9/dstk/ml/_ml.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/__init__.py` & `dstk_x250-3.8.9/dstk/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_base.py` & `dstk_x250-3.8.9/dstk/pytorch/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,18 +251,14 @@
         ----------
         path_or_bytes : Union[str, ByteString]
             path directory du modèle ou bytes représentant le modèles
         **kargs_load :
             paramètres attachés à Pickle.load(file, **kargs_load) si path ou 
             Pickle.loads(data, **kargs_load) si bytes.
         """
-        # mother_classes = self.__class__.__bases__
-        # dans le cadre d'un apprentissage distribué on ne garantie pas que le
-        # build soit présent (simplifie l'interfaçage entre DSTK et DDP).
-        # if DDP not in mother_classes and not is_dist_avail_and_initialized():
         if not hasattr(self, 'build'):
             raise NotImplementedError(
                 "Le modèle PyTorch n'a pas de méthode build (réf. doc de "
                 "la classe)."
             )
         self.build()
         if isinstance(path_or_bytes, str):
```

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_callback.py` & `dstk_x250-3.8.9/dstk/pytorch/_callback.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_classifier.py` & `dstk_x250-3.8.9/dstk/pytorch/_classifier.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_random_search.py` & `dstk_x250-3.8.9/dstk/pytorch/_random_search.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_regressor.py` & `dstk_x250-3.8.9/dstk/pytorch/_regressor.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_swa.py` & `dstk_x250-3.8.9/dstk/pytorch/_swa.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_utils.py` & `dstk_x250-3.8.9/dstk/pytorch/_utils.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/_utils_distrib.py` & `dstk_x250-3.8.9/dstk/pytorch/_utils_distrib.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,25 @@
 
 Created on Sat Oct 22 14:50:47 2022
 
 @author: Cyrile Delestre
 """
 
 import os
-from typing import Optional, Dict, Any, Callable
-from itertools import product
+from typing import Optional, Dict, Any
 from warnings import warn
 
 import torch
 import torch.distributed as dist
 from torch.nn import Module, SyncBatchNorm
 from torch.nn.parallel import DistributedDataParallel as DDP
 from torch.utils.data import Dataset, DataLoader
 from torch.utils.data.distributed import DistributedSampler
 
 from dstk.pytorch._utils import is_dist_avail_and_initialized
-from dstk.pytorch._base import BaseEnvironnement
-from dstk.pytorch._classifier import BaseClassifier, BaseClassifierOnline
-from dstk.pytorch._regressor import BaseRegressor, BaseRegressorOnline
 
 
 def is_main_process():
     r"""
     Permet de check si le process ce trouve sur le device maître.
     """
     return get_rank() == 0
@@ -84,91 +80,14 @@
         rank=rank
     )
     torch.cuda.set_device(local_rank)
     dist.barrier()
     return local_rank
 
 
-def _overload_distributed_data_parallel(
-    model: Module,
-    master_class: Optional[Callable] = None
-):
-    r"""
-    Fonction qui vien surchargé la classe
-    torch.nn.parallel.DistributedDataParallel afin de s'interfacer avec
-    les classes DSTK. Pour connaitre les arguements de cette classe ce
-    référer à la doc PyTorch.
-
-    Parameters
-    ----------
-    model: Module
-        Modèle PyTorch vania ou hérité des classes DSTK.
-    master_class: Optional[Callable]
-        Classe mère que l'on souhaite faire hérité. Si cette variable est
-        a None une recherce de maching sera exécutée sur les classes types
-        de base de DSTK.
-    """
-    def gen_class(module):
-        class DistributedDataParallel(DDP, module):
-            def __init__(
-                self,
-                module,
-                device_ids=None,
-                output_device=None,
-                dim=0,
-                broadcast_buffers=True,
-                process_group=None,
-                bucket_cap_mb=25,
-                find_unused_parameters=False,
-                check_reduction=False,
-                gradient_as_bucket_view=False,
-                static_graph=False,
-            ):
-                super().__init__(
-                    module=module,
-                    device_ids=device_ids,
-                    output_device=output_device,
-                    dim=dim,
-                    broadcast_buffers=broadcast_buffers,
-                    process_group=process_group,
-                    bucket_cap_mb=bucket_cap_mb,
-                    find_unused_parameters=find_unused_parameters,
-                    check_reduction=check_reduction,
-                    gradient_as_bucket_view=gradient_as_bucket_view,
-                    static_graph=static_graph,
-                )
-        return DistributedDataParallel
-
-    if not master_class is None:
-        return gen_class(master_class)
-
-    mother_model = model.__class__.__bases__
-    dstk_module = [BaseEnvironnement, BaseClassifier, BaseClassifierOnline,
-                   BaseRegressor, BaseRegressorOnline]
-    match = list(
-        filter(
-            lambda x: x[0] == x[1],
-            product(mother_model, dstk_module)
-        )
-    )
-    if len(match) == 0:
-        return DDP
-    elif len(match) == 1:
-        return gen_class(match[0][1])
-    else:
-        match = list(filter(lambda x: x[0] != BaseEnvironnement, match))
-        if len(match) == 1:
-            return gen_class(match[0][1])
-        else:
-            raise AttributeError(
-                "L'héritage du module PyTorch est incompatible avec le "
-                "système d'hérithage de DSTK."
-            )
-
-
 def overload_distributed_data_parallel(model: Module):
     r"""
     Fonction qui vien surchargé la classe
     torch.nn.parallel.DistributedDataParallel afin de s'interfacer avec
     les classes DSTK. Pour connaitre les arguements de cette classe ce
     référer à la doc PyTorch.
 
@@ -201,32 +120,42 @@
                 process_group=process_group,
                 bucket_cap_mb=bucket_cap_mb,
                 find_unused_parameters=find_unused_parameters,
                 check_reduction=check_reduction,
                 gradient_as_bucket_view=gradient_as_bucket_view,
                 static_graph=static_graph,
             )
+
     attr = list(filter(lambda x: not x.startswith('__'), dir(model)))
     attr_ddp = list(filter(lambda x: not x.startswith('__'), dir(DDP)))
     for ii in attr:
         if not ii in attr_ddp:
             setattr(DistributedDataParallel, ii, getattr(model, ii))
+        else:
+            warn(
+                f"L'attribut {ii} est commun à la classe "
+                f"{model.__class__.__name__} et à la classe DPP de PyTorch. "
+                "La prioriété est donnée a DDP et peut ne pas avoir "
+                "d'impacte sur la suite de l'entrainement. Dans le cas "
+                "contraire changer le nom de l'attribut pour ne pas "
+                "rentrer en conflict avec DDP."
+            )
+
     return DistributedDataParallel
 
 
 def auto_init_distributed(
     model: Module,
     train_dataset: Dataset,
     kwargs_train_dataloader: Dict[str, Any],
     eval_dataset: Optional[Dataset] = None,
     kwargs_eval_dataloader: Optional[Dict[str, Any]] = None,
     dist_url: str = "env://",
     backend: str = "nccl",
-    seed: int = 42,
-    master_class: Optional[Callable] = None
+    seed: int = 42
 ):
     r"""
     
     Parameters
     ----------
     model: Module
         Modèle PyTorch a paralléliser.
@@ -248,18 +177,14 @@
         NCCL est spécifique pour le multi-GPU et GLOO spécifique au
         multi-CPU. Voir la documentation PyTorch pour les autres backend
         possible.
     seed: int (=42)
         Seed à destination du DistributedSampler afin de garantir que tous
         les processes aient la même seed pour le mélange (sinon les processes
         pourraient avoir des observations commune dans une eproch).
-    master_class: Optional[Callable]
-        Classe mère que l'on souhaite faire hérité. Si cette variable est
-        a None une recherce de maching sera exécutée sur les classes de types
-        de base de DSTK.
 
     Notes
     -----
     Il est important de bien initialiser PyTorch afin que tous les processes
     soit inialiser avec les mêmes poids aléatoires, sinon l'apprentissage
     sera inconsistant.
 
@@ -283,18 +208,14 @@
         if eval_dataset:
             eval_data = DataLoader(eval_dataset, **kwargs_eval_dataloader)
             return model, train_data, eval_data
         return model, train_data
 
     model = model.cuda()
     model = SyncBatchNorm.convert_sync_batchnorm(model)
-    # model = overload_distributed_data_parallel(model, master_class)(
-    #     module=model,
-    #     device_ids=[local_rank]
-    # )
     model = overload_distributed_data_parallel(model)(
         module=model,
         device_ids=[local_rank]
     )
     shuffle = None
     drop_last = None
     if 'shuffle' in kwargs_train_dataloader:
```

### Comparing `dstk_x250-3.8.8/dstk/pytorch/metrics.py` & `dstk_x250-3.8.9/dstk/pytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/networks.py` & `dstk_x250-3.8.9/dstk/pytorch/networks.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/pytorch/supervision.py` & `dstk_x250-3.8.9/dstk/pytorch/supervision.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/ssh/_ssh.py` & `dstk_x250-3.8.9/dstk/ssh/_ssh.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/ssh/_utils.py` & `dstk_x250-3.8.9/dstk/ssh/_utils.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/__init__.py` & `dstk_x250-3.8.9/dstk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_check.py` & `dstk_x250-3.8.9/dstk/utils/_check.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_chunk.py` & `dstk_x250-3.8.9/dstk/utils/_chunk.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_date.py` & `dstk_x250-3.8.9/dstk/utils/_date.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_rolling.py` & `dstk_x250-3.8.9/dstk/utils/_rolling.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_seed.py` & `dstk_x250-3.8.9/dstk/utils/_seed.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_set_deep_params.py` & `dstk_x250-3.8.9/dstk/utils/_set_deep_params.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_statistique.py` & `dstk_x250-3.8.9/dstk/utils/_statistique.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_timeout.py` & `dstk_x250-3.8.9/dstk/utils/_timeout.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_transpose.py` & `dstk_x250-3.8.9/dstk/utils/_transpose.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/_trie.py` & `dstk_x250-3.8.9/dstk/utils/_trie.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/deprecated.py` & `dstk_x250-3.8.9/dstk/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/errors.py` & `dstk_x250-3.8.9/dstk/utils/errors.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/utils/meta_interface.py` & `dstk_x250-3.8.9/dstk/utils/meta_interface.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/visualization/_bias_analyzer.py` & `dstk_x250-3.8.9/dstk/visualization/_bias_analyzer.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/visualization/_roc_analyser.py` & `dstk_x250-3.8.9/dstk/visualization/_roc_analyser.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk/visualization/statistique.py` & `dstk_x250-3.8.9/dstk/visualization/statistique.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/dstk_x250.egg-info/PKG-INFO` & `dstk_x250-3.8.9/dstk_x250.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dstk-x250
-Version: 3.8.8
+Version: 3.8.9
 Summary: Package d'utilitaires pour les projets de data science.
 Home-page: https://gitlab.com/Kirire/x250
 Author: Cyrile Delestre
 Author-email: cyrile.ufr.orsay@gmail.com
 License: Apache Software License 2.0
 Platform: any
 Requires-Python: >=3.5
```

### Comparing `dstk_x250-3.8.8/dstk_x250.egg-info/SOURCES.txt` & `dstk_x250-3.8.9/dstk_x250.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/setup.py` & `dstk_x250-3.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/_libgcc_mutex-0.1-conda_forge.json` & `dstk_x250-3.8.9/venv/conda-meta/_libgcc_mutex-0.1-conda_forge.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/_openmp_mutex-4.5-2_kmp_llvm.json` & `dstk_x250-3.8.9/venv/conda-meta/_openmp_mutex-4.5-2_kmp_llvm.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/absl-py-1.3.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/absl-py-1.3.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/aiohttp-3.8.1-py38h7f8727e_1.json` & `dstk_x250-3.8.9/venv/conda-meta/aiohttp-3.8.1-py38h7f8727e_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/aiosignal-1.2.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/aiosignal-1.2.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/alabaster-0.7.12-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/alabaster-0.7.12-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/asttokens-2.0.5-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/asttokens-2.0.5-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/async-timeout-4.0.2-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/async-timeout-4.0.2-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/attrs-21.4.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/attrs-21.4.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/babel-2.9.1-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/babel-2.9.1-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/backcall-0.2.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/backcall-0.2.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/blas-2.116-openblas.json` & `dstk_x250-3.8.9/venv/conda-meta/blas-2.116-openblas.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/blas-devel-3.9.0-16_linux64_openblas.json` & `dstk_x250-3.8.9/venv/conda-meta/blas-devel-3.9.0-16_linux64_openblas.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/blinker-1.4-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/blinker-1.4-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/bottleneck-1.3.5-py38h7deecbd_0.json` & `dstk_x250-3.8.9/venv/conda-meta/bottleneck-1.3.5-py38h7deecbd_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/brotli-1.0.9-h5eee18b_7.json` & `dstk_x250-3.8.9/venv/conda-meta/brotli-1.0.9-h5eee18b_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/brotli-bin-1.0.9-h5eee18b_7.json` & `dstk_x250-3.8.9/venv/conda-meta/brotli-bin-1.0.9-h5eee18b_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/brotlipy-0.7.0-py38h27cfd23_1003.json` & `dstk_x250-3.8.9/venv/conda-meta/brotlipy-0.7.0-py38h27cfd23_1003.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/c-ares-1.18.1-h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/c-ares-1.18.1-h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ca-certificates-2022.07.19-h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/ca-certificates-2022.07.19-h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/cachetools-4.2.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/cachetools-4.2.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/certifi-2022.9.24-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/certifi-2022.9.24-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/cffi-1.15.1-py38h74dc2b5_0.json` & `dstk_x250-3.8.9/venv/conda-meta/cffi-1.15.1-py38h74dc2b5_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/charset-normalizer-2.0.4-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/charset-normalizer-2.0.4-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/click-8.0.4-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/click-8.0.4-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/cloudpickle-2.0.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/cloudpickle-2.0.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/colorama-0.4.5-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/colorama-0.4.5-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/cryptography-37.0.1-py38h9ce1e76_0.json` & `dstk_x250-3.8.9/venv/conda-meta/cryptography-37.0.1-py38h9ce1e76_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/cycler-0.11.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/cycler-0.11.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/dataclasses-0.8-pyh6d0b6a4_7.json` & `dstk_x250-3.8.9/venv/conda-meta/dataclasses-0.8-pyh6d0b6a4_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/dbus-1.13.18-hb2f20db_0.json` & `dstk_x250-3.8.9/venv/conda-meta/dbus-1.13.18-hb2f20db_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/debugpy-1.5.1-py38h295c915_0.json` & `dstk_x250-3.8.9/venv/conda-meta/debugpy-1.5.1-py38h295c915_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/decorator-5.1.1-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/decorator-5.1.1-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/docutils-0.16-py38_1.json` & `dstk_x250-3.8.9/venv/conda-meta/docutils-0.16-py38_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/entrypoints-0.4-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/entrypoints-0.4-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/executing-0.8.3-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/executing-0.8.3-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/expat-2.4.9-h6a678d5_0.json` & `dstk_x250-3.8.9/venv/conda-meta/expat-2.4.9-h6a678d5_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/fftw-3.3.9-h27cfd23_1.json` & `dstk_x250-3.8.9/venv/conda-meta/fftw-3.3.9-h27cfd23_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/fontconfig-2.13.1-h6c09931_0.json` & `dstk_x250-3.8.9/venv/conda-meta/fontconfig-2.13.1-h6c09931_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/fonttools-4.25.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/fonttools-4.25.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/freetype-2.11.0-h70c0345_0.json` & `dstk_x250-3.8.9/venv/conda-meta/freetype-2.11.0-h70c0345_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/frozenlist-1.2.0-py38h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/frozenlist-1.2.0-py38h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/giflib-5.2.1-h7b6447c_0.json` & `dstk_x250-3.8.9/venv/conda-meta/giflib-5.2.1-h7b6447c_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/glib-2.69.1-h4ff587b_1.json` & `dstk_x250-3.8.9/venv/conda-meta/glib-2.69.1-h4ff587b_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/google-auth-2.6.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/google-auth-2.6.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/google-auth-oauthlib-0.4.4-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/google-auth-oauthlib-0.4.4-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/greenlet-1.1.1-py38h295c915_0.json` & `dstk_x250-3.8.9/venv/conda-meta/greenlet-1.1.1-py38h295c915_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/grpcio-1.42.0-py38hce63b2e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/grpcio-1.42.0-py38hce63b2e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/gst-plugins-base-1.14.0-h8213a91_2.json` & `dstk_x250-3.8.9/venv/conda-meta/gst-plugins-base-1.14.0-h8213a91_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/gstreamer-1.14.0-h28cd5cc_2.json` & `dstk_x250-3.8.9/venv/conda-meta/gstreamer-1.14.0-h28cd5cc_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/icu-58.2-he6710b0_3.json` & `dstk_x250-3.8.9/venv/conda-meta/icu-58.2-he6710b0_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/idna-3.4-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/idna-3.4-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/imagesize-1.4.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/imagesize-1.4.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/importlib-metadata-4.11.3-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/importlib-metadata-4.11.3-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/intel-openmp-2022.1.0-h9e868ea_3769.json` & `dstk_x250-3.8.9/venv/conda-meta/intel-openmp-2022.1.0-h9e868ea_3769.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ipykernel-6.15.2-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/ipykernel-6.15.2-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ipython-8.4.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/ipython-8.4.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/jedi-0.18.1-py38h06a4308_1.json` & `dstk_x250-3.8.9/venv/conda-meta/jedi-0.18.1-py38h06a4308_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/jinja2-3.0.3-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/jinja2-3.0.3-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/joblib-0.17.0-py_0.json` & `dstk_x250-3.8.9/venv/conda-meta/joblib-0.17.0-py_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/jpeg-9e-h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/jpeg-9e-h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/jupyter_client-7.3.5-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/jupyter_client-7.3.5-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/jupyter_core-4.11.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/jupyter_core-4.11.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/kiwisolver-1.4.2-py38h295c915_0.json` & `dstk_x250-3.8.9/venv/conda-meta/kiwisolver-1.4.2-py38h295c915_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/krb5-1.19.2-hac12032_0.json` & `dstk_x250-3.8.9/venv/conda-meta/krb5-1.19.2-hac12032_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/lcms2-2.12-h3be6417_0.json` & `dstk_x250-3.8.9/venv/conda-meta/lcms2-2.12-h3be6417_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ld_impl_linux-64-2.38-h1181459_1.json` & `dstk_x250-3.8.9/venv/conda-meta/ld_impl_linux-64-2.38-h1181459_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/lerc-3.0-h295c915_0.json` & `dstk_x250-3.8.9/venv/conda-meta/lerc-3.0-h295c915_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libblas-3.9.0-16_linux64_openblas.json` & `dstk_x250-3.8.9/venv/conda-meta/libblas-3.9.0-16_linux64_openblas.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libbrotlicommon-1.0.9-h5eee18b_7.json` & `dstk_x250-3.8.9/venv/conda-meta/libbrotlicommon-1.0.9-h5eee18b_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libbrotlidec-1.0.9-h5eee18b_7.json` & `dstk_x250-3.8.9/venv/conda-meta/libbrotlidec-1.0.9-h5eee18b_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libbrotlienc-1.0.9-h5eee18b_7.json` & `dstk_x250-3.8.9/venv/conda-meta/libbrotlienc-1.0.9-h5eee18b_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libcblas-3.9.0-16_linux64_openblas.json` & `dstk_x250-3.8.9/venv/conda-meta/libcblas-3.9.0-16_linux64_openblas.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libclang-10.0.1-default_hb85057a_2.json` & `dstk_x250-3.8.9/venv/conda-meta/libclang-10.0.1-default_hb85057a_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libdeflate-1.8-h7f8727e_5.json` & `dstk_x250-3.8.9/venv/conda-meta/libdeflate-1.8-h7f8727e_5.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libedit-3.1.20210910-h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libedit-3.1.20210910-h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libevent-2.1.12-h8f2d780_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libevent-2.1.12-h8f2d780_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libffi-3.3-he6710b0_2.json` & `dstk_x250-3.8.9/venv/conda-meta/libffi-3.3-he6710b0_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libgcc-ng-12.2.0-h65d4601_18.json` & `dstk_x250-3.8.9/venv/conda-meta/libgcc-ng-12.2.0-h65d4601_18.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libgfortran-ng-11.2.0-h00389a5_1.json` & `dstk_x250-3.8.9/venv/conda-meta/libgfortran-ng-11.2.0-h00389a5_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libgfortran5-11.2.0-h1234567_1.json` & `dstk_x250-3.8.9/venv/conda-meta/libgfortran5-11.2.0-h1234567_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/liblapack-3.9.0-16_linux64_openblas.json` & `dstk_x250-3.8.9/venv/conda-meta/liblapack-3.9.0-16_linux64_openblas.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/liblapacke-3.9.0-16_linux64_openblas.json` & `dstk_x250-3.8.9/venv/conda-meta/liblapacke-3.9.0-16_linux64_openblas.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libllvm10-10.0.1-hbcb73fb_5.json` & `dstk_x250-3.8.9/venv/conda-meta/libllvm10-10.0.1-hbcb73fb_5.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libopenblas-0.3.21-pthreads_h78a6416_3.json` & `dstk_x250-3.8.9/venv/conda-meta/libopenblas-0.3.21-pthreads_h78a6416_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libpng-1.6.37-hbc83047_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libpng-1.6.37-hbc83047_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libpq-12.9-h16c4e8d_3.json` & `dstk_x250-3.8.9/venv/conda-meta/libpq-12.9-h16c4e8d_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libprotobuf-3.21.7-h6239696_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libprotobuf-3.21.7-h6239696_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libsodium-1.0.18-h7b6447c_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libsodium-1.0.18-h7b6447c_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libstdcxx-ng-12.2.0-h46fd767_18.json` & `dstk_x250-3.8.9/venv/conda-meta/libstdcxx-ng-12.2.0-h46fd767_18.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libtiff-4.4.0-hecacb30_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libtiff-4.4.0-hecacb30_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libuuid-1.0.3-h7f8727e_2.json` & `dstk_x250-3.8.9/venv/conda-meta/libuuid-1.0.3-h7f8727e_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libwebp-1.2.4-h11a3e52_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libwebp-1.2.4-h11a3e52_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libwebp-base-1.2.4-h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libwebp-base-1.2.4-h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libxcb-1.15-h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libxcb-1.15-h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libxkbcommon-1.0.1-hfa300c1_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libxkbcommon-1.0.1-hfa300c1_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libxml2-2.9.14-h74e7548_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libxml2-2.9.14-h74e7548_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libxslt-1.1.35-h4e12654_0.json` & `dstk_x250-3.8.9/venv/conda-meta/libxslt-1.1.35-h4e12654_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/libzlib-1.2.12-h166bdaf_3.json` & `dstk_x250-3.8.9/venv/conda-meta/libzlib-1.2.12-h166bdaf_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/llvm-openmp-14.0.6-h9e868ea_0.json` & `dstk_x250-3.8.9/venv/conda-meta/llvm-openmp-14.0.6-h9e868ea_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/lz4-c-1.9.3-h295c915_1.json` & `dstk_x250-3.8.9/venv/conda-meta/lz4-c-1.9.3-h295c915_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/markdown-3.3.4-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/markdown-3.3.4-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/markupsafe-2.1.1-py38h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/markupsafe-2.1.1-py38h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/matplotlib-3.5.2-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/matplotlib-3.5.2-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/matplotlib-base-3.5.2-py38hf590b9c_0.json` & `dstk_x250-3.8.9/venv/conda-meta/matplotlib-base-3.5.2-py38hf590b9c_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/matplotlib-inline-0.1.6-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/matplotlib-inline-0.1.6-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/mkl-2022.1.0-hc2b9512_224.json` & `dstk_x250-3.8.9/venv/conda-meta/mkl-2022.1.0-hc2b9512_224.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/multidict-6.0.2-py38h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/multidict-6.0.2-py38h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/munkres-1.1.4-py_0.json` & `dstk_x250-3.8.9/venv/conda-meta/munkres-1.1.4-py_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ncurses-6.3-h5eee18b_3.json` & `dstk_x250-3.8.9/venv/conda-meta/ncurses-6.3-h5eee18b_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/nest-asyncio-1.5.5-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/nest-asyncio-1.5.5-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ninja-1.10.2-h06a4308_5.json` & `dstk_x250-3.8.9/venv/conda-meta/ninja-1.10.2-h06a4308_5.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ninja-base-1.10.2-hd09550d_5.json` & `dstk_x250-3.8.9/venv/conda-meta/ninja-base-1.10.2-hd09550d_5.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/nspr-4.33-h295c915_0.json` & `dstk_x250-3.8.9/venv/conda-meta/nspr-4.33-h295c915_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/nss-3.74-h0370c37_0.json` & `dstk_x250-3.8.9/venv/conda-meta/nss-3.74-h0370c37_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/numexpr-2.8.3-py38hd2a5715_0.json` & `dstk_x250-3.8.9/venv/conda-meta/numexpr-2.8.3-py38hd2a5715_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/numpy-1.23.3-py38hf838250_0.json` & `dstk_x250-3.8.9/venv/conda-meta/numpy-1.23.3-py38hf838250_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/numpy-base-1.23.3-py38h1e6e340_0.json` & `dstk_x250-3.8.9/venv/conda-meta/numpy-base-1.23.3-py38h1e6e340_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/numpydoc-1.4.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/numpydoc-1.4.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/oauthlib-3.2.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/oauthlib-3.2.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/openblas-0.3.21-pthreads_h320a7e8_3.json` & `dstk_x250-3.8.9/venv/conda-meta/openblas-0.3.21-pthreads_h320a7e8_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/openssl-1.1.1q-h7f8727e_0.json` & `dstk_x250-3.8.9/venv/conda-meta/openssl-1.1.1q-h7f8727e_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/packaging-21.3-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/packaging-21.3-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pandas-1.4.4-py38h6a678d5_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pandas-1.4.4-py38h6a678d5_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/parso-0.8.3-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/parso-0.8.3-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pcre-8.45-h295c915_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pcre-8.45-h295c915_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pexpect-4.8.0-pyhd3eb1b0_3.json` & `dstk_x250-3.8.9/venv/conda-meta/pexpect-4.8.0-pyhd3eb1b0_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pickleshare-0.7.5-pyhd3eb1b0_1003.json` & `dstk_x250-3.8.9/venv/conda-meta/pickleshare-0.7.5-pyhd3eb1b0_1003.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pillow-9.2.0-py38hace64e9_1.json` & `dstk_x250-3.8.9/venv/conda-meta/pillow-9.2.0-py38hace64e9_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pip-22.2.2-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pip-22.2.2-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ply-3.11-py38_0.json` & `dstk_x250-3.8.9/venv/conda-meta/ply-3.11-py38_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/prompt-toolkit-3.0.20-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/prompt-toolkit-3.0.20-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/protobuf-4.21.7-py38hfa26641_0.json` & `dstk_x250-3.8.9/venv/conda-meta/protobuf-4.21.7-py38hfa26641_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/psutil-5.9.0-py38h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/psutil-5.9.0-py38h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/ptyprocess-0.7.0-pyhd3eb1b0_2.json` & `dstk_x250-3.8.9/venv/conda-meta/ptyprocess-0.7.0-pyhd3eb1b0_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pure_eval-0.2.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pure_eval-0.2.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyasn1-0.4.8-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pyasn1-0.4.8-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyasn1-modules-0.2.8-py_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pyasn1-modules-0.2.8-py_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pycparser-2.21-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pycparser-2.21-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pygments-2.11.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pygments-2.11.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyjwt-2.4.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pyjwt-2.4.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyopenssl-22.0.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pyopenssl-22.0.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyparsing-3.0.9-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pyparsing-3.0.9-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyqt-5.15.7-py38h6a678d5_1.json` & `dstk_x250-3.8.9/venv/conda-meta/pyqt-5.15.7-py38h6a678d5_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyqt5-sip-12.11.0-py38h6a678d5_1.json` & `dstk_x250-3.8.9/venv/conda-meta/pyqt5-sip-12.11.0-py38h6a678d5_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pysocks-1.7.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pysocks-1.7.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/python-3.8.13-h12debd9_0.json` & `dstk_x250-3.8.9/venv/conda-meta/python-3.8.13-h12debd9_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/python-dateutil-2.8.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/python-dateutil-2.8.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/python_abi-3.8-2_cp38.json` & `dstk_x250-3.8.9/venv/conda-meta/python_abi-3.8-2_cp38.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pytorch-1.12.1-cpu_py38h23e632a_1.json` & `dstk_x250-3.8.9/venv/conda-meta/pytorch-1.12.1-cpu_py38h23e632a_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pytz-2022.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pytz-2022.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/pyzmq-23.2.0-py38h6a678d5_0.json` & `dstk_x250-3.8.9/venv/conda-meta/pyzmq-23.2.0-py38h6a678d5_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/qt-main-5.15.2-h327a75a_7.json` & `dstk_x250-3.8.9/venv/conda-meta/qt-main-5.15.2-h327a75a_7.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/qt-webengine-5.15.9-hd2b0992_4.json` & `dstk_x250-3.8.9/venv/conda-meta/qt-webengine-5.15.9-hd2b0992_4.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/qtwebkit-5.212-h4eab89a_4.json` & `dstk_x250-3.8.9/venv/conda-meta/qtwebkit-5.212-h4eab89a_4.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/readline-8.1.2-h7f8727e_1.json` & `dstk_x250-3.8.9/venv/conda-meta/readline-8.1.2-h7f8727e_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/requests-2.28.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/requests-2.28.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/requests-oauthlib-1.3.0-py_0.json` & `dstk_x250-3.8.9/venv/conda-meta/requests-oauthlib-1.3.0-py_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/rsa-4.7.2-pyhd3eb1b0_1.json` & `dstk_x250-3.8.9/venv/conda-meta/rsa-4.7.2-pyhd3eb1b0_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/scikit-learn-0.24.2-py38ha9443f7_0.json` & `dstk_x250-3.8.9/venv/conda-meta/scikit-learn-0.24.2-py38ha9443f7_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/scipy-1.9.1-py38h32ae08f_0.json` & `dstk_x250-3.8.9/venv/conda-meta/scipy-1.9.1-py38h32ae08f_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/setuptools-63.4.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/setuptools-63.4.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sip-6.6.2-py38h6a678d5_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sip-6.6.2-py38h6a678d5_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/six-1.16.0-pyhd3eb1b0_1.json` & `dstk_x250-3.8.9/venv/conda-meta/six-1.16.0-pyhd3eb1b0_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sleef-3.5.1-h9b69904_2.json` & `dstk_x250-3.8.9/venv/conda-meta/sleef-3.5.1-h9b69904_2.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/snowballstemmer-2.2.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/snowballstemmer-2.2.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinx-3.3.1-pyhd8ed1ab_1.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinx-3.3.1-pyhd8ed1ab_1.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-applehelp-1.0.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-applehelp-1.0.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-devhelp-1.0.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-devhelp-1.0.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-htmlhelp-2.0.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-htmlhelp-2.0.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-jsmath-1.0.1-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-jsmath-1.0.1-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-qthelp-1.0.3-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-qthelp-1.0.3-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sphinxcontrib-serializinghtml-1.1.5-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sphinxcontrib-serializinghtml-1.1.5-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/spyder-kernels-1.10.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/spyder-kernels-1.10.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sqlalchemy-1.4.39-py38h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sqlalchemy-1.4.39-py38h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/sqlite-3.39.3-h5082296_0.json` & `dstk_x250-3.8.9/venv/conda-meta/sqlite-3.39.3-h5082296_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/stack_data-0.2.0-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/stack_data-0.2.0-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/tensorboard-2.9.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/tensorboard-2.9.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/tensorboard-data-server-0.6.0-py38hca6d32c_0.json` & `dstk_x250-3.8.9/venv/conda-meta/tensorboard-data-server-0.6.0-py38hca6d32c_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/tensorboard-plugin-wit-1.8.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/tensorboard-plugin-wit-1.8.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/threadpoolctl-2.2.0-pyh0d69192_0.json` & `dstk_x250-3.8.9/venv/conda-meta/threadpoolctl-2.2.0-pyh0d69192_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/tk-8.6.12-h1ccaba5_0.json` & `dstk_x250-3.8.9/venv/conda-meta/tk-8.6.12-h1ccaba5_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/toml-0.10.2-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/toml-0.10.2-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/torchvision-0.13.0-cpu_py38h08bc92c_0.json` & `dstk_x250-3.8.9/venv/conda-meta/torchvision-0.13.0-cpu_py38h08bc92c_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/tornado-6.2-py38h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/tornado-6.2-py38h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/tqdm-4.64.1-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/tqdm-4.64.1-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/traitlets-5.1.1-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/traitlets-5.1.1-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/typing_extensions-4.3.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/typing_extensions-4.3.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/urllib3-1.26.12-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/urllib3-1.26.12-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/wcwidth-0.2.5-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/wcwidth-0.2.5-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/werkzeug-2.0.3-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/werkzeug-2.0.3-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json` & `dstk_x250-3.8.9/venv/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/wurlitzer-3.0.2-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/wurlitzer-3.0.2-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/xz-5.2.6-h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/xz-5.2.6-h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/yarl-1.8.1-py38h5eee18b_0.json` & `dstk_x250-3.8.9/venv/conda-meta/yarl-1.8.1-py38h5eee18b_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/zeromq-4.3.4-h2531618_0.json` & `dstk_x250-3.8.9/venv/conda-meta/zeromq-4.3.4-h2531618_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/zipp-3.8.0-py38h06a4308_0.json` & `dstk_x250-3.8.9/venv/conda-meta/zipp-3.8.0-py38h06a4308_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/zlib-1.2.12-h5eee18b_3.json` & `dstk_x250-3.8.9/venv/conda-meta/zlib-1.2.12-h5eee18b_3.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/conda-meta/zstd-1.5.2-ha4553b6_0.json` & `dstk_x250-3.8.9/venv/conda-meta/zstd-1.5.2-ha4553b6_0.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5core_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5core_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5gui_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5gui_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5qml_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5qml_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5qmlmodels_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5qmlmodels_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5qmlworkerscript_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5qmlworkerscript_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5quick_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5quick_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5quickparticles_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5quickparticles_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5quickshapes_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5quickshapes_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5quicktest_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5quicktest_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/metatypes/qt5widgets_metatypes.json` & `dstk_x250-3.8.9/venv/lib/metatypes/qt5widgets_metatypes.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocol.json` & `dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocol.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocolCustom.json` & `dstk_x250-3.8.9/venv/lib/python3.8/site-packages/debugpy/_vendored/pydevd/_pydevd_bundle/_debug_adapter/debugProtocolCustom.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/package.json` & `dstk_x250-3.8.9/venv/lib/python3.8/site-packages/matplotlib/backends/web_backend/package.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/lib/python3.8/site-packages/scipy/stats/tests/data/studentized_range_mpmath_ref.json` & `dstk_x250-3.8.9/venv/lib/python3.8/site-packages/scipy/stats/tests/data/studentized_range_mpmath_ref.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/mkspecs/features/data/configure.json` & `dstk_x250-3.8.9/venv/mkspecs/features/data/configure.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/.eslintrc.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/.eslintrc.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/debug/package.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/debug/package.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/nopt/package.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/node_modules/nopt/package.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/package.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/license-checker/package.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/index.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/index.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/package.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/spdx-license-ids/package.json`

 * *Files identical despite different names*

### Comparing `dstk_x250-3.8.8/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/validate-npm-package-license/package.json` & `dstk_x250-3.8.9/venv/share/qt/3rd_party_licenses/qtwebengine/src/3rdparty/chromium/third_party/devtools-frontend/src/node_modules/validate-npm-package-license/package.json`

 * *Files identical despite different names*

