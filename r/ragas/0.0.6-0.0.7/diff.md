# Comparing `tmp/ragas-0.0.6.tar.gz` & `tmp/ragas-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.6.tar", last modified: Sat Jul 15 06:28:35 2023, max compression
+gzip compressed data, was "ragas-0.0.7.tar", last modified: Thu Jul 20 16:46:52 2023, max compression
```

## Comparing `ragas-0.0.6.tar` & `ragas-0.0.7.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:22.000000 ragas-0.0.6/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.619446 ragas-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-15 06:28:22.000000 ragas-0.0.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-15 06:28:22.000000 ragas-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-15 06:28:22.000000 ragas-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 06:28:22.000000 ragas-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-15 06:28:22.000000 ragas-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-15 06:28:35.631446 ragas-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-15 06:28:22.000000 ragas-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/assets/bar-graph.svg
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/guides/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/metrics.md
--rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-15 06:28:22.000000 ragas-0.0.6/docs/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.627446 ragas-0.0.6/experiments/assesments/
--rw-r--r--   0 runner    (1001) docker     (123)    47692 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/assesments/metrics_assesments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.623446 ragas-0.0.6/experiments/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/experiments/baselines/fiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/fiqa/improving-baselines.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/experiments/baselines/hotpotqa/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/hotpotqa/explore-dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/experiments/baselines/wikiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-15 06:28:22.000000 ragas-0.0.6/experiments/baselines/wikiqa/failed_wikis
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-15 06:28:22.000000 ragas-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-15 06:28:22.000000 ragas-0.0.6/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-15 06:28:22.000000 ragas-0.0.6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-15 06:28:22.000000 ragas-0.0.6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 06:28:35.631446 ragas-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.623446 ragas-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7640 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/context_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/faithfulnes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/metrics/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-15 06:28:22.000000 ragas-0.0.6/src/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 06:28:35.000000 ragas-0.0.6/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.623446 ragas-0.0.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 06:28:35.631446 ragas-0.0.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-15 06:28:22.000000 ragas-0.0.6/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:38.000000 ragas-0.0.7/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-07-20 16:46:38.000000 ragas-0.0.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-07-20 16:46:38.000000 ragas-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-07-20 16:46:38.000000 ragas-0.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 16:46:38.000000 ragas-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-20 16:46:38.000000 ragas-0.0.7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-20 16:46:52.878661 ragas-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-20 16:46:38.000000 ragas-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/assets/bar-graph.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/guides/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/guides/llms.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/metrics.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-20 16:46:38.000000 ragas-0.0.7/docs/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/assesments/
+-rw-r--r--   0 runner    (1001) docker     (123)    47837 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/assesments/metrics_assesments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/experiments/baselines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/baselines/fiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    47254 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/fiqa/improving-baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/baselines/hotpotqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/hotpotqa/explore-dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/experiments/baselines/wikiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 16:46:38.000000 ragas-0.0.7/experiments/baselines/wikiqa/failed_wikis
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-20 16:46:38.000000 ragas-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-20 16:46:38.000000 ragas-0.0.7/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.874661 ragas-0.0.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:46:38.000000 ragas-0.0.7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-20 16:46:38.000000 ragas-0.0.7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 16:46:52.878661 ragas-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/async_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/context_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/faithfulnes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/metrics/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-20 16:46:38.000000 ragas-0.0.7/src/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 16:46:52.000000 ragas-0.0.7/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.870660 ragas-0.0.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:46:52.878661 ragas-0.0.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 16:46:38.000000 ragas-0.0.7/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.6/.github/workflows/ci.yaml` & `ragas-0.0.7/.github/workflows/ci.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -34,29 +34,28 @@
               - .github/workflows/ci.yml
               - codecov.yml
               - pyproject.toml
               - requirements/test.txt
             ragas:
               - "src/ragas/**"
               - "tests/**"
-              - "examples/**"
             docs:
               - *related
               - requirements/docs-requirements.txt
               - "docs/**"
 
   unit_tests:
     needs:
       - diff
 
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10"]
 
     if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.ragas == 'true') || github.event_name == 'push' }}
     name: python${{ matrix.python-version }}_unit_tests (${{ matrix.os }})
     runs-on: ${{ matrix.os }}
 
     steps:
       - uses: actions/checkout@v3
@@ -82,23 +81,24 @@
           key: ${{ runner.os }}-tests-${{ hashFiles('requirements/test.txt') }}
 
       - name: Install dependencies
         run: |
           pip install "."
           pip install -r requirements/test.txt
 
+
       - name: Run unit tests
         run: |
           # OPTS=(--cov-config pyproject.toml --cov=src/bentoml --cov-append)
           if [ "${{ matrix.os }}" != 'windows-latest' ]; then
             # we will use pytest-xdist to improve tests run-time.
             OPTS=(--dist loadfile -n auto)
           fi
           # Now run the unit tests
-          pytest tests/unit "${OPTS[@]}"
+          OPENAI_API_KEY="test" pytest tests/unit "${OPTS[@]}"
 
   codestyle_check:
     runs-on: ubuntu-latest
     needs:
       - diff
 
     if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.ragas == 'true') || github.event_name == 'push' }}
```

### Comparing `ragas-0.0.6/.github/workflows/python-publish.yml` & `ragas-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/.gitignore` & `ragas-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/LICENSE` & `ragas-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/Makefile` & `ragas-0.0.7/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/PKG-INFO` & `ragas-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.6 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.7 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
```

### Comparing `ragas-0.0.6/README.md` & `ragas-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/docs/assets/bar-graph.svg` & `ragas-0.0.7/docs/assets/bar-graph.svg`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/docs/assets/logo.png` & `ragas-0.0.7/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/docs/guides/data_prep.py` & `ragas-0.0.7/docs/guides/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/docs/metrics.md` & `ragas-0.0.7/docs/metrics.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/docs/quickstart.ipynb` & `ragas-0.0.7/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/experiments/README.md` & `ragas-0.0.7/experiments/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/experiments/assesments/metrics_assesments.ipynb` & `ragas-0.0.7/experiments/assesments/metrics_assesments.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998789607717445%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(2, \'\\n\'), (6, \'    model="gpt-3.5-turbo",\\n\'), (7, '*

 * *            '\'    messages=[\\n\'), (8, \'        {"role": "system", "content": "You are a '*

 * *            'helpful assistant."},\\n\'), (9, \'    ],\\n\'), (12, '*

 * *            "'print(completion.choices[0].message)')], delete: [11, 8, 7, 6, 5]}}, 7: {'source': "*

 * *            '{insert: [(2, \'        model=kwargs.get("model", "gpt-3.5-turbo-16k"),\\n\'), (3, '*

 * *            '\'        messages=[{"role": "system",  […]*

```diff
@@ -102,47 +102,48 @@
                         "}\n"
                     ]
                 }
             ],
             "source": [
                 "import os\n",
                 "import openai\n",
+                "\n",
                 "openai.api_key = os.getenv(\"OPENAI_API_KEY\")\n",
                 "\n",
                 "completion = openai.ChatCompletion.create(\n",
-                "  model=\"gpt-3.5-turbo\",\n",
-                "  messages=[\n",
-                "    {\"role\": \"system\", \"content\": \"You are a helpful assistant.\"},\n",
-                "  ]\n",
+                "    model=\"gpt-3.5-turbo\",\n",
+                "    messages=[\n",
+                "        {\"role\": \"system\", \"content\": \"You are a helpful assistant.\"},\n",
+                "    ],\n",
                 ")\n",
                 "\n",
-                "print(completion.choices[0].message)\n"
+                "print(completion.choices[0].message)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 13,
             "id": "4bce4c53",
             "metadata": {},
             "outputs": [],
             "source": [
-                "\n",
                 "def llm2(prompt, **kwargs):\n",
                 "    response = openai.ChatCompletion.create(\n",
-                "        model=kwargs.get(\"model\",\"gpt-3.5-turbo-16k\"),\n",
-                "        messages=[{\"role\": \"system\", \"content\":prompt}],\n",
+                "        model=kwargs.get(\"model\", \"gpt-3.5-turbo-16k\"),\n",
+                "        messages=[{\"role\": \"system\", \"content\": prompt}],\n",
                 "        temperature=kwargs.get(\"temperature\", 0),\n",
                 "        top_p=kwargs.get(\"top_p\", 1),\n",
                 "        frequency_penalty=kwargs.get(\"frequency_penalty\", 0.0),\n",
                 "        presence_penalty=kwargs.get(\"presence_penalty\", 0.0),\n",
                 "        max_tokens=kwargs.get(\"max_tokens\", 500),\n",
                 "        n=kwargs.get(\"n\", 1),\n",
                 "    )\n",
                 "    return response\n",
                 "\n",
+                "\n",
                 "def llm(prompt, **kwargs):\n",
                 "    response = openai.Completion.create(\n",
                 "        model=kwargs.get(\"model\", \"text-davinci-003\"),\n",
                 "        prompt=prompt,\n",
                 "        temperature=kwargs.get(\"temperature\", 0),\n",
                 "        top_p=kwargs.get(\"top_p\", 1),\n",
                 "        frequency_penalty=kwargs.get(\"frequency_penalty\", 0.0),\n",
@@ -371,15 +372,15 @@
                     },
                     "execution_count": 22,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "llm2([Question_generation.format(2,answer)])"
+                "llm2([Question_generation.format(2, answer)])"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e2078ece",
             "metadata": {},
             "source": [
@@ -1035,18 +1036,20 @@
                     "text": [
                         "                                                                                        \r"
                     ]
                 }
             ],
             "source": [
                 "def get_all_facts(item):\n",
-                "    all_facts = item['context']['sentences']\n",
+                "    all_facts = item[\"context\"][\"sentences\"]\n",
                 "    all_facts = [sent for para in all_facts for sent in para]\n",
-                "    return {\"full_context\":''.join(all_facts)}\n",
-                "hotpot_qa = hotpot_qa.map(get_all_facts, batched=False)   "
+                "    return {\"full_context\": \"\".join(all_facts)}\n",
+                "\n",
+                "\n",
+                "hotpot_qa = hotpot_qa.map(get_all_facts, batched=False)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 73,
             "id": "f26aec50",
             "metadata": {},
@@ -1086,16 +1089,16 @@
         {
             "cell_type": "code",
             "execution_count": 179,
             "id": "f649eaf8",
             "metadata": {},
             "outputs": [],
             "source": [
-                "i=15\n",
-                "q,c = hotpot_qa[i]['question'],hotpot_qa[i]['full_context']"
+                "i = 15\n",
+                "q, c = hotpot_qa[i][\"question\"], hotpot_qa[i][\"full_context\"]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 183,
             "id": "b9f5e0b4",
             "metadata": {},
@@ -1108,39 +1111,40 @@
             "cell_type": "code",
             "execution_count": 349,
             "id": "b711de8a",
             "metadata": {},
             "outputs": [],
             "source": [
                 "q = \"what is general relativity?\"\n",
-                "n=2"
+                "n = 2"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 300,
             "id": "11a83f10",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import wikipediaapi\n",
+                "\n",
                 "wiki_wiki = wikipediaapi.Wikipedia(\n",
-                "        language='en',\n",
-                "        extract_format=wikipediaapi.ExtractFormat.WIKI\n",
+                "    language=\"en\", extract_format=wikipediaapi.ExtractFormat.WIKI\n",
                 ")\n",
                 "\n",
                 "p_wiki = wiki_wiki.page(\"Black hole\")\n",
                 "\n",
+                "\n",
                 "def get_page_section(page, section):\n",
                 "    all_text = \"\"\n",
                 "    p_wiki = wiki_wiki.page(page)\n",
                 "    sections = p_wiki.sections_by_title(section)\n",
                 "    for s in sections:\n",
                 "        all_text += s.full_text()\n",
-                "    return all_text\n"
+                "    return all_text"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 21,
             "id": "2755ba79",
             "metadata": {},
@@ -1148,108 +1152,113 @@
             "source": [
                 "from typing import List\n",
                 "from itertools import combinations\n",
                 "from sentence_transformers import CrossEncoder\n",
                 "\n",
                 "cross_encoder = CrossEncoder(\"cross-encoder/stsb-TinyBERT-L-4\")\n",
                 "\n",
-                "        \n",
+                "\n",
                 "def sent_tokenize(sent):\n",
-                "    return [s[:-1] if  s.endswith('.') else s for s in sent.strip().split('. ')]\n",
+                "    return [s[:-1] if s.endswith(\".\") else s for s in sent.strip().split(\". \")]\n",
+                "\n",
                 "\n",
                 "class SentenceAgreement:\n",
-                "    \n",
                 "    def __init__(self, scoring=\"bert_score\"):\n",
-                "        \n",
                 "        self.scoring = scoring\n",
                 "\n",
-                "        \n",
                 "    @staticmethod\n",
                 "    def bert_score(para1, para2):\n",
-                "        \n",
                 "        sentences1, sentences2 = sent_tokenize(para1), sent_tokenize(para2)\n",
                 "        scores = cross_encoder.predict(list(itertools.product(sentences1, sentences2)))\n",
                 "        scores = scores.reshape(len(sentences1), len(sentences2))\n",
                 "        return scores.max(axis=1).mean()\n",
                 "\n",
                 "    @staticmethod\n",
                 "    def jaccard_score(para1, para2):\n",
-                "        \n",
                 "        sentences1, sentences2 = sent_tokenize(para1), sent_tokenize(para2)\n",
                 "        intersect = len(np.intersect1d(sentences1, sentences2))\n",
                 "        union = len(np.union1d(sentences1, sentences2))\n",
-                "        return intersect/union\n",
-                "    \n",
-                "    def evaluate(self,answers:List[List[str]]):\n",
-                "        \n",
+                "        return intersect / union\n",
+                "\n",
+                "    def evaluate(self, answers: List[List[str]]):\n",
                 "        \"\"\"\n",
                 "        eval nC2 combinations\n",
                 "        \"\"\"\n",
                 "        scores = []\n",
-                "        groups = combinations(answers,2)\n",
+                "        groups = combinations(answers, 2)\n",
                 "        for group in groups:\n",
                 "            if self.scoring == \"jaccard\":\n",
                 "                score = self.jaccard_score(*group)\n",
                 "            elif self.scoring == \"bert_score\":\n",
                 "                score = self.bert_score(*group)\n",
                 "            scores.append(score)\n",
-                "        return np.mean(scores)\n",
-                "            "
+                "        return np.mean(scores)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "id": "8d3aa09e",
             "metadata": {},
             "outputs": [],
             "source": [
                 "class ContextRelevacy:\n",
-                "    \n",
-                "    def __init__(self, strictness = 2, agreement_metric=\"bert_score\"):\n",
-                "        \n",
+                "    def __init__(self, strictness=2, agreement_metric=\"bert_score\"):\n",
                 "        self.strictness = strictness\n",
                 "        self.sent_agreement = SentenceAgreement(agreement_metric)\n",
-                "        \n",
-                "    def score(self,question,context):\n",
+                "\n",
+                "    def score(self, question, context):\n",
                 "        scores = []\n",
-                "        outputs = llm(Context_relevency.format(q,c),n=self.strictness,temperature=1)\n",
-                "        outputs = [outputs['choices'][i]['text'].strip() for i in range(self.strictness)]\n",
+                "        outputs = llm(Context_relevency.format(q, c), n=self.strictness, temperature=1)\n",
+                "        outputs = [\n",
+                "            outputs[\"choices\"][i][\"text\"].strip() for i in range(self.strictness)\n",
+                "        ]\n",
                 "        context_sents = sent_tokenize(context)\n",
                 "        for output in outputs:\n",
-                "            indices = [context.find(sent) for sent in sent_tokenize(output) if context.find(sent)!=-1]\n",
-                "            scores.append(len(indices)/len(context_sents))\n",
-                "        \n",
+                "            indices = [\n",
+                "                context.find(sent)\n",
+                "                for sent in sent_tokenize(output)\n",
+                "                if context.find(sent) != -1\n",
+                "            ]\n",
+                "            scores.append(len(indices) / len(context_sents))\n",
+                "\n",
                 "        if self.strictness > 1:\n",
                 "            agr_score = self.sent_agreement.evaluate(outputs)\n",
                 "        else:\n",
-                "            agr_score =1 \n",
-                "        return agr_score * np.mean(scores)\n"
+                "            agr_score = 1\n",
+                "        return agr_score * np.mean(scores)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 491,
             "id": "6985c4bf",
             "metadata": {},
             "outputs": [],
             "source": [
                 "c = get_page_section(\"HIV/AIDS\", \"Prevention\")\n",
-                "c = ' '.join(c.split(' ')[:500])\n",
+                "c = \" \".join(c.split(\" \")[:500])\n",
                 "q = \"When was the first HIV case detected?\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 501,
             "id": "689e1aca",
             "metadata": {},
             "outputs": [],
             "source": [
-                "output = llm([Context_relevency.format(q,c), Context_relevency.format(\"How to prevent AIDS?\",c)],n=n,temperature=1)"
+                "output = llm(\n",
+                "    [\n",
+                "        Context_relevency.format(q, c),\n",
+                "        Context_relevency.format(\"How to prevent AIDS?\", c),\n",
+                "    ],\n",
+                "    n=n,\n",
+                "    temperature=1,\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "id": "a6aee1fa",
             "metadata": {},
@@ -1393,15 +1402,15 @@
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "context_relevancy.score(dataset[\"baseline\"].select(range(0,3)))"
+                "context_relevancy.score(dataset[\"baseline\"].select(range(0, 3)))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "id": "07a4a2ba",
             "metadata": {},
@@ -1487,15 +1496,15 @@
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "context_relevancy.score(dataset[\"baseline\"].select(range(0,3)))"
+                "context_relevancy.score(dataset[\"baseline\"].select(range(0, 3)))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "364d9627",
             "metadata": {},
```

### Comparing `ragas-0.0.6/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.7/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/experiments/baselines/fiqa/improving-baselines.ipynb` & `ragas-0.0.7/experiments/baselines/fiqa/improving-baselines.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/experiments/baselines/hotpotqa/explore-dataset.ipynb` & `ragas-0.0.7/experiments/baselines/hotpotqa/explore-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.7/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/pyproject.toml` & `ragas-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 name = "ragas"
 dependencies = [
     "numpy",
     "transformers",
     "sentence-transformers",
     "datasets",
     "protobuf<=3.20.0",
-    "backoff",
+    "langchain>=0.0.218",
     "openai",
+    "pydantic<2.0"
 ]
 dynamic = ["version", "readme"]
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
```

### Comparing `ragas-0.0.6/references.md` & `ragas-0.0.7/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/src/ragas/_analytics.py` & `ragas-0.0.7/src/ragas/_analytics.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/src/ragas/evaluation.py` & `ragas-0.0.7/src/ragas/evaluation.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/src/ragas/metrics/answer_relevance.py` & `ragas-0.0.7/src/ragas/metrics/answer_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/src/ragas/metrics/base.py` & `ragas-0.0.7/src/ragas/metrics/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 import typing as t
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from math import floor
 
 from datasets import Dataset
+from langchain.chat_models.base import BaseChatModel
+from langchain.llms.base import BaseLLM
 
 
 def make_batches(total_size: int, batch_size: int) -> list[range]:
     """
     Take a total size and batch size and return a list of ranges for the batches
     """
     tail = total_size % batch_size
@@ -27,25 +29,26 @@
         batches.append(range(batch_size * num_batches, batch_size * num_batches + tail))
 
     return batches
 
 
 @dataclass
 class Metric(ABC):
-    @property
-    @abstractmethod
-    def batch_size(self: t.Self) -> int:
-        ...
+    batch_size: int
+    llm: t.Optional[BaseLLM | BaseChatModel] = None
+
+    def __post_init__(self: t.Self):
+        if self.llm is None:
+            from langchain.chat_models import ChatOpenAI
+
+            self.llm = ChatOpenAI(model_name="gpt-3.5-turbo-16k")  # type: ignore
 
     @property
     @abstractmethod
-    def name(self: t.Self) -> str:
-        """
-        the metric name
-        """
+    def name(self) -> str:
         ...
 
     @abstractmethod
     def init_model():
         """
         This method will lazy initialize the model.
         """
```

### Comparing `ragas-0.0.6/src/ragas/metrics/context_relevance.py` & `ragas-0.0.7/src/ragas/metrics/context_relevance.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,37 +3,42 @@
 import typing as t
 from dataclasses import dataclass
 from itertools import combinations, product
 from typing import List
 
 import numpy as np
 from datasets import Dataset
+from langchain.chat_models.base import BaseChatModel
+from langchain.llms.base import BaseLLM
+from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 from sentence_transformers import CrossEncoder
 from tqdm import tqdm
 
 from ragas.metrics.base import Metric
-from ragas.metrics.llms import openai_completion
+from ragas.metrics.llms import generate
 
-CONTEXT_RELEVANCE = """
+CONTEXT_RELEVANCE = HumanMessagePromptTemplate.from_template(
+    """\
 Task: Candidate sentence extraction.
 Given the question and context, extract minimum number of sentences from context required to answer the question. If the context do not contain information required to answer the question return "No candidate sentences found".
 
 question: Which equation is known as worlds most famous equation?
 context:\nAlbert Einstein (14 March 1879 – 18 April 1955) was a German-born theoretical physicist,[5] widely ranked among the greatest and most influential scientists of all time. Best known for developing the theory of relativity, he also made important contributions to quantum mechanics, and was thus a central figure in the revolutionary reshaping of the scientific understanding of nature that modern physics accomplished in the first decades of the twentieth century.
 His mass–energy equivalence formula E = mc2, which arises from relativity theory, has been called "the world's most famous equation".
 sentences:His mass–energy equivalence formula E = mc2, which arises from relativity theory, has been called "the world's most famous equation".
 
 question: Were Scott Derrickson and Ed Wood of the same nationality?
 context :\nScott Derrickson (born July 16, 1966) is an American director, screenwriter and producer He lives in Los Angeles, California He is best known for directing horror films such as "Sinister", "The Exorcism of Emily Rose", and "Deliver Us From Evil", as well as the 2016 Marvel Cinematic Universe installment, "Doctor Strange"Tyler Bates is an American musician, music producer, and composer for films, television, and video games. Adam Collis is an American filmmaker and actor.Conrad Brooks is an American actor.Edward Davis Wood Jr. (October 10, 1924 – December 10, 1978) was an American filmmaker, actor, writer, producer, and director.
 Now given a question and context, extract the minimum number of sentences from the given context required to answer the question completely. 
 sentences:Scott Derrickson (born July 16, 1966) is an American director, screenwriter and producer. Edward Davis Wood Jr. (October 10, 1924 – December 10, 1978) was an American filmmaker, actor, writer, producer, and director.
 
-question:{}
-context:\n{}
+question:{question}
+context:\n{context}
 sentences:"""  # noqa: E501
+)
 
 
 def sent_tokenize(sent: str) -> List[str]:
     return [s[:-1] if s.endswith(".") else s for s in sent.strip().split(". ")]
 
 
 class SentenceAgreement:
@@ -57,15 +62,15 @@
     @staticmethod
     def jaccard_score(para1: str, para2: str) -> float:
         sentences1, sentences2 = sent_tokenize(para1), sent_tokenize(para2)
         intersect = len(np.intersect1d(sentences1, sentences2))
         union = len(np.union1d(sentences1, sentences2))
         return intersect / union
 
-    def evaluate(self, answers: List[List[str]]) -> np.float_:
+    def evaluate(self, answers: List[str]) -> np.float_:
         """
         eval nC2 combinations
         """
         scores = []
         groups = combinations(answers, 2)
         for group in groups:
             if self.metric == "jaccard":
@@ -99,23 +104,25 @@
         samples.
     model_name : str
         any encoder model. Used for calculating bert_score.
     """
 
     name: str = "context_relavency"
     batch_size: int = 15
+    llm: t.Optional[BaseLLM | BaseChatModel] = None
     strictness: int = 2
     agreement_metric: str = "bert_score"
     model_name: str = "cross-encoder/stsb-TinyBERT-L-4"
 
     def __post_init__(self: t.Self):
         if self.agreement_metric == "bert_score" and self.model_name is None:
             raise ValueError(
                 "model_name must be provided when agreement_metric is bert_score"
             )
+        super().__post_init__()
 
     def init_model(self: t.Self):
         self.sent_agreement = SentenceAgreement(
             model_name=self.model_name, metric=self.agreement_metric
         )
 
     def score(self: t.Self, dataset: Dataset) -> Dataset:
@@ -125,49 +132,44 @@
         dataset: Dataset[question: list[str], contexts: list[list[str]]]
 
         Returns
         -------
         Dataset[question: list[str], contexts: list[list[str]], scores: list[float]]
             Dataset with the scores for each row.
         """
+        if self.llm is None:
+            raise ValueError("llm must not be None")
         prompts = []
         questions, contexts = dataset["question"], dataset["contexts"]
         for q, c in zip(questions, contexts):
-            prompt = CONTEXT_RELEVANCE.format(q, "\n".join(c))
-            prompts.append(prompt)
+            human_prompt = CONTEXT_RELEVANCE.format(question=q, context="\n".join(c))
+            prompts.append(ChatPromptTemplate.from_messages([human_prompt]))
 
-        responses = []
+        responses: list[list[str]] = []
         for batch_idx in tqdm(range(0, len(prompts), 20)):
-            batch_responses = openai_completion(
-                prompts[batch_idx : batch_idx + 20], n=self.strictness
+            results = generate(
+                prompts[batch_idx : batch_idx + 20], self.llm, n=self.strictness
             )
-            responses.extend(batch_responses["choices"])  # type: ignore
-
-        prev = 0
-        outputs = []
-        for i in range(self.strictness, len(responses) + 1, self.strictness):
-            output = [responses[idx]["text"].strip() for idx in range(prev, i)]
-
-            outputs.append(output)
-            prev = i
+            batch_responses = [[i.text for i in r] for r in results.generations]
+            responses.extend(batch_responses)  # type: ignore
 
         scores = []
-        for context, n_output in zip(contexts, outputs):
+        for context, n_response in zip(contexts, responses):
             context = "\n".join(context)
             overlap_scores = []
             context_sents = sent_tokenize(context)
-            for output in n_output:
+            for output in n_response:
                 indices = [
                     context.find(sent)
                     for sent in sent_tokenize(output)
                     if context.find(sent) != -1
                 ]
                 overlap_scores.append(len(indices) / len(context_sents))
             if self.strictness > 1:
-                agr_score = self.sent_agreement.evaluate(n_output)
+                agr_score = self.sent_agreement.evaluate(n_response)
             else:
                 agr_score = 1
             scores.append(agr_score * np.mean(overlap_scores))
 
         return dataset.add_column(f"{self.name}", scores)  # type: ignore
```

### Comparing `ragas-0.0.6/src/ragas/metrics/faithfulnes.py` & `ragas-0.0.7/src/ragas/metrics/faithfulnes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import dataclass
 
 from datasets import concatenate_datasets
+from langchain.chat_models.base import BaseChatModel
+from langchain.llms.base import BaseLLM
+from langchain.prompts import ChatPromptTemplate, HumanMessagePromptTemplate
 from tqdm import tqdm
 
 from ragas.metrics.base import Metric
-from ragas.metrics.llms import openai_completion
+from ragas.metrics.llms import generate
 
 if t.TYPE_CHECKING:
     from datasets import Dataset
 
 #################
 # NLI Score
 #################
-LONG_FORM_ANSWER = """
+LONG_FORM_ANSWER_PROMPT = HumanMessagePromptTemplate.from_template(
+    """\
 Given a question and answer, create one or more statements from answer.
 question: Who was  Albert Einstein and what is he best known for?
 answer: He was a German-born theoretical physicist, widely acknowledged to be one of the greatest and most influential physicists of all time. He was best known for developing the theory of relativity, he also made important contributions to the development of the theory of quantum mechanics.
 statements:\nAlbert Einstein was born in Germany.\nAlbert Einstein was best known for his theory of relativity.
 question: Cadmium Chloride is slightly soluble in this chemical, it is also called what?
 answer: alochol
 statements:\nCadmium Chloride is slightly soluble in alcohol.
 question: Were Shahul and Jithin of the same nationality?
 answer: They were from different countries.
 statements:\nShahul and Jithin were from different countries.
-question:{}
-answer: {}
+question:{question}
+answer: {answer}
 statements:\n"""  # noqa: E501
+)
 
-NLI_STATEMENTS = """
+
+NLI_STATEMENTS_MESSAGE = HumanMessagePromptTemplate.from_template(
+    """
 Prompt: Natural language inference
 Consider the following context:
 Context:
 John is a student at XYZ University. He is pursuing a degree in Computer Science. He is enrolled in several courses this semester, including Data Structures, Algorithms, and Database Management. John is a diligent student and spends a significant amount of time studying and completing assignments. He often stays late in the library to work on his projects.
 Now, read the following statements and determine whether they are supported by the information present in the context. Provide a brief explanation for each statement. Also provide a Final Answer (Yes/No) at the end. 
 statements:\n1. John is majoring in Biology.\n2. John is taking a course on Artificial Intelligence.\n3. John is a dedicated student.\n4. John has a part-time job.\n5. John is interested in computer programming.\n
 Answer:
@@ -45,28 +52,27 @@
 3. John is a dedicated student.
 Explanation: The prompt states that he spends a significant amount of time studying and completing assignments. Additionally, it mentions that he often stays late in the library to work on his projects, which implies dedication.So answer is Yes.
 4. John has a part-time job.
 Explanation: There is no information given in the context about John having a part-time job. Therefore, it cannot be deduced that John has a part-time job. So answer is No.
 5. John is interested in computer programming.
 Explanation: The context states that John is pursuing a degree in Computer Science, which implies an interest in computer programming.So answer is Yes.
 Final answer: No. No. Yes. No. Yes.
-context:\n{}
-statements:\n{}
+context:\n{context}
+statements:\n{statements}
 Now, read the following statements and determine whether they are supported by the information present in the context. Provide a brief explanation for each statement. Also provide a Final Answer (Yes/No) at the end. 
 Answer:
 """  # noqa: E501
+)
 
 
 @dataclass
 class Faithfulness(Metric):
+    name: str = "faithfulness"
     batch_size: int = 15
-
-    @property
-    def name(self):
-        return "faithfulness"
+    llm: t.Optional[BaseLLM | BaseChatModel] = None
 
     def init_model(self: t.Self):
         pass
 
     def score(self: t.Self, dataset: Dataset) -> Dataset:
         scores = []
         for batch in tqdm(self.get_batches(len(dataset))):
@@ -75,41 +81,46 @@
 
         return concatenate_datasets(scores)
 
     def _score_batch(self: t.Self, ds: Dataset) -> Dataset:
         """
         returns the NLI score for each (q, c, a) pair
         """
+        assert self.llm is not None, "LLM not initialized"
+
         question, answer, contexts = ds["question"], ds["answer"], ds["contexts"]
         prompts = []
         for q, a in zip(question, answer):
-            prompt = LONG_FORM_ANSWER.format(q, a)
-            prompts.append(prompt)
+            human_prompt = LONG_FORM_ANSWER_PROMPT.format(question=q, answer=a)
+            prompts.append(ChatPromptTemplate.from_messages([human_prompt]))
 
-        response = openai_completion(prompts)
+        result = generate(prompts, self.llm)
         list_statements: list[list[str]] = []
-        for output in response["choices"]:  # type: ignore
-            statements = output["text"].split("\n")
+        for output in result.generations:
+            # use only the first generation for each prompt
+            statements = output[0].text.split("\n")
             list_statements.append(statements)
 
         prompts = []
         for context, statements in zip(contexts, list_statements):
             statements_str: str = "\n".join(
                 [f"{i+1}.{st}" for i, st in enumerate(statements)]
             )
             contexts_str: str = "\n".join(context)
-            prompt = NLI_STATEMENTS.format(contexts_str, statements_str)
-            prompts.append(prompt)
+            human_prompt = NLI_STATEMENTS_MESSAGE.format(
+                context=contexts_str, statements=statements_str
+            )
+            prompts.append(ChatPromptTemplate.from_messages([human_prompt]))
 
-        response = openai_completion(prompts)
-        outputs = response["choices"]  # type: ignore
+        result = generate(prompts, self.llm)
+        outputs = result.generations
 
         scores = []
         for i, output in enumerate(outputs):
-            output = output["text"].lower().strip()
+            output = output[0].text.lower().strip()
             if output.find("final answer:") != -1:
                 output = output[output.find("final answer:") + len("final answer:") :]
                 score = sum(
                     0 if "yes" in answer else 1
                     for answer in output.strip().split(".")
                     if answer != ""
                 )
```

### Comparing `ragas-0.0.6/src/ragas/utils.py` & `ragas-0.0.7/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.6/src/ragas.egg-info/PKG-INFO` & `ragas-0.0.7/src/ragas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.6
+Version: 0.0.7
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.6 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.7 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
  Evaluation framework for your Retrieval Augmented Generation (RAG) pipelines
 [GitHub_release] [Build] [License] [Open_In_Colab] [discord-invite] [Downloads]
  *** Installation | Quickstart | Metrics | Community | Open_Analytics | FAQ |
                                Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
```

### Comparing `ragas-0.0.6/src/ragas.egg-info/SOURCES.txt` & `ragas-0.0.7/src/ragas.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 .github/workflows/ci.yaml
 .github/workflows/python-publish.yml
 docs/metrics.md
 docs/quickstart.ipynb
 docs/assets/bar-graph.svg
 docs/assets/logo.png
 docs/guides/data_prep.py
+docs/guides/llms.ipynb
 experiments/README.md
 experiments/assesments/metrics_assesments.ipynb
 experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
 experiments/baselines/fiqa/improving-baselines.ipynb
 experiments/baselines/hotpotqa/explore-dataset.ipynb
 experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
 experiments/baselines/wikiqa/failed_wikis
 requirements/dev.txt
 requirements/test.txt
 src/ragas/__init__.py
 src/ragas/_analytics.py
 src/ragas/_version.py
+src/ragas/async_utils.py
 src/ragas/evaluation.py
 src/ragas/exceptions.py
 src/ragas/utils.py
 src/ragas.egg-info/PKG-INFO
 src/ragas.egg-info/SOURCES.txt
 src/ragas.egg-info/dependency_links.txt
 src/ragas.egg-info/requires.txt
```

### Comparing `ragas-0.0.6/tests/benchmarks/utils.py` & `ragas-0.0.7/tests/benchmarks/utils.py`

 * *Files identical despite different names*

