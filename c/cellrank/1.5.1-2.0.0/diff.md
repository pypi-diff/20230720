# Comparing `tmp/cellrank-1.5.1.tar.gz` & `tmp/cellrank-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellrank-1.5.1.tar", last modified: Thu Jan 13 16:42:28 2022, max compression
+gzip compressed data, was "cellrank-2.0.0.tar", last modified: Thu Jul 20 11:41:06 2023, max compression
```

## Comparing `cellrank-1.5.1.tar` & `cellrank-2.0.0.tar`

### file list

```diff
@@ -1,177 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.631389 cellrank-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-01-13 16:42:18.000000 cellrank-1.5.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-01-13 16:42:18.000000 cellrank-1.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-01-13 16:42:18.000000 cellrank-1.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-01-13 16:42:18.000000 cellrank-1.5.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-01-13 16:42:18.000000 cellrank-1.5.1/.rstcheck.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    12136 2022-01-13 16:42:18.000000 cellrank-1.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-01-13 16:42:18.000000 cellrank-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-01-13 16:42:18.000000 cellrank-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9600 2022-01-13 16:42:28.631389 cellrank-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8105 2022-01-13 16:42:18.000000 cellrank-1.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.619389 cellrank-1.5.1/cellrank/
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2902 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/_key.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.619389 cellrank-1.5.1/cellrank/datasets/
--rw-r--r--   0 runner    (1001) docker     (121)      167 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8365 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/datasets/_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/estimators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.619389 cellrank-1.5.1/cellrank/external/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      702 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/_error_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.619389 cellrank-1.5.1/cellrank/external/estimators/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/estimators/_import_error_estim.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.619389 cellrank-1.5.1/cellrank/external/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/kernels/_import_error_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/kernels/_statot_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7356 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/kernels/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22566 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/kernels/_wot_kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/external/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/external/models/_import_error_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/logging/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/logging/_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/pl/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12078 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_circular_projection.py
--rw-r--r--   0 runner    (1001) docker     (121)    17411 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_cluster_fates.py
--rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_cluster_lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)    11836 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_gene_trend.py
--rw-r--r--   0 runner    (1001) docker     (121)    19473 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    20085 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     4173 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_init_term_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     3475 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_lineages.py
--rw-r--r--   0 runner    (1001) docker     (121)    10724 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_log_odds.py
--rw-r--r--   0 runner    (1001) docker     (121)    42693 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/pl/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/settings/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/settings/_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/tl/
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12666 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_colors.py
--rw-r--r--   0 runner    (1001) docker     (121)     2345 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     9641 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_init_term_states.py
--rw-r--r--   0 runner    (1001) docker     (121)    44878 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4066 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_lineages.py
--rw-r--r--   0 runner    (1001) docker     (121)    15929 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_linear_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/tl/_mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_mixins/_anndata.py
--rw-r--r--   0 runner    (1001) docker     (121)     3756 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_mixins/_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_mixins/_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     4335 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_transition_matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    54049 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/tl/estimators/
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16475 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/_base_estimator.py
--rw-r--r--   0 runner    (1001) docker     (121)     2100 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.623389 cellrank-1.5.1/cellrank/tl/estimators/mixins/
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19670 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/_absorption_probabilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    22622 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/_lineage_drivers.py
--rw-r--r--   0 runner    (1001) docker     (121)    13595 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/cellrank/tl/estimators/mixins/decomposition/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/decomposition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12392 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/decomposition/_eigen.py
--rw-r--r--   0 runner    (1001) docker     (121)    10837 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/mixins/decomposition/_schur.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/cellrank/tl/estimators/terminal_states/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/terminal_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10167 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/terminal_states/_cflare.py
--rw-r--r--   0 runner    (1001) docker     (121)    45551 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/terminal_states/_gpcca.py
--rw-r--r--   0 runner    (1001) docker     (121)    11542 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/estimators/terminal_states/_term_states_estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/cellrank/tl/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46769 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_base_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_connectivity_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    10532 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_cytotrace_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     6573 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_exp_time_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_precomputed_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7495 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_pseudotime_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)     8038 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_pseudotime_schemes.py
--rw-r--r--   0 runner    (1001) docker     (121)     5969 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (121)    20329 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_tmat_flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     8070 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19187 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_velocity_kernel.py
--rw-r--r--   0 runner    (1001) docker     (121)    10358 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/tl/kernels/_velocity_schemes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/cellrank/ul/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9067 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/_docs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4650 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/_parallelize.py
--rw-r--r--   0 runner    (1001) docker     (121)     7733 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/cellrank/ul/models/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    52108 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/models/_base_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    12489 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/models/_gamr_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     8428 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/models/_pygam_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     7266 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/models/_sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    16085 2022-01-13 16:42:18.000000 cellrank-1.5.1/cellrank/ul/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.619389 cellrank-1.5.1/cellrank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9600 2022-01-13 16:42:28.000000 cellrank-1.5.1/cellrank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-01-13 16:42:28.000000 cellrank-1.5.1/cellrank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 16:42:28.000000 cellrank-1.5.1/cellrank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-13 16:42:28.000000 cellrank-1.5.1/cellrank.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-01-13 16:42:28.000000 cellrank-1.5.1/cellrank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-01-13 16:42:28.000000 cellrank-1.5.1/cellrank.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-01-13 16:42:18.000000 cellrank-1.5.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/examples/estimators/
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/estimators/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/estimators/compute_abs_probs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/estimators/compute_coarse_T.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/estimators/compute_lineage_drivers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2436 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/estimators/compute_macrostates.py
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/estimators/compute_terminal_states_gpcca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.627389 cellrank-1.5.1/examples/kernels/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/kernels/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4433 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/kernels/compute_kernel_tricks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/kernels/plot_projection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1523 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/kernels/plot_random_walks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.631389 cellrank-1.5.1/examples/other/
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/other/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2539 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/other/compute_lineage_tricks.py
--rw-r--r--   0 runner    (1001) docker     (121)     3524 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/other/plot_model.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.631389 cellrank-1.5.1/examples/plotting/
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_circular_embedding.py
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_cluster_fates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_cluster_lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_directed_paga.py
--rw-r--r--   0 runner    (1001) docker     (121)     3183 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_gene_trends.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1862 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_initial_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_lineage_drivers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_lineages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-01-13 16:42:18.000000 cellrank-1.5.1/examples/plotting/plot_terminal_states.py
--rw-r--r--   0 runner    (1001) docker     (121)     1717 2022-01-13 16:42:18.000000 cellrank-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-01-13 16:42:18.000000 cellrank-1.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-13 16:42:28.631389 cellrank-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-01-13 16:42:18.000000 cellrank-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-13 16:42:28.631389 cellrank-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    14157 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    12069 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    24769 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_cflare.py
--rw-r--r--   0 runner    (1001) docker     (121)     9420 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_colors.py
--rw-r--r--   0 runner    (1001) docker     (121)      971 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)    13967 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_external.py
--rw-r--r--   0 runner    (1001) docker     (121)    51594 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_gpcca.py
--rw-r--r--   0 runner    (1001) docker     (121)    56554 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_kernels.py
--rw-r--r--   0 runner    (1001) docker     (121)    36862 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (121)     9274 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     3203 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    29167 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)    11824 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (121)   111702 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_random_walk.py
--rw-r--r--   0 runner    (1001) docker     (121)     3450 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     7984 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    38013 2022-01-13 16:42:18.000000 cellrank-1.5.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5947 2022-01-13 16:42:18.000000 cellrank-1.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.426280 cellrank-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-20 11:38:39.000000 cellrank-2.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-07-20 11:38:39.000000 cellrank-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 11:38:39.000000 cellrank-2.0.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-20 11:38:39.000000 cellrank-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 11:38:39.000000 cellrank-2.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 11:38:39.000000 cellrank-2.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-20 11:38:39.000000 cellrank-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 11:38:39.000000 cellrank-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-20 11:41:06.426280 cellrank-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-20 11:38:39.000000 cellrank-2.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-20 11:38:39.000000 cellrank-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 11:41:06.426280 cellrank-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.414279 cellrank-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.418280 cellrank-2.0.0/src/cellrank/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.418280 cellrank-2.0.0/src/cellrank/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10893 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9941 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43645 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15802 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_parallelize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54106 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.418280 cellrank-2.0.0/src/cellrank/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/_base_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.418280 cellrank-2.0.0/src/cellrank/estimators/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21431 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/_fate_probabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22301 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/_lineage_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5205 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.418280 cellrank-2.0.0/src/cellrank/estimators/mixins/decomposition/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/decomposition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/decomposition/_eigen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/mixins/decomposition/_schur.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.422280 cellrank-2.0.0/src/cellrank/estimators/terminal_states/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/terminal_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/terminal_states/_cflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50326 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/terminal_states/_gpcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26796 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/estimators/terminal_states/_term_states_estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.422280 cellrank-2.0.0/src/cellrank/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30804 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_base_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_connectivity_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_cytotrace_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_experimental_time_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_precomputed_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_pseudotime_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_real_time_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/_velocity_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.422280 cellrank-2.0.0/src/cellrank/kernels/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/mixins/_anndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/mixins/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/mixins/_kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.422280 cellrank-2.0.0/src/cellrank/kernels/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/_pseudotime_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/_random_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19811 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/_tmat_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/kernels/utils/_velocity_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.422280 cellrank-2.0.0/src/cellrank/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/logging/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.426280 cellrank-2.0.0/src/cellrank/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49708 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/models/_base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12442 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/models/_gamr_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/models/_pygam_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/models/_sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.426280 cellrank-2.0.0/src/cellrank/pl/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16515 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_aggregate_fate_probs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_circular_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10560 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_cluster_trends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11742 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_gene_trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_log_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36890 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/pl/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.426280 cellrank-2.0.0/src/cellrank/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-20 11:38:39.000000 cellrank-2.0.0/src/cellrank/settings/_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:41:06.418280 cellrank-2.0.0/src/cellrank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-20 11:41:06.000000 cellrank-2.0.0/src/cellrank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-20 11:41:06.000000 cellrank-2.0.0/src/cellrank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:41:06.000000 cellrank-2.0.0/src/cellrank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-20 11:41:06.000000 cellrank-2.0.0/src/cellrank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 11:41:06.000000 cellrank-2.0.0/src/cellrank.egg-info/top_level.txt
```

### Comparing `cellrank-1.5.1/LICENSE` & `cellrank-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cellrank-1.5.1/cellrank/_key.py` & `cellrank-2.0.0/src/cellrank/_utils/_key.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Callable, Optional
 
+__all__ = ["Key"]
+
 
 class cprop:
     """Class property."""
 
     def __init__(self, f: Callable[..., str]):
         self.f = f
 
@@ -11,93 +13,94 @@
         return self.f(owner)
 
 
 class Key:
     """Class which manages keys in :class:`anndata.AnnData`."""
 
     @classmethod
-    def backward(cls, bwd: bool) -> str:
+    def backward(cls, bwd: Optional[bool]) -> str:
         return "bwd" if bwd else "fwd"
 
     @classmethod
-    def where(cls, bwd: bool) -> str:
+    def where(cls, bwd: Optional[bool]) -> str:
         return "from" if bwd else "to"
 
     @classmethod
-    def initial(cls, bwd: bool) -> str:
+    def initial(cls, bwd: Optional[bool]) -> str:
         return "initial" if bwd else "terminal"
 
     @classmethod
     def cytotrace(cls, key: str) -> str:
         return f"ct_{key}"
 
     class obs:
         @classmethod
         def probs(cls, key: str) -> str:
             return f"{key}_probs"
 
         @classmethod
-        def macrostates(cls, bwd: bool) -> str:
+        def macrostates(cls, bwd: Optional[bool]) -> str:
             return f"macrostates_{Key.backward(bwd)}"
 
         @classmethod
-        def term_states(cls, bwd: bool) -> str:
-            return f"{Key.initial(bwd)}_states"
+        def term_states(cls, estim_bwd: Optional[bool], *, bwd: bool = False) -> str:
+            states = "init_states" if bwd else "term_states"
+            return f"{states}_{Key.backward(estim_bwd)}"
 
         @classmethod
-        def priming_degree(cls, bwd: bool) -> str:
+        def priming_degree(cls, bwd: Optional[bool]) -> str:
             return f"priming_degree_{Key.backward(bwd)}"
 
     class obsm:
         @classmethod
         def memberships(cls, key: str) -> str:
             return f"{key}_memberships"
 
         @classmethod
-        def schur_vectors(cls, bwd: bool) -> str:
+        def schur_vectors(cls, bwd: Optional[bool]) -> str:
             return f"schur_vectors_{Key.backward(bwd)}"
 
         @classmethod
-        def macrostates(cls, bwd: bool) -> str:
+        def macrostates(cls, bwd: Optional[bool]) -> str:
             return f"macrostates_{Key.backward(bwd)}"
 
         @classmethod
-        def abs_probs(cls, bwd: bool) -> str:
-            return ("from" if bwd else "to") + "_" + Key.obs.term_states(bwd)
+        def fate_probs(cls, bwd: Optional[bool]) -> str:
+            return f"lineages_{Key.backward(bwd)}"
 
         @classmethod
-        def abs_times(cls, bwd: bool) -> str:
+        def abs_times(cls, bwd: Optional[bool]) -> str:
             return f"absorption_times_{Key.backward(bwd)}"
 
     class varm:
         @classmethod
-        def lineage_drivers(cls, bwd: bool):
-            return ("initial" if bwd else "terminal") + "_lineage_drivers"
+        def lineage_drivers(cls, bwd: Optional[bool]):
+            return Key.initial(bwd) + "_lineage_drivers"
 
     class uns:
         @classmethod
-        def kernel(cls, bwd: bool, key: Optional[str] = None) -> str:
+        def kernel(cls, bwd: Optional[bool], key: Optional[str] = None) -> str:
             return key if key is not None else f"T_{Key.backward(bwd)}"
 
         @classmethod
-        def estimator(cls, bwd: bool, key: Optional[str] = None) -> str:
+        def estimator(cls, bwd: Optional[bool], key: Optional[str] = None) -> str:
             return key if key is not None else f"{Key.backward(bwd)}_estimator"
 
         @classmethod
         def names(cls, key: str) -> str:
             return f"{key}_names"
 
         @classmethod
         def colors(cls, key: str) -> str:
             return f"{key}_colors"
 
         @classmethod
-        def eigen(cls, bwd: bool) -> str:
+        def eigen(cls, bwd: Optional[bool]) -> str:
             return f"eigendecomposition_{Key.backward(bwd)}"
 
         @classmethod
-        def schur_matrix(cls, bwd: bool) -> str:
+        def schur_matrix(cls, bwd: Optional[bool]) -> str:
             return f"schur_matrix_{Key.backward(bwd)}"
 
         @classmethod
-        def coarse(cls, bwd: bool) -> str:
+        def coarse(cls, bwd: Optional[bool]) -> str:
             return f"coarse_{Key.backward(bwd)}"
```

### Comparing `cellrank-1.5.1/cellrank/external/kernels/_wot_kernel.py` & `cellrank-2.0.0/src/cellrank/estimators/mixins/_fate_probabilities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,561 +1,607 @@
-from typing import Any, Dict, Tuple, Union, Mapping, Optional
-from typing_extensions import Literal
+import types
+from typing import Any, Dict, Literal, Mapping, NamedTuple, Optional, Sequence, Union
 
-from types import MappingProxyType
-from tqdm.auto import tqdm
+import numpy as np
+import pandas as pd
+import scipy.sparse as sp
+from pandas.api.types import infer_dtype, is_categorical_dtype
 
-import scanpy as sc
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank.ul._docs import d, inject_docs
-from cellrank.tl._utils import _maybe_subset_hvgs
-from cellrank.external.kernels._utils import MarkerGenes
-from cellrank.tl.kernels._exp_time_kernel import LastTimePoint
+from cellrank._utils._docs import d
+from cellrank._utils._enum import DEFAULT_BACKEND, Backend_t
+from cellrank._utils._key import Key
+from cellrank._utils._lineage import Lineage
+from cellrank._utils._linear_solver import _solve_lin_system
+from cellrank._utils._utils import (
+    _calculate_lineage_absorption_time_means,
+    _get_cat_and_null_indices,
+    _pairwise,
+    _process_series,
+)
+from cellrank.estimators.mixins._utils import (
+    BaseProtocol,
+    PlotMode,
+    SafeGetter,
+    StatesHolder,
+    logger,
+    shadow,
+)
+
+__all__ = ["FateProbsMixin"]
+
+
+class RecTransStates(NamedTuple):
+    q: Union[np.ndarray, sp.spmatrix]
+    s: Union[np.ndarray, sp.spmatrix]
+    trans_indices: np.ndarray
+    rec_indices: np.ndarray
+    name_to_ixs: Dict[str, np.ndarray]
+    term_states: pd.Series
+    term_states_colors: Sequence[Any]
 
-import numpy as np
-import pandas as pd
 
-_error = None
-try:
-    import wot
-
-    from cellrank.tl.kernels import TransportMapKernel as Kernel
-except ImportError as e:
-    from cellrank.external.kernels._import_error_kernel import ErroredKernel as Kernel
-
-    _error = e
-    wot = None
-
-
-class nstr(str):  # used for params+cache (precomputed cost matrices)
-    """String class that is not equal to any other string."""
-
-    def __eq__(self, other: str) -> bool:
-        return False
-
-
-@d.dedent
-class WOTKernel(Kernel, error=_error):
-    """
-    Waddington optimal transport kernel from :cite:`schiebinger:19`.
-
-    This class requires the `wot` package, which can be installed as
-    `pip install git+https://github.com/broadinstitute/wot`.
-
-    Parameters
-    ----------
-    %(adata)s
-    %(backward)s
-    time_key
-        Key in :attr:`adata` ``.obs`` where experimental time is stored.
-        The experimental time can be of either of a numeric or an ordered categorical type.
-    %(cond_num)s
-
-    Examples
-    --------
-    Workflow::
-
-        # import packages, load data
-        import scanpy as sc
-        import cellrank as cr
-        adata = cr.datasets.lung()
-
-        # filter, normalize and annotate highly variable genes
-        sc.pp.filter_genes(adata, min_cells=10)
-        sc.pp.normalize_total(adata)
-        sc.pp.log1p(adata)
-        sc.pp.highly_variable_genes(adata)
-
-        # estimate proliferation and apoptosis from gene sets (see. e.g. WOT tutorial for example lists)
-        proliferation_genes = ...
-        apoptosis_genes = ...
-        sc.tl.score_genes(adata, gene_list=proliferation_genes, score_name='proliferation')
-        sc.tl.score_genes(adata, gene_list=apoptosis_genes, score_name='apoptosis')
-
-        # initialize kernel, estimate initial growth rate based on scores from above
-        from cellrank.external.kernels import WOTKernel
-        ot = WOTKernel(adata, time_key='day')
-        ot.compute_initial_growth_rates(proliferation_key='proliferation',
-                                        apoptosis_key='apoptosis',
-                                        key_added='initial_growth_rates')
-
-        # compute transport maps, aggregate into one single transition matrix
-        ot.compute_transition_matrix(growth_rate_key='initial_growth_rates', growth_iters=3)
-    """
-
-    __import_error_message__ = (
-        "Unable to import the kernel. Please install `wot` first as "
-        "`pip install git+https://github.com/broadinstitute/wot`."
-    )
+class FateProbsProtocol(BaseProtocol):
+    _term_states: StatesHolder
+
+    @property
+    def transition_matrix(self) -> Union[np.ndarray, sp.spmatrix]:
+        ...
+
+    @property
+    def terminal_states(self) -> pd.Series:
+        ...
+
+    @property
+    def fate_probabilities(self) -> Optional[Lineage]:
+        ...
 
-    def __init__(
+    @property
+    def absorption_times(self) -> Optional[pd.DataFrame]:
+        ...
+
+    @property
+    def priming_degree(self) -> Optional[pd.Series]:
+        ...
+
+    def __len__(self) -> int:
+        ...
+
+    def _compute_fate_probabilities(
         self,
-        adata: AnnData,
-        backward: bool = False,
-        time_key: str = "exp_time",
-        compute_cond_num: bool = False,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            adata,
-            backward=backward,
-            time_key=time_key,
-            compute_cond_num=compute_cond_num,
-            **kwargs,
-        )
+        q: Union[np.ndarray, sp.spmatrix],
+        s: Union[np.ndarray, sp.spmatrix],
+        trans_indices: np.ndarray,
+        term_states: np.ndim,
+        solver: str,
+        use_petsc: bool,
+        n_jobs: Optional[int],
+        backend: str,
+        tol: float,
+        show_progress_bar: bool,
+        preconditioner: str,
+    ) -> np.ndarray:
+        ...
 
-        # WOT's requirements
-        cats = self.experimental_time.cat.categories
-        self._exp_time = self.experimental_time.cat.rename_categories(
-            dict(zip(cats, map(float, cats)))
-        )
-        self.adata.obs[self._time_key] = self.experimental_time
-        self._growth_rates = None
+    def _rec_trans_states(
+        self,
+        keys: Optional[Sequence[str]],
+        *,
+        ctx: Literal["fate_probs", "time_to_absorption"],
+    ) -> RecTransStates:
+        ...
 
-    def _read_from_adata(
+    def _ensure_lineage_object(
         self,
-        conn_key: Optional[str] = "connectivities",
-        read_conn: bool = True,
+        obj: Union[str, np.ndarray, Lineage],
+        *,
+        kind: Literal["macrostates", "term_states", "fate_probs"],
+        backward: bool,
         **kwargs: Any,
-    ) -> None:
-        super()._read_from_adata(conn_key=conn_key, read_conn=False, **kwargs)
+    ) -> Lineage:
+        ...
+
+    def _write_fate_probabilities(
+        self,
+        fate_probs: Optional[Lineage],
+    ) -> str:
+        ...
+
+    def _write_absorption_times(
+        self,
+        abs_times: Optional[pd.DataFrame],
+        params: Mapping[str, Any] = types.MappingProxyType({}),
+    ) -> str:
+        ...
 
-    def compute_initial_growth_rates(
+    def _write_lineage_priming(
         self,
-        proliferation_key: Optional[str] = None,
-        apoptosis_key: Optional[str] = None,
-        organism: Optional[Literal["human", "mouse"]] = None,
-        beta_min: float = 0.3,
-        beta_max: float = 1.7,
-        delta_min: float = 0.3,
-        delta_max: float = 1.7,
-        key_added: Optional[str] = None,
+        priming_degree: Optional[pd.Series],
+    ) -> str:
+        ...
+
+    def _plot_continuous(
+        self,
+        _data: Lineage,
+        _colors: Optional[np.ndarray] = None,
+        _title: Optional[str] = None,
+        states: Optional[Union[str, Sequence[str]]] = None,
+        color: Optional[str] = None,
+        mode: Literal["embedding", "time"] = PlotMode.EMBEDDING,
+        time_key: Optional[str] = None,
+        title: Optional[Union[str, Sequence[str]]] = None,
+        same_plot: bool = True,
+        cmap: str = "viridis",
         **kwargs: Any,
-    ) -> Optional[pd.Series]:
-        r"""
-        Estimate initial growth rates using a birth-death process as described in :cite:`schiebinger:19`.
-
-        The doubling time is defined as :math:`\frac{\ln 2}{\beta - \delta}` (similarly defined for half-time).
-        The logistic function is used to transform the birth/death rate scores and to smoothly interpolate between
-        specified minimum and maximum birth/death rates.
+    ) -> None:
+        ...
 
-        Parameters
-        ----------
-        proliferation_key
-            Key in :attr:`anndata.AnnData.obs` where the birth rate score is saved.
-        apoptosis_key
-            Key in :attr:`anndata.AnnData.obs` where the death rate score is saved.
-        organism
-            Organism for which to calculate the birth/death scores, if they cannot be found in :attr:`adata`.
-            In this case, :func:`scanpy.tl.score_genes` is used to calculate the scores based on an organism-dependent
-            set of marker genes for proliferation and apoptosis.
-        beta_min
-            Minimum birth rate.
-        beta_max
-            Maximum birth rate.
-        delta_min
-            Minimum death rate.
-        delta_max
-            Maximum death rate.
-        key_added
-            Key in :attr:`adata` ``.obs`` where to add the estimated growth rates. If `None`, just return them.
-        kwargs
-            Keyword arguments for :func:`scanpy.tl.score_genes`. Only used when ``proliferation_key``
-            or ``apoptosis_key`` cannot be found in :attr:`adata.AnnData.obs`.
 
-        Returns
-        -------
-        :class:`pandas.Series`
-            The estimated initial growth rates if ``key_added = None``, otherwise `None`.
+class FateProbsMixin:
+    """Mixin that supports computation of fate probabilities and mean times to absorption."""
 
-        Notes
-        -----
-        If you don't have access to proliferation/apoptosis gene sets, you can use the ones defined in :mod:`cellrank`
-        for a specific organism. Alternatively, you can also use WOT without an estimate of initial growth rates. In
-        that case, make sure to use several iterations in
-        :meth:`cellrank.external.kernels.WOTKernel.compute_transition_matrix` by increasing the ``growth_iters``
-        parameter. A value around 3 works well in most cases.
-
-        The markers used here were taken from the following sources:
-
-            - human, proliferation - :cite:`tirosh:16:science`.
-            - human, apoptosis - `Hallmark Apoptosis, MSigDB <https://www.gsea-msigdb.org/gsea/msigdb/cards/HALLMARK_APOPTOSIS>`_.
-            - mouse, proliferation - :cite:`tirosh:16:nature`.
-            - mouse, apoptosis - `Hallmark P53 Pathway, MSigDB <https://www.gsea-msigdb.org/gsea/msigdb/cards/HALLMARK_P53_PATHWAY>`_.
-
-        For more information about WOT, see the official `tutorial <https://broadinstitute.github.io/wot/tutorial/>`_.
-        """  # noqa: E501
-
-        def get_scores(
-            key: str,
-            *,
-            kind: Literal["proliferation", "apoptosis"],
-            organism: Optional[Literal["human", "mouse"]],
-        ) -> np.ndarray:
-            try:
-                return np.asarray(self.adata.obs[key])
-            except KeyError:
-                if organism is None:
-                    raise KeyError(
-                        f"Unable to find `{kind}` scores in `adata.obs[{kind!r}]`. Consider specifying `organism=...`."
-                    ) from None
-
-                logg.info(f"Computing `{kind}` scores")
-                score_name = f"{kind}_score" if key is None else key
-
-                sc.tl.score_genes(
-                    self.adata,
-                    gene_list=getattr(MarkerGenes, f"{kind}_markers")(organism),
-                    score_name=score_name,
-                    **kwargs,
-                )
+    def __init__(self, **kwargs: Any):
+        super().__init__(**kwargs)
 
-                return get_scores(score_name, kind=kind, organism=None)
+        self._fate_probabilities: Optional[Lineage] = None
+        self._absorption_times: Optional[pd.DataFrame] = None
+        self._priming_degree: Optional[pd.Series] = None
 
-        def logistic(x: np.ndarray, L: float, k: float, x0: float = 0) -> np.ndarray:
-            return L / (1 + np.exp(-k * (x - x0)))
+    @property
+    @d.get_summary(base="fate_probs")
+    def fate_probabilities(self) -> Optional[Lineage]:
+        """Fate probabilities.
+
+        Informally, given a (finite, discrete) Markov chain with a set of transient states :math:`T` and
+        a set of absorbing states :math:`A`, the absorption probability for cell :math:`i` from :math:`T`
+        to reach cell :math:`j` from :math:`R` is the probability that a random walk initialized in :math:`i`
+        will reach absorbing state :math:`j`.
 
-        def gen_logistic(
-            p: np.ndarray, beta_max: float, beta_min: float, center: float, width: float
-        ) -> np.ndarray:
-            return beta_min + logistic(p, L=beta_max - beta_min, k=4 / width, x0=center)
-
-        def beta(
-            p: np.ndarray,
-            beta_max: float = 1.7,
-            beta_min: float = 0.3,
-            center: float = 0.25,
-        ) -> np.ndarray:
-            return gen_logistic(p, beta_max, beta_min, center, width=0.5)
-
-        def delta(
-            a: np.ndarray,
-            delta_max: float = 1.7,
-            delta_min: float = 0.3,
-            center: float = 0.1,
-        ) -> np.ndarray:
-            return gen_logistic(a, delta_max, delta_min, center, width=0.2)
-
-        birth = beta(
-            get_scores(proliferation_key, kind="proliferation", organism=organism),
-            beta_min=beta_min,
-            beta_max=beta_max,
-        )
-        death = delta(
-            get_scores(apoptosis_key, kind="apoptosis", organism=organism),
-            delta_min=delta_min,
-            delta_max=delta_max,
-        )
-        gr = np.exp(birth - death)
+        In our context, states correspond to cells, in particular, absorbing states correspond to cells
+        in :attr:`terminal_states`.
+        """
+        return self._fate_probabilities
 
-        if key_added is None:
-            return pd.Series(gr, index=self.adata.obs_names)
-        self.adata.obs[key_added] = gr
+    @property
+    @d.get_summary(base="abs_times")
+    def absorption_times(self) -> Optional[pd.DataFrame]:
+        """Mean and variance of the time until absorption.
 
-    @inject_docs(ltp=LastTimePoint)
-    def compute_transition_matrix(
-        self,
-        cost_matrices: Optional[
-            Union[str, Mapping[Tuple[float, float], np.ndarray]]
-        ] = None,
-        lambda1: float = 1,
-        lambda2: float = 50,
-        epsilon: float = 0.05,
-        growth_iters: int = 1,
-        solver: Literal["fixed_iters", "duality_gap"] = "duality_gap",
-        growth_rate_key: Optional[str] = None,
-        use_highly_variable: Optional[Union[str, bool]] = True,
-        last_time_point: Literal[
-            "uniform", "diagonal", "connectivities"
-        ] = LastTimePoint.UNIFORM,
-        threshold: Optional[Union[float, Literal["auto"]]] = "auto",
-        conn_kwargs: Mapping[str, Any] = MappingProxyType({}),
-        **kwargs: Any,
-    ) -> "WOTKernel":
+        Related to conditional mean first passage times. Corresponds to the expectation of the time until absorption,
+        depending on initialization, and the variance.
         """
-        Compute transition matrix using Waddington OT :cite:`schiebinger:19`.
+        return self._absorption_times
+
+    @property
+    @d.get_summary(base="priming_degree")
+    def priming_degree(self) -> Optional[pd.Series]:
+        """Priming degree.
+
+        Given a cell :math:`i` and a set of terminal states, this quantifies how committed vs. naive cell :math:`i` is,
+        i.e. its degree of pluripotency. Low values correspond to naive cells (high degree of pluripotency), high values
+        correspond to committed cells (low degree of pluripotency).
+        """
+        return self._priming_degree
+
+    @d.dedent
+    def compute_fate_probabilities(
+        self: FateProbsProtocol,
+        keys: Optional[Sequence[str]] = None,
+        solver: Union[str, Literal["direct", "gmres", "lgmres", "bicgstab", "gcrotmk"]] = "gmres",
+        use_petsc: bool = True,
+        n_jobs: Optional[int] = None,
+        backend: Backend_t = DEFAULT_BACKEND,
+        show_progress_bar: bool = True,
+        tol: float = 1e-6,
+        preconditioner: Optional[str] = None,
+    ) -> None:
+        """Compute fate probabilities.
 
-        Computes transport maps linking together pairs of time points for time-series single cell data using unbalanced
-        optimal transport, taking into account cell birth and death rates. From the sequence of transition maps linking
-        pairs of sequential time points, we construct one large transition matrix which contains the normalized
-        transport maps as blocks on the 1st upper diagonal.
+        For each cell, this computes the probability of being absorbed in any of the :attr:`terminal_states`. In
+        particular, this corresponds to the probability that a random walk initialized in transient cell :math:`i`
+        will reach any cell from a fixed transient state before reaching a cell from any other transient state.
 
         Parameters
         ----------
-        cost_matrices
-            Cost matrices for each consecutive pair of time points.
-            If a :class:`str`, it specifies a key in :attr:`anndata.AnnData.layers` or :attr:`anndata.AnnData.obsm`.
-            containing cell features that are used to compute cost matrices. If `None`, use `WOT`'s default, i.e.
-            compute distances in PCA space derived from :attr:`anndata.AnnData.X` for each time point pair separately.
-        lambda1
-            Regularization parameter for the marginal constraint on :math:`p`, the transport map row sums.
-            Smaller value is useful when precise information about the growth rate is not present.
-        lambda2
-            Regularization parameter for the marginal constraint on :math:`q`, the transport map column sums.
-        epsilon
-            Entropy regularization parameter. Larger value gives more entropic descendant distributions.
-        growth_iters
-            Number of iterations for growth rate estimates. If growth rates are not known, consider using more
-            iterations.
-        solver
-            Which solver to use.
-        growth_rate_key
-            Key in :attr:`anndata.AnnData.obs` where initial cell growth rates are stored.
-            See :meth:`compute_initial_growth_rates` on how to estimate them.
-        use_highly_variable
-            Key in :attr:`anndata.AnnData.var` where highly variable genes are stored.
-            If `True`, use `'highly_variable'`. If `None`, use all genes.
-        last_time_point
-            How to define transitions within the last time point. Valid options are:
-
-                - `{ltp.UNIFORM!r}` - row-normalized matrix of 1s for transitions within the last time point.
-                - `{ltp.DIAGONAL!r}` - diagonal matrix with 1s on the diagonal.
-                - `{ltp.CONNECTIVITIES!r}` - use transitions from :class:`cellrank.tl.kernels.ConnectivityKernel`
-                  derived from the last time point subset of :attr:`adata`.
-        threshold
-            How to remove small non-zero values from the transition matrix. Valid options are:
-
-                - `'auto'` - find the maximum threshold value which will not remove every non-zero value from any row.
-                - :class:`float` - value in `[0, 100]` corresponding to a percentage of non-zeros to remove.
-                  Rows where all values are removed will have uniform distribution.
-                - `None` - do not threshold.
-
-        conn_kwargs
-            Keyword arguments for :func:`scanpy.pp.neighbors`, when using ``last_time_point = {ltp.CONNECTIVITIES!r}``.
-            Can contain `'density_normalize'` for
-            :meth:`cellrank.tl.kernels.ConnectivityKernel.compute_transition_matrix`.
-        kwargs
-            Additional keyword arguments for optimal transport configuration.
+        keys
+            Terminal states for which to compute the fate probabilities.
+            If :obj:`None`, use all states defined in :attr:`terminal_states`.
+        %(absorption_utils)s
 
         Returns
         -------
-        :class:`cellrank.external.kernels.WOTKernel`
-            Makes :attr:`transition_matrix`, :attr:`transport_maps` and :attr:`growth_rates` available.
-            Also modifies :attr:`anndata.AnnData.obs` with the following key:
-
-                - `'estimated_growth_rates'` - the estimated final growth rates.
-
-        Notes
-        -----
-        For more information about WOT, see the official `tutorial <https://broadinstitute.github.io/wot/tutorial/>`_.
-        """
-        # disallow these params (because they e.g. subset the data)
-        _ = kwargs.pop("cell_day_filter", None)
-        _ = kwargs.pop("covariate_field", None)
-        _ = kwargs.pop("ncounts", None)
-        _ = kwargs.pop("ncells", None)
-        _ = kwargs.pop("parameters", None)  # parameters file
-        kwargs["lambda1"] = lambda1
-        kwargs["lambda2"] = lambda2
-        kwargs["epsilon"] = epsilon
-        kwargs["growth_iters"] = max(growth_iters, 1)
-        last_time_point = LastTimePoint(last_time_point)
+        Nothing, just updates the following fields:
 
-        start = logg.info(
-            "Computing transition matrix using Waddington optimal transport"
+        - :attr:`fate_probabilities` - %(fate_probs.summary)s
+        """
+        start = logg.info("Computing fate probabilities")
+        data = self._rec_trans_states(keys, ctx="fate_probs")
+        fate_probs = self._compute_fate_probabilities(
+            data.q,
+            data.s,
+            trans_indices=data.trans_indices,
+            term_states=data.term_states,
+            solver=solver,
+            use_petsc=use_petsc,
+            n_jobs=n_jobs,
+            backend=backend,
+            tol=tol,
+            show_progress_bar=show_progress_bar,
+            preconditioner=preconditioner,
+        )
+        fate_probs = Lineage(
+            fate_probs,
+            names=list(data.term_states.cat.categories),
+            colors=data.term_states_colors,
+        )
+
+        params = self._create_params(remove=["use_petsc", "n_jobs", "backend", "show_progress_bar"])
+        self._write_fate_probabilities(
+            fate_probs,
+            params=params,
+            time=start,
         )
 
-        adata = _maybe_subset_hvgs(self.adata, use_highly_variable=use_highly_variable)
-        cost_matrices, cmat_param = self._generate_cost_matrices(adata, cost_matrices)
-        if self._reuse_cache(
-            {
-                "cost_matrices": cmat_param,
-                "solver": solver,
-                "growth_rate_key": growth_rate_key,
-                "use_highly_variable": use_highly_variable,
-                "last_time_point": last_time_point,
-                "threshold": threshold,
-                **kwargs,
-            },
-            time=start,
-        ):
-            return self
+    @d.dedent
+    def plot_fate_probabilities(
+        self: FateProbsProtocol,
+        states: Optional[Union[str, Sequence[str]]] = None,
+        color: Optional[str] = None,
+        mode: Literal["embedding", "time"] = PlotMode.EMBEDDING,
+        time_key: Optional[str] = None,
+        same_plot: bool = True,
+        title: Optional[Union[str, Sequence[str]]] = None,
+        cmap: str = "viridis",
+        **kwargs: Any,
+    ) -> None:
+        """Plot fate probabilities.
 
-        tmap = self._compute_pairwise_tmaps(
-            adata,
-            cost_matrices=cost_matrices,
-            solver=solver,
-            growth_rate_field=growth_rate_key,
+        Parameters
+        ----------
+        states
+            Subset of the macrostates to show. If :obj:`None`, plot all macrostates.
+        color
+            Key in :attr:`~anndata.AnnData.obs` or :attr:`anndata.AnnData.var` used to color the observations.
+        mode
+            Whether to plot the probabilities in an embedding or along the pseudotime.
+        time_key
+            Key in :attr:`~anndata.AnnData.obs` where pseudotime is stored. Only used when ``mode = 'time'``.
+        title
+            Title of the plot.
+        same_plot
+            Whether to plot the data on the same plot or not. Only use when ``mode = 'embedding'``.
+            If `True` and ``discrete = False``, ``color`` is ignored.
+        cmap
+            Colormap for continuous annotations.
+        kwargs
+            Keyword arguments for :func:`~scvelo.pl.scatter`.
+
+        Returns
+        -------
+        %(just_plots)s
+        """
+        if self.fate_probabilities is None:
+            raise RuntimeError("Compute fate probabilities first as `.compute_fate_probabilities()`.")
+
+        return self._plot_continuous(
+            _data=self.fate_probabilities,
+            _colors=self.fate_probabilities.colors,
+            _title="fate probabilities",
+            states=states,
+            color=color,
+            mode=mode,
+            time_key=time_key,
+            same_plot=same_plot,
+            title=title,
+            cmap=cmap,
             **kwargs,
         )
-        tmap = self._restich_tmaps(tmap, last_time_point, conn_kwargs=conn_kwargs)
-        self._growth_rates = tmap.obs
 
-        self._compute_transition_matrix(
-            matrix=tmap.X,
-            density_normalize=False,
-            check_irreducibility=False,
-        )
-        if threshold:
-            self._threshold_transition_matrix(threshold)
-        self.adata.obs["estimated_growth_rates"] = self.growth_rates[f"g{growth_iters}"]
+    @d.dedent
+    def compute_absorption_times(
+        self: FateProbsProtocol,
+        keys: Optional[Sequence[str]] = None,
+        calculate_variance: bool = False,
+        solver: Union[str, Literal["direct", "gmres", "lgmres", "bicgstab", "gcrotmk"]] = "gmres",
+        use_petsc: bool = True,
+        n_jobs: Optional[int] = None,
+        backend: Backend_t = DEFAULT_BACKEND,
+        show_progress_bar: Optional[bool] = None,
+        tol: float = 1e-6,
+        preconditioner: Optional[str] = None,
+    ) -> None:
+        """Compute the mean time to absorption and optionally its variance.
 
-        logg.info("    Finish", time=start)
+        Parameters
+        ----------
+        keys
+            Terminal states for which to compute the fate probabilities.
+            If :obj:`None`, use all states defined in :attr:`terminal_states`.
+        calculate_variance
+            Whether to calculate the variance.
+        %(absorption_utils)s
 
-        return self
+        Returns
+        -------
+        Nothing, just updates the following fields:
 
-    def _compute_pairwise_tmaps(
-        self,
-        adata: AnnData,
-        cost_matrices: Optional[
-            Union[str, Mapping[Tuple[float, float], np.ndarray]]
-        ] = None,
-        solver: Literal["fixed_iters", "duality_gap"] = "duality_gap",
-        growth_rate_field: Optional[str] = None,
-        **kwargs: Any,
-    ) -> Dict[Tuple[float, float], AnnData]:
-        _ = wot.ot.OTModel(
-            adata,
-            day_field=self._time_key,
-            covariate_field=None,
-            growth_rate_field=growth_rate_field,
-        )
-        for k in kwargs:
-            if k not in _.ot_config:
-                raise TypeError(f"WOT got an unexpected keyword argument {k!r}.")
-
-        self._ot_model = wot.ot.OTModel(
-            adata,
-            day_field=self._time_key,
-            covariate_field=None,
-            growth_rate_field=growth_rate_field,
+        - :attr:`absorption_times` - %(abs_times.summary)s
+        """
+        start = logg.info("Computing absorption times")
+        if show_progress_bar is None:
+            # prevent from displaying too many progress bars
+            show_progress_bar = not calculate_variance
+
+        data = self._rec_trans_states(keys, ctx="time_to_absorption")
+        abs_times = _calculate_lineage_absorption_time_means(
+            data.q,
+            data.s,
+            calculate_variance=calculate_variance,
+            trans_indices=data.trans_indices,
+            ixs=data.name_to_ixs,
             solver=solver,
-            **kwargs,
+            use_petsc=use_petsc,
+            n_jobs=n_jobs,
+            backend=backend,
+            tol=tol,
+            show_progress_bar=show_progress_bar,
+            preconditioner=preconditioner,
+            index=self.adata.obs_names,
         )
 
-        self._tmaps: Dict[Tuple[float, float], AnnData] = {}
-        start = logg.info(
-            f"Computing transport maps for `{len(cost_matrices)}` time pairs"
+        params = self._create_params(remove=["use_petsc", "n_jobs", "backend", "show_progress_bar"])
+        self._write_absorption_times(
+            abs_times,
+            params=params,
+            time=start,
         )
-        for tpair, cost_matrix in tqdm(cost_matrices.items(), unit="time pair"):
-            tmap: Optional[AnnData] = self._ot_model.compute_transport_map(
-                *tpair, cost_matrix=cost_matrix
-            )
-            if tmap is None:
-                raise TypeError(
-                    f"Unable to compute transport map for time pair `{tpair}`. "
-                    f"Please ensure `adata.obs[{self._time_key!r}]` has the correct dtype (float)."
-                )
-            tmap.X = tmap.X.astype(np.float64)
-            nans = int(np.sum(~np.isfinite(tmap.X)))
-            if nans:
-                raise ValueError(
-                    f"Encountered `{nans}` non-finite values for time pair `{tpair}`."
-                )
-            self._tmaps[tpair] = tmap
 
-        logg.info("    Finish", time=start)
+    @d.dedent
+    def compute_lineage_priming(
+        self: FateProbsProtocol,
+        method: Literal["kl_divergence", "entropy"] = "kl_divergence",
+        early_cells: Optional[Union[Mapping[str, Sequence[str]], Sequence[str]]] = None,
+    ) -> pd.Series:
+        """%(lin_pd.full_desc)s
 
-        return self._tmaps
+        Parameters
+        ----------
+        %(lin_pd.parameters)s
+            If a :class:`dict`, the key specifies a cluster key in :attr:`~anndata.AnnData.obs` and the values
+            specify cluster labels containing early cells.
 
-    def _generate_cost_matrices(
-        self,
-        adata: AnnData,
-        cost_matrices: Optional[
-            Union[str, Mapping[Tuple[float, float], np.ndarray]]
-        ] = None,
-    ) -> Tuple[Mapping[Tuple[float, float], Optional[np.ndarray]], str]:
-        timepoints = self.experimental_time.cat.categories
-        timepoints = list(zip(timepoints[:-1], timepoints[1:]))
-
-        if cost_matrices is None:
-            logg.info("Using default cost matrices")
-            return {tpair: None for tpair in timepoints}, "default"
-
-        if isinstance(cost_matrices, dict):
-            logg.info("Using precomputed cost matrices")
-
-            cmats = {}
-            for tpair in timepoints:
-                if tpair not in cost_matrices:
-                    logg.warning(
-                        f"Unable to find cost matrix for pair `{tpair}`. Using default"
-                    )
-                cmats[tpair] = cmat = cost_matrices.get(tpair, None)
-                if cmat is not None:
-                    n_start = len(np.where(self.experimental_time == tpair[0])[0])
-                    n_end = len(np.where(self.experimental_time == tpair[1])[0])
-                    try:
-                        if cmat.shape != (n_start, n_end):
-                            raise ValueError(
-                                f"Expected cost matrix for time pair `{tpair}` to be "
-                                f"of shape `{(n_start, n_end)}`, found `{cmat.shape}`."
-                            )
-                    except AttributeError:
-                        logg.warning(
-                            f"Unable to verify whether supplied cost matrix for time pair `{tpair}` "
-                            f"has the correct shape `{(n_start, n_end)}`"
-                        )
-
-            # prevent equality comparison when comparing with cache
-            return cmats, nstr("precomputed")
-
-        if isinstance(cost_matrices, str):
-            logg.info(f"Computing cost matrices using `{cost_matrices!r}` key")
-            if cost_matrices == "X":
-                cost_matrices = None
-
-            try:
-                features = adata._get_X(layer=cost_matrices)
-                modifier = "layer"
-            except KeyError:
-                try:
-                    features = adata.obsm[cost_matrices]
-                    modifier = "obsm"
-                except KeyError:
-                    raise KeyError(
-                        f"Unable to find key `{cost_matrices!r}` in `adata.layers` or `adata.obsm`."
-                    ) from None
-
-            cmats = {}
-            for tpair in tqdm(timepoints, unit="cost matrix"):
-                start_ixs = np.where(self.experimental_time == tpair[0])[0]
-                end_ixs = np.where(self.experimental_time == tpair[1])[0]
-
-                # being sparse is handled in WOT's function below
-                cmats[tpair] = wot.ot.OTModel.compute_default_cost_matrix(
-                    features[start_ixs], features[end_ixs]
+        Returns
+        -------
+        Returns the priming degree and updates the following fields:
+
+        - :attr:`priming_degree` - %(priming_degree.summary)s
+        """  # noqa: D400
+        fate_probs = self.fate_probabilities
+        if fate_probs is None:
+            raise RuntimeError("Compute fate probabilities first as `.compute_fate_probabilities()`.")
+        if isinstance(early_cells, dict):
+            if len(early_cells) != 1:
+                raise ValueError(f"Expected a dictionary with only 1 key, found `{len(early_cells)}`.")
+            key = next(iter(early_cells.keys()))
+            if key not in self.adata.obs:
+                raise KeyError(f"Unable to find clusters in `adata.obs[{key!r}]`.")
+            if not is_categorical_dtype(self.adata.obs[key]):
+                raise TypeError(
+                    f"Expected `adata.obs[{key!r}]` to be categorical, " f"found `{infer_dtype(self.adata.obs[key])}`."
                 )
+            early_cells = self.adata.obs[key].isin(early_cells[key])
+        elif early_cells is not None:
+            early_cells = np.asarray(early_cells)
+            if not np.issubdtype(early_cells.dtype, np.bool_):
+                early_cells = np.isin(self.adata.obs_names, early_cells)
+
+        values = pd.Series(fate_probs.priming_degree(method, early_cells), index=self.adata.obs_names)
+        self._write_lineage_priming(values)
+
+        return values
+
+    def _rec_trans_states(
+        self: FateProbsProtocol,
+        keys: Optional[Sequence[str]] = None,
+        *,
+        ctx: Literal["fate_probs", "time_to_absorption"],
+    ) -> RecTransStates:
+        if self.terminal_states is None:
+            raise RuntimeError("Compute terminal states first as `.predict_terminal_states()`.")
+        if keys is not None:
+            keys = sorted(set(keys))
+
+        # get the transition matrix
+        if not sp.issparse(self.transition_matrix):
+            logg.warning("Attempting to solve a potentially large linear system with dense transition matrix")
+
+        # process the current annotations according to `keys`
+        term_states, colors = _process_series(series=self.terminal_states, keys=keys, cols=self._term_states.colors)
+        # warn in case only one state is left
+        keys = list(term_states.cat.categories)
+        if ctx == "fate_probs" and len(keys) == 1:
+            logg.warning("There is only `1` terminal state, all cells will have probability `1` of going there")
+
+        # get indices corresponding to recurrent and transient states
+        rec_indices, trans_indices, name_to_ixs = _get_cat_and_null_indices(term_states)
+        if not len(trans_indices):
+            raise RuntimeError("Markov chain is irreducible.")
+
+        # create Q (restriction transient-transient), S (restriction transient-recurrent)
+        q = self.transition_matrix[trans_indices, :][:, trans_indices]
+        s = self.transition_matrix[trans_indices, :][:, rec_indices]
+
+        # take individual solutions and piece them together to get absorption probabilities towards the classes
+        macro_ix_helper = np.cumsum([0] + [len(indices) for indices in name_to_ixs.values()])
+        # `s` can be sparse or dense, ensure the correct shape
+        s = np.concatenate(
+            [s[:, np.arange(a, b)].sum(axis=1).reshape(-1, 1) for a, b in _pairwise(macro_ix_helper)],
+            axis=1,
+        )
+
+        return RecTransStates(
+            q=q,
+            s=s,
+            trans_indices=trans_indices,
+            rec_indices=rec_indices,
+            name_to_ixs=name_to_ixs,
+            term_states=term_states,
+            term_states_colors=colors,
+        )
+
+    def _compute_fate_probabilities(
+        self: FateProbsProtocol,
+        q: Union[np.ndarray, sp.spmatrix],
+        s: Union[np.ndarray, sp.spmatrix],
+        trans_indices: np.ndarray,
+        term_states: np.ndim,
+        solver: str,
+        use_petsc: bool,
+        n_jobs: Optional[int],
+        backend: str,
+        tol: float,
+        show_progress_bar: bool,
+        preconditioner: str,
+    ) -> np.ndarray:
+        _abs_classes = _solve_lin_system(
+            q,
+            s,
+            solver=solver,
+            use_petsc=use_petsc,
+            n_jobs=n_jobs,
+            backend=backend,
+            tol=tol,
+            use_eye=True,
+            show_progress_bar=show_progress_bar,
+            preconditioner=preconditioner,
+        )
+        abs_classes = np.zeros(shape=(len(self), len(term_states.cat.categories)), dtype=np.float64)
+        for col, rec_class in enumerate(term_states.cat.categories):
+            rec_indices = np.where(term_states == rec_class)[0]
+            abs_classes[trans_indices, col] = _abs_classes[:, col]
+            abs_classes[rec_indices, col] = 1.0
+
+        mask = abs_classes >= 0
+        if not np.all(mask):
+            raise ValueError(
+                f"`{np.sum(~mask)}` value(s) are negative. Try decreasing the tolerance as `tol=...`, "
+                f"specifying a preconditioner as `preconditioner=...` or "
+                f"use a direct solver as `solver='direct'` if the matrix is small."
+            )
+        mask = np.isclose(abs_classes.sum(1), 1.0, rtol=1e-3)
+        if not np.all(mask):
+            raise ValueError(
+                f"`{np.sum(~mask)}` value(s) do not sum to 1 (rtol=1e-3). Try decreasing the tolerance as `tol=...`, "
+                f"specifying a preconditioner as `preconditioner=...` or "
+                f"use a direct solver as `solver='direct'` if the matrix is small."
+            )
 
-            return cmats, f"{modifier}:{cost_matrices}"
+        return abs_classes
 
-        raise NotImplementedError(
-            f"Specifying cost matrices as "
-            f"`{type(cost_matrices).__name__}` is not yet implemented."
-        )
+    @logger
+    @shadow
+    def _write_fate_probabilities(
+        self: FateProbsProtocol,
+        fate_probs: Optional[Lineage],
+        params: Mapping[str, Any] = types.MappingProxyType({}),
+    ) -> str:
+        # fmt: off
+        key = Key.obsm.fate_probs(self.backward)
+        self._set("_fate_probabilities", self.adata.obsm, key=key, value=fate_probs)
+        self._write_lineage_priming(None, log=False)
+        self.params[key] = dict(params)
+        # fmt: on
+
+        return f"Adding `adata.obsm[{key!r}]`\n" f"       `.fate_probabilities`\n" f"    Finish"
+
+    @logger
+    @shadow
+    def _write_absorption_times(
+        self: FateProbsProtocol,
+        abs_times: Optional[pd.DataFrame],
+        params: Mapping[str, Any] = types.MappingProxyType({}),
+    ) -> str:
+        key = Key.obsm.abs_times(self.backward)
+        self._set("_absorption_times", self.adata.obsm, key=key, value=abs_times)
+        self.params[key] = dict(params)
+
+        return f"Adding `adata.obsm[{key!r}]`\n       `.absorption_times`\n    Finish"
+
+    @logger
+    @shadow
+    def _write_lineage_priming(self: FateProbsProtocol, priming_degree: Optional[pd.Series]) -> str:
+        self._priming_degree = priming_degree
+        key = Key.obs.priming_degree(self.backward)
+        self._set("_priming_degree", self.adata.obs, key=key, value=priming_degree)
+
+        # fmt: off
+        return (
+            f"Adding `adata.obs[{key!r}]`\n"
+            f"       `.priming_degree`\n"
+            f"    Finish"
+        )
+        # fmt: on
+
+    def _read_fate_probabilities(self: FateProbsProtocol, adata: AnnData) -> bool:
+        with SafeGetter(self, allowed=KeyError) as sg:
+            key1 = Key.obsm.fate_probs(self.backward)
+            fate_probs = self._get(
+                obj=adata.obsm,
+                key=key1,
+                shadow_attr="obsm",
+                dtype=(np.ndarray, Lineage),
+            )
+            self._fate_probabilities = self._ensure_lineage_object(
+                fate_probs, backward=self.backward, kind="fate_probs"
+            )
+            key = Key.obs.priming_degree(self.backward)
+            self._priming_degree = self._get(
+                obj=adata.obs,
+                key=key,
+                shadow_attr="obs",
+                dtype=pd.Series,
+                allow_missing=True,
+            )
+            self.params[key1] = self._read_params(key1)
 
-    def _threshold_transition_matrix(
-        self, threshold: Union[float, Literal["auto"]]
-    ) -> None:
-        tmat = self.transition_matrix
-        if threshold == "auto":
-            threshold = min(np.max(tmat[i].data) for i in range(tmat.shape[0]))
-            logg.info(f"Using `threshold={threshold}`")
-            tmat.data[tmat.data < threshold] = 0.0
-        else:
-            if not (0 <= threshold <= 100):
-                raise ValueError(
-                    f"Expected `threshold to be in `[0, 100]`, found `{threshold}`.`"
-                )
-            threshold = np.percentile(tmat.data, threshold)
-            logg.info(f"Using `threshold={threshold}`")
-            tmat.data[tmat.data <= threshold] = 0.0
-
-        tmat.eliminate_zeros()
-
-        self._compute_transition_matrix(
-            matrix=tmat,
-            density_normalize=False,
-            check_irreducibility=False,
-        )
+        return sg.ok
 
-    @property
-    def growth_rates(self) -> Optional[pd.DataFrame]:
-        """Estimated cell growth rates for each growth rate iteration."""
-        return self._growth_rates
-
-    def __invert__(self) -> "WOTKernel":
-        super().__invert__()
-        # because WOT reads from `adata`
-        self.adata.obs[self._time_key] = self.experimental_time
-        return self
+    def _read_absorption_times(self: FateProbsProtocol, adata: AnnData) -> bool:
+        with SafeGetter(self, allowed=KeyError) as sg:
+            key = Key.obsm.abs_times(self.backward)
+            self._absorption_times = self._get(
+                obj=adata.obsm,
+                key=key,
+                shadow_attr="obsm",
+                dtype=pd.DataFrame,
+                allow_missing=True,
+            )
+            self.params[key] = self._read_params(key)
+
+        return sg.ok
+
+    def _ensure_lineage_object(
+        self: FateProbsProtocol,
+        obj: Union[str, np.ndarray, Lineage],
+        *,
+        kind: Literal["macrostates", "term_states", "fate_probs"],
+        backward: bool,
+        **kwargs: Any,
+    ) -> Lineage:
+        if isinstance(obj, str):
+            obj = getattr(self, obj)
+        if isinstance(obj, Lineage):
+            return obj
+
+        try:
+            return Lineage.from_adata(
+                self.adata,
+                backward=backward,
+                kind=kind,
+                estimator_backward=self.backward,
+                copy=True,
+                **kwargs,
+            )
+        except Exception as e:  # noqa: BLE001
+            raise RuntimeError(f"Unable to reconstruct `.fate_probabilities`. Reason: `{e}`.") from None
```

### Comparing `cellrank-1.5.1/cellrank/logging/_logging.py` & `cellrank-2.0.0/src/cellrank/logging/_logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-"""Logging module."""
-
-from typing import Optional
-
+import datetime
+import functools
 import logging
-from logging import INFO, DEBUG, ERROR, WARNING, CRITICAL
-from datetime import datetime, timezone, timedelta
-from functools import partial, update_wrapper
+from typing import Iterable, Optional
+
+__all__ = [
+    "print_versions",
+    "print_version_and_date",
+    "hint",
+    "info",
+    "warning",
+    "error",
+    "debug",
+]
 
-HINT = (INFO + DEBUG) // 2
+HINT = (logging.INFO + logging.DEBUG) // 2
 logging.addLevelName(HINT, "HINT")
 
 
 class _RootLogger(logging.RootLogger):
     def __init__(self, level):
         super().__init__(level)
         self.propagate = False
@@ -19,76 +25,70 @@
 
     def log(
         self,
         level: int,
         msg: str,
         *,
         extra: Optional[dict] = None,
-        time: datetime = None,
+        time: datetime.datetime = None,
         deep: Optional[str] = None,
-    ) -> datetime:
+    ) -> datetime.datetime:
         from cellrank import settings
 
         # this will correctly initialize the handles if doing
         # just from cellrank import logging
         settings.verbosity = settings.verbosity
 
-        now = datetime.now(timezone.utc)
-        time_passed: timedelta = None if time is None else now - time
+        now = datetime.datetime.now(datetime.timezone.utc)
+        time_passed: datetime.timedelta = None if time is None else now - time
         extra = {
             **(extra or {}),
             "deep": deep if settings.verbosity.level < level else None,
             "time_passed": time_passed,
         }
-        super().log(level, msg, extra=extra)
+        _ = super().log(level, msg, extra=extra)
         return now
 
-    def critical(self, msg, *, time=None, deep=None, extra=None) -> datetime:
-        return self.log(CRITICAL, msg, time=time, deep=deep, extra=extra)
+    def critical(self, msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
+        return self.log(logging.CRITICAL, msg, time=time, deep=deep, extra=extra)
 
-    def error(self, msg, *, time=None, deep=None, extra=None) -> datetime:
-        return self.log(ERROR, msg, time=time, deep=deep, extra=extra)
+    def error(self, msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
+        return self.log(logging.ERROR, msg, time=time, deep=deep, extra=extra)
 
-    def warning(self, msg, *, time=None, deep=None, extra=None) -> datetime:
-        return self.log(WARNING, msg, time=time, deep=deep, extra=extra)
+    def warning(self, msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
+        return self.log(logging.WARNING, msg, time=time, deep=deep, extra=extra)
 
-    def info(self, msg, *, time=None, deep=None, extra=None) -> datetime:
-        return self.log(INFO, msg, time=time, deep=deep, extra=extra)
+    def info(self, msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
+        return self.log(logging.INFO, msg, time=time, deep=deep, extra=extra)
 
-    def hint(self, msg, *, time=None, deep=None, extra=None) -> datetime:
+    def hint(self, msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
         return self.log(HINT, msg, time=time, deep=deep, extra=extra)
 
-    def debug(self, msg, *, time=None, deep=None, extra=None) -> datetime:
-        return self.log(DEBUG, msg, time=time, deep=deep, extra=extra)
+    def debug(self, msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
+        return self.log(logging.DEBUG, msg, time=time, deep=deep, extra=extra)
 
 
 class _LogFormatter(logging.Formatter):
-    def __init__(
-        self, fmt="{levelname}: {message}", datefmt="%Y-%m-%d %H:%M", style="{"
-    ):
+    def __init__(self, fmt="{levelname}: {message}", datefmt="%Y-%m-%d %H:%M", style="{"):
         super().__init__(fmt, datefmt, style)
 
     def format(self, record: logging.LogRecord):
         format_orig = self._style._fmt
-        if record.levelno == INFO:
+        if record.levelno == logging.INFO:
             self._style._fmt = "{message}"
         elif record.levelno == HINT:
             self._style._fmt = "--> {message}"
-        elif record.levelno == DEBUG:
+        elif record.levelno == logging.DEBUG:
             self._style._fmt = "DEBUG: {message}"
         if record.time_passed:
             # strip microseconds
             if record.time_passed.microseconds:
-                record.time_passed = timedelta(
-                    seconds=int(record.time_passed.total_seconds())
-                )
+                record.time_passed = datetime.timedelta(seconds=int(record.time_passed.total_seconds()))
             if "{time_passed}" in record.msg:
-                record.msg = record.msg.replace(
-                    "{time_passed}", str(record.time_passed)
-                )
+                record.msg = record.msg.replace("{time_passed}", str(record.time_passed))
             else:
                 self._style._fmt += " ({time_passed})"
         if record.deep:
             record.msg = f"{record.msg}: {record.deep}"
         result = logging.Formatter.format(self, record)
         self._style._fmt = format_orig
         return result
@@ -109,24 +109,21 @@
     "pygam",
 ]
 
 
 _DEPENDENCIES_PLOTTING = ["matplotlib", "seaborn"]
 
 
-def _versions_dependencies(dependencies):
+def _versions_dependencies(dependencies: Iterable[str]):
     # this is not the same as the requirements!
     for mod in dependencies:
         mod_name, dist_name = mod if isinstance(mod, tuple) else (mod, mod)
         try:
             imp = __import__(mod_name)
-            if mod == "cellrank":
-                yield dist_name, imp.__full_version__
-            else:
-                yield dist_name, imp.__version__
+            yield dist_name, imp.__version__
         except (ImportError, AttributeError):
             pass
 
 
 def print_versions():
     """Print package versions that might influence the numerical and plotting results."""
     from cellrank import settings
@@ -140,34 +137,33 @@
 
 def print_version_and_date():
     """
     Print version and date.
 
     Useful for starting a notebook so you see when you started working.
     """
-
-    from cellrank import settings, __full_version__
+    from cellrank import __version__, settings
 
     print(
-        f"Running CellRank {__full_version__}, on {datetime.now():%Y-%m-%d %H:%M}.",
+        f"Running CellRank {__version__}, on {datetime.datetime.now():%Y-%m-%d %H:%M}.",
         file=settings.logfile,
     )
 
 
 def _copy_docs_and_signature(fn):
-    return partial(update_wrapper, wrapped=fn, assigned=["__doc__", "__annotations__"])
+    return functools.partial(functools.update_wrapper, wrapped=fn, assigned=["__doc__", "__annotations__"])
 
 
 def error(
     msg: str,
     *,
-    time: datetime = None,
+    time: datetime.datetime = None,
     deep: Optional[str] = None,
     extra: Optional[dict] = None,
-) -> datetime:
+) -> datetime.datetime:
     """
     Log message with specific level and return current time.
 
     Parameters
     ----------
     msg
         Message to display.
@@ -180,41 +176,40 @@
         If the current verbosity is higher than the log function’s level,
         this gets displayed as well
     extra
         Additional values you can specify in `msg` like `{time_passed}`.
 
     Returns
     -------
-    :class:`datetime.datetime`
-        The current time.
+    The current time.
     """
     from cellrank import settings
 
     return settings._root_logger.error(msg, time=time, deep=deep, extra=extra)
 
 
 @_copy_docs_and_signature(error)
-def warning(msg: str, *, time=None, deep=None, extra=None) -> datetime:  # noqa
+def warning(msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
     from cellrank import settings
 
     return settings._root_logger.warning(msg, time=time, deep=deep, extra=extra)
 
 
 @_copy_docs_and_signature(error)
-def info(msg: str, *, time=None, deep=None, extra=None) -> datetime:  # noqa
+def info(msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
     from cellrank import settings
 
     return settings._root_logger.info(msg, time=time, deep=deep, extra=extra)
 
 
 @_copy_docs_and_signature(error)
-def hint(msg: str, *, time=None, deep=None, extra=None) -> datetime:  # noqa
+def hint(msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
     from cellrank import settings
 
     return settings._root_logger.hint(msg, time=time, deep=deep, extra=extra)
 
 
 @_copy_docs_and_signature(error)
-def debug(msg: str, *, time=None, deep=None, extra=None) -> datetime:  # noqa
+def debug(msg: str, *, time=None, deep=None, extra=None) -> datetime.datetime:
     from cellrank import settings
 
     return settings._root_logger.debug(msg, time=time, deep=deep, extra=extra)
```

### Comparing `cellrank-1.5.1/cellrank/pl/_circular_projection.py` & `cellrank-2.0.0/src/cellrank/pl/_circular_projection.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-from typing import Any, Tuple, Union, Mapping, Callable, Optional, Sequence
-from typing_extensions import Literal
-
-from enum import auto
-from types import MappingProxyType
-from pathlib import Path
+import enum
+import pathlib
+import types
+from typing import Any, Callable, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import scvelo as scv
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank.tl import Lineage
-from cellrank._key import Key
-from scanpy._utils import deprecated_arg_names
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d
-from cellrank.pl._utils import _held_karp
-from cellrank.tl._utils import save_fig, _unique_order_preserving
-from cellrank.ul._utils import _check_collection
-from cellrank.tl._lineage import PrimingDegree
 
 import numpy as np
 import pandas as pd
 from sklearn.metrics import pairwise_distances
 
 import matplotlib.pyplot as plt
-from matplotlib.colors import LogNorm, LinearSegmentedColormap
 from matplotlib.collections import LineCollection
+from matplotlib.colors import LinearSegmentedColormap, LogNorm
+
+from anndata import AnnData
+from scanpy._utils import deprecated_arg_names
+
+from cellrank import logging as logg
+from cellrank._utils import Lineage
+from cellrank._utils._docs import d
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._key import Key
+from cellrank._utils._lineage import PrimingDegree
+from cellrank._utils._utils import _check_collection, _unique_order_preserving, save_fig
+from cellrank.pl._utils import _held_karp
+
+__all__ = ["circular_projection"]
 
 
-class LineageOrder(ModeEnum):  # noqa: D101
-    DEFAULT = auto()
-    OPTIMAL = auto()
+class LineageOrder(ModeEnum):
+    DEFAULT = enum.auto()
+    OPTIMAL = enum.auto()
 
 
-class LabelRot(ModeEnum):  # noqa: D101
-    DEFAULT = auto()
-    BEST = auto()
+class LabelRot(ModeEnum):
+    DEFAULT = enum.auto()
+    BEST = enum.auto()
 
 
 Metric_T = Union[str, Callable, np.ndarray, pd.DataFrame]
 _N = 200
 
 
 def _get_distances(data: Union[np.ndarray, Lineage], metric: Metric_T) -> np.ndarray:
@@ -77,162 +78,150 @@
     early_cells: Optional[Union[Mapping[str, Sequence[str]], Sequence[str]]] = None,
     lineage_order: Optional[Literal["default", "optimal"]] = None,
     metric: Union[str, Callable, np.ndarray, pd.DataFrame] = "correlation",
     normalize_by_mean: bool = True,
     ncols: int = 4,
     space: float = 0.25,
     use_raw: bool = False,
-    text_kwargs: Mapping[str, Any] = MappingProxyType({}),
+    text_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
     label_distance: float = 1.25,
     label_rot: Union[Literal["default", "best"], float] = "best",
     show_edges: bool = True,
     key_added: Optional[str] = None,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
+    save: Optional[Union[str, pathlib.Path]] = None,
     **kwargs: Any,
-):
-    r"""
-    Plot absorption probabilities on a circular embedding as in :cite:`velten:17`.
+) -> None:
+    r"""Visualize fate probabilities in a circular embedding :cite:`velten:17,jaitin:14`.
+
+    We arrange all computed terminal states evenly spaced around the unit circle and place
+    cells inside the unit circle in a way that reflects their fate probabilities. In other words,
+    the more certain we are that a cell will transition towards a given terminal state, the closer
+    we place it to that terminal state. Uncommitted cells thus reside in the middle of the circle.
 
     Parameters
     ----------
     %(adata)s
     keys
-        Keys in :attr:`anndata.AnnData.obs` or :attr:`anndata.AnnData.var_names`. Additional keys are:
-
-            - `'kl_divergence'` - as in :cite:`velten:17`, computes KL-divergence between the fate probabilities
-              of a cell and the average fate probabilities. See ``early_cells`` for more information.
-            - `'entropy'` - as in :cite:`setty:19`, computes entropy over a cells fate probabilities.
+        Keys in :attr:`~anndata.AnnData.obs` or :attr:`~anndata.AnnData.var_names`. Additional keys are:
 
+        - ``'kl_divergence'`` - as in :cite:`velten:17`, computes KL-divergence between the fate probabilities
+          of a cell and the average fate probabilities. See ``early_cells`` for more information.
+        - ``'entropy'`` - as in :cite:`setty:19`, computes entropy over a cells fate probabilities.
     %(backward)s
     lineages
-        Lineages to plot. If `None`, plot all lineages.
+        Lineages to plot. If :obj:`None`, plot all lineages.
     early_cells
-        Cell ids or a mask marking early cells used to define the average fate probabilities. If `None`, use all cells.
-        Only used when `'kl_divergence'` is in ``keys``. If a :class:`dict`, key specifies a cluster key in
-        :attr:`anndata.AnnData.obs` and the values specify cluster labels containing early cells.
+        Cell ids or a mask marking early cells used to define the average fate probabilities. If :obj:`None`,
+        use all cells. Only used when ``'kl_divergence'`` is in the ``keys``. If a :class:`dict`, key specifies
+        a cluster key in :attr:`~anndata.AnnData.obs` and the values specify cluster labels containing early cells.
     lineage_order
         Can be one of the following:
 
-            - `None` - it will determined automatically, based on the number of lineages.
-            - `'optimal'` - order lineages optimally by solving the Travelling salesman problem (TSP).
-              Recommended for <= `20` lineages.
-            - `'default'` - use the order as specified by ``lineages``.
-
+        - :obj:`None` - it will be determined automatically, based on the number of lineages.
+        - ``'optimal'`` - order lineages optimally by solving the Traveling salesman problem (TSP).
+          Recommended for <= :math:`20` lineages.
+        - ``'default'`` - use the order as specified by ``lineages``.
     metric
         Metric to use when constructing pairwise distance matrix when ``lineage_order = 'optimal'``. For available
-        options, see :func:`sklearn.metrics.pairwise_distances`.
+        options, see :func:`~sklearn.metrics.pairwise_distances`.
     normalize_by_mean
-        If `True`, normalize each lineage by its mean probability, as done in :cite:`velten:17`.
+        If :obj:`True`, normalize each lineage by its mean probability, as done in :cite:`velten:17`.
     ncols
         Number of columns when plotting multiple ``keys``.
     space
-        Horizontal and vertical space between for :func:`matplotlib.pyplot.subplots_adjust`.
+        Horizontal and vertical space between for :func:`~matplotlib.pyplot.subplots_adjust`.
     use_raw
-        Whether to access :attr:`anndata.AnnData.raw` when there are ``keys`` in :attr:`anndata.AnnData.var_names`.
+        Whether to access :attr:`~anndata.AnnData.raw` when there are ``keys`` in :attr:`~anndata.AnnData.var_names`.
     text_kwargs
-        Keyword arguments for :func:`matplotlib.pyplot.text`.
+        Keyword arguments for :meth:`~matplotlib.axes.Axes.text`.
     label_distance
         Distance at which the lineage labels will be drawn.
     label_rot
         How to rotate the labels. Valid options are:
 
-            - `'best'` - rotate labels so that they are easily readable.
-            - `'default'` - use :mod:`matplotlib`'s default.
-            - `None` - same as `'default'`.
-
-        If a :class:`float`, all labels will be rotated by this many degrees.
+        - ``'best'`` - rotate labels so that they are easily readable.
+        - ``'default'`` - use :mod:`matplotlib`'s default.
+        - :obj:`None` - same as ``'default'``.
+        - :class:`float`, all labels will be rotated by this many degrees.
     show_edges
         Whether to show the edges surrounding the simplex.
     key_added
-        Key in :attr:`anndata.AnnData.obsm` where to add the circular embedding. If `None`, it will be set to
-        `'X_fate_simplex_{fwd,bwd}'`, based on ``backward``.
+        Key in :attr:`~anndata.AnnData.obsm` where to add the circular embedding. If :obj:`None`, it will be set to
+        ``'X_fate_simplex_{fwd,bwd}'``, based on the ``backward``.
     %(plotting)s
     kwargs
-        Keyword arguments for :func:`scvelo.pl.scatter`.
+        Keyword arguments for :func:`~scvelo.pl.scatter`.
 
     Returns
     -------
-    %(just_plots)s
-        Also updates ``adata`` with the following fields:
+    %(just_plots)s Also updates ``adata`` with the following fields:
 
-            - :attr:`anndata.AnnData.obsm` ``['{key_added}']`` - the circular projection.
-            - :attr:`anndata.AnnData.obs` ``['to_{initial,terminal}_states_{method}']`` - the priming degree,
-              if a method is present in ``keys``.
+    - :attr:`adata.obsm['{key_added}'] <anndata.AnnData.obsm>` - the circular projection.
+    - :attr:`adata.obs['to_{initial,terminal}_states_{method}'] <anndata.AnnData.obs>` - the priming degree,
+      if a method is present in the ``keys``.
     """
     if label_distance is not None and label_distance < 0:
-        raise ValueError(
-            f"Expected `label_distance` to be positive, found `{label_distance}`."
-        )
+        raise ValueError(f"Expected `label_distance` to be positive, found `{label_distance}`.")
 
     if label_rot is None:
         label_rot = LabelRot.DEFAULT
     label_rot = LabelRot(label_rot)
 
     suffix = "bwd" if backward else "fwd"
     if key_added is None:
         key_added = "X_fate_simplex_" + suffix
 
     if isinstance(keys, str):
         keys = (keys,)
 
     keys = _unique_order_preserving(keys)
-    keys_ = _check_collection(
-        adata, keys, "obs", key_name="Observation", raise_exc=False
-    ) + _check_collection(
+    keys_ = _check_collection(adata, keys, "obs", key_name="Observation", raise_exc=False) + _check_collection(
         adata, keys, "var_names", key_name="Gene", raise_exc=False, use_raw=use_raw
     )
     haystack = set(PrimingDegree)
     keys = keys_ + [k for k in keys if k in haystack]
     keys = _unique_order_preserving(keys)
 
     if not len(keys):
         raise ValueError("No valid keys have been selected.")
 
-    lineage_key = Key.obsm.abs_probs(backward)
-    if lineage_key not in adata.obsm:
-        raise KeyError(f"Lineages key `{lineage_key!r}` not found in `adata.obsm`.")
-
-    probs: Lineage = adata.obsm[lineage_key]
-
+    probs = Lineage.from_adata(adata, backward=backward)
     if isinstance(lineages, str):
-        lineages = (lineages,)
+        lineages = [lineages]
     elif lineages is None:
         lineages = probs.names
-
-    probs = adata.obsm[lineage_key][lineages]
-    n_lin = probs.shape[1]
-    if n_lin < 3:
-        raise ValueError(f"Expected at least `3` lineages, found `{n_lin}`.")
+    lineages = _unique_order_preserving(lineages)
+    probs = probs[lineages]
+    if probs.nlin < 3:
+        raise ValueError(f"Expected at least `3` lineages, found `{probs.nlin}`.")
 
     X = probs.X.copy()
     if normalize_by_mean:
         X /= np.mean(X, axis=0)[None, :]
         X /= X.sum(1)[:, None]
         # this happens when cells for sel. lineages sum to 1 (or when the lineage average is 0, which is unlikely)
-        X = np.nan_to_num(X, nan=1.0 / n_lin, copy=False)
+        X = np.nan_to_num(X, nan=1.0 / probs.nlin, copy=False)
 
     if lineage_order is None:
-        lineage_order = (
-            LineageOrder.OPTIMAL if 3 < n_lin <= 20 else LineageOrder.DEFAULT
-        )
+        lineage_order = LineageOrder.OPTIMAL if 3 < probs.nlin <= 20 else LineageOrder.DEFAULT
         logg.debug(f"Set ordering to `{lineage_order}`")
     lineage_order = LineageOrder(lineage_order)
 
     if lineage_order == LineageOrder.OPTIMAL:
-        logg.info(f"Solving TSP for `{n_lin}` states")
+        logg.info(f"Solving TSP for `{probs.nlin}` states")
         _, order = _get_optimal_order(X, metric=metric)
     else:
-        order = np.arange(n_lin)
+        order = np.arange(probs.nlin)
 
     probs = probs[:, order]
     X = X[:, order]
 
-    angle_vec = np.linspace(0, 2 * np.pi, n_lin, endpoint=False)
+    angle_vec = np.linspace(0, 2 * np.pi, probs.nlin, endpoint=False)
     angle_vec_sin = np.cos(angle_vec)
     angle_vec_cos = np.sin(angle_vec)
 
     x = np.sum(X * angle_vec_sin, axis=1)
     y = np.sum(X * angle_vec_cos, axis=1)
     adata.obsm[key_added] = np.c_[x, y]
 
@@ -247,25 +236,25 @@
     fig.subplots_adjust(wspace=space, hspace=space)
     axes = np.ravel([ax])
 
     text_kwargs = dict(text_kwargs)
     text_kwargs["ha"] = "center"
     text_kwargs["va"] = "center"
 
-    _i = 0
+    _i, lineage_key = 0, Key.obsm.fate_probs(backward)
     for _i, (k, ax) in enumerate(zip(keys, axes)):
-
         set_lognorm, colorbar = False, kwargs.pop("colorbar", True)
         try:
             _ = PrimingDegree(k)
             logg.debug(f"Calculating priming degree using `method={k}`")
             val = probs.priming_degree(method=k, early_cells=early_cells)
             k = f"{lineage_key}_{k}"
             adata.obs[k] = val
         except ValueError:
+            # TODO(michalk8): parse the exception
             pass
 
         scv.pl.scatter(
             adata,
             basis=key_added,
             color=k,
             show=False,
@@ -301,32 +290,28 @@
         for color, text in zip(probs.colors[::-1], texts):
             if isinstance(label_rot, (int, float)):
                 text.set_rotation(label_rot)
             elif label_rot == LabelRot.BEST:
                 rot = text.get_rotation()
                 text.set_rotation(rot + 90 + (1 - rot // 180) * 180)
             elif label_rot != LabelRot.DEFAULT:
-                raise NotImplementedError(
-                    f"Label rotation `{label_rot}` is not yet implemented."
-                )
+                raise NotImplementedError(f"Label rotation `{label_rot}` is not yet implemented.")
             text.set_color(color)
 
         if not show_edges:
             continue
 
         for i, color in enumerate(probs.colors):
-            next = (i + 1) % n_lin
+            next = (i + 1) % probs.nlin
             x = 1.04 * np.linspace(angle_vec_sin[i], angle_vec_sin[next], _N)
             y = 1.04 * np.linspace(angle_vec_cos[i], angle_vec_cos[next], _N)
             points = np.array([x, y]).T.reshape(-1, 1, 2)
             segments = np.concatenate([points[:-1], points[1:]], axis=1)
 
-            cmap = LinearSegmentedColormap.from_list(
-                "abs_prob_cmap", [color, probs.colors[next]], N=_N
-            )
+            cmap = LinearSegmentedColormap.from_list("fate_prob_cmap", [color, probs.colors[next]], N=_N)
             lc = LineCollection(segments, cmap=cmap, zorder=-1)
             lc.set_array(np.linspace(0, 1, _N))
             lc.set_linewidth(2)
             ax.add_collection(lc)
 
     for j in range(_i + 1, len(axes)):
         axes[j].remove()
```

### Comparing `cellrank-1.5.1/cellrank/pl/_cluster_fates.py` & `cellrank-2.0.0/src/cellrank/pl/_aggregate_fate_probs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,174 +1,175 @@
-from typing import Any, Tuple, Union, Mapping, Optional, Sequence
-from typing_extensions import Literal
+import collections
+import enum
+import math
+import pathlib
+import types
+from typing import Any, Literal, Mapping, Optional, Sequence, Tuple, Union
 
-from enum import auto
-from math import ceil
-from types import MappingProxyType
-from pathlib import Path
-from collections import OrderedDict as odict
-
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank._key import Key
-from scanpy.plotting import violin
 from scvelo.plotting import paga
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d, inject_docs
-from cellrank.pl._utils import _position_legend
-from cellrank.tl._utils import RandomKeys, save_fig, _unique_order_preserving
-from cellrank.ul._utils import valuedispatch
 
 import numpy as np
 import pandas as pd
-from scipy.sparse import csr_matrix
+import scipy.sparse as sp
 
 import matplotlib as mpl
-import matplotlib.colors
 import matplotlib.pyplot as plt
-from seaborn import heatmap, clustermap
-from matplotlib import cm
+import seaborn as sns
+from matplotlib import cm, colors
+
+from anndata import AnnData
+from scanpy.plotting import violin
+
+from cellrank import logging as logg
+from cellrank._utils import Lineage
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._key import Key
+from cellrank._utils._utils import (
+    RandomKeys,
+    _unique_order_preserving,
+    save_fig,
+    valuedispatch,
+)
+from cellrank.pl._utils import _position_legend
 
+__all__ = ["aggregate_fate_probabilities"]
 
-class ClusterFatesMode(ModeEnum):  # noqa: D101
-    BAR = auto()
-    PAGA = auto()
-    PAGA_PIE = auto()
-    VIOLIN = auto()
-    HEATMAP = auto()
-    CLUSTERMAP = auto()
+
+class AggregationMode(ModeEnum):
+    BAR = enum.auto()
+    PAGA = enum.auto()
+    PAGA_PIE = enum.auto()
+    VIOLIN = enum.auto()
+    HEATMAP = enum.auto()
+    CLUSTERMAP = enum.auto()
 
 
 @d.dedent
-@inject_docs(m=ClusterFatesMode)
-def cluster_fates(
+@inject_docs(m=AggregationMode)
+def aggregate_fate_probabilities(
     adata: AnnData,
-    mode: Literal[
-        "bar", "paga", "paga_pie", "violin", "heatmap", "clustermap"
-    ] = ClusterFatesMode.PAGA_PIE,
+    mode: Literal["bar", "paga", "paga_pie", "violin", "heatmap", "clustermap"] = AggregationMode.PAGA_PIE,
     backward: bool = False,
     lineages: Optional[Union[str, Sequence[str]]] = None,
     cluster_key: Optional[str] = "clusters",
     clusters: Optional[Union[str, Sequence[str]]] = None,
     basis: Optional[str] = None,
     cbar: bool = True,
     ncols: Optional[int] = None,
     sharey: bool = False,
     fmt: str = "0.2f",
     xrot: float = 90,
-    legend_kwargs: Mapping[str, Any] = MappingProxyType({"loc": "best"}),
+    legend_kwargs: Mapping[str, Any] = types.MappingProxyType({"loc": "best"}),
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
+    save: Optional[Union[str, pathlib.Path]] = None,
     **kwargs: Any,
 ) -> None:
-    """
-    Plot aggregate lineage probabilities at a cluster level.
+    """Plot aggregate lineage probabilities at a cluster level.
 
-    This can be used to investigate how likely a certain cluster is to go to the %(terminal)s states, or in turn to have
-    descended from the %(initial)s states.
-    For mode `{m.PAGA!r}` and `{m.PAGA_PIE!r}`, we use *PAGA*, see :cite:`wolf:19`.
+    This can be used to investigate how likely a certain cluster is to go to the %(terminal)s states,
+    or in turn to have descended from the %(initial)s states.
+    For mode `{m.PAGA!r}` and `{m.PAGA_PIE!r}`, we use *PAGA* :cite:`wolf:19`.
 
     Parameters
     ----------
     %(adata)s
     mode
         Type of plot to show. Valid options are:
 
-            - `{m.BAR!r}` - barplot, one panel per cluster. The whiskers correspond to the standard error of the mean.
-            - `{m.PAGA!r}` - scanpy's PAGA, one per %(initial_or_terminal)s state, colored in by fate.
-            - `{m.PAGA_PIE!r}` - scanpy's PAGA with pie charts indicating aggregated fates.
-            - `{m.VIOLIN!r}` - violin plots, one per %(initial_or_terminal)s state.
-            - `{m.HEATMAP!r}` - a heatmap, showing average fates per cluster.
-            - `{m.CLUSTERMAP!r}` - same as a heatmap, but with a dendrogram.
+        - ``{m.BAR!r}`` - barplot, one panel per cluster. The whiskers correspond to the standard error of the mean.
+        - ``{m.PAGA!r}`` - :func:`~scvelo.pl.paga`, one per %(initial_or_terminal)s state, colored in by fate.
+        - ``{m.PAGA_PIE!r}`` - :func:`~scvelo.pl.paga` with pie charts indicating aggregated fates.
+        - ``{m.VIOLIN!r}`` - violin plots, one per %(initial_or_terminal)s state.
+        - ``{m.HEATMAP!r}`` - a heatmap, showing average fates per cluster.
+        - ``{m.CLUSTERMAP!r}`` - same as a heatmap, but with a dendrogram.
     %(backward)s
     lineages
-        Lineages for which to visualize absorption probabilities. If `None`, use all lineages.
+        Lineages for which to visualize the fate probabilities. If :obj:`None`, use all lineages.
     cluster_key
-        Key in ``adata.obs`` containing the clusters.
+        Key in :attr:`~anndata.AnnData.obs` containing the clusters.
     clusters
-        Clusters to visualize. If `None`, all clusters will be plotted.
+        Clusters to visualize. If :obj:`None`, all clusters will be plotted.
     basis
-        Basis for scatterplot to use when ``mode = {m.PAGA_PIE!r}``. If `None`, don't show the scatterplot.
+        Basis for scatterplot to use when ``mode = {m.PAGA_PIE!r}``. If :obj:`None`, don't show the scatterplot.
     cbar
         Whether to show colorbar when ``mode = {m.PAGA_PIE!r}``.
     ncols
         Number of columns when ``mode = {m.BAR!r}`` or ``mode = {m.PAGA!r}``.
     sharey
         Whether to share y-axis when ``mode = {m.BAR!r}``.
     fmt
         Format when using ``mode = {m.HEATMAP!r}`` or ``mode = {m.CLUSTERMAP!r}``.
     xrot
         Rotation of the labels on the x-axis.
     figsize
         Size of the figure.
     legend_kwargs
-        Keyword arguments for :func:`matplotlib.axes.Axes.legend`, such as `'loc'` for legend position.
+        Keyword arguments for :meth:`~matplotlib.axes.Axes.legend`.
         For ``mode = {m.PAGA_PIE!r}`` and ``basis = '...'``, this controls the placement of the
-        absorption probabilities legend.
+        fate probabilities legend.
     %(plotting)s
     kwargs
-        Keyword arguments for :func:`scvelo.pl.paga`, :func:`scanpy.pl.violin` or :func:`matplotlib.pyplot.bar`,
-        depending on the ``mode``.
+        Keyword arguments for :func:`~scvelo.pl.paga`, :func:`~scanpy.pl.violin` or
+        :func:`~matplotlib.pyplot.bar`, depending on the ``mode``.
 
     Returns
     -------
     %(just_plots)s
     """
 
     @valuedispatch
-    def plot(mode: ClusterFatesMode, *_args, **_kwargs):
+    def plot(mode: AggregationMode, *_args, **_kwargs):
         raise NotImplementedError(mode.value)
 
-    @plot.register(ClusterFatesMode.BAR)
+    @plot.register(AggregationMode.BAR)
     def _():
         cols = 4 if ncols is None else ncols
-        n_rows = ceil(len(clusters) / cols)
-        fig = plt.figure(
-            None, (3.5 * cols, 5 * n_rows) if figsize is None else figsize, dpi=dpi
-        )
+        n_rows = math.ceil(len(clusters) / cols)
+        fig = plt.figure(None, (3.5 * cols, 5 * n_rows) if figsize is None else figsize, dpi=dpi)
         fig.tight_layout()
 
         gs = plt.GridSpec(n_rows, cols, figure=fig, wspace=0.5, hspace=0.5)
 
         ax = None
-        colors = list(adata.obsm[lineage_key][:, lin_names].colors)
+        colors = list(probs.colors)
 
         for g, k in zip(gs, d.keys()):
             current_ax = fig.add_subplot(g, sharey=ax)
             current_ax.bar(
-                x=np.arange(len(lin_names)),
+                x=np.arange(probs.nlin),
                 height=d[k][0],
                 color=colors,
                 yerr=d[k][1],
                 ecolor="black",
                 capsize=10,
                 **kwargs,
             )
             if sharey:
                 ax = current_ax
 
-            current_ax.set_xticks(np.arange(len(lin_names)))
-            current_ax.set_xticklabels(lin_names, rotation=xrot)
+            current_ax.set_xticks(np.arange(probs.nlin))
+            current_ax.set_xticklabels(probs.names, rotation=xrot)
             if not is_all:
                 current_ax.set_xlabel(term_states)
-            current_ax.set_ylabel("absorption probability")
+            current_ax.set_ylabel("fate probability")
             current_ax.set_title(k)
 
         return fig
 
-    @plot.register(ClusterFatesMode.PAGA)
+    @plot.register(AggregationMode.PAGA)
     def _():
         kwargs["save"] = None
         kwargs["show"] = False
         if "cmap" not in kwargs:
             kwargs["cmap"] = cm.viridis
 
-        cols = len(lin_names) if ncols is None else ncols
-        nrows = ceil(len(lin_names) / cols)
+        cols = probs.nlin if ncols is None else ncols
+        nrows = math.ceil(probs.nlin / cols)
         fig, axes = plt.subplots(
             nrows,
             cols,
             figsize=(7 * cols, 4 * nrows) if figsize is None else figsize,
             constrained_layout=True,
             dpi=dpi,
         )
@@ -179,45 +180,44 @@
         vmin, vmax = np.inf, -np.inf
 
         if basis is not None:
             kwargs["basis"] = basis
             kwargs["scatter_flag"] = True
             kwargs["color"] = cluster_key
 
-        for i, (ax, lineage_name) in enumerate(zip(axes, lin_names)):
-            colors = [v[0][i] for v in d.values()]
+        for i, (ax, lineage_name) in enumerate(zip(axes, probs.names)):
+            cols = [v[0][i] for v in d.values()]
             kwargs["ax"] = ax
-            kwargs["colors"] = tuple(colors)
+            kwargs["colors"] = tuple(cols)
             kwargs["title"] = f"{direction} {lineage_name}"
 
-            vmin = np.min(colors + [vmin])
-            vmax = np.max(colors + [vmax])
+            vmin = np.min(cols + [vmin])
+            vmax = np.max(cols + [vmax])
 
             paga(adata, **kwargs)
 
         if cbar:
-            norm = matplotlib.colors.Normalize(vmin=vmin, vmax=vmax)
+            norm = colors.Normalize(vmin=vmin, vmax=vmax)
             cax, _ = mpl.colorbar.make_axes(ax, aspect=60)
             _ = mpl.colorbar.ColorbarBase(
                 cax,
                 ticks=np.linspace(norm.vmin, norm.vmax, 5),
                 norm=norm,
                 cmap=kwargs["cmap"],
-                label="average absorption probability",
+                label="average fate probability",
             )
 
         for ax in axes[i + 1 :]:
             ax.remove()
 
         return fig
 
-    @plot.register(ClusterFatesMode.PAGA_PIE)
+    @plot.register(AggregationMode.PAGA_PIE)
     def _():
-        colors = list(adata.obsm[lineage_key][:, lin_names].colors)
-        colors = {i: odict(zip(colors, mean)) for i, (mean, _) in enumerate(d.values())}
+        colors = {i: collections.OrderedDict(zip(probs.colors, mean)) for i, (mean, _) in enumerate(d.values())}
 
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
         fig.tight_layout()
 
         kwargs["ax"] = ax
         kwargs["show"] = False
         kwargs["colorbar"] = False  # has to be disabled
@@ -259,42 +259,42 @@
             )
             fig.add_artist(first_legend)
 
         if legend_kwargs.get("loc", None) not in ("none", "on data", None):
             # we need to use these, because scvelo can have its own handles and
             # they would be plotted here
             handles = []
-            for lineage_name, color in zip(lin_names, colors[0].keys()):
+            for lineage_name, color in zip(probs.names, colors[0].keys()):
                 handles += [ax.scatter([], [], label=lineage_name, c=color)]
-            if len(colors[0].keys()) != len(adata.obsm[lineage_key].names):
+            if len(colors[0].keys()) != Lineage.from_adata(adata, backward=backward).nlin:
                 handles += [ax.scatter([], [], label="Rest", c="grey")]
 
             second_legend = _position_legend(
                 ax,
                 legend_loc=legend_kwargs["loc"],
                 handles=handles,
                 **{k: v for k, v in legend_kwargs.items() if k != "loc"},
                 title=term_states,
             )
             fig.add_artist(second_legend)
 
         return fig
 
-    @plot.register(ClusterFatesMode.VIOLIN)
+    @plot.register(AggregationMode.VIOLIN)
     def _():
         kwargs.pop("ax", None)
         kwargs.pop("keys", None)
         kwargs.pop("save", None)  # we will handle saving
 
         kwargs["show"] = False
         kwargs["groupby"] = cluster_key
         kwargs["rotation"] = xrot
 
-        cols = len(lin_names) if ncols is None else ncols
-        nrows = ceil(len(lin_names) / cols)
+        cols = probs.nlin if ncols is None else ncols
+        nrows = math.ceil(probs.nlin / cols)
 
         fig, axes = plt.subplots(
             nrows,
             cols,
             figsize=(6 * cols, 4 * nrows) if figsize is None else figsize,
             sharey=sharey,
             dpi=dpi,
@@ -302,22 +302,20 @@
         fig.tight_layout()
         fig.subplots_adjust(wspace=0.2, hspace=0.3)
 
         if not isinstance(axes, np.ndarray):
             axes = [axes]
         axes = np.ravel(axes)
 
-        with RandomKeys(adata, len(lin_names), where="obs") as keys:
+        with RandomKeys(adata, probs.nlin, where="obs") as keys:
             _i = 0
-            for _i, (name, key, ax) in enumerate(zip(lin_names, keys, axes)):
-                adata.obs[key] = adata.obsm[lineage_key][name].X
+            for _i, (name, key, ax) in enumerate(zip(probs.names, keys, axes)):
+                adata.obs[key] = probs[name].X[:, 0]
                 ax.set_title(f"{direction} {name}")
-                violin(
-                    adata, ylabel="absorption probability", keys=key, ax=ax, **kwargs
-                )
+                violin(adata, ylabel="fate probability", keys=key, ax=ax, **kwargs)
             for ax in axes[_i + 1 :]:
                 ax.remove()
 
         return fig
 
     def plot_violin_no_cluster_key():
         kwargs.pop("ax", None)
@@ -325,69 +323,58 @@
         kwargs.pop("save", None)
 
         kwargs["show"] = False
         kwargs["groupby"] = term_states
         kwargs["xlabel"] = None
         kwargs["rotation"] = xrot
 
-        data = np.ravel(adata.obsm[lineage_key].X.T)[..., np.newaxis]
-        tmp = AnnData(csr_matrix(data.shape, dtype=np.float32))
-        tmp.obs["absorption probability"] = data
+        data = np.ravel(probs.X.T)[..., None]
+        tmp = AnnData(sp.csr_matrix(data.shape, dtype=data.dtype), dtype=data.dtype)
+        tmp.obs["fate probability"] = data
         tmp.obs[term_states] = (
-            pd.Series(
-                np.concatenate(
-                    [
-                        [f"{direction.lower()} {n}"] * adata.n_obs
-                        for n in adata.obsm[lineage_key].names
-                    ]
-                )
-            )
+            pd.Series(np.concatenate([[f"{direction.lower()} {n}"] * adata.n_obs for n in probs.names]))
             .astype("category")
             .values
         )
         tmp.obs[term_states] = tmp.obs[term_states].cat.reorder_categories(
-            [f"{direction.lower()} {n}" for n in adata.obsm[lineage_key].names]
+            [f"{direction.lower()} {n}" for n in probs.names]
         )
-        tmp.uns[f"{term_states}_colors"] = adata.obsm[lineage_key].colors
+        tmp.uns[f"{term_states}_colors"] = probs.colors
 
-        fig, ax = plt.subplots(
-            figsize=figsize if figsize is not None else (8, 6), dpi=dpi
-        )
+        fig, ax = plt.subplots(figsize=figsize if figsize is not None else (8, 6), dpi=dpi)
         ax.set_title(term_states.capitalize())
 
-        violin(tmp, keys=["absorption probability"], ax=ax, **kwargs)
+        violin(tmp, keys=["fate probability"], ax=ax, **kwargs)
 
         return fig
 
-    @plot.register(ClusterFatesMode.HEATMAP)
+    @plot.register(AggregationMode.HEATMAP)
     def _():
-        data = pd.DataFrame(
-            [mean for mean, _ in d.values()], columns=lin_names, index=clusters
-        ).T
+        data = pd.DataFrame([mean for mean, _ in d.values()], columns=probs.names, index=clusters).T
 
         title = kwargs.pop("title", "average fate per cluster")
         vmin, vmax = data.values.min(), data.values.max()
         cbar_kws = {
             "label": "probability",
             "ticks": np.linspace(vmin, vmax, 5),
             "format": "%.3f",
         }
         kwargs.setdefault("cmap", "viridis")
 
         if use_clustermap:
             kwargs["cbar_pos"] = (0, 0.9, 0.025, 0.15) if cbar else None
             max_size = float(max(data.shape))
 
-            g = clustermap(
+            g = sns.clustermap(
                 data=data,
                 annot=True,
                 vmin=vmin,
                 vmax=vmax,
                 fmt=fmt,
-                row_colors=adata.obsm[lineage_key][lin_names].colors,
+                row_colors=probs.colors,
                 dendrogram_ratio=(
                     0.15 * data.shape[0] / max_size,
                     0.15 * data.shape[1] / max_size,
                 ),
                 cbar_kws=cbar_kws,
                 figsize=figsize,
                 **kwargs,
@@ -396,15 +383,15 @@
             g.ax_heatmap.set_ylabel("lineage")
             g.ax_col_dendrogram.set_title(title)
 
             fig = g.fig
             g = g.ax_heatmap
         else:
             fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
-            g = heatmap(
+            g = sns.heatmap(
                 data=data,
                 vmin=vmin,
                 vmax=vmax,
                 annot=True,
                 fmt=fmt,
                 cbar=cbar,
                 cbar_kws=cbar_kws,
@@ -416,92 +403,72 @@
             ax.set_ylabel("lineage")
 
         g.set_xticklabels(g.get_xticklabels(), rotation=xrot)
         g.set_yticklabels(g.get_yticklabels(), rotation=0)
 
         return fig
 
-    mode = ClusterFatesMode(mode)
+    mode = AggregationMode(mode)
 
     if cluster_key is not None:
         if cluster_key not in adata.obs:
             raise KeyError(f"Key `{cluster_key!r}` not found in `adata.obs`.")
     elif mode not in (mode.BAR, mode.VIOLIN):
         raise ValueError(
             f"Not specifying cluster key is only available for modes "
-            f"`{ClusterFatesMode.BAR!r}` and `{ClusterFatesMode.VIOLIN!r}`, found `mode={mode!r}`."
+            f"`{AggregationMode.BAR!r}` and `{AggregationMode.VIOLIN!r}`, found `mode={mode!r}`."
         )
 
-    lineage_key = Key.obsm.abs_probs(backward)
     term_states = Key.obs.term_states(backward)
     direction = Key.where(backward)
-
     if cluster_key is not None:
         is_all = False
         if clusters is not None:
             if isinstance(clusters, str):
                 clusters = [clusters]
             clusters = _unique_order_preserving(clusters)
             if mode in (mode.PAGA, mode.PAGA_PIE):
-                logg.debug(
-                    f"Setting `clusters` to all available ones because of `mode={mode!r}`"
-                )
+                logg.debug(f"Setting `clusters` to all available ones because of `mode={mode!r}`")
                 clusters = list(adata.obs[cluster_key].cat.categories)
             else:
                 for cname in clusters:
                     if cname not in adata.obs[cluster_key].cat.categories:
-                        raise KeyError(
-                            f"Cluster `{cname!r}` not found in `adata.obs[{cluster_key!r}]`."
-                        )
+                        raise KeyError(f"Cluster `{cname!r}` not found in `adata.obs[{cluster_key!r}]`.")
         else:
             clusters = list(adata.obs[cluster_key].cat.categories)
     else:
         is_all = True
         clusters = [term_states]
 
-    if lineage_key not in adata.obsm:
-        raise KeyError(f"Lineage key `{lineage_key!r}` not found in `adata.obsm`.")
-
-    if lineages is not None:
-        if isinstance(lineages, str):
-            lineages = [lineages]
-        lin_names = _unique_order_preserving(lineages)
-    else:
+    probs = Lineage.from_adata(adata, backward=backward)
+    if lineages is None:
         # must be list for `sc.pl.violin`, else cats str
-        lin_names = list(adata.obsm[lineage_key].names)
-    _ = adata.obsm[lineage_key][lin_names]
+        lineages = list(probs.names)
+    elif isinstance(lineages, str):
+        lineages = [lineages]
+    lineages = _unique_order_preserving(lineages)
+    probs = probs[:, lineages]
 
     if mode == mode.VIOLIN and not is_all:
-        adata = adata[np.isin(adata.obs[cluster_key], clusters)].copy()
+        mask = np.isin(adata.obs[cluster_key], clusters)
+        adata = adata[mask].copy()
+        probs = probs[mask]
 
-    d = odict()
+    d = collections.OrderedDict()
     for name in clusters:
-        mask = (
-            np.ones((adata.n_obs,), dtype=bool)
-            if is_all
-            else (adata.obs[cluster_key] == name).values
-        )
-        mask = np.array(mask, dtype=bool)
-        data = adata.obsm[lineage_key][mask, lin_names].X
+        data = probs.X if is_all else probs.X[(adata.obs[cluster_key] == name).to_numpy()]
         mean = np.nanmean(data, axis=0)
         std = np.nanstd(data, axis=0) / np.sqrt(data.shape[0])
         d[name] = [mean, std]
 
     logg.debug(f"Plotting in mode `{mode!r}`")
     use_clustermap = False
     if mode == mode.CLUSTERMAP:
         use_clustermap = True
         mode = mode.HEATMAP
-    elif (
-        mode in (ClusterFatesMode.PAGA, ClusterFatesMode.PAGA_PIE)
-        and "paga" not in adata.uns
-    ):
-        raise KeyError("Compute PAGA first as `scvelo.tl.paga()`.")
-
-    fig = (
-        plot_violin_no_cluster_key()
-        if mode == ClusterFatesMode.VIOLIN and cluster_key is None
-        else plot(mode)
-    )
+    elif mode in (AggregationMode.PAGA, AggregationMode.PAGA_PIE) and "paga" not in adata.uns:
+        raise KeyError("Compute PAGA first as `scvelo.tl.paga()` or `scanpy.tl.paga()`.")
+
+    fig = plot_violin_no_cluster_key() if mode == AggregationMode.VIOLIN and cluster_key is None else plot(mode)
 
     if save is not None:
         save_fig(fig, save)
```

### Comparing `cellrank-1.5.1/cellrank/pl/_cluster_lineage.py` & `cellrank-2.0.0/src/cellrank/pl/_cluster_trends.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,143 +1,149 @@
-from typing import Any, Dict, Tuple, Union, Optional, Sequence
+import pathlib
+import types
+from typing import Any, Dict, Optional, Sequence, Tuple, Union
 
-from types import MappingProxyType
-from pathlib import Path
+import numpy as np
+from sklearn.preprocessing import StandardScaler
+
+import matplotlib.pyplot as plt
+from matplotlib.colors import ListedColormap, is_color_like
+from matplotlib.gridspec import GridSpec, GridSpecFromSubplotSpec
 
 import scanpy as sc
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import _DEFAULT_BACKEND, Backend_t
-from cellrank.ul._docs import d
+from cellrank._utils import Lineage
+from cellrank._utils._docs import d
+from cellrank._utils._enum import DEFAULT_BACKEND, Backend_t
+from cellrank._utils._parallelize import _get_n_cores
+from cellrank._utils._utils import (
+    _check_collection,
+    _genesymbols,
+    _unique_order_preserving,
+    save_fig,
+)
 from cellrank.pl._utils import (
-    _fit_bulk,
-    _get_backend,
     _callback_type,
-    _create_models,
-    _time_range_type,
     _create_callbacks,
-    _input_model_type,
+    _create_models,
+    _fit_bulk,
+    _get_backend,
     _get_sorted_colors,
+    _input_model_type,
     _return_model_type,
+    _time_range_type,
 )
-from cellrank.tl._utils import save_fig, _unique_order_preserving
-from cellrank.ul._utils import _genesymbols, _get_n_cores, _check_collection
 
-import numpy as np
-from sklearn.preprocessing import StandardScaler
-
-import matplotlib.pyplot as plt
-from matplotlib.colors import ListedColormap, is_color_like
-from matplotlib.gridspec import GridSpec, GridSpecFromSubplotSpec
+__all__ = ["cluster_trends"]
 
 
 @d.dedent
 @_genesymbols
-def cluster_lineage(
+def cluster_trends(
     adata: AnnData,
     model: _input_model_type,
     genes: Sequence[str],
     lineage: str,
+    time_key: str,
     backward: bool = False,
     time_range: _time_range_type = None,
     clusters: Optional[Sequence[str]] = None,
     n_points: int = 200,
-    time_key: str = "latent_time",
     covariate_key: Optional[Union[str, Sequence[str]]] = None,
     ratio: float = 0.05,
     cmap: Optional[str] = "viridis",
     norm: bool = True,
     recompute: bool = False,
     callback: _callback_type = None,
     ncols: int = 3,
     sharey: Union[str, bool] = False,
     key: Optional[str] = None,
     random_state: Optional[int] = None,
     show_progress_bar: bool = True,
     n_jobs: Optional[int] = 1,
-    backend: Backend_t = _DEFAULT_BACKEND,
+    backend: Backend_t = DEFAULT_BACKEND,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
-    pca_kwargs: Dict = MappingProxyType({"svd_solver": "arpack"}),
-    neighbors_kwargs: Dict = MappingProxyType({"use_rep": "X"}),
-    clustering_kwargs: Dict = MappingProxyType({}),
+    save: Optional[Union[str, pathlib.Path]] = None,
+    pca_kwargs: Dict = types.MappingProxyType({"svd_solver": "arpack"}),
+    neighbors_kwargs: Dict = types.MappingProxyType({"use_rep": "X"}),
+    clustering_kwargs: Dict = types.MappingProxyType({}),
     return_models: bool = False,
     **kwargs: Any,
 ) -> Optional[_return_model_type]:
-    """
-    Cluster gene expression trends within a lineage and plot the clusters.
+    """Cluster and plot gene expression trends within a lineage.
+
+    .. seealso::
+        - See :doc:`../../../notebooks/tutorials/estimators/800_gene_trends` on how to
+          visualize the gene trends.
 
-    This function is based on Palantir, see :cite:`setty:19`. It can be used to discover modules of genes that drive
+    This function is based on *Palantir* :cite:`setty:19`. It can be used to discover modules of genes that drive
     development along a given lineage. Consider running this function on a subset of genes which are potential
-    lineage drivers, identified e.g. by running :func:`cellrank.tl.lineage_drivers`.
+    lineage drivers.
 
     Parameters
     ----------
     %(adata)s
     %(model)s
     %(genes)s
     lineage
         Name of the lineage for which to cluster the genes.
+    time_key
+        Key in :attr:`~anndata.AnnData.obs` where the pseudotime is stored.
     %(backward)s
     %(time_range)s
     clusters
-        Cluster identifiers to plot. If `None`, all clusters will be considered. Useful when
+        Cluster identifiers to plot. If :obj:`None`, all clusters will be considered. Useful when
         plotting previously computed clusters.
     n_points
         Number of points used for prediction.
-    time_key
-        Key in :attr:`anndata.AnnData.obs` where the pseudotime is stored.
     covariate_key
-        Key(s) in :attr:`anndata.AnnData.obs` containing observations to be plotted at the bottom of each plot.
+        Keys in :attr:`~anndata.AnnData.obs` containing observations to be plotted at the bottom of each plot.
     %(gene_symbols)s
     ratio
         Height ratio of each covariate in ``covariate_key``.
     cmap
         Colormap to use for continuous covariates in ``covariate_key``.
     norm
         Whether to z-normalize each trend to have zero mean, unit variance.
     recompute
-        If `True`, recompute the clustering, otherwise try to find already existing one.
+        If :obj:`True`, recompute the clustering, otherwise try to find already existing one.
     %(model_callback)s
     ncols
         Number of columns for the plot.
     sharey
         Whether to share y-axis across multiple plots.
     key
-        Key in :attr:`anndata.AnnData.uns` where to save the results.
-        If `None`, it will be saved as ``'lineage_{lineage}_trend'`` .
+        Key in :attr:`~anndata.AnnData.uns` where to save the results.
+        If :obj:`None`, it will be saved as ``'lineage_{lineage}_trend'`` .
     random_state
         Random seed for reproducibility.
     %(parallel)s
     %(plotting)s
     pca_kwargs
-        Keyword arguments for :func:`scanpy.pp.pca`.
+        Keyword arguments for :func:`~scanpy.pp.pca`.
     neighbors_kwargs
-        Keyword arguments for :func:`scanpy.pp.neighbors`.
+        Keyword arguments for :func:`~scanpy.pp.neighbors`.
     clustering_kwargs
-        Keyword arguments for :func:`scanpy.tl.leiden`.
+        Keyword arguments for :func:`~scanpy.tl.leiden`.
     %(return_models)s
-    kwargs:
-        Keyword arguments for :meth:`cellrank.ul.models.BaseModel.prepare`.
+    kwargs
+        Keyword arguments for :meth:`~cellrank.models.BaseModel.prepare`.
 
     Returns
     -------
-    %(plots_or_returns_models)s
+    %(plots_or_returns_models)s Also updates :attr:`adata.uns <anndata.AnnData.uns>` with the following:
 
-        Also updates ``adata.uns`` with the following:
-
-            - ``key`` or ``lineage_{lineage}_trend`` - an :class:`anndata.AnnData` object of
-              shape `(n_genes, n_points)` containing the clustered genes.
+    - ``key`` or ``'lineage_{lineage}_trend'`` - :class:`~anndata.AnnData` object of
+      shape ``(n_genes, n_points)`` containing the clustered genes.
     """
 
-    def plot_cluster(
-        row: int, col: int, cluster: str, sharey_ax: Optional[str] = None
-    ) -> Optional[plt.Axes]:
+    def plot_cluster(row: int, col: int, cluster: str, sharey_ax: Optional[str] = None) -> Optional[plt.Axes]:
         gss = GridSpecFromSubplotSpec(
             row_delta,
             1,
             subplot_spec=gs[row : row + row_delta, col],
             hspace=0,
             height_ratios=[1.0] + [ratio] * (row_delta - 1),
         )
@@ -148,17 +154,15 @@
 
         for i in range(data.shape[0]):
             ax.plot(data[i], color="gray", lw=0.5)
 
         ax.plot(mean, lw=2, color="black")
         ax.plot(mean - sd, lw=1.5, color="black", linestyle="--")
         ax.plot(mean + sd, lw=1.5, color="black", linestyle="--")
-        ax.fill_between(
-            range(len(mean)), mean - sd, mean + sd, color="black", alpha=0.1
-        )
+        ax.fill_between(range(len(mean)), mean - sd, mean + sd, color="black", alpha=0.1)
 
         ax.set_title(f"cluster {cluster}")
         ax.set_xticks([])
         if sharey:
             ax.set_yticks([])
         ax.margins(0)
 
@@ -171,26 +175,20 @@
                 else:
                     cm = plt.get_cmap(cmap)
                     ax_clusters.imshow(colors[None, :], cmap=cm, aspect="auto")
                 ax_clusters.set_xticks([])
                 ax_clusters.set_yticks([])
 
             ax_clusters.set_xticks(np.linspace(0, len(colors), 5))
-            ax_clusters.set_xticklabels(
-                [f"{v:.3f}" for v in np.linspace(tmin, tmax, 5)]
-            )
+            ax_clusters.set_xticklabels([f"{v:.3f}" for v in np.linspace(tmin, tmax, 5)])
 
         return ax if sharey else None
 
     use_raw = kwargs.get("use_raw", False)
-    lineage_key = Key.obsm.abs_probs(backward)
-    if lineage_key not in adata.obsm:
-        raise KeyError(f"Lineages not found in `adata.obsm[{lineage_key!r}]`.")
-
-    _ = adata.obsm[lineage_key][lineage]
+    _ = Lineage.from_adata(adata, backward=backward)[lineage]  # sanity check
 
     genes = _unique_order_preserving(genes)
     _check_collection(adata, genes, "var_names", use_raw=use_raw)
 
     if key is None:
         key = f"lineage_{lineage}_trend"
 
@@ -225,23 +223,19 @@
         mod = next(mod for tmp in all_models.values() for mod in tmp.values())
         trends = AnnData(trends.T)
         trends.obs_names = genes
         trends.var["x_test"] = x_test = mod.x_test
 
         # sanity check
         if trends.n_obs != len(genes):
-            raise RuntimeError(
-                f"Expected to find `{len(genes)}` genes, found `{trends.n_obs}`."
-            )
+            raise RuntimeError(f"Expected to find `{len(genes)}` genes, found `{trends.n_obs}`.")
         if trends.n_vars != n_points:
-            raise RuntimeError(
-                f"Expected to find `{n_points}` points, found `{trends.n_vars}`."
-            )
+            raise RuntimeError(f"Expected to find `{n_points}` points, found `{trends.n_vars}`.")
 
-        random_state = np.random.mtrand.RandomState(random_state).randint(2 ** 16)
+        random_state = np.random.RandomState(random_state).randint(2**16)
 
         pca_kwargs = dict(pca_kwargs)
         pca_kwargs.setdefault("n_comps", min(50, n_points, len(genes)) - 1)
         pca_kwargs.setdefault("random_state", random_state)
         sc.pp.pca(trends, **pca_kwargs)
 
         neighbors_kwargs = dict(neighbors_kwargs)
@@ -265,16 +259,15 @@
         raise KeyError("Unable to find the clustering in `trends.obs['clusters']`.")
 
     if clusters is None:
         clusters = trends.obs["clusters"].cat.categories
     for c in clusters:
         if c not in trends.obs["clusters"].cat.categories:
             raise ValueError(
-                f"Invalid cluster name `{c!r}`. "
-                f"Valid options are `{list(trends.obs['clusters'].cat.categories)}`."
+                f"Invalid cluster name `{c!r}`. " f"Valid options are `{list(trends.obs['clusters'].cat.categories)}`."
             )
 
     nrows = int(np.ceil(len(clusters) / ncols))
     fig = plt.figure(
         dpi=dpi,
         figsize=(ncols * 10, nrows * 10) if figsize is None else figsize,
         tight_layout=True,
```

### Comparing `cellrank-1.5.1/cellrank/pl/_gene_trend.py` & `cellrank-2.0.0/src/cellrank/pl/_gene_trend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,65 @@
-from typing import Any, List, Tuple, Union, Mapping, Optional, Sequence
+import pathlib
+import types
+from typing import Any, List, Mapping, Optional, Sequence, Tuple, Union
 
-from types import MappingProxyType
-from pathlib import Path
+import numpy as np
+import pandas as pd
+
+import matplotlib
+import matplotlib.pyplot as plt
+from matplotlib import cm
 
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import _DEFAULT_BACKEND, Backend_t
-from cellrank.ul._docs import d
+from cellrank._utils import Lineage
+from cellrank._utils._docs import d
+from cellrank._utils._enum import DEFAULT_BACKEND, Backend_t
+from cellrank._utils._parallelize import _get_n_cores
+from cellrank._utils._utils import (
+    _check_collection,
+    _genesymbols,
+    _unique_order_preserving,
+    save_fig,
+)
 from cellrank.pl._utils import (
-    _fit_bulk,
-    _get_backend,
     _callback_type,
-    _create_models,
-    _trends_helper,
-    _time_range_type,
     _create_callbacks,
+    _create_models,
+    _fit_bulk,
+    _get_backend,
     _input_model_type,
     _return_model_type,
+    _time_range_type,
+    _trends_helper,
 )
-from cellrank.tl._utils import save_fig, _unique_order_preserving
-from cellrank.ul._utils import _genesymbols, _get_n_cores, _check_collection
-
-import numpy as np
-import pandas as pd
 
-import matplotlib
-import matplotlib.pyplot as plt
-from matplotlib import cm
+__all__ = ["gene_trends"]
 
 
 @d.dedent
 @_genesymbols
 def gene_trends(
     adata: AnnData,
     model: _input_model_type,
     genes: Union[str, Sequence[str]],
+    time_key: str,
     lineages: Optional[Union[str, Sequence[str]]] = None,
     backward: bool = False,
     data_key: str = "X",
-    time_key: str = "latent_time",
     time_range: Optional[Union[_time_range_type, List[_time_range_type]]] = None,
     transpose: bool = False,
     callback: _callback_type = None,
     conf_int: Union[bool, float] = True,
     same_plot: bool = False,
     hide_cells: bool = False,
     perc: Optional[Union[Tuple[float, float], Sequence[Tuple[float, float]]]] = None,
     lineage_cmap: Optional[matplotlib.colors.ListedColormap] = None,
-    abs_prob_cmap: matplotlib.colors.ListedColormap = cm.viridis,
+    fate_prob_cmap: matplotlib.colors.ListedColormap = cm.viridis,
     cell_color: Optional[str] = None,
     cell_alpha: float = 0.6,
     lineage_alpha: float = 0.2,
     size: float = 15,
     lw: float = 2,
     cbar: bool = True,
     margins: float = 0.015,
@@ -61,102 +68,107 @@
     gene_as_title: Optional[bool] = None,
     legend_loc: Optional[str] = "best",
     obs_legend_loc: Optional[str] = "best",
     ncols: int = 2,
     suptitle: Optional[str] = None,
     return_models: bool = False,
     n_jobs: Optional[int] = 1,
-    backend: Backend_t = _DEFAULT_BACKEND,
+    backend: Backend_t = DEFAULT_BACKEND,
     show_progress_bar: bool = True,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
-    plot_kwargs: Mapping[str, Any] = MappingProxyType({}),
+    save: Optional[Union[str, pathlib.Path]] = None,
+    return_figure: bool = False,
+    plot_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
     **kwargs: Any,
 ) -> Optional[_return_model_type]:
-    """
-    Plot gene expression trends along lineages.
+    """Plot gene expression trends along lineages.
 
-    Each lineage is defined via it's lineage weights which we compute using :func:`cellrank.tl.lineages`. This
-    function accepts any model based off :class:`cellrank.ul.models.BaseModel` to fit gene expression,
-    where we take the lineage weights into account in the loss function.
+    .. seealso::
+        - See :doc:`../../../notebooks/tutorials/estimators/800_gene_trends` on how to
+          visualize the gene trends.
+
+    Each lineage is defined via its lineage weights. This function accepts any model based off
+    :class:`~cellrank.models.BaseModel` to fit gene expression, where we take the lineage weights
+    into account in the loss function.
 
     Parameters
     ----------
     %(adata)s
     %(model)s
     %(genes)s
+    time_key
+        Key in :attr:`~anndata.AnnData.obs` where the pseudotime is stored.
     lineages
-        Names of the lineages to plot. If `None`, plot all lineages.
+        Names of the lineages to plot. If :obj:`None`, plot all lineages.
     %(backward)s
     data_key
-        Key in :attr:`anndata.AnnData.layers` or `'X'` for :attr:`anndata.AnnData.X` where the data is stored.
-    time_key
-        Key in :attr:`anndata.AnnData.obs` where the pseudotime is stored.
+        Key in :attr:`~anndata.AnnData.layers` or ``'X'`` for :attr:`~anndata.AnnData.X` where the data is stored.
     %(time_range)s
-
         This can also be specified on per-lineage basis.
     %(gene_symbols)s
     transpose
         If ``same_plot = True``, group the trends by ``lineages`` instead of ``genes``.
         This forces ``hide_cells = True``.
         If ``same_plot = False``, show ``lineages`` in rows and ``genes`` in columns.
     %(model_callback)s
     conf_int
-        Whether to compute and show confidence interval. If the ``model`` is :class:`cellrank.ul.models.GAMR`,
-        it can also specify the confidence level, the default is `0.95`.
+        Whether to compute and show confidence interval. If the ``model`` is :class:`~cellrank.models.GAMR`,
+        it can also specify the confidence level, the default is :math:`0.95`.
     same_plot
         Whether to plot all lineages for each gene in the same plot.
     hide_cells
-        If `True`, hide all cells.
+        If :obj:`True`, hide all cells.
     perc
-        Percentile for colors. Valid values are in interval `[0, 100]`.
+        Percentile for colors. Valid values are in :math:`[0, 100]`.
         This can improve visualization. Can be specified individually for each lineage.
     lineage_cmap
-        Categorical colormap to use when coloring in the lineages. If `None` and ``same_plot``,
-        use the corresponding colors in :attr:`anndata.AnnData.uns`, otherwise use `'black'`.
-    abs_prob_cmap
-        Continuous colormap to use when visualizing the absorption probabilities for each lineage.
+        Categorical colormap to use when coloring in the lineages. If :obj:`None` and ``same_plot = True``,
+        use the corresponding colors in :attr:`~anndata.AnnData.uns`, otherwise use ``'black'``.
+    fate_prob_cmap
+        Continuous colormap to use when visualizing the fate probabilities for each lineage.
         Only used when ``same_plot = False``.
     cell_color
-        Key in :attr:`anndata.AnnData.obs` or :attr:`anndata.AnnData.var_names` used for coloring the cells.
+        Key in :attr:`~anndata.AnnData.obs` or :attr:`~anndata.AnnData.var_names` used for coloring the cells.
     cell_alpha
         Alpha channel for cells.
     lineage_alpha
         Alpha channel for lineage confidence intervals.
     size
         Size of the points.
     lw
         Line width of the smoothed values.
     cbar
         Whether to show colorbar. Always shown when percentiles for lineages differ.
         Only used when ``same_plot = False``.
     margins
         Margins around the plot.
     sharex
-        Whether to share x-axis. Valid options are `'row'`, `'col'` or `'none'`.
+        Whether to share x-axis. Valid options are ``'row'``, ``'col'`` or ``'none'``.
     sharey
-        Whether to share y-axis. Valid options are `'row'`, `'col'` or `'none'`.
+        Whether to share y-axis. Valid options are ``'row'`, ``'col'`` or ``'none'``.
     gene_as_title
         Whether to show gene names as titles instead on y-axis.
     legend_loc
-        Location of the legend displaying lineages. Only used when `same_plot = True`.
+        Location of the legend displaying lineages. Only used when ``same_plot = True``.
     obs_legend_loc
         Location of the legend when ``cell_color`` corresponds to a categorical variable.
     ncols
         Number of columns of the plot when plotting multiple genes. Only used when ``same_plot = True``.
     suptitle
         Suptitle of the figure.
+    return_figure
+        Whether to return the figure object.
     %(return_models)s
     %(parallel)s
     %(plotting)s
     plot_kwargs
-        Keyword arguments for :meth:`cellrank.ul.models.BaseModel.plot`.
+        Keyword arguments for the :meth:`~cellrank.models.BaseModel.plot`.
     kwargs
-        Keyword arguments for :meth:`cellrank.ul.models.BaseModel.prepare`.
+        Keyword arguments for :meth:`~cellrank.models.BaseModel.prepare`.
 
     Returns
     -------
     %(plots_or_returns_models)s
     """
     if isinstance(genes, str):
         genes = [genes]
@@ -165,34 +177,29 @@
     _check_collection(
         adata,
         genes,
         "obs" if data_key == "obs" else "var_names",
         use_raw=kwargs.get("use_raw", False),
     )
 
-    lineage_key = Key.obsm.abs_probs(backward)
-    if lineage_key not in adata.obsm:
-        raise KeyError(f"Lineages key `{lineage_key!r}` not found in `adata.obsm`.")
-
+    probs = Lineage.from_adata(adata, backward=backward)
     if lineages is None:
-        lineages = adata.obsm[lineage_key].names
+        lineages = probs.names
     elif isinstance(lineages, str):
         lineages = [lineages]
     elif all(ln is None for ln in lineages):  # no lineage, all the weights are 1
         lineages = [None]
         cbar = False
         logg.debug("All lineages are `None`, setting the weights to `1`")
     lineages = _unique_order_preserving(lineages)
 
     if isinstance(time_range, (tuple, float, int, type(None))):
         time_range = [time_range] * len(lineages)
     elif len(time_range) != len(lineages):
-        raise ValueError(
-            f"Expected time ranges to be of length `{len(lineages)}`, found `{len(time_range)}`."
-        )
+        raise ValueError(f"Expected time ranges to be of length `{len(lineages)}`, found `{len(time_range)}`.")
 
     kwargs["time_key"] = time_key
     kwargs["data_key"] = data_key
     kwargs["backward"] = backward
     kwargs["conf_int"] = conf_int  # prepare doesnt take or need this
     models = _create_models(model, genes, lineages)
 
@@ -209,17 +216,17 @@
             "n_jobs": _get_n_cores(n_jobs, len(genes)),
             "backend": _get_backend(models, backend),
         },
         **kwargs,
     )
 
     lineages = sorted(lineages)
-    tmp = adata.obsm[lineage_key][lineages].colors
+    probs = probs[lineages]
     if lineage_cmap is None and not transpose:
-        lineage_cmap = tmp
+        lineage_cmap = probs.colors
 
     plot_kwargs = dict(plot_kwargs)
     plot_kwargs["obs_legend_loc"] = obs_legend_loc
     if transpose:
         all_models = pd.DataFrame(all_models).T.to_dict()
         models = pd.DataFrame(models).T.to_dict()
         genes, lineages = lineages, genes
@@ -240,19 +247,15 @@
             sharey = "row" if plot_kwargs.get("lineage_probability", False) else "none"
         ncols = len(genes) if ncols >= len(genes) else ncols
         nrows = int(np.ceil(len(genes) / ncols))
     else:
         gene_as_title = False if gene_as_title is None else gene_as_title
         sharex = "col" if sharex is None else sharex
         if sharey is None:
-            sharey = (
-                "row"
-                if not hide_cells or plot_kwargs.get("lineage_probability", False)
-                else "none"
-            )
+            sharey = "row" if not hide_cells or plot_kwargs.get("lineage_probability", False) else "none"
         nrows = len(genes)
         ncols = len(lineages)
 
     plot_kwargs = dict(plot_kwargs)
     if plot_kwargs.get("xlabel", None) is None:
         plot_kwargs["xlabel"] = time_key
 
@@ -272,38 +275,32 @@
 
     logg.info("Plotting trends")
     for row in range(len(axes)):
         for col in range(len(axes[row])):
             if cnt >= len(genes):
                 break
             gene = genes[cnt]
-            if (
-                same_plot
-                and plot_kwargs.get("lineage_probability", False)
-                and transpose
-            ):
-                lpc = adata.obsm[lineage_key][gene].colors[0]
+            if same_plot and plot_kwargs.get("lineage_probability", False) and transpose:
+                lpc = probs[gene].colors[0]
             else:
                 lpc = None
 
             if same_plot:
-                plot_kwargs["obs_legend_loc"] = (
-                    obs_legend_loc if row == 0 and col == len(axes[0]) - 1 else None
-                )
+                plot_kwargs["obs_legend_loc"] = obs_legend_loc if row == 0 and col == len(axes[0]) - 1 else None
 
             _trends_helper(
                 models,
                 gene=gene,
                 lineage_names=lineages,
                 transpose=transpose,
                 same_plot=same_plot,
                 hide_cells=hide_cells,
                 perc=perc,
                 lineage_cmap=lineage_cmap,
-                abs_prob_cmap=abs_prob_cmap,
+                fate_prob_cmap=fate_prob_cmap,
                 lineage_probability_color=lpc,
                 cell_color=cell_color,
                 alpha=cell_alpha,
                 lineage_alpha=lineage_alpha,
                 size=size,
                 lw=lw,
                 cbar=cbar,
@@ -312,29 +309,29 @@
                 gene_as_title=gene_as_title,
                 legend_loc=legend_loc,
                 figsize=figsize,
                 fig=fig,
                 axes=axes[row, col] if same_plot else axes[cnt],
                 show_ylabel=col == 0,
                 show_lineage=same_plot or (cnt == start_rows),
-                show_xticks_and_label=((row + 1) * ncols + col >= len(genes))
-                if same_plot
-                else (cnt == end_rows),
+                show_xticks_and_label=((row + 1) * ncols + col >= len(genes)) if same_plot else (cnt == end_rows),
                 **plot_kwargs,
             )
-            # plot legend on the 1st plot
-            cnt += 1
+            cnt += 1  # plot legend on the 1st plot
 
             if not same_plot:
                 plot_kwargs["obs_legend_loc"] = None
 
     if same_plot and (col != ncols):
         for ax in np.ravel(axes)[cnt:]:
             ax.remove()
 
     fig.suptitle(suptitle, y=1.05)
 
+    if return_figure:
+        return fig
+
     if save is not None:
         save_fig(fig, save)
 
     if return_models:
         return all_models
```

### Comparing `cellrank-1.5.1/cellrank/pl/_heatmap.py` & `cellrank-2.0.0/src/cellrank/pl/_heatmap.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,226 +1,225 @@
-from typing import Any, Dict, List, Tuple, Union, Optional, Sequence
-from typing_extensions import Literal
-
+import collections
+import enum
+import math
 import os
-from enum import auto
-from math import fabs
-from pathlib import Path
-from collections import Iterable, defaultdict
+import pathlib
+from typing import Any, Dict, List, Literal, Optional, Sequence, Tuple, Union
+
+import numpy as np
+import pandas as pd
+from scipy.ndimage.filters import convolve
+
+import matplotlib as mpl
+import matplotlib.pyplot as plt
+import seaborn as sns
+from matplotlib import cm, colors
+from matplotlib.ticker import FormatStrFormatter
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import _DEFAULT_BACKEND, ModeEnum, Backend_t
-from cellrank.ul._docs import d, inject_docs
+from cellrank._utils import Lineage
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import DEFAULT_BACKEND, Backend_t, ModeEnum
+from cellrank._utils._parallelize import _get_n_cores
+from cellrank._utils._utils import (
+    _check_collection,
+    _genesymbols,
+    _min_max_scale,
+    _unique_order_preserving,
+    save_fig,
+    valuedispatch,
+)
 from cellrank.pl._utils import (
-    _fit_bulk,
-    _get_backend,
     _callback_type,
-    _create_models,
-    _time_range_type,
     _create_callbacks,
+    _create_models,
+    _fit_bulk,
+    _get_backend,
+    _get_categorical_colors,
     _input_model_type,
     _return_model_type,
-    _get_categorical_colors,
-)
-from cellrank.tl._utils import save_fig, _min_max_scale, _unique_order_preserving
-from cellrank.ul._utils import (
-    _genesymbols,
-    _get_n_cores,
-    valuedispatch,
-    _check_collection,
+    _time_range_type,
 )
 
-import numpy as np
-import pandas as pd
-from scipy.ndimage.filters import convolve
-
-import matplotlib as mpl
-import matplotlib.colors as mcolors
-import matplotlib.pyplot as plt
-from seaborn import clustermap
-from matplotlib import cm
-from matplotlib.ticker import FormatStrFormatter
-from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+__all__ = ["heatmap"]
 
 _N_XTICKS = 10
 
 
-class HeatmapMode(ModeEnum):  # noqa: D101
-    GENES = auto()
-    LINEAGES = auto()
+class HeatmapMode(ModeEnum):
+    GENES = enum.auto()
+    LINEAGES = enum.auto()
 
 
 @d.dedent
 @inject_docs(m=HeatmapMode)
 @_genesymbols
 def heatmap(
     adata: AnnData,
     model: _input_model_type,
     genes: Sequence[str],
+    time_key: str,
     lineages: Optional[Union[str, Sequence[str]]] = None,
     backward: bool = False,
     mode: Literal["genes", "lineages"] = HeatmapMode.LINEAGES,
-    time_key: str = "latent_time",
     time_range: Optional[Union[_time_range_type, List[_time_range_type]]] = None,
     callback: _callback_type = None,
     cluster_key: Optional[Union[str, Sequence[str]]] = None,
-    show_absorption_probabilities: bool = False,
+    show_fate_probabilities: bool = False,
     cluster_genes: bool = False,
     keep_gene_order: bool = False,
     scale: bool = True,
     n_convolve: Optional[int] = 5,
     show_all_genes: bool = False,
     cbar: bool = True,
     lineage_height: float = 0.33,
     fontsize: Optional[float] = None,
     xlabel: Optional[str] = None,
-    cmap: mcolors.ListedColormap = cm.viridis,
+    cmap: colors.ListedColormap = cm.viridis,
     dendrogram: bool = True,
     return_genes: bool = False,
     return_models: bool = False,
+    return_figure: bool = False,
     n_jobs: Optional[int] = 1,
-    backend: Backend_t = _DEFAULT_BACKEND,
+    backend: Backend_t = DEFAULT_BACKEND,
     show_progress_bar: bool = True,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
+    save: Optional[Union[str, pathlib.Path]] = None,
     **kwargs: Any,
-) -> Optional[
-    Union[Dict[str, pd.DataFrame], Tuple[_return_model_type, Dict[str, pd.DataFrame]]]
-]:
-    """
-    Plot a heatmap of smoothed gene expression along specified lineages.
+) -> Optional[Union[Dict[str, pd.DataFrame], Tuple[_return_model_type, Dict[str, pd.DataFrame]]]]:
+    """Plot a heatmap of smoothed gene expression along specified lineages.
+
+    .. seealso::
+        - See :doc:`../../../notebooks/tutorials/estimators/800_gene_trends` on how to
+          visualize the gene trends.
+
+    This requires a pseudotemporal ordering of cellular dynamics, computed using a method like
+    DPT :cite:`haghverdi:16` or Palantir :cite:`setty:19`. The function combines the pseudotemporal
+    ordering with CellRank's fate probabilities to visualize each gene's expression along specific
+    trajectories. In the heatmap, genes are ordered according to their peak in pseudotime, which
+    emphasizes expression cascades of sequential activation.
 
     Parameters
     ----------
     %(adata)s
     %(model)s
     %(genes)s
+    time_key
+        Key in :attr:`~anndata.AnnData.obs` where the pseudotime is stored.
     lineages
-        Names of the lineages for which to plot. If `None`, plot all lineages.
+        Names of the lineages for which to plot. If :obj:`None`, plot all lineages.
     %(backward)s
     mode
         Valid options are:
 
-            - `{m.LINEAGES!r}` - group by ``genes`` for each lineage in ``lineages``.
-            - `{m.GENES!r}` - group by ``lineages`` for each gene in ``genes``.
-    time_key
-        Key in attr:`anndata.AnnData.obs` where the pseudotime is stored.
+        - ``{m.LINEAGES!r}`` - group by ``genes`` for each lineage in ``lineages``.
+        - ``{m.GENES!r}`` - group by ``lineages`` for each gene in ``genes``.
     %(time_range)s
-
         This can also be specified on per-lineage basis.
     %(gene_symbols)s
     %(model_callback)s
     cluster_key
-        Key(s) in :attr:`anndata.AnnData.obs` containing categorical observations to be plotted on the top of heatmap.
+        Key in :attr:`~anndata.AnnData.obs` containing categorical observations to be plotted on the top of heatmap.
         Only available when ``mode = {m.LINEAGES!r}``.
-    show_absorption_probabilities
-        Whether to also plot absorption probabilities alongside the smoothed expression.
+    show_fate_probabilities
+        Whether to also plot fate probabilities alongside the smoothed expression.
         Only available when ``mode = {m.LINEAGES!r}``.
     cluster_genes
-        Whether to cluster genes using :func:`seaborn.clustermap` when ``mode = 'lineages'``.
+        Whether to cluster genes using :func:`~seaborn.clustermap` when ``mode = 'lineages'``.
     keep_gene_order
         Whether to keep the gene order for later lineages after the first was sorted.
         Only available when ``cluster_genes = False`` and ``mode = {m.LINEAGES!r}``.
     scale
-        Whether to normalize the gene expression `[0, 1]` range.
+        Whether to normalize the gene expression to :math:`[0, 1]`.
     n_convolve
-        Size of the convolution window when smoothing absorption probabilities.
+        Size of the convolution window when smoothing fate probabilities.
     show_all_genes
         Whether to show all genes on y-axis.
     cbar
         Whether to show the colorbar.
     lineage_height
         Height of a bar when ``mode = {m.GENES!r}``.
     fontsize
         Size of the title's font.
     xlabel
-        Label on the x-axis. If `None`, it is determined based on ``time_key``.
+        Label on the x-axis. If :obj:`None`, it is determined based on ``time_key``.
     cmap
         Colormap to use when visualizing the smoothed expression.
     dendrogram
         Whether to show dendrogram when ``cluster_genes = True``.
     return_genes
         Whether to return the sorted or clustered genes. Only available when ``mode = {m.LINEAGES!r}``.
     %(return_models)s
+    return_figure
+        Whether to return the figure object. Sets ``return_genes = True``
     %(parallel)s
     %(plotting)s
     kwargs
-        Keyword arguments for :meth:`cellrank.ul.models.BaseModel.prepare`.
+        Keyword arguments for :meth:`~cellrank.models.BaseModel.prepare`.
 
     Returns
     -------
     %(plots_or_returns_models)s
 
-    If ``return_genes = True`` and ``mode = {m.LINEAGES!r}``, returns :class:`pandas.DataFrame`
+    - If ``return_genes = True`` and ``mode = {m.LINEAGES!r}``, returns a :class:`~pandas.DataFrame`
     containing the clustered or sorted genes.
+    - If ``return_figure = True``, returns a tuple containing the figure and genes.
     """
 
-    def find_indices(series: pd.Series, values) -> Tuple[Any]:
+    def find_indices(series: pd.Series, values) -> List[int]:
         def find_nearest(array: np.ndarray, value: float) -> int:
             ix = np.searchsorted(array, value, side="left")
-            if ix > 0 and (
-                ix == len(array)
-                or fabs(value - array[ix - 1]) < fabs(value - array[ix])
-            ):
+            if ix > 0 and (ix == len(array) or math.fabs(value - array[ix - 1]) < math.fabs(value - array[ix])):
                 return int(ix - 1)
             return int(ix)
 
-        series = series[np.argsort(series.values)]
-
-        return tuple(series[[find_nearest(series.values, v) for v in values]].index)
+        series = series.sort_values(ascending=True)
+        return list(series[[find_nearest(series.values, v) for v in values]].index)
 
     def subset_lineage(lname: str, rng: np.ndarray) -> np.ndarray:
         time_series = adata.obs[time_key]
         ixs = find_indices(time_series, rng)
+        lin = Lineage.from_adata(adata[ixs], backward=backward)
+        lin = lin[lname].X.squeeze(1).copy()
+        if n_convolve is None:
+            return lin.copy()
+        return convolve(lin, np.ones(n_convolve) / n_convolve, mode="nearest")
 
-        lin = adata[ixs, :].obsm[lineage_key][lname]
-
-        lin = lin.X.copy().squeeze()
-        if n_convolve is not None:
-            lin = convolve(lin, np.ones(n_convolve) / n_convolve, mode="nearest")
-
-        return lin
-
-    def create_col_colors(
-        lname: str, rng: np.ndarray
-    ) -> Tuple[np.ndarray, mcolors.Colormap, mcolors.Normalize]:
-        color = adata.obsm[lineage_key][lname].colors[0]
+    def create_col_colors(lname: str, rng: np.ndarray) -> Tuple[np.ndarray, colors.Colormap, colors.Normalize]:
+        color = probs[lname].colors[0]
         lin = subset_lineage(lname, rng)
 
-        h, _, v = mcolors.rgb_to_hsv(mcolors.to_rgb(color))
-        end_color = mcolors.hsv_to_rgb([h, 1, v])
+        h, _, v = colors.rgb_to_hsv(colors.to_rgb(color))
+        end_color = colors.hsv_to_rgb([h, 1, v])
 
-        lineage_cmap = mcolors.LinearSegmentedColormap.from_list(
-            "lineage_cmap", ["#ffffff", end_color], N=len(rng)
-        )
-        norm = mcolors.Normalize(vmin=np.min(lin), vmax=np.max(lin))
+        lineage_cmap = colors.LinearSegmentedColormap.from_list("lineage_cmap", ["#ffffff", end_color], N=len(rng))
+        norm = colors.Normalize(vmin=np.min(lin), vmax=np.max(lin))
         scalar_map = cm.ScalarMappable(cmap=lineage_cmap, norm=norm)
 
         return (
-            np.array([mcolors.to_hex(c) for c in scalar_map.to_rgba(lin)]),
+            np.array([colors.to_hex(c) for c in scalar_map.to_rgba(lin)]),
             lineage_cmap,
             norm,
         )
 
     def create_col_categorical_color(cluster_key: str, rng: np.ndarray) -> np.ndarray:
-        colors, mapper = _get_categorical_colors(adata, cluster_key)
+        cols, mapper = _get_categorical_colors(adata, cluster_key)
         ixs = find_indices(adata.obs[time_key], rng)
 
-        return np.array(
-            [mcolors.to_hex(mapper[v]) for v in adata[ixs, :].obs[cluster_key].values]
-        )
+        return np.array([colors.to_hex(mapper[v]) for v in adata[ixs, :].obs[cluster_key].values])
 
     def create_cbar(
         ax,
         x_delta: float,
-        cmap: mcolors.Colormap,
-        norm: mcolors.Normalize,
+        cmap: colors.Colormap,
+        norm: colors.Normalize,
         label: Optional[str] = None,
     ) -> plt.Axes:
         cax = inset_axes(
             ax,
             width="1%",
             height="100%",
             loc="lower right",
@@ -244,82 +243,69 @@
 
     @_plot_heatmap.register(HeatmapMode.GENES)
     def _() -> Tuple[plt.Figure, None]:
         def color_fill_rec(ax, xs, y1, y2, colors=None, cmap=cmap, **kwargs) -> None:
             colors = colors if cmap is None else cmap(colors)
 
             x = 0
-            for i, (color, x, y1, y2) in enumerate(zip(colors, xs, y1, y2)):
+            for i, (color, x, y1, y2) in enumerate(zip(colors, xs, y1, y2)):  # noqa: B020
                 dx = (xs[i + 1] - xs[i]) if i < len(x) else (xs[-1] - xs[-2])
-                ax.add_patch(
-                    plt.Rectangle((x, y1), dx, y2 - y1, color=color, ec=color, **kwargs)
-                )
+                ax.add_patch(plt.Rectangle((x, y1), dx, y2 - y1, color=color, ec=color, **kwargs))
 
             ax.plot(x, y2, lw=0)
 
         fig, axes = plt.subplots(
-            nrows=len(genes) + show_absorption_probabilities,
-            figsize=(12, len(genes) + len(lineages) * lineage_height)
-            if figsize is None
-            else figsize,
+            nrows=len(genes) + show_fate_probabilities,
+            figsize=(12, len(genes) + len(lineages) * lineage_height) if figsize is None else figsize,
             dpi=dpi,
             constrained_layout=True,
         )
+        axes = np.ravel([axes])
 
-        if not isinstance(axes, Iterable):
-            axes = [axes]
-        axes = np.ravel(axes)
-
-        if show_absorption_probabilities:
-            data["absorption probability"] = data[next(iter(data.keys()))]
+        if show_fate_probabilities:
+            data["fate probability"] = data[next(iter(data.keys()))]
 
         for ax, (gene, models) in zip(axes, data.items()):
             if scale:
                 vmin, vmax = 0, 1
             else:
                 c = np.array([m.y_test for m in models.values()])
                 vmin, vmax = np.nanmin(c), np.nanmax(c)
 
-            norm = mcolors.Normalize(vmin=vmin, vmax=vmax)
+            norm = colors.Normalize(vmin=vmin, vmax=vmax)
 
             ix = 0
             ys = [ix]
 
-            if gene == "absorption probability":
-                norm = mcolors.Normalize(vmin=0, vmax=1)
+            if gene == "fate probability":
+                norm = colors.Normalize(vmin=0, vmax=1)
                 for ln, x in ((ln, m.x_test) for ln, m in models.items()):
                     y = np.ones_like(x)
                     c = subset_lineage(ln, x.squeeze())
 
-                    color_fill_rec(
-                        ax, x, y * ix, y * (ix + lineage_height), colors=norm(c)
-                    )
+                    color_fill_rec(ax, x, y * ix, y * (ix + lineage_height), colors=norm(c))
 
                     ix += lineage_height
                     ys.append(ix)
             else:
                 for x, c in ((m.x_test, m.y_test) for m in models.values()):
                     y = np.ones_like(x)
                     c = _min_max_scale(c) if scale else c
 
-                    color_fill_rec(
-                        ax, x, y * ix, y * (ix + lineage_height), colors=norm(c)
-                    )
+                    color_fill_rec(ax, x, y * ix, y * (ix + lineage_height), colors=norm(c))
 
                     ix += lineage_height
                     ys.append(ix)
 
             xs = np.array([m.x_test for m in models.values()])
             x_min, x_max = np.min(xs), np.max(xs)
             ax.set_xticks(np.linspace(x_min, x_max, _N_XTICKS))
 
             ax.set_yticks(np.array(ys[:-1]) + lineage_height / 2)
-            ax.spines["left"].set_position(
-                ("data", 0)
-            )  # move the left spine to the rectangles to get nicer yticks
+            ax.spines["left"].set_position(("data", 0))  # move the left spine to the rectangles to get nicer yticks
             ax.set_yticklabels(models.keys(), ha="right")
 
             ax.set_title(gene, fontdict={"fontsize": fontsize})
             ax.set_ylabel("lineage")
 
             for pos in ["top", "bottom", "left", "right"]:
                 ax.spines[pos].set_visible(False)
@@ -327,19 +313,15 @@
             if cbar:
                 cax, _ = mpl.colorbar.make_axes(ax)
                 _ = mpl.colorbar.ColorbarBase(
                     cax,
                     ticks=np.linspace(vmin, vmax, 5),
                     norm=norm,
                     cmap=cmap,
-                    label="value"
-                    if gene == "absorption probability"
-                    else "scaled expression"
-                    if scale
-                    else "expression",
+                    label="value" if gene == "fate probability" else "scaled expression" if scale else "expression",
                 )
 
             ax.tick_params(
                 top=False,
                 bottom=False,
                 left=True,
                 right=False,
@@ -358,15 +340,15 @@
         )
         ax.set_xlabel(xlabel)
 
         return fig, None
 
     @_plot_heatmap.register(HeatmapMode.LINEAGES)
     def _() -> Tuple[List[plt.Figure], pd.DataFrame]:
-        data_t = defaultdict(dict)  # transpose
+        data_t = collections.defaultdict(dict)  # transpose
         for gene, lns in data.items():
             for ln, y in lns.items():
                 data_t[ln][gene] = y
 
         figs = []
         gene_order = None
         sorted_genes = pd.DataFrame() if return_genes else None
@@ -378,51 +360,40 @@
             df = pd.DataFrame([m.y_test for m in models.values()], index=models.keys())
             df.index.name = "genes"
 
             if not cluster_genes:
                 if gene_order is not None:
                     df = df.loc[gene_order]
                 else:
-                    max_sort = np.argsort(
-                        np.argmax(df.apply(_min_max_scale, axis=1).values, axis=1)
-                    )
+                    max_sort = np.argsort(np.argmax(df.apply(_min_max_scale, axis=1).values, axis=1))
                     df = df.iloc[max_sort, :]
                     if keep_gene_order:
                         gene_order = df.index
 
             cat_colors = None
             if cluster_key is not None:
                 cat_colors = np.stack(
-                    [
-                        create_col_categorical_color(
-                            c, np.linspace(x_min, x_max, df.shape[1])
-                        )
-                        for c in cluster_key
-                    ],
+                    [create_col_categorical_color(c, np.linspace(x_min, x_max, df.shape[1])) for c in cluster_key],
                     axis=0,
                 )
 
-            if show_absorption_probabilities:
-                col_colors, col_cmap, col_norm = create_col_colors(
-                    lname, np.linspace(x_min, x_max, df.shape[1])
-                )
+            if show_fate_probabilities:
+                col_colors, col_cmap, col_norm = create_col_colors(lname, np.linspace(x_min, x_max, df.shape[1]))
                 if cat_colors is not None:
                     col_colors = np.vstack([cat_colors, col_colors[None, :]])
             else:
                 col_colors, col_cmap, col_norm = cat_colors, None, None
 
             row_cluster = cluster_genes and df.shape[0] > 1
             show_clust = row_cluster and dendrogram
 
-            g = clustermap(
+            g = sns.clustermap(
                 data=df,
                 cmap=cmap,
-                figsize=(10, min(len(genes) / 8 + 1, 10))
-                if figsize is None
-                else figsize,
+                figsize=(10, min(len(genes) / 8 + 1, 10)) if figsize is None else figsize,
                 xticklabels=False,
                 row_cluster=row_cluster,
                 col_colors=col_colors,
                 colors_ratio=0,
                 col_cluster=False,
                 cbar_pos=None,
                 yticklabels=show_all_genes or "auto",
@@ -430,72 +401,62 @@
             )
 
             if cbar:
                 cax = create_cbar(
                     g.ax_heatmap,
                     0.1,
                     cmap=cmap,
-                    norm=mcolors.Normalize(
+                    norm=colors.Normalize(
                         vmin=0 if scale else np.min(df.values),
                         vmax=1 if scale else np.max(df.values),
                     ),
                     label="scaled expression" if scale else "expression",
                 )
                 g.fig.add_axes(cax)
 
                 if col_cmap is not None and col_norm is not None:
                     cax = create_cbar(
                         g.ax_heatmap,
                         0.25,
                         cmap=col_cmap,
                         norm=col_norm,
-                        label="absorption probability",
+                        label="fate probability",
                     )
                     g.fig.add_axes(cax)
 
             if g.ax_col_colors:
                 main_bbox = _get_ax_bbox(g.fig, g.ax_heatmap)
-                n_bars = show_absorption_probabilities + (
-                    len(cluster_key) if cluster_key is not None else 0
-                )
+                n_bars = show_fate_probabilities + (len(cluster_key) if cluster_key is not None else 0)
                 _set_ax_height_to_cm(
                     g.fig,
                     g.ax_col_colors,
-                    height=min(
-                        5, max(n_bars * main_bbox.height / len(df), 0.25 * n_bars)
-                    ),
+                    height=min(5, max(n_bars * main_bbox.height / len(df), 0.25 * n_bars)),
                 )
                 g.ax_col_colors.set_title(lname, fontdict={"fontsize": fontsize})
             else:
                 g.ax_heatmap.set_title(lname, fontdict={"fontsize": fontsize})
 
             g.ax_col_dendrogram.set_visible(False)  # gets rid of top free space
-
             g.ax_heatmap.yaxis.tick_left()
             g.ax_heatmap.yaxis.set_label_position("right")
-
+            # fmt: off
             g.ax_heatmap.set_xlabel(xlabel)
             g.ax_heatmap.set_xticks(np.linspace(0, len(df.columns), _N_XTICKS))
-            g.ax_heatmap.set_xticklabels(
-                list(map(lambda n: round(n, 3), np.linspace(x_min, x_max, _N_XTICKS)))
-            )
-
+            g.ax_heatmap.set_xticklabels([round(n, 3) for n in np.linspace(x_min, x_max, _N_XTICKS)])
+            # fmt: on
             if show_clust:
                 # robustly show dendrogram, because gene names can be long
                 g.ax_row_dendrogram.set_visible(True)
                 dendro_box = g.ax_row_dendrogram.get_position()
-
                 pad = 0.005
-                bb = g.ax_heatmap.yaxis.get_tightbbox(
-                    g.fig.canvas.get_renderer()
-                ).transformed(g.fig.transFigure.inverted())
-
+                bb = g.ax_heatmap.yaxis.get_tightbbox(g.fig.canvas.get_renderer()).transformed(
+                    g.fig.transFigure.inverted()
+                )
                 dendro_box.x0 = bb.x0 - dendro_box.width - pad
                 dendro_box.x1 = bb.x0 - pad
-
                 g.ax_row_dendrogram.set_position(dendro_box)
             else:
                 g.ax_row_dendrogram.set_visible(False)
 
             if return_genes:
                 sorted_genes[lname] = (
                     df.index[g.dendrogram_row.reordered_ind]
@@ -505,25 +466,21 @@
 
             figs.append(g)
 
         return figs, sorted_genes
 
     mode = HeatmapMode(mode)
 
-    lineage_key = Key.obsm.abs_probs(backward)
-    if lineage_key not in adata.obsm:
-        raise KeyError(f"Lineages key `{lineage_key!r}` not found in `adata.obsm`.")
-
+    probs = Lineage.from_adata(adata, backward=backward)
     if lineages is None:
-        lineages = adata.obsm[lineage_key].names
+        lineages = probs.names
     elif isinstance(lineages, str):
         lineages = [lineages]
     lineages = _unique_order_preserving(lineages)
-
-    _ = adata.obsm[lineage_key][lineages]
+    probs = probs[lineages]
 
     if cluster_key is not None:
         if isinstance(cluster_key, str):
             cluster_key = [cluster_key]
         cluster_key = _unique_order_preserving(cluster_key)
 
     if isinstance(genes, str):
@@ -551,35 +508,38 @@
     )
 
     xlabel = time_key if xlabel is None else xlabel
 
     logg.debug(f"Plotting `{mode!r}` heatmap")
     fig, genes = _plot_heatmap(mode)
 
+    if return_figure:
+        return fig, genes
+
     if save is not None and fig is not None:
-        if not isinstance(fig, Iterable):
+        if isinstance(fig, plt.Figure):
             save_fig(fig, save)
         elif len(fig) == 1:
             save_fig(fig[0], save)
         else:
             for ln, f in zip(lineages, fig):
                 save_fig(f, os.path.join(save, f"lineage_{ln}"))
 
     if return_genes and mode == HeatmapMode.LINEAGES:
         return (all_models, genes) if return_models else genes
-    elif return_models:
+    if return_models:
         return all_models
 
 
 def _get_ax_bbox(fig: plt.Figure, ax: plt.Axes):
     return ax.get_window_extent().transformed(fig.dpi_scale_trans.inverted())
 
 
 def _set_ax_height_to_cm(fig: plt.Figure, ax: plt.Axes, height: float) -> None:
-    from mpl_toolkits.axes_grid1 import Size, Divider
+    from mpl_toolkits.axes_grid1 import Divider, Size
 
     height /= 2.54  # cm to inches
 
     bbox = _get_ax_bbox(fig, ax)
 
     hori = [Size.Fixed(bbox.x0), Size.Fixed(bbox.width), Size.Fixed(bbox.x1)]
     vert = [Size.Fixed(bbox.y0), Size.Fixed(height), Size.Fixed(bbox.y1)]
```

### Comparing `cellrank-1.5.1/cellrank/pl/_log_odds.py` & `cellrank-2.0.0/src/cellrank/pl/_log_odds.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from typing import Any, Tuple, Union, Iterable, Optional, Sequence
-
-from copy import copy
-from pathlib import Path
-
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.ul._docs import d
-from cellrank.pl._utils import _position_legend, _get_categorical_colors
-from cellrank.tl._utils import save_fig, _unique_order_preserving
+import copy
+import pathlib
+from typing import Any, Iterable, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 import matplotlib.pyplot as plt
-from seaborn import stripplot
-from matplotlib.cm import ScalarMappable
+import seaborn as sns
 from matplotlib.axes import Axes
+from matplotlib.cm import ScalarMappable
 from matplotlib.colors import Normalize, to_hex
 
+from anndata import AnnData
+
+from cellrank import logging as logg
+from cellrank._utils import Lineage
+from cellrank._utils._docs import d
+from cellrank._utils._utils import _unique_order_preserving, save_fig
+from cellrank.pl._utils import _get_categorical_colors, _position_legend
+
+__all__ = ["log_odds"]
+
 
 @d.dedent
 def log_odds(
     adata: AnnData,
     lineage_1: str,
     lineage_2: Optional[str] = None,
     time_key: str = "exp_time",
@@ -39,124 +41,122 @@
     fontsize: Optional[Union[float, str]] = None,
     xticks_step_size: Optional[int] = 1,
     legend_loc: Optional[str] = "best",
     jitter: Union[bool, float] = True,
     seed: Optional[int] = None,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[int] = None,
-    save: Optional[Union[str, Path]] = None,
+    save: Optional[Union[str, pathlib.Path]] = None,
     show: bool = True,
     **kwargs: Any,
 ) -> Optional[Union[Axes, Sequence[Axes]]]:
-    """
-    Plot log-odds ratio between lineages.
+    """Plot log-odds ratio between trajectories.
 
-    Log-odds are plotted as a function of the experimental time.
+    This plotting function is geared towards time-series datasets that have been analyzed
+    using the :class:`~cellrank.kernels.RealTimeKernel`. It visualizes log-odd ratios
+    between different trajectories per cell, with the option to color in certain
+    molecular features, like genes. This can be useful to detect and visualize fate-decisive genes.
 
     Parameters
     ----------
     %(adata)s
     lineage_1
         The first lineage for which to compute the log-odds.
     lineage_2
-        The second lineage for which to compute the log-odds. If `None`, use the rest of the lineages.
+        The second lineage for which to compute the log-odds. If :obj:`None`, use the rest of the lineages.
     time_key
-        Key in :attr:`anndata.AnnData.obs` containing the experimental time.
+        Key in :attr:`~anndata.AnnData.obs` containing the experimental time.
     %(backward)s
     keys
-        Key in :attr:`anndata.AnnData.obs` or :attr:`anndata.AnnData.var_names`.
+        Key in :attr:`~anndata.AnnData.obs` or :attr:`~anndata.AnnData.var_names`.
     threshold
         Visualize whether total expression per cell is greater than ``threshold``.
-        If a :class:`typing.Sequence`, it should be the same length as ``keys``.
+        If a :class:`~typing.Sequence`, it should be the same length as ``keys``.
     threshold_color
         Color to use when plotting thresholded expression values.
     layer
-        Which layer to use to get expression values. If `None` or `'X'`, use :attr:`anndata.AnnData.X`.
+        Which layer to use to get expression values. If :obj:`None` or ``'X'``, use :attr:`~anndata.AnnData.X`.
     use_raw
-        Whether to access :attr:`anndata.AnnData.raw`. If `True`, ``layer`` is ignored.
+        Whether to access :attr:`~anndata.AnnData.raw`. If :obj:`True`, ``layer`` is ignored.
     size
         Size of the dots.
     cmap
         Colormap to use for continuous variables in ``keys``.
     alpha
         Alpha values for the dots.
     ncols
         Number of columns.
     fontsize
         Size of the font for the title, x- and y-label.
     xticks_step_size
-        Show only every n-th ticks on x-axis. If `None`, don't show any ticks.
+        Show only every other *n-th* tick on the x-axis. If :obj:`None`, don't show any ticks.
     legend_loc
-        Position of the legend. If `None`, do not show the legend.
+        Position of the legend. If :obj:`None`, do not show the legend.
     jitter
         Amount of jitter to apply along x-axis.
     seed
         Seed for ``jitter`` to ensure reproducibility.
     %(plotting)s
     show
-        If `False`, return :class:`matplotlib.pyplot.Axes` or a sequence of them.
+        If `False`, return :class:`~matplotlib.axes.Axes` or a sequence of them.
     kwargs
-        Keyword arguments for :func:`seaborn.stripplot`.
+        Keyword arguments for :func:`~seaborn.stripplot`.
 
     Returns
     -------
-    The axes object(s), if ``show = False``.
     %(just_plots)s
+    If ``show = False``, returns the axes object.
     """
-    from cellrank.tl.kernels._utils import _ensure_numeric_ordered
+    from cellrank.kernels._utils import _ensure_numeric_ordered
 
-    def decorate(
-        ax: Axes, *, title: Optional[str] = None, show_ylabel: bool = True
-    ) -> None:
+    def decorate(ax: Axes, *, title: Optional[str] = None, show_ylabel: bool = True) -> None:
         ax.set_xlabel(time_key, fontsize=fontsize)
         ax.set_title(title, fontdict={"fontsize": fontsize})
         ax.set_ylabel(ylabel if show_ylabel else "", fontsize=fontsize)
 
         if xticks_step_size is None:
             ax.set_xticks([])
         else:
             step = max(1, xticks_step_size)
             ax.set_xticks(np.arange(0, n_cats, step))
             ax.set_xticklabels(df[time_key].cat.categories[::step])
 
-    def cont_palette(values: np.ndarray) -> Tuple[np.ndarray, ScalarMappable]:
-        cm = copy(plt.get_cmap(cmap))
+    def cont_palette(values: np.ndarray) -> Tuple[List[str], ScalarMappable]:
+        cm = copy.copy(plt.get_cmap(cmap))
         cm.set_bad("grey")
-        sm = ScalarMappable(
-            cmap=cm, norm=Normalize(vmin=np.nanmin(values), vmax=np.nanmax(values))
-        )
-        return np.array([to_hex(v) for v in (sm.to_rgba(values))]), sm
+        sm = ScalarMappable(cmap=cm, norm=Normalize(vmin=np.nanmin(values), vmax=np.nanmax(values)))
+        return [to_hex(v) for v in (sm.to_rgba(values))], sm
 
     def get_data(
         key: str,
         thresh: Optional[float] = None,
-    ) -> Tuple[
-        Optional[str], Optional[np.ndarray], Optional[np.ndarray], ScalarMappable
-    ]:
+    ) -> Tuple[Optional[str], Optional[np.ndarray], Optional[np.ndarray], ScalarMappable]:
         try:
             _, palette = _get_categorical_colors(adata, key)
             df[key] = adata.obs[key].values[mask]
             df[key] = df[key].cat.remove_unused_categories()
             try:
                 # seaborn doesn't like numeric categories
                 df[key] = df[key].astype(float)
                 palette = {float(k): v for k, v in palette.items()}
             except ValueError:
                 pass
             # otherwise seaborn plots all
             palette = {k: palette[k] for k in df[key].unique()}
             hue, thresh_mask, sm = key, None, None
         except TypeError:
+            # not a categorical
             palette, hue, thresh_mask, sm = (
                 cont_palette(adata.obs[key].values[mask])[0],
                 None,
                 None,
                 None,
             )
         except KeyError:
+            # unable to find data in `adata.obs`, try res
             try:
                 # fmt: off
                 if thresh is None:
                     values = adata.raw.obs_vector(key) if use_raw else adata.obs_vector(key, layer=layer)
                     palette, sm = cont_palette(values)
                     hue, thresh_mask = None, None
                 else:
@@ -170,33 +170,30 @@
                     hue, palette, sm = None, None, None
                 # fmt: on
             except KeyError as e:
                 raise e from None
 
         return hue, palette, thresh_mask, sm
 
-    np.random.seed(seed)
+    np.random.seed(seed)  # noqa: NPY002
     _ = kwargs.pop("orient", None)
     if use_raw and adata.raw is None:
         logg.warning("No raw attribute set. Setting `use_raw=False`")
         use_raw = False
 
-    # define log-odds
-    lineage_key = Key.obsm.abs_probs(backward)
-    if lineage_key not in adata.obsm:
-        raise KeyError(f"Lineages key `{lineage_key!r}` not found in `adata.obsm`.")
+    probs = Lineage.from_adata(adata, backward=backward)
     time = _ensure_numeric_ordered(adata, time_key)
     order = time.cat.categories[:: -1 if backward else 1]
 
-    fate1 = adata.obsm[lineage_key][lineage_1].X.squeeze(-1)
+    fate1 = probs[lineage_1].X.squeeze(-1)
     if lineage_2 is None:
         fate2 = 1 - fate1
         ylabel = rf"$\log{{\frac{{{lineage_1}}}{{rest}}}}$"
     else:
-        fate2 = adata.obsm[lineage_key][lineage_2].X.squeeze(-1)
+        fate2 = probs[lineage_2].X.squeeze(-1)
         ylabel = rf"$\log{{\frac{{{lineage_1}}}{{{lineage_2}}}}}$"
 
     # fmt: off
     df = pd.DataFrame(
         {
             "log_odds": np.log(np.divide(fate1, fate2, where=fate2 != 0, out=np.zeros_like(fate1)) + 1e-12),
             time_key: time,
@@ -208,15 +205,15 @@
     # fmt: on
 
     if keys is None:
         if figsize is None:
             figsize = np.array([n_cats, n_cats * 4 / 6]) / 2
 
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi, tight_layout=True)
-        ax = stripplot(
+        ax = sns.stripplot(
             x=time_key,
             y="log_odds",
             data=df,
             order=order,
             jitter=jitter,
             color="k",
             size=size,
@@ -233,17 +230,15 @@
     if not len(keys):
         raise ValueError("No keys have been selected.")
     keys = _unique_order_preserving(keys)
 
     if not isinstance(threshold, Iterable):
         threshold = (threshold,) * len(keys)
     if len(threshold) != len(keys):
-        raise ValueError(
-            f"Expected `threshold` to be of length `{len(keys)}`, found `{len(threshold)}`."
-        )
+        raise ValueError(f"Expected `threshold` to be of length `{len(keys)}`, found `{len(threshold)}`.")
 
     ncols = max(len(keys) if ncols is None else ncols, 1)
     nrows = int(np.ceil(len(keys) / ncols))
     if figsize is None:
         figsize = np.array([n_cats * ncols, n_cats * nrows * 4 / 6]) / 2
 
     fig, axes = plt.subplots(
@@ -257,30 +252,30 @@
     axes = np.ravel([axes])
 
     i = 0
     for i, (key, ax, thresh) in enumerate(zip(keys, axes, threshold)):
         hue, palette, thresh_mask, sm = get_data(key, thresh)
         show_ylabel = i % ncols == 0
 
-        ax = stripplot(
+        ax = sns.stripplot(
             x=time_key,
             y="log_odds",
             data=df if thresh_mask is None else df[~thresh_mask],
             hue=hue,
             order=order,
             jitter=jitter,
             color="black",
             palette=palette,
             size=size,
             alpha=alpha if alpha is not None else None if thresh_mask is None else 0.8,
             ax=ax,
             **kwargs,
         )
         if thresh_mask is not None:
-            stripplot(
+            sns.stripplot(
                 x=time_key,
                 y="log_odds",
                 data=df if thresh_mask is None else df[thresh_mask],
                 hue=hue,
                 order=order,
                 jitter=jitter,
                 color=threshold_color,
@@ -298,17 +293,15 @@
             if legend_loc in (None, "none"):
                 legend = ax.get_legend()
                 if legend is not None:
                     legend.remove()
             else:
                 handles, labels = ax.get_legend_handles_labels()
                 if len(handles):
-                    _position_legend(
-                        ax, legend_loc=legend_loc, handles=handles, labels=labels
-                    )
+                    _position_legend(ax, legend_loc=legend_loc, handles=handles, labels=labels)
 
         decorate(ax, title=key, show_ylabel=show_ylabel)
 
     for ax in axes[i + 1 :]:
         ax.remove()
     axes = axes[: i + 1]
```

### Comparing `cellrank-1.5.1/cellrank/pl/_utils.py` & `cellrank-2.0.0/src/cellrank/pl/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,238 +1,102 @@
+import collections
+import copy
+import itertools
+import pathlib
 from typing import (
     Any,
+    Callable,
     Dict,
     List,
-    Tuple,
-    Union,
     Mapping,
-    TypeVar,
-    Callable,
+    NamedTuple,
     Optional,
     Sequence,
+    Tuple,
+    TypeVar,
+    Union,
 )
 
-from copy import copy
-from pathlib import Path
-from itertools import combinations
-from collections import namedtuple, defaultdict
-
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank.tl._enum import _DEFAULT_BACKEND
-from cellrank.ul._docs import d
-from cellrank.tl._utils import save_fig, _unique_order_preserving
-from cellrank.ul.models import GAMR, BaseModel, FailedModel, SKLearnModel
-from cellrank.tl._colors import _create_categorical_colors
-from cellrank.ul._parallelize import parallelize
-from cellrank.ul.models._base_model import ColorType
-
 import numpy as np
 import pandas as pd
-from pandas.api.types import infer_dtype, is_numeric_dtype, is_categorical_dtype
+from pandas.api.types import infer_dtype, is_categorical_dtype, is_numeric_dtype
 
 import matplotlib as mpl
-import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
-from matplotlib import cm
+from matplotlib import cm, colors
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
+from anndata import AnnData
+
+from cellrank import logging as logg
+from cellrank._utils._colors import _create_categorical_colors
+from cellrank._utils._docs import d
+from cellrank._utils._enum import DEFAULT_BACKEND
+from cellrank._utils._parallelize import parallelize
+from cellrank._utils._utils import _unique_order_preserving, save_fig
+from cellrank.models import GAMR, BaseModel, FailedModel, SKLearnModel
+from cellrank.models._base_model import ColorType
+
+__all__ = ["composition"]
+
 Queue = TypeVar("Queue")
 Graph = TypeVar("Graph")
 
 
-_ERROR_INCOMPLETE_SPEC = (
-    "No options were specified for {}. "
-    "Consider specifying a fallback model using '*'."
-)
+_ERROR_INCOMPLETE_SPEC = "No options were specified for {}. " "Consider specifying a fallback model using '*'."
 _time_range_type = Optional[Union[float, Tuple[Optional[float], Optional[float]]]]
 _return_model_type = Mapping[str, Mapping[str, BaseModel]]
 _input_model_type = Union[BaseModel, _return_model_type]
 _callback_type = Optional[Union[Callable, Mapping[str, Mapping[str, Callable]]]]
 
-BulkRes = namedtuple("BulkRes", ["x_test", "y_test"])
-
-
-def _curved_edges(
-    G: Graph,
-    pos: Mapping,
-    radius_fraction: float,
-    dist_ratio: float = 0.2,
-    bezier_precision: int = 20,
-    polarity: str = "directed",
-) -> np.ndarray:
-    """
-    Create curved edges from a graph. Modified from: https://github.com/beyondbeneath/bezier-curved-edges-networkx.
-
-    Parameters
-    ----------
-    G: :class:`networkx.Graph`
-        Graph for which to create curved edges.
-    pos
-        Mapping of nodes to positions.
-    radius_fraction
-        Fraction of a unit circle when self loops are present.
-    dist_ratio
-        Distance of control points of bezier curves.
-    bezier_precision
-        Number of points in the curves.
-    polarity
-        Polarity of curves, one of `'random', 'directed' or 'fixed'`.
-        If using `'random'`, incoming and outgoing edges may overlap.
-
-    Returns
-    -------
-    Array of shape ``(n_edges, bezier_precision, 2)`` containing the curved edges.
-    """
-
-    try:
-        import bezier
-    except ImportError as e:
-        raise ImportError("Please install `bezier` as `pip install bezier`.") from e
-
-    # Get nodes into np array
-    edges = np.array(G.edges())
-    n_edges = edges.shape[0]
-
-    self_loop_mask = edges[:, 0] == edges[:, 1]
-    pos_sl = {edge[0]: pos[edge[0]] for edge in edges[self_loop_mask, ...]}
-
-    if polarity == "random":
-        # Random polarity of curve
-        rnd = np.where(np.random.randint(2, size=n_edges) == 0, -1, 1)
-    elif polarity == "directed":
-        rnd = np.where(edges[:, 0] > edges[:, 1], -1, 1)
-    elif polarity == "fixed":
-        # Create a fixed (hashed) polarity column in the case we use fixed polarity
-        # This is useful, e.g., for animations
-        rnd = np.where(
-            np.mod(np.vectorize(hash)(edges[:, 0]) + np.vectorize(hash)(edges[:, 1]), 2)
-            == 0,
-            -1,
-            1,
-        )
-    else:
-        raise ValueError(
-            f"Polarity `{polarity!r}` is not a valid option. "
-            f"Valid options are: `'random', 'directed' or 'fixed'`."
-        )
-
-    # Coordinates (x, y) of both nodes for each edge
-    # Note the np.vectorize method doesn't work for all node position dictionaries for some reason
-    u, inv = np.unique(edges, return_inverse=True)
-    coords = np.array([pos[x] for x in u])[inv].reshape(
-        [edges.shape[0], 2, edges.shape[1]]
-    )
-    coords_node1 = coords[:, 0, :]
-    coords_node2 = coords[:, 1, :]
-
-    # Swap node1/node2 allocations to make sure the directionality works correctly
-    should_swap = coords_node1[:, 0] > coords_node2[:, 0]
-    coords_node1[should_swap], coords_node2[should_swap] = (
-        coords_node2[should_swap],
-        coords_node1[should_swap],
-    )
-
-    # Distance for control points
-    dist = dist_ratio * np.sqrt(np.sum((coords_node1 - coords_node2) ** 2, axis=1))
 
-    # Gradients of line connecting node & perpendicular
-    m1 = (coords_node2[:, 1] - coords_node1[:, 1]) / (
-        coords_node2[:, 0] - coords_node1[:, 0]
-    )
-    m2 = -1 / m1
-
-    # Temporary points along the line which connects two nodes
-    t1 = dist / np.sqrt(1 + m1 ** 2)
-    v1 = np.array([np.ones(n_edges), m1])
-    coords_node1_displace = coords_node1 + (v1 * t1).T
-    coords_node2_displace = coords_node2 - (v1 * t1).T
-
-    # Control points, same distance but along perpendicular line
-    # rnd gives the 'polarity' to determine which side of the line the curve should arc
-    t2 = dist / np.sqrt(1 + m2 ** 2)
-    v2 = np.array([np.ones(len(edges)), m2])
-    coords_node1_ctrl = coords_node1_displace + (rnd * v2 * t2).T
-    coords_node2_ctrl = coords_node2_displace + (rnd * v2 * t2).T
-
-    # Combine all these four (x,y) columns into a 'node matrix'
-    node_matrix = np.array(
-        [coords_node1, coords_node1_ctrl, coords_node2_ctrl, coords_node2]
-    )
-
-    nums = np.linspace(0, 2 * np.pi, bezier_precision)
-
-    # Create the Bezier curves and store them in a list
-
-    self_loops = []
-    for p in pos_sl.values():
-        self_loops.append(np.c_[np.cos(nums), np.sin(nums)] * radius_fraction + p)
-
-    curveplots = []
-    for i in range(len(edges)):
-        nodes = node_matrix[:, i, :].T
-        curveplots.append(
-            bezier.Curve(nodes, degree=3)
-            .evaluate_multi(np.linspace(0, 1, bezier_precision))
-            .T
-        )
-
-    # Return an array of these curves
-    curves = np.array(curveplots)
-    if np.any(self_loop_mask):
-        curves[self_loop_mask, ...] = self_loops
-
-    return curves
+class BulkRes(NamedTuple):
+    x_test: np.ndarray
+    y_test: np.ndarray
 
 
 def _is_any_gam_mgcv(models: Union[BaseModel, Dict[str, Dict[str, BaseModel]]]) -> bool:
-    """
-    Return whether any models to be fit are from R's `mgcv` package.
+    """Return whether any models to be fit are from R's `mgcv` package.
 
     Parameters
     ----------
     models
-        Model(s) used for fitting.
+        Model used for fitting.
 
     Returns
     -------
-    `True` if any of the models is from R's mgcv package, else `False`.
+    :obj:`True` if any of the models is from R's mgcv package, else :obj:`False`.
     """
-
     return isinstance(models, GAMR) or (
-        isinstance(models, dict)
-        and any(isinstance(m, GAMR) for ms in models.values() for m in ms.values())
+        isinstance(models, dict) and any(isinstance(m, GAMR) for ms in models.values() for m in ms.values())
     )
 
 
 def _create_models(
     model: _input_model_type, obs: Sequence[str], lineages: Sequence[Optional[str]]
 ) -> _return_model_type:
-    """
-    Create models for each gene and lineage.
+    """Create models for each gene and lineage.
 
     Parameters
     ----------
     obs
         Sequence of observations, such as genes.
     lineages
         Sequence of genes.
 
     Returns
     -------
     The created models.
     """
 
-    def process_lineages(
-        obs_name: str, lin_names: Union[BaseModel, Dict[Optional[str], Any]]
-    ):
+    def process_lineages(obs_name: str, lin_names: Union[BaseModel, Dict[Optional[str], Any]]):
         if isinstance(lin_names, BaseModel):
             # sharing the same models for all lineages
             for lin_name in lineages:
-                models[obs_name][lin_name] = copy(lin_names)
+                models[obs_name][lin_name] = copy.copy(lin_names)
             return
         if not isinstance(lin_names, dict):
             raise TypeError(
                 f"Expected the model to be either a lineage specific `dict` or a `BaseModel`, "
                 f"found `{type(lin_names).__name__!r}`."
             )
 
@@ -247,44 +111,42 @@
             if lin_name == "*":
                 continue
             if not isinstance(mod, BaseModel):
                 raise TypeError(
                     f"Expected the model for gene `{obs_name!r}` and lineage `{lin_name!r}` "
                     f"to be of type `BaseModel`, found `{type(mod).__name__!r}`."
                 )
-            models[obs_name][lin_name] = copy(mod)
+            models[obs_name][lin_name] = copy.copy(mod)
 
         if set(models[obs_name].keys()) & lineages == lineages:
             return
 
         if lin_rest_model is not None:
             for lin_name in lineages - set(models[obs_name].keys()):
-                models[obs_name][lin_name] = copy(lin_rest_model)
+                models[obs_name][lin_name] = copy.copy(lin_rest_model)
         else:
-            raise ValueError(
-                _ERROR_INCOMPLETE_SPEC.format(f"all lineages for gene `{obs_name!r}`")
-            )
+            raise ValueError(_ERROR_INCOMPLETE_SPEC.format(f"all lineages for gene `{obs_name!r}`"))
 
     if not len(lineages):
         raise ValueError("No lineages have been selected.")
 
     if not len(obs):
         raise ValueError("No genes have been selected.")
 
     if isinstance(model, BaseModel):
         return {
-            o: {lin: copy(model) for lin in _unique_order_preserving(lineages)}
+            o: {lin: copy.copy(model) for lin in _unique_order_preserving(lineages)}
             for o in _unique_order_preserving(obs)
         }
 
     lineages, obs = (
         set(_unique_order_preserving(lineages)),
         set(_unique_order_preserving(obs)),
     )
-    models = defaultdict(dict)
+    models = collections.defaultdict(dict)
 
     if isinstance(model, dict):
         obs_rest_model = model.pop("*", None)
         if obs_rest_model is not None and not isinstance(obs_rest_model, BaseModel):
             raise TypeError(
                 f"Expected the gene fallback model to be of type `BaseModel`, "
                 f"found `{type(obs_rest_model).__name__!r}`."
@@ -293,51 +155,42 @@
         for obs_name, lin_names in model.items():
             process_lineages(obs_name, lin_names)
 
         if obs_rest_model is not None:
             for obs_name in obs - set(model.keys()):
                 process_lineages(obs_name, model.get(obs_name, obs_rest_model))
         elif set(model.keys()) != obs:
-            raise ValueError(
-                _ERROR_INCOMPLETE_SPEC.format(
-                    f"genes `{list(obs - set(model.keys()))}`."
-                )
-            )
+            raise ValueError(_ERROR_INCOMPLETE_SPEC.format(f"genes `{list(obs - set(model.keys()))}`."))
     else:
         raise TypeError(
             f"Class `{type(model).__name__!r}` must be of type `BaseModel` or "
             f"a gene and lineage specific `dict` of `BaseModel`.."
         )
 
     if set(models.keys()) & obs != obs:
-        raise ValueError(
-            f"Missing gene models for the following genes: `{list(obs - set(models.keys()))}`."
-        )
+        raise ValueError(f"Missing gene models for the following genes: `{list(obs - set(models.keys()))}`.")
 
     for gene, vs in models.items():
         if set(vs.keys()) & lineages != lineages:
-            raise ValueError(
-                f"Missing lineage models for the gene `{gene!r}`: `{list(lineages - set(vs.keys()))}`."
-            )
+            raise ValueError(f"Missing lineage models for the gene `{gene!r}`: `{list(lineages - set(vs.keys()))}`.")
 
     return models
 
 
 def _fit_bulk_helper(
     genes: Sequence[str],
     models: _input_model_type,
     callbacks: _callback_type,
     lineages: Sequence[Optional[str]],
     time_range: Sequence[Union[float, Tuple[float, float]]],
     return_models: bool = False,
     queue: Optional[Queue] = None,
     **kwargs,
 ) -> Dict[str, Dict[str, BaseModel]]:
-    """
-    Fit model for given genes and lineages.
+    """Fit model for given genes and lineages.
 
     Parameters
     ----------
     genes
         Genes for which to fit the models.
     models
         Gene and lineage specific models.
@@ -348,21 +201,21 @@
     time_range
         Minimum and maximum pseudotimes.
     return_models
         Whether to return the full models or just tuple ``(x_test,  y_test)``.
     queue
         Signalling queue in the parent process/thread used to update the progress bar.
     kwargs
-        Keyword arguments for :func:`cellrank.ul.models.BaseModel.prepare`.
+        Keyword arguments for :func:`~cellrank.models.BaseModel.prepare`.
 
     Returns
     -------
     The fitted models, optionally containing the confidence interval in the form of
-    `{'gene1': {'lineage1': <model11>, ...}, ...}`.
-    If any step has failed, the model will be of type :class:`cellrank.ul.models.FailedModel`.
+    ``{'gene1': {'lineage1': <model11>, ...}, ...}``.
+    If any step has failed, the model will be of type :class:`~cellrank.models.FailedModel`.
     """
     if len(lineages) != len(time_range):
         raise ValueError(
             f"Expected `lineage` and `time_range` to be of same length, "
             f"found `{len(lineages)}` != `{len(time_range)}`."
         )
 
@@ -384,17 +237,15 @@
                 model.predict()
             elif _is_any_gam_mgcv(model):
                 model.predict(level=conf_int if isinstance(conf_int, float) else 0.95)
             else:
                 model.predict()
                 model.confidence_interval()
 
-            res[gene][ln] = (
-                model if return_models else BulkRes(model.x_test, model.y_test)
-            )
+            res[gene][ln] = model if return_models else BulkRes(model.x_test, model.y_test)
 
         if queue is not None:
             queue.put(1)
 
     if queue is not None:
         queue.put(None)
 
@@ -408,34 +259,33 @@
     lineages: Union[str, Sequence[str]],
     time_range: _time_range_type,
     parallel_kwargs: dict,
     return_models: bool = False,
     filter_all_failed: bool = True,
     **kwargs,
 ) -> Tuple[_return_model_type, _return_model_type, Sequence[str], Sequence[str]]:
-    """
-    Fit models for given genes and lineages.
+    """Fit models for given genes and lineages.
 
     Parameters
     ----------
     models
         Gene and lineage specific estimators.
     callbacks
-        Functions which are called to prepare the ``models`.
+        Functions which are called to prepare the ``models``.
     genes
         Genes for which to fit the ``models``.
     lineages
         Lineages for which to fit the ``models``.
     time_range
         Possibly ``lineages`` specific start- and endtimes.
     parallel_kwargs
-        Keyword arguments for :func:`cellrank.ul._utils.parallelize`.
+        Keyword arguments for :func:`~cellrank._utils._parallelize.parallelize`.
     return_models
-        Whether to return the full models or just a dictionary of dictionaries of :class:`collections.namedtuple`,
-        `(x_test, y_test)`. This is highly discouraged because no meaningful error messages will be produced.
+        Whether to return the full models or just a dictionary of dictionaries of :class:`~typing.NamedTuple`,
+        ``(x_test, y_test)``. This is highly discouraged because no meaningful error messages will be produced.
     filter_all_failed
         Whether to filter out all models which have failed.
 
     Returns
     -------
     All the models, including the failed ones. It is a nested dictionary where keys are the ``genes`` and the values
     is again a :class:`dict`, where keys are ``lineages`` and values are the failed or fitted models or
@@ -445,27 +295,23 @@
     that this dictionary will contain only genes which have been successfully fitted for at least 1 lineage.
     If ``return_models = True``, the models are just a :class:`collections.namedtuple` of `(x_test, y_test)`.
 
     All the genes of the filtered models.
 
     All the lineage of the filtered models.
     """
-
     if isinstance(genes, str):
         genes = [genes]
-
     if isinstance(lineages, str):
         lineages = [lineages]
 
     if isinstance(time_range, (tuple, float, int, type(None))):
         time_range = [time_range] * len(lineages)
     elif len(time_range) != len(lineages):
-        raise ValueError(
-            f"Expected time ranges to be of length `{len(lineages)}`, found `{len(time_range)}`."
-        )
+        raise ValueError(f"Expected time ranges to be of length `{len(lineages)}`, found `{len(time_range)}`.")
 
     n_jobs = parallel_kwargs.pop("n_jobs", 1)
 
     start = logg.info(f"Computing trends using `{n_jobs}` core(s)")
     models = parallelize(
         _fit_bulk_helper,
         genes,
@@ -478,77 +324,59 @@
         lineages=lineages,
         time_range=time_range,
         return_models=return_models,
         **kwargs,
     )
     logg.info("    Finish", time=start)
 
-    return _filter_models(
-        models, return_models=return_models, filter_all_failed=filter_all_failed
-    )
+    return _filter_models(models, return_models=return_models, filter_all_failed=filter_all_failed)
 
 
 def _filter_models(
     models, return_models: bool = False, filter_all_failed: bool = True
 ) -> Tuple[_return_model_type, _return_model_type, Sequence[str], Sequence[str]]:
     def is_valid(x: Union[BaseModel, BulkRes]) -> bool:
         if return_models:
-            assert isinstance(
-                x, BaseModel
-            ), f"Expected `BaseModel`, found `{type(x).__name__!r}`."
+            assert isinstance(x, BaseModel), f"Expected `BaseModel`, found `{type(x).__name__!r}`."
             return bool(x)
 
-        return (
-            x.x_test is not None
-            and x.y_test is not None
-            and np.all(np.isfinite(x.y_test))
-        )
+        return x.x_test is not None and x.y_test is not None and np.all(np.isfinite(x.y_test))
 
     modelmat = pd.DataFrame(models).T
     modelmask = modelmat.applymap(is_valid)
     to_keep = modelmask[modelmask.any(axis=1)]
     to_keep = to_keep.loc[:, to_keep.any(axis=0)].T
 
     filtered_models = {
         gene: {
             ln: models[gene][ln]
-            for ln in (
-                ln
-                for ln in v.keys()
-                if (is_valid(models[gene][ln]) if filter_all_failed else True)
-            )
+            for ln in (ln for ln in v if (is_valid(models[gene][ln]) if filter_all_failed else True))
         }
         for gene, v in to_keep.to_dict().items()
     }
 
     if not len(filtered_models):
         if not return_models:
             raise RuntimeError(
                 "Fitting has failed for all gene/lineage combinations. "
                 "Specify `return_models=True` for more information."
             )
         for ms in models.values():
             for model in ms.values():
-                assert isinstance(
-                    model, FailedModel
-                ), f"Expected `FailedModel`, found `{type(model).__name__!r}`."
+                assert isinstance(model, FailedModel), f"Expected `FailedModel`, found `{type(model).__name__!r}`."
                 model.reraise()
 
     if not np.all(modelmask.values):
         failed_models = modelmat.values[~modelmask.values]
         logg.warning(
             f"Unable to fit `{len(failed_models)}` models." + ""
             if return_models
             else "Consider specify `return_models=True` for further inspection."
         )
-        logg.debug(
-            "The failed models were:\n`{}`".format(
-                "\n".join(f"    {m}" for m in failed_models)
-            )
-        )
+        logg.debug("The failed models were:\n`{}`".format("\n".join(f"    {m}" for m in failed_models)))
 
     # lineages is the max number of lineages
     return models, filtered_models, tuple(filtered_models.keys()), tuple(to_keep.index)
 
 
 @d.dedent
 def _trends_helper(
@@ -559,124 +387,112 @@
     same_plot: bool = False,
     sharey: Union[str, bool] = False,
     show_ylabel: bool = True,
     show_lineage: Union[bool, np.ndarray] = True,
     show_xticks_and_label: Union[bool, np.ndarray] = True,
     lineage_cmap: Optional[Union[mpl.colors.ListedColormap, Sequence]] = None,
     lineage_probability_color: Optional[str] = None,
-    abs_prob_cmap=cm.viridis,
+    fate_prob_cmap=cm.viridis,
     gene_as_title: bool = False,
     cell_color: Optional[str] = None,
     legend_loc: Optional[str] = "best",
     fig: mpl.figure.Figure = None,
     axes: Union[mpl.axes.Axes, Sequence[mpl.axes.Axes]] = None,
     **kwargs: Any,
 ) -> None:
-    """
-    Plot an expression gene for some lineages.
+    """Plot an expression gene for some lineages.
 
     Parameters
     ----------
     %(adata)s
     %(model)s
     gene
-        Name of the gene in `adata.var_names``.
+        Name of the gene in :attr:`~anndata.AnnData.var_names`.
     ln_key
-        Key in ``adata.obsm`` where to find the lineages.
+        Key in :attr:`~anndata.AnnData.bosm` where to find the lineages.
     lineage_names
         Names of lineages to plot.
     same_plot
         Whether to plot all lineages in the same plot or separately.
     sharey
         Whether the y-axis is being shared.
     show_ylabel
         Whether to show y-label on the y-axis. Usually, only the first column will contain the y-label.
     show_lineage
         Whether to show the lineage as the title. Usually, only first row will contain the lineage names.
     show_xticks_and_label
         Whether to show x-ticks and x-label. Usually, only the last row will show this.
     lineage_cmap
-        Colormap to use when coloring the the lineage. When ``transpose``, this corresponds to the color of genes.
+        Colormap to use when coloring the lineage. When ``transpose = True``, this corresponds to the color of genes.
     lineage_probability_color
-        Actual color of 1 ``lineage``. Only used when ``same_plot=True`` and ``transpose=True`` and
-        ``lineage_probability=True``.
-    abs_prob_cmap:
-        Colormap to use when coloring in the absorption probabilities, if they are being plotted.
+        Actual color of one ``lineage``. Only used when ``same_plot = True`` and ``transpose = True`` and
+        ``lineage_probability = True``.
+    fate_prob_cmap:
+        Colormap to use when coloring in the fate probabilities, if they are being plotted.
     gene_as_title
         Whether to use the gene names as titles (with lineage names as well) or on the y-axis.
     legend_loc
-        Location of the legend. If `None`, don't show any legend.
+        Location of the legend. If :obj:`None`, don't show any legend.
     fig
         Figure to use.
     ax
         Ax to use.
     kwargs
-        Keyword arguments for :meth:`cellrank.ul.models.BaseModel.plot`.
+        Keyword arguments for :meth:`~cellrank.models.BaseModel.plot`.
 
     Returns
     -------
     %(just_plots)s
     """
-
     n_lineages = len(lineage_names)
     if same_plot:
         axes = [axes] * len(lineage_names)
 
     axes = np.ravel(axes)
 
     percs = kwargs.pop("perc", None)
     if percs is None or not isinstance(percs[0], (tuple, list)):
         percs = [percs]
 
     same_perc = False  # we need to show colorbar always if percs differ
     if len(percs) != n_lineages or n_lineages == 1:
         if len(percs) != 1:
-            raise ValueError(
-                f"Percentile must be a collection of size `1` or `{n_lineages}`, got `{len(percs)}`."
-            )
+            raise ValueError(f"Percentile must be a collection of size `1` or `{n_lineages}`, got `{len(percs)}`.")
         same_perc = True
         percs = percs * n_lineages
 
     hide_cells = kwargs.pop("hide_cells", False)
     show_cbar = kwargs.pop("cbar", True)
     show_prob = kwargs.pop("lineage_probability", False)
 
     if same_plot:
         if not transpose:
             lineage_colors = (
-                lineage_cmap.colors
-                if lineage_cmap is not None and hasattr(lineage_cmap, "colors")
-                else lineage_cmap
+                lineage_cmap.colors if lineage_cmap is not None and hasattr(lineage_cmap, "colors") else lineage_cmap
             )
         else:
             # this should be fine w.r.t. to the missing genes, since they are in the same order AND
             # we're also passing the failed models (this is important)
             # these are actually gene colors
             if lineage_cmap is not None:
                 lineage_colors = (
                     lineage_cmap.colors
                     if hasattr(lineage_cmap, "colors")
                     else [c for _, c in zip(lineage_names, lineage_cmap)]
                 )
             else:
                 lineage_colors = _create_categorical_colors(n_lineages)
     else:
-        lineage_colors = (
-            ("black" if not mcolors.is_color_like(lineage_cmap) else lineage_cmap),
-        ) * n_lineages
+        lineage_colors = (("black" if not colors.is_color_like(lineage_cmap) else lineage_cmap),) * n_lineages
 
     if n_lineages > len(lineage_colors):
-        raise ValueError(
-            f"Expected at least `{n_lineages}` colors, found `{len(lineage_colors)}`."
-        )
+        raise ValueError(f"Expected at least `{n_lineages}` colors, found `{len(lineage_colors)}`.")
 
     lineage_color_mapper = {ln: lineage_colors[i] for i, ln in enumerate(lineage_names)}
-    successful_models = {
-        ln: models[gene][ln] for ln in lineage_names if models[gene][ln]
-    }
+    successful_models = {ln: models[gene][ln] for ln in lineage_names if models[gene][ln]}
 
     if show_prob and same_plot:
         minns, maxxs = zip(
             *(
                 models[gene][n]._return_min_max(
                     show_conf_int=kwargs.get("conf_int", False),
                 )
@@ -725,34 +541,30 @@
                 title = ""
                 ylabel = gene
         else:
             if gene_as_title:
                 title = None
                 ylabel = "expression" if not ylabel_shown else None
             else:
-                title = (
-                    (name if name is not None else "no lineage")
-                    if show_lineage[i]
-                    else ""
-                )
+                title = (name if name is not None else "no lineage") if show_lineage[i] else ""
                 ylabel = gene if not ylabel_shown else None
 
         model.plot(
             ax=ax,
             fig=fig,
             perc=perc,
             cell_color=cell_color,
             cbar=False,
             obs_legend_loc=None,
             title=title,
             hide_cells=True if hide_cells else cells_shown if same_plot else False,
             same_plot=same_plot,
             lineage_color=lineage_color_mapper[name],
             lineage_probability_color=lineage_probability_color,
-            abs_prob_cmap=abs_prob_cmap,
+            fate_prob_cmap=fate_prob_cmap,
             lineage_probability=show_prob,
             ylabel=ylabel,
             **kwargs,
         )
         if sharey in ("row", "all", True) and not ylabel_shown:
             plt.setp(ax.get_yticklabels(), visible=True)
 
@@ -764,95 +576,82 @@
         last_ax = ax
         ylabel_shown = True
         cells_shown = True
 
     key, color, typp, mapper = model._get_colors(cell_color, same_plot=same_plot)
     if typp == ColorType.CAT:
         if not hide_cells:
-            model._maybe_add_legend(
-                fig, ax, mapper=mapper, title=key, loc=obs_legend_loc, is_line=False
-            )
-    elif typp == ColorType.CONT:
-        if same_perc and show_cbar and not hide_cells:
-            if isinstance(color, np.ndarray):
-                # plotting cont. observation other than lin. probs as a color
-                vmin = np.min(color)
-                vmax = np.max(color)
-            else:
-                vmin = np.min([model.w_all for model in successful_models.values()])
-                vmax = np.max([model.w_all for model in successful_models.values()])
-            norm = mcolors.Normalize(vmin=vmin, vmax=vmax)
-
-            for ax in axes:
-                children = [
-                    c
-                    for c in ax.get_children()
-                    if isinstance(c, mpl.collections.PathCollection)
-                ]
-                if len(children):
-                    children[0].set_norm(norm)
-
-            divider = make_axes_locatable(last_ax)
-            cax = divider.append_axes("right", size="2%", pad=0.1)
-            _ = mpl.colorbar.ColorbarBase(
-                cax,
-                norm=norm,
-                cmap=abs_prob_cmap,
-                label=key,
-                ticks=np.linspace(norm.vmin, norm.vmax, 5),
-            )
+            model._maybe_add_legend(fig, ax, mapper=mapper, title=key, loc=obs_legend_loc, is_line=False)
+    elif typp == ColorType.CONT and same_perc and show_cbar and not hide_cells:
+        if isinstance(color, np.ndarray):
+            # plotting cont. observation other than lin. probs as a color
+            vmin = np.min(color)
+            vmax = np.max(color)
+        else:
+            vmin = np.min([model.w_all for model in successful_models.values()])
+            vmax = np.max([model.w_all for model in successful_models.values()])
+        norm = colors.Normalize(vmin=vmin, vmax=vmax)
+
+        for ax in axes:
+            children = [c for c in ax.get_children() if isinstance(c, mpl.collections.PathCollection)]
+            if len(children):
+                children[0].set_norm(norm)
+
+        divider = make_axes_locatable(last_ax)
+        cax = divider.append_axes("right", size="2%", pad=0.1)
+        _ = mpl.colorbar.ColorbarBase(
+            cax,
+            norm=norm,
+            cmap=fate_prob_cmap,
+            label=key,
+            ticks=np.linspace(norm.vmin, norm.vmax, 5),
+        )
 
     if same_plot and lineage_names != [None]:
         model._maybe_add_legend(
             fig,
             ax,
-            mapper={ln: lineage_color_mapper[ln] for ln in successful_models.keys()},
+            mapper={ln: lineage_color_mapper[ln] for ln in successful_models},
             loc=legend_loc,
         )
 
 
 def _position_legend(ax: mpl.axes.Axes, legend_loc: str, **kwargs) -> mpl.legend.Legend:
-    """
-    Position legend in- or outside the figure.
+    """Position legend inside or outside the figure.
 
     Parameters
     ----------
     ax
         Ax where to position the legend.
     legend_loc
         Position of legend.
     kwargs
-        Keyword arguments for :func:`matplotlib.pyplot.legend`.
+        Keyword arguments for :meth:`matplotlib.axes.Axes.legend`.
 
     Returns
     -------
     The created legend.
     """
-
     if legend_loc == "center center out":
         raise ValueError("Invalid option: `'center center out'`.")
     if legend_loc == "best":
         return ax.legend(loc="best", **kwargs)
 
     tmp, loc = legend_loc.split(" "), ""
 
     if len(tmp) == 1:
         height, rest = tmp[0], []
         width = "right" if height in ("upper", "top", "center") else "left"
     else:
         height, width, *rest = legend_loc.split(" ")
         if rest:
             if len(rest) != 1:
-                raise ValueError(
-                    f"Expected only 1 additional modifier ('in' or 'out'), found `{list(rest)}`."
-                )
-            elif rest[0] not in ("in", "out"):
-                raise ValueError(
-                    f"Invalid modifier `{rest[0]!r}`. Valid options are: `'in', 'out'`."
-                )
+                raise ValueError(f"Expected only 1 additional modifier ('in' or 'out'), found `{list(rest)}`.")
+            if rest[0] not in ("in", "out"):
+                raise ValueError(f"Invalid modifier `{rest[0]!r}`. Valid options are: `'in', 'out'`.")
             if rest[0] == "in":  # ignore in, it's default
                 rest = []
 
     if height in ("upper", "top"):
         y = 1.55 if width == "center" else 1.025
         loc += "upper"
     elif height == "center":
@@ -875,82 +674,75 @@
         if height != "center":  # causes to be like top center
             loc += " center"
     elif width == "right":
         x = 1.05
         loc += " left" if rest else " right"
     else:
         raise ValueError(
-            f"Invalid legend position on x-axis: `{width!r}`. "
-            f"Valid options are: `'left', 'center', 'right'`."
+            f"Invalid legend position on x-axis: `{width!r}`. " f"Valid options are: `'left', 'center', 'right'`."
         )
 
     if rest:
         kwargs["bbox_to_anchor"] = (x, y)
 
     return ax.legend(loc=loc, **kwargs)
 
 
 def _get_backend(model, backend: str) -> str:
-    return _DEFAULT_BACKEND if _is_any_gam_mgcv(model) else backend
+    return DEFAULT_BACKEND if _is_any_gam_mgcv(model) else backend
 
 
 @d.dedent
 def _create_callbacks(
     adata: AnnData,
     callback: Optional[Callable],
     obs: Sequence[str],
     lineages: Sequence[Optional[str]],
     perform_sanity_check: Optional[bool] = None,
     **kwargs,
 ) -> Dict[str, Dict[str, Callable]]:
-    """
-    Create models for each gene and lineage.
+    """Create models for each gene and lineage.
 
     Parameters
     ----------
     %(adata)s
     callback
         Gene and lineage specific prepare callbacks.
     obs
         Sequence of observations, such as genes.
     lineages
         Sequence of genes.
     perform_sanity_check
         Whether to check if all callbacks have the correct signature. This is done by instantiating
         dummy model and running the function. We're assuming that the callback isn't really a pricey operation.
-
-        If `None`, it is only performed for non-default callbacks.
+        If :obj:`None`, it is only performed for non-default callbacks.
     kwargs
         Keyword arguments for ``callback`` when performing the sanity check.
 
     Returns
     -------
     The created callbacks.
     """
 
-    def process_lineages(
-        obs_name: str, lin_names: Optional[Union[Callable, Dict[Optional[str], Any]]]
-    ) -> None:
+    def process_lineages(obs_name: str, lin_names: Optional[Union[Callable, Dict[Optional[str], Any]]]) -> None:
         if lin_names is None:
             lin_names = _default_model_callback
 
         if callable(lin_names):
             # sharing the same models for all lineages
             for lin_name in lineages:
                 callbacks[obs_name][lin_name] = lin_names
             return
-        elif not isinstance(lin_names, dict):
+        if not isinstance(lin_names, dict):
             raise TypeError(
                 f"Expected the lineage callback to be either `callable` or a dictionary of callables, "
                 f"found `{type(lin_names).__name__!r}`."
             )
 
-        lin_rest_callback = (
-            lin_names.get("*", _default_model_callback) or _default_model_callback
-        )  # do not pop
+        lin_rest_callback = lin_names.get("*", _default_model_callback) or _default_model_callback  # do not pop
         if not callable(lin_rest_callback):
             raise TypeError(
                 f"Expected the lineage fallback callback for gene `{obs_name!r}` to be `callable`, "
                 f"found `{type(lin_rest_callback).__name__!r}`."
             )
 
         for lin_name, cb in lin_names.items():
@@ -969,36 +761,31 @@
     def maybe_sanity_check(callbacks: Dict[str, Dict[str, Callable]]) -> None:
         if not perform_sanity_check:
             return
 
         from sklearn.svm import SVR
 
         logg.debug("Performing callback sanity checks")
-        for gene in callbacks.keys():
+        for gene in callbacks:
             for lineage, cb in callbacks[gene].items():
                 # create the model here because the callback can search the attribute
                 dummy_model = SKLearnModel(adata, model=SVR())
                 try:
                     model = cb(dummy_model, gene=gene, lineage=lineage, **kwargs)
                     assert model is dummy_model, (
-                        "Creation of new models is not allowed. "
-                        "Ensure that callback returns the same model."
+                        "Creation of new models is not allowed. " "Ensure that callback returns the same model."
                     )
-                    assert (
-                        model.prepared
-                    ), "Model is not prepared. Ensure that callback calls `.prepare()`."
-                    assert (
-                        model._gene == gene
-                    ), f"Callback modified the gene from `{gene!r}` to `{model._gene!r}`."
+                    assert model.prepared, "Model is not prepared. Ensure that callback calls `.prepare()`."
+                    assert model._gene == gene, f"Callback modified the gene from `{gene!r}` to `{model._gene!r}`."
                     assert (
                         model._lineage == lineage
                     ), f"Callback modified the lineage from `{lineage!r}` to `{model._lineage!r}`."
                     if isinstance(model, FailedModel):
                         model.reraise()
-                except Exception as e:  # noqa: B902
+                except Exception as e:  # noqa: BLE001
                     raise RuntimeError(
                         f"Callback validation failed for gene `{gene!r}` and lineage `{lineage!r}`."
                     ) from e
 
     def all_callbacks_are_default(cbs: dict) -> bool:
         # this correctly implicitly handles '*': None
         for vs in cbs.values():
@@ -1032,21 +819,19 @@
         maybe_sanity_check(callbacks)
         return callbacks
 
     lineages, obs = (
         set(_unique_order_preserving(lineages)),
         set(_unique_order_preserving(obs)),
     )
-    callbacks = defaultdict(dict)
+    callbacks = collections.defaultdict(dict)
 
     if isinstance(callback, dict):
         # can be specified as None
-        obs_rest_callback = (
-            callback.pop("*", _default_model_callback) or _default_model_callback
-        )
+        obs_rest_callback = callback.pop("*", _default_model_callback) or _default_model_callback
 
         for obs_name, lin_names in callback.items():
             process_lineages(obs_name, lin_names)
 
         if callable(obs_rest_callback):
             for obs_name in obs - set(callback.keys()):
                 process_lineages(obs_name, callback.get(obs_name, obs_rest_callback))
@@ -1058,23 +843,19 @@
     else:
         raise TypeError(
             f"Class `{type(callback).__name__!r}` must be `callable` or "
             f"a gene and lineage specific `dict` of `callables`."
         )
 
     if set(callbacks.keys()) & obs != obs:
-        raise ValueError(
-            f"Missing gene callbacks for the following genes: `{list(obs - set(callbacks.keys()))}`."
-        )
+        raise ValueError(f"Missing gene callbacks for the following genes: `{list(obs - set(callbacks.keys()))}`.")
 
     for gene, vs in callbacks.items():
         if set(vs.keys()) & lineages != lineages:
-            raise ValueError(
-                f"Missing lineage callbacks for gene `{gene!r}`: `{list(lineages - set(vs.keys()))}`."
-            )
+            raise ValueError(f"Missing lineage callbacks for gene `{gene!r}`: `{list(lineages - set(vs.keys()))}`.")
 
     maybe_sanity_check(callbacks)
 
     return callbacks
 
 
 def _default_model_callback(model: BaseModel, **kwargs) -> BaseModel:
@@ -1085,43 +866,38 @@
 @d.dedent
 def composition(
     adata: AnnData,
     key: str,
     fontsize: Optional[str] = None,
     figsize: Optional[Tuple[float, float]] = None,
     dpi: Optional[float] = None,
-    save: Optional[Union[str, Path]] = None,
+    save: Optional[Union[str, pathlib.Path]] = None,
     **kwargs: Any,
 ) -> None:
-    """
-    Plot a pie chart for categorical annotation.
+    """Plot a pie chart for categorical annotation.
 
     Parameters
     ----------
     %(adata)s
     key
-        Key in :attr:`anndata.AnnData.obs` containing categorical observation.
+        Key in :attr:`~anndata.AnnData.obs` containing categorical observation.
     fontsize
         Font size for the pie chart labels.
     %(plotting)s
     kwargs
-        Keyword arguments for :func:`matplotlib.pyplot.pie`.
+        Keyword arguments for :meth:`~matplotlib.axes.Axes.pie`.
 
     Returns
     -------
     %(just_plots)s
     """
-
     if key not in adata.obs:
         raise KeyError(f"Data not found in `adata.obs[{key!r}]`.")
     if not is_categorical_dtype(adata.obs[key]):
-        raise TypeError(
-            f"Expected `adata.obs[{key!r}]` is not `categorical`, "
-            f"found `{infer_dtype(adata.obs[key])}`."
-        )
+        raise TypeError(f"Expected `adata.obs[{key!r}]` is not `categorical`, found `{infer_dtype(adata.obs[key])}`.")
 
     colors = adata.uns.get(f"{key}_colors", None)
     x = adata.obs[key].value_counts()
 
     # plot these fractions in a pie plot
     fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
 
@@ -1136,16 +912,15 @@
 
     if save is not None:
         save_fig(fig, save)
 
 
 # modified from: https://github.com/CarlEkerot/held-karp
 def _held_karp(dists: np.ndarray) -> Tuple[float, np.ndarray]:
-    """
-    Held-Karp algorithm solves the Traveling Salesman Problem.
+    """Held-Karp algorithm solves the Traveling Salesman Problem.
 
     This algorithm uses dynamic programming with memoization.
 
     Parameters
     ----------
     dists
         Distance matrix.
@@ -1164,15 +939,15 @@
     # Set transition cost from initial state
     for k in range(1, n):
         C[1 << k, k] = (dists[0][k], 0)
 
     # Iterate subsets of increasing length and store intermediate results
     # in classic dynamic programming manner
     for subset_size in range(2, n):
-        for subset in combinations(range(1, n), subset_size):
+        for subset in itertools.combinations(range(1, n), subset_size):
             # Set bits for all nodes in this subset
             bits = 0
             for bit in subset:
                 bits |= 1 << bit
 
             # Find the lowest cost to get to this subset
             for k in subset:
@@ -1182,15 +957,15 @@
                 for m in subset:
                     if m == 0 or m == k:
                         continue
                     res.append((C[prev, m][0] + dists[m][k], m))
                 C[bits, k] = min(res)
 
     # We're interested in all bits but the least significant (the start state)
-    bits = (2 ** n - 1) - 1
+    bits = (2**n - 1) - 1
 
     # Calculate optimal cost
     res = []
     for k in range(1, n):
         res.append((C[bits, k][0] + dists[k][0], k))
     opt, parent = min(res)
 
@@ -1204,32 +979,28 @@
 
     # Add implicit start state
     path.append(0)
 
     return opt, np.array(path)[::-1]
 
 
-def _get_categorical_colors(
-    adata: AnnData, cluster_key: str
-) -> Tuple[np.ndarray, Mapping[str, str]]:
+def _get_categorical_colors(adata: AnnData, cluster_key: str) -> Tuple[np.ndarray, Mapping[str, str]]:
     if cluster_key not in adata.obs:
         raise KeyError(f"Unable to find data in `adata.obs[{cluster_key!r}].`")
     if not is_categorical_dtype(adata.obs[cluster_key]):
         raise TypeError(
             f"Expected `adata.obs[{cluster_key!r}]` to be categorical, "
             f"found `{infer_dtype(adata.obs[cluster_key])}`."
         )
 
     color_key = f"{cluster_key}_colors"
     try:
         colors = adata.uns[color_key]
     except KeyError:
-        adata.uns[color_key] = colors = _create_categorical_colors(
-            len(adata.obs[cluster_key].cat.categories)
-        )
+        adata.uns[color_key] = colors = _create_categorical_colors(len(adata.obs[cluster_key].cat.categories))
     mapper = dict(zip(adata.obs[cluster_key].cat.categories, colors))
     mapper[np.nan] = "grey"
 
     return colors, mapper
 
 
 def _get_sorted_colors(
@@ -1240,36 +1011,30 @@
     tmax: float = np.inf,
 ) -> List[np.ndarray]:
     if time_key is not None:
         if time_key not in adata.obs:
             raise KeyError(f"Unable to find time in `adata.obs[{time_key!r}]`.")
         adata = adata[(adata.obs[time_key] >= tmin) & (adata.obs[time_key] <= tmax)]
         if not adata.n_obs:
-            raise ValueError(
-                f"Specified time range `{[tmin, tmax]}` does not contain any data."
-            )
+            raise ValueError(f"Specified time range `{[tmin, tmax]}` does not contain any data.")
         order = np.argsort(adata.obs[time_key].values)
     else:
         order = np.arange(adata.n_obs)
 
     if isinstance(cluster_key, str):
         cluster_key = (cluster_key,)
     cluster_key = _unique_order_preserving(cluster_key)
 
     res = []
     for ck in cluster_key:
         try:
-            colors, mapper = _get_categorical_colors(adata, ck)
-            res.append(
-                np.array(
-                    [mcolors.to_hex(mapper[v]) for v in adata.obs[ck].values[order]]
-                )
-            )
+            cols, mapper = _get_categorical_colors(adata, ck)
+            res.append(np.array([colors.to_hex(mapper[v]) for v in adata.obs[ck].values[order]]))
         except TypeError:
             if not is_numeric_dtype(adata.obs[ck]):
                 raise TypeError(
                     f"Expected `adata.obs[{cluster_key!r}]` to be numeric, "
                     f"found `{infer_dtype(adata.obs[cluster_key])}`."
-                )
+                ) from None
             res.append(np.asarray(adata.obs[ck])[order])
 
     return res
```

### Comparing `cellrank-1.5.1/cellrank/settings/_settings.py` & `cellrank-2.0.0/src/cellrank/settings/_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import copy
 import logging
-from copy import copy
 
 from scanpy import settings
-from cellrank.logging._logging import _RootLogger, _LogFormatter
+
+from cellrank.logging._logging import _LogFormatter, _RootLogger
+
+__all__ = ["settings"]
 
 
 def _set_log_file(settings):
     file = settings.logfile
     name = settings.logpath
     root = settings._root_logger
     h = logging.StreamHandler(file) if name is None else logging.FileHandler(name)
@@ -17,13 +20,13 @@
         root.removeHandler(root.handlers[0])
     elif len(root.handlers) > 1:
         raise RuntimeError("CellRank's root logger somehow got more than one handler.")
 
     root.addHandler(h)
 
 
-settings = copy(settings)
+settings = copy.copy(settings)
 settings._root_logger = _RootLogger(settings.verbosity)
 # these 2 lines are necessary to get it working (otherwise no logger is found)
 # this is a hacky way of modifying the logging, in the future, use our own
 _set_log_file(settings)
 settings.verbosity = settings.verbosity
```

### Comparing `cellrank-1.5.1/cellrank/tl/_colors.py` & `cellrank-2.0.0/src/cellrank/_utils/_colors.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-"""Color handling module."""
-
-from typing import Any, List, Tuple, Union, Iterable, Optional, Sequence
-
-from cellrank import logging as logg
+from typing import Any, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
-from pandas import Series, DataFrame, to_numeric
-from scipy.stats import entropy
-from pandas._libs.lib import infer_dtype
-from pandas.core.dtypes.common import is_categorical_dtype
+import pandas as pd
+import scipy.stats as st
+from pandas.api.types import infer_dtype, is_categorical_dtype
 
-from matplotlib import cm
-from matplotlib import colors as mcolors
+from matplotlib import cm, colors
+
+from cellrank import logging as logg
 
 
 def _create_colors(
     base_color: Union[str, Tuple[float, float, float]],
     n: int,
     hue_range: Optional[Tuple[float, float]] = (-0.1, 0.1),
     saturation_range: Optional[Tuple[float, float]] = (-0.3, 0.3),
     value_range: Optional[Tuple[float, float]] = (-0.3, 0.3),
     convert_to_rgb: bool = True,
     as_hex: bool = True,
 ) -> List[Any]:
-    """
-    Create variations of colors from base color.
+    """Create variations of colors from base color.
 
     Parameters
     ----------
     base_color
         Base color which serves as a starting point.
     n
         Number of colors to create.
@@ -46,85 +41,80 @@
     as_hex:
         Whether to return colors as hex string.
 
     Returns
     -------
     List of colors, either as a hex string or an RGB array.
     """
-
-    if not mcolors.is_color_like(base_color):
+    if not colors.is_color_like(base_color):
         raise ValueError("Base color is not color-like.")
     if n <= 0:
         raise ValueError(f"Number of colors must be > 0, found `{n}`.")
 
-    base_color = mcolors.rgb_to_hsv(mcolors.to_rgb(base_color))
+    base_color = colors.rgb_to_hsv(colors.to_rgb(base_color))
 
     if n == 1:
-        colors = [base_color]
+        res = [base_color]
     else:
         n *= 2  # sometimes the colors are too similar, we take every 2nd one
-        colors = np.repeat(base_color[..., np.newaxis], n, axis=1).T
+        res = np.repeat(base_color[..., np.newaxis], n, axis=1).T
 
         for i, r in enumerate((hue_range, saturation_range, value_range)):
             if r is None:
                 continue
             r_low, r_high = sorted(r)
             c = base_color[i]
 
-            colors[:, i] = np.linspace(max(c + r_low, 0), min(c + r_high, 1), n)
+            res[:, i] = np.linspace(max(c + r_low, 0), min(c + r_high, 1), n)
 
     if convert_to_rgb:
-        colors = map(mcolors.hsv_to_rgb, colors)
+        res = [colors.hsv_to_rgb(c) for c in res]
     if as_hex:
-        colors = map(mcolors.to_hex, colors)
+        res = [colors.to_hex(c) for c in res]
 
-    return list(colors)[::2]  # we've created twice as much colors, select every other
+    return res[::2]  # we've created twice as many colors, select every other
 
 
-def _convert_to_hex_colors(colors: Sequence[Any]) -> List[str]:
-    if not all(mcolors.is_color_like(c) for c in colors):
+def _convert_to_hex_colors(cols: Sequence[Any]) -> List[str]:
+    if not all(colors.is_color_like(c) for c in cols):
         raise ValueError("Not all values are color-like.")
 
-    return [mcolors.to_hex(c) for c in colors]
+    return [colors.to_hex(c) for c in cols]
 
 
 def _create_categorical_colors(n_categories: Optional[int] = None):
     from scanpy.plotting.palettes import vega_20_scanpy
 
     cmaps = [
-        mcolors.ListedColormap(vega_20_scanpy),
+        colors.ListedColormap(vega_20_scanpy),
         cm.Accent,
-        mcolors.ListedColormap(np.array(cm.Dark2.colors)[[1, 2, 4, 5, 6]]),
+        colors.ListedColormap(np.array(cm.Dark2.colors)[[1, 2, 4, 5, 6]]),
         cm.Set1,
         cm.Set2,
         cm.Set3,
     ]
     max_cats = sum(c.N for c in cmaps)
 
     if n_categories is None:
         n_categories = max_cats
     if n_categories > max_cats:
-        raise ValueError(
-            f"Number of categories `{n_categories}` exceeded the maximum number of colors `{max_cats}`."
-        )
+        raise ValueError(f"Number of categories `{n_categories}` exceeded the maximum number of colors `{max_cats}`.")
 
-    colors = []
+    res = []
     for cmap in cmaps:
-        colors += [cmap(i) for i in range(cmap.N)][: n_categories - len(colors)]
-        if len(colors) == n_categories:
-            return _convert_to_hex_colors(colors)
+        res += [cmap(i) for i in range(cmap.N)][: n_categories - len(res)]
+        if len(res) == n_categories:
+            return _convert_to_hex_colors(res)
 
     raise RuntimeError(f"Unable to create `{n_categories}` colors.")
 
 
 def _insert_categorical_colors(seen_colors: Union[np.ndarray, List], n_categories: int):
     seen_colors = set(_convert_to_hex_colors(seen_colors))
-    candidates = list(
-        filter(lambda c: c not in seen_colors, _create_categorical_colors())
-    )[:n_categories]
+    candidates = list(filter(lambda c: c not in seen_colors, _create_categorical_colors()))[:n_categories]
 
     if len(candidates) != n_categories:
         raise RuntimeError(f"Unable to create `{n_categories}` categorical colors.")
 
     return candidates
 
 
@@ -132,44 +122,45 @@
     for val in [r, g, b]:
         assert 0 <= val <= 255
 
     return "#000000" if r * 0.299 + g * 0.587 + b * 0.114 > 186 else "#ffffff"
 
 
 def _get_black_or_white(value: float, cmap) -> str:
+    if np.isnan(value):
+        return "#000000"
     if not (0.0 <= value <= 1.0):
         raise ValueError(f"Value must be in range `[0, 1]`, found `{value}`.")
 
     r, g, b, *_ = (int(c * 255) for c in cmap(value))
     return _contrasting_color(r, g, b)
 
 
 def _get_bg_fg_colors(color, sat_scale: Optional[float] = None) -> Tuple[str, str]:
-    if not mcolors.is_color_like(color):
+    if not colors.is_color_like(color):
         raise ValueError(f"Value `{color}` is not color-like.")
 
-    color = np.squeeze(mcolors.to_rgba_array(color, alpha=1))[:3]
+    color = np.squeeze(colors.to_rgba_array(color, alpha=1))[:3]
     if sat_scale is not None:
-        h, s, v = mcolors.rgb_to_hsv(color)
-        color = mcolors.hsv_to_rgb([h, s * sat_scale, v])
+        h, s, v = colors.rgb_to_hsv(color)
+        color = colors.hsv_to_rgb([h, s * sat_scale, v])
 
     return (
-        mcolors.to_hex(color),
+        colors.to_hex(color),
         _contrasting_color(*np.array(color * 255).astype(int)),
     )
 
 
 def _map_names_and_colors(
-    series_reference: Series,
-    series_query: Series,
+    series_reference: pd.Series,
+    series_query: pd.Series,
     colors_reference: Optional[np.array] = None,
     en_cutoff: Optional[float] = None,
-) -> Union[Series, Tuple[Series, List[Any]]]:
-    """
-    Map annotations and colors from one series to another.
+) -> Union[pd.Series, Tuple[pd.Series, List[Any]]]:
+    """Map annotations and colors from one series to another.
 
     Parameters
     ----------
     series_reference
         Series object with categorical annotations.
     series_query
         Series for which we would like to query the category names.
@@ -179,95 +170,82 @@
         In case of a non-perfect overlap between categories of the two series,
         this decides when to label a category in the query as 'Unknown'.
 
     Returns
     -------
     Series with updated category names and a corresponding array of colors.
     """
-
     # checks: dtypes, matching indices, make sure colors match the categories
     if not is_categorical_dtype(series_reference):
-        raise TypeError(
-            f"Reference series must be `categorical`, found `{infer_dtype(series_reference)}`."
-        )
+        raise TypeError(f"Reference series must be `categorical`, found `{infer_dtype(series_reference)}`.")
     if not is_categorical_dtype(series_query):
-        raise TypeError(
-            f"Query series must be `categorical`, found `{infer_dtype(series_query)}`."
-        )
+        raise TypeError(f"Query series must be `categorical`, found `{infer_dtype(series_query)}`.")
     if len(series_reference) != len(series_query):
         raise ValueError(
-            f"Expected the reference and query to have same length,"
+            f"Expected the reference and query to have the same length, "
             f"found `{len(series_reference)}`, `{len(series_query)}`."
         )
 
     if en_cutoff is not None and en_cutoff < 0:
-        raise ValueError(
-            f"Expected entropy cutoff to be non-negative, found `{en_cutoff}`."
-        )
+        raise ValueError(f"Expected entropy cutoff to be non-negative, found `{en_cutoff}`.")
 
     if not np.all(series_reference.index == series_query.index):
         raise ValueError("Series indices do not match, cannot map names and colors.")
 
     process_colors = colors_reference is not None
 
     if not len(series_query):
-        res = Series([], dtype="category")
+        res = pd.Series([], dtype="category")
         return (res, []) if process_colors else res
 
     if process_colors:
         if len(colors_reference) < len(series_reference.cat.categories):
             raise ValueError(
                 f"Length of reference colors `{len(colors_reference)}` is smaller than "
                 f"length of reference categories `{len(series_reference.cat.categories)}`."
             )
         colors_reference = colors_reference[: len(series_reference.cat.categories)]
-        if not all(mcolors.is_color_like(c) for c in colors_reference):
+        if not all(colors.is_color_like(c) for c in colors_reference):
             raise ValueError("Not all values are valid colors.")
         if len(set(colors_reference)) != len(colors_reference):
             logg.warning("Color sequence contains non-unique elements")
 
     # create dataframe to store the associations between reference and query
     cats_query = series_query.cat.categories
     cats_reference = series_reference.cat.categories
-    association_df = DataFrame(None, index=cats_query, columns=cats_reference)
+    association_df = pd.DataFrame(None, index=cats_query, columns=cats_reference)
 
     # populate the dataframe - compute the overlap
     for cl in cats_query:
-        row = [
-            np.sum(series_reference.loc[np.array(series_query == cl)] == key)
-            for key in cats_reference
-        ]
+        row = [np.sum(series_reference.loc[np.array(series_query == cl)] == key) for key in cats_reference]
         association_df.loc[cl] = row
-    association_df = association_df.apply(to_numeric)
+    association_df = association_df.apply(pd.to_numeric)
 
     # find the mapping which maximizes overlap
     names_query = association_df.T.idxmax()
     if en_cutoff is not None:
-        association_df["entropy"] = entropy(association_df.T)
+        association_df["entropy"] = st.entropy(association_df.T)
     association_df["name"] = names_query
 
     # assign query colors
     if process_colors:
         association_df["color"] = colors_query = [
-            colors_reference[np.where(cats_reference == name)[0][0]]
-            for name in names_query
+            colors_reference[np.where(cats_reference == name)[0][0]] for name in names_query
         ]
 
     # next, we need to make sure that we have unique names and colors. In a first step, compute how many repetitions
     # we have
-    names_query_series = Series(names_query, dtype="category")
-    frequ = {
-        key: np.sum(names_query == key) for key in names_query_series.cat.categories
-    }
+    names_query_series = pd.Series(names_query, dtype="category")
+    frequ = {key: np.sum(names_query == key) for key in names_query_series.cat.categories}
 
     # warning: do NOT use np.array - if I pass for e.g. colors ['red'], the dtype will be '<U3'
     # but _create_colors convert them to hex, which will leave them trimmed to #ff or similar
-    names_query_new = Series(names_query.copy())
+    names_query_new = pd.Series(names_query.copy())
     if process_colors:
-        colors_query_new = Series(colors_query.copy())
+        colors_query_new = pd.Series(colors_query.copy())
 
     # Create unique names by adding suffixes "..._1, ..._2" etc and unique colors by shifting the original color
     for key, value in frequ.items():
         if value == 1:
             continue  # already unique, skip
         # deal with non-unique names
         unique_names = [f"{key}_{rep}" for rep in np.arange(1, value + 1)]
@@ -281,82 +259,22 @@
     # warnings: if it's categorical and assigning to `.cat.categories`, it will
     # take the categorical information, making the 2nd line below necessary
     names_query_new = names_query_new.astype("category")
     names_query_new = names_query_new.cat.reorder_categories(np.array(names_query_new))
 
     # issue a warning for mapping with high entropy
     if en_cutoff is not None:
-        critical_cats = sorted(
-            set(
-                association_df.loc[association_df["entropy"] > en_cutoff, "name"].values
-            )
-        )
+        critical_cats = sorted(set(association_df.loc[association_df["entropy"] > en_cutoff, "name"].values))
         if len(critical_cats) > 0:
-            logg.warning(
-                f"The following states could not be mapped uniquely: `{critical_cats}`"
-            )
+            logg.warning(f"The following states could not be mapped uniquely: `{critical_cats}`")
 
-    return (
-        (names_query_new, list(_convert_to_hex_colors(colors_query_new)))
-        if process_colors
-        else names_query_new
-    )
+    return (names_query_new, list(_convert_to_hex_colors(colors_query_new))) if process_colors else names_query_new
 
 
-def _compute_mean_color(color_list: List[str]) -> str:
+def _compute_mean_color(cols: List[str]) -> str:
     """Compute mean color."""
+    if not all(colors.is_color_like(c) for c in cols):
+        raise ValueError(f"Not all values are valid colors `{cols}`.")
 
-    if not all(map(lambda c: mcolors.is_color_like(c), color_list)):
-        raise ValueError(f"Not all values are valid colors `{color_list}`.")
-
-    color_list = np.array([mcolors.rgb_to_hsv(mcolors.to_rgb(c)) for c in color_list])
-
-    return mcolors.to_hex(mcolors.hsv_to_rgb(np.mean(color_list, axis=0)))
-
-
-def _colors_in_order(
-    adata,
-    clusters: Optional[Iterable[str]] = None,
-    cluster_key: str = "clusters",
-) -> List[Any]:
-    """
-    Get list of colors from AnnData in defined order.
-
-    Extracts a list of colors from ``adata.uns[cluster_key]`` in the order defined by the ``clusters``.
-
-    Parameters
-    ----------
-    %(adata)s
-    clusters
-        Subset of the clusters we want the color for. Must be a subset of ``adata.obs[cluster_key].cat.categories``.
-    cluster_key
-        Key from ``adata.obs``.
-
-    Returns
-    -------
-    List of colors in order defined by `clusters`.
-    """
-
-    assert (
-        cluster_key in adata.obs.keys()
-    ), f"Could not find {cluster_key} in `adata.obs`."
-
-    if clusters is not None:
-        assert np.all(
-            np.in1d(clusters, adata.obs[cluster_key].cat.categories)
-        ), "Not all `clusters` found."
-
-    assert (
-        f"{cluster_key}_colors" in adata.uns.keys()
-    ), f"No colors associated to {cluster_key} in `adata.uns`."
-
-    if clusters is None:
-        clusters = adata.obs[cluster_key].cat.categories
-
-    color_list = []
-    all_clusters = adata.obs[cluster_key].cat.categories
-
-    for cl in clusters:
-        mask = np.in1d(all_clusters, cl)
-        color_list.append(adata.uns[f"{cluster_key}_colors"][mask][0])
+    cols = np.array([colors.rgb_to_hsv(colors.to_rgb(c)) for c in cols])
 
-    return color_list
+    return colors.to_hex(colors.hsv_to_rgb(np.mean(cols, axis=0)))
```

### Comparing `cellrank-1.5.1/cellrank/tl/_enum.py` & `cellrank-2.0.0/src/cellrank/_utils/_enum.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Dict, Type, Tuple, Callable
-from typing_extensions import Literal
+import abc
+import enum
+import functools
+from typing import Any, Callable, Dict, Literal, Tuple, Type
 
-from abc import ABC, ABCMeta
-from enum import Enum, EnumMeta
-from functools import wraps
+__all__ = ["ModeEnum", "DEFAULT_BACKEND"]
 
-_DEFAULT_BACKEND = "loky"
+DEFAULT_BACKEND = "loky"
 Backend_t = Literal["loky", "multiprocessing", "threading"]
 
 
-class PrettyEnum(Enum):
+class PrettyEnum(enum.Enum):
     """Enum with a pretty :meth:`__str__` and :meth:`__repr__`."""
 
     @property
     def v(self) -> Any:
         """Alias for :attr`value`."""
         return self.value
 
@@ -21,55 +21,48 @@
         return f"{self.value!r}"
 
     def __str__(self) -> str:
         return f"{self.value!s}"
 
 
 def _pretty_raise_enum(cls: Type["ErrorFormatterABC"], func: Callable) -> Callable:
-    @wraps(func)
+    @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> "ErrorFormatterABC":
         try:
             return func(*args, **kwargs)
         except ValueError as e:
             _cls, value, *_ = args
             e.args = (cls._format(value),)
             raise e
 
     if not issubclass(cls, ErrorFormatterABC):
         raise TypeError(f"Class `{cls}` must be subtype of `ErrorFormatterABC`.")
-    elif not len(cls.__members__):
+    if not len(cls.__members__):
         # empty enum, for class hierarchy
         return func
 
     return wrapper
 
 
-class ABCEnumMeta(EnumMeta, ABCMeta):  # noqa: D101
+class ABCEnumMeta(enum.EnumMeta, abc.ABCMeta):  # noqa: D101
     def __call__(cls, *args, **kwargs):  # noqa
         if getattr(cls, "__error_format__", None) is None:
-            raise TypeError(
-                f"Can't instantiate class `{cls.__name__}` "
-                f"without `__error_format__` class attribute."
-            )
+            raise TypeError(f"Can't instantiate class `{cls.__name__}` " f"without `__error_format__` class attribute.")
         return super().__call__(*args, **kwargs)
 
-    def __new__(  # noqa: D102
-        cls, clsname: str, superclasses: Tuple[type], attributedict: Dict[str, Any]
-    ):
+    def __new__(cls, clsname: str, superclasses: Tuple[type], attributedict: Dict[str, Any]):  # noqa: D102
         res = super().__new__(cls, clsname, superclasses, attributedict)
         res.__new__ = _pretty_raise_enum(res, res.__new__)
         return res
 
 
-class ErrorFormatterABC(ABC):  # noqa: D101
+class ErrorFormatterABC(abc.ABC):  # noqa: D101
     __error_format__ = "Invalid option `{!r}` for `{}`. Valid options are: `{}`."
 
     @classmethod
     def _format(cls, value) -> str:
-        return cls.__error_format__.format(
-            value, cls.__name__, [m.value for m in cls.__members__.values()]
-        )
+        return cls.__error_format__.format(value, cls.__name__, [m.value for m in cls.__members__.values()])
 
 
 class ModeEnum(str, ErrorFormatterABC, PrettyEnum, metaclass=ABCEnumMeta):  # noqa: D101
     def _generate_next_value_(self, start, count, last_values):
         return str(self).lower()
```

### Comparing `cellrank-1.5.1/cellrank/tl/_lineage.py` & `cellrank-2.0.0/src/cellrank/_utils/_lineage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,114 @@
-from typing import List, Tuple, Union, Mapping, TypeVar, Callable, Iterable, Optional
-from typing_extensions import Literal
+import copy as copy_
+import enum
+import functools
+import inspect
+import itertools
+import pathlib
+import types
+from typing import (
+    Any,
+    Callable,
+    Iterable,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
-from copy import copy
-from enum import auto
-from types import FunctionType, MappingProxyType
-from inspect import signature
-from pathlib import Path
-from functools import wraps
-from itertools import combinations
+import numpy as np
+import pandas as pd
+import scipy.stats as st
+from pandas.api.types import infer_dtype, is_categorical_dtype
+
+import matplotlib.pyplot as plt
+from matplotlib import colors
 
 from anndata import AnnData
+from anndata._io.specs.methods import H5Group, ZarrGroup, write_basic
+from anndata._io.specs.registry import _REGISTRY, IOSpec
+
 from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d, inject_docs
-from cellrank.tl._utils import save_fig, _convert_lineage_name, _unique_order_preserving
-from cellrank.tl._colors import (
-    _get_bg_fg_colors,
+from cellrank._utils._colors import (
     _compute_mean_color,
     _create_categorical_colors,
+    _get_bg_fg_colors,
 )
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._key import Key
 
-import numpy as np
-import pandas as pd
-from scipy.stats import entropy
-from pandas.api.types import infer_dtype, is_categorical_dtype
-
-import matplotlib.colors as c
-import matplotlib.pyplot as plt
+__all__ = ["Lineage", "LineageView"]
 
 ColorLike = TypeVar("ColorLike")
 _ERROR_NOT_ITERABLE = "Expected `{}` to be iterable, found type `{}`."
 _ERROR_WRONG_SIZE = "Expected `{}` to be of size `{{}}`, found `{{}}`."
 
 _HT_CELLS = 10  # head and tail cells to show
 _HTML_REPR_THRESH = 100
 _DUMMY_CELL = "<td style='text-align: right;'>...</td>"
 _ORDER = "C"
 
 
 class PrimingDegree(ModeEnum):  # noqa: D101
-    KL_DIVERGENCE = auto()
-    ENTROPY = auto()
-
-
-class Lin(ModeEnum):  # noqa: D101
-    REST = auto()
-    OTHERS = auto()
+    KL_DIVERGENCE = enum.auto()
+    ENTROPY = enum.auto()
 
 
 class DistanceMeasure(ModeEnum):  # noqa: D101
-    COSINE_SIM = auto()
-    WASSERSTEIN_DIST = auto()
-    KL_DIV = auto()
-    JS_DIV = auto()
-    MUTUAL_INFO = auto()
-    EQUAL = auto()
+    COSINE_SIM = enum.auto()
+    WASSERSTEIN_DIST = enum.auto()
+    KL_DIV = enum.auto()
+    JS_DIV = enum.auto()
+    MUTUAL_INFO = enum.auto()
+    EQUAL = enum.auto()
 
 
 class NormWeights(ModeEnum):  # noqa: D101
-    SCALE = auto()
-    SOFTMAX = auto()
+    SCALE = enum.auto()
+    SOFTMAX = enum.auto()
 
 
 class Reduction(ModeEnum):  # noqa: D101
-    DIST = auto()
-    SCALE = auto()
+    DIST = enum.auto()
+    SCALE = enum.auto()
 
 
 class LinKind(ModeEnum):  # noqa: D101
-    MACROSTATES = auto()
-    TERM_STATES = auto()
-    ABS_PROBS = auto()
+    MACROSTATES = enum.auto()
+    TERM_STATES = enum.auto()
+    FATE_PROBS = enum.auto()
 
 
 def _at_least_2d(array: np.ndarray, dim: int):
     return np.expand_dims(array, dim) if array.ndim < 2 else array
 
 
 def wrap(numpy_func: Callable) -> Callable:
-    """
-    Wrap an numpy function.
+    """Wrap a :mod:`numpy` function.
 
     Modifies functionality of some function (e.g. ignoring `.squeeze`, retaining dimensions).
 
     Parameters
     ----------
     numpy_func
         Function to be wrapped.
 
     Returns
     -------
-    Wrapped function which takes a :class:`cellrank.tl.Lineage` and return :class:`cellrank.tl.Lineage`.
+    Wrapped function which takes a :class:`cellrank.Lineage` and return :class:`cellrank.Lineage`.
     """
 
-    @wraps(numpy_func)
+    @functools.wraps(numpy_func)
     def decorator(array, *args, **kwargs):
         if not isinstance(array, Lineage):
-            raise TypeError(
-                f"Expected array to be of type `Lineage`, found `{type(array).__name__}`."
-            )
+            raise TypeError(f"Expected array to be of type `Lineage`, found `{type(array).__name__}`.")
         if fname == "squeeze":
             return array
         if fname == "array_repr":
             return repr(array)
 
         if "axis" in kwargs:
             axis = kwargs["axis"]
@@ -135,141 +140,128 @@
             lin = Lineage(
                 res,
                 names=[f"{fname} of {', '.join(array.names)}"],
                 colors=["grey"],
             )
 
         if res.shape[1] == array.shape[1 - is_t]:
-            lin = Lineage(
-                res, names=[f"{fname} of {n}" for n in array.names], colors=array.colors
-            )
+            lin = Lineage(res, names=[f"{fname} of {n}" for n in array.names], colors=array.colors)
 
         if lin is not None:
             return lin.T if is_t else lin
 
         raise RuntimeError(
-            f"Unable to interpret result of function `{fname}` called "
-            f"with args `{args}`, kwargs: `{kwargs}`."
+            f"Unable to interpret result of function `{fname}` called " f"with args `{args}`, kwargs: `{kwargs}`."
         )
 
-    params = signature(numpy_func).parameters
+    params = inspect.signature(numpy_func).parameters
     if "axis" in params:
         axis_ix = list(params.keys()).index("axis") - 1
         default_axis = params["axis"].default
     else:
         axis_ix = 256
         default_axis = None
-    assert (
-        axis_ix >= 0
-    ), f"Expected argument `'axis'` not to be first for function `{numpy_func.__name__}`."
+    assert axis_ix >= 0, f"Expected argument `'axis'` not to be first for function `{numpy_func.__name__}`."
 
     fname = numpy_func.__name__
     if fname == "amin":
         fname = "min"
     elif fname == "amax":
         fname = "max"
 
     return decorator
 
 
 def _register_handled_functions():
     handled_fns = {}
-
     for attrname in dir(np):
         fn = getattr(np, attrname)
-        if isinstance(fn, FunctionType):
+        if isinstance(fn, types.FunctionType):
             try:
-                sig = signature(fn)
-                if "axis" in sig.parameters.keys():
+                sig = inspect.signature(fn)
+                if "axis" in sig.parameters:
                     handled_fns[fn] = wrap(fn)
             except ValueError:
                 pass
 
     handled_fns.pop(np.expand_dims, None)
 
     handled_fns[np.allclose] = wrap(np.allclose)
     handled_fns[np.array_repr] = wrap(np.array_repr)
-    handled_fns[entropy] = wrap(entropy)  # qol change
+    handled_fns[st.entropy] = wrap(st.entropy)  # qol change
 
     return handled_fns
 
 
 _HANDLED_FUNCTIONS = _register_handled_functions()
 
 
 class LineageMeta(type):
-    """
-    Metaclass for Lineaage.
+    """Metaclass for Lineage.
 
-    Registers functions which are handled by us and overloads common attributes, such as `.sum` with these functions.
+    It registers functions which are handled by us and overloads common attributes, such as `.sum` with these functions.
     """
 
     __overloaded_functions__ = dict(  # noqa
         sum=np.sum,
         mean=np.mean,
         min=np.min,
         argmin=np.argmin,
         max=np.max,
         argmax=np.argmax,
         std=np.std,
         var=np.var,
         sort=np.sort,
         squeeze=np.squeeze,
-        entropy=entropy,
+        entropy=st.entropy,
     )
 
     def __new__(cls, clsname, superclasses, attributedict):  # noqa
         res = type.__new__(cls, clsname, superclasses, attributedict)
         for attrname, fn in LineageMeta.__overloaded_functions__.items():
             wrapped_fn = _HANDLED_FUNCTIONS.get(fn, None)
             if wrapped_fn:
                 setattr(res, attrname, wrapped_fn)
 
         return res
 
 
 class Lineage(np.ndarray, metaclass=LineageMeta):
-    """
-    Lightweight :class:`numpy.ndarray` wrapper that adds names and colors.
+    """Lightweight :class:`~numpy.ndarray` wrapper that adds names and colors.
 
     Parameters
     ----------
     input_array
-        Input array containing lineage probabilities, each lineage being stored in a column.
+        Input array containing lineage probabilities stored in columns.
     names
-        Names of the lineages.
+        Lineage names.
     colors
-        Colors of the lineages.
+        Lineage colors.
     """
 
     def __new__(
         cls,
         input_array: np.ndarray,
         *,
         names: Iterable[str],
         colors: Optional[Iterable[ColorLike]] = None,
     ) -> "Lineage":
         """Create and return a new object."""
-
         if not isinstance(input_array, np.ndarray):
-            raise TypeError(
-                f"Input array must be of type `numpy.ndarray`, found `{type(input_array).__name__!r}`."
-            )
+            raise TypeError(f"Input array must be of type `numpy.ndarray`, found `{type(input_array).__name__!r}`.")
 
         if input_array.ndim == 1:
             input_array = np.expand_dims(input_array, -1)
         elif input_array.ndim > 2:
-            raise ValueError(
-                f"Input array must be 2-dimensional, found `{input_array.ndim}`."
-            )
+            raise ValueError(f"Input array must be 2-dimensional, found `{input_array.ndim}`.")
 
-        if input_array.shape[0] == 0:
-            raise ValueError("Expected number cells to be at least 1, found 0.")
-        if input_array.shape[1] == 0:
-            raise ValueError("Expected number of lineages to be at least 1, found 0.")
+        if not input_array.shape[0]:
+            raise ValueError("Expected number cells to be at least `1`, found `0`.")
+        if not input_array.shape[1]:
+            raise ValueError("Expected number of lineages to be at least `1`, found `0`.")
 
         obj = np.array(input_array, copy=True).view(cls)
         obj._n_lineages = obj.shape[1]
         obj._is_transposed = False
         obj.names = names  # these always create a copy, which is a good thing
         obj.colors = colors
 
@@ -283,577 +275,330 @@
         if _names is not None:
             self._names = _names
             self._n_lineages = len(_names)
             self._names_to_ixs = {n: i for i, n in enumerate(self.names)}
         else:
             self._names = None
             self._names_to_ixs = None
-            self._n_lineages = getattr(
-                obj, "_n_lineages", obj.shape[1] if obj.ndim == 2 else 0
-            )
+            self._n_lineages = getattr(obj, "_n_lineages", obj.shape[1] if obj.ndim == 2 else 0)
 
         self._colors = getattr(obj, "colors", None)
         self._is_transposed = getattr(obj, "_is_transposed", False)
 
-    def _mixer(self, rows, mixtures):
-        def update_entries(key):
-            if key:
-                res.append(self[rows, key].X.sum(1))
-                # item = (key, rows) if self._is_transposed else (rows, key)
-                # res.append(self[item].X.sum(int(not self._is_transposed)))
-                names.append(" or ".join(self.names[key]))
-                colors.append(_compute_mean_color(self.colors[key]))
+    def __array_function__(self, func, types, args, kwargs):
+        if func not in _HANDLED_FUNCTIONS:
+            return NotImplemented
+        # Note: this allows subclasses that don't override
+        # __array_function__ to handle MyArray objects
+        if not all(issubclass(t, type(self)) for t in types):
+            return NotImplemented
 
-        lin_kind = [_ for _ in mixtures if isinstance(_, Lin)]
-        if len(lin_kind) > 1:
-            raise ValueError(
-                f"`Lin` enum is allowed only once in the expression, found `{len(lin_kind)}`."
-            )
+        return _HANDLED_FUNCTIONS[func](*args, **kwargs)
+
+    def __getitem__(self, item) -> "Lineage":
+        was_transposed = False
+        if self._is_transposed:
+            was_transposed = True
+            self = self.T
+            if isinstance(item, tuple):
+                item = item[::-1]
+
+        obj = self.__getitem(item)
+
+        return obj.T if was_transposed else obj
+
+    def _mix_lineages(self, rows, mixtures: Iterable[Union[str, Any]]) -> "Lineage":
+        from cellrank._utils._utils import _unique_order_preserving
+
+        def unsplit(names: str) -> Tuple[str, ...]:
+            return tuple(sorted({name.strip(" ") for name in names.strip(" ,").split(",")}))
 
         keys = [
-            tuple(
-                self._maybe_convert_names(
-                    _convert_lineage_name(mixture), default=mixture
-                )
-            )
+            tuple(self._maybe_convert_names(unsplit(mixture), default=mixture))
             if isinstance(mixture, str)
             else (mixture,)
             for mixture in mixtures
-            if not (isinstance(mixture, Lin))
         ]
         keys = _unique_order_preserving(keys)
 
         # check the `keys` are unique
         overlap = [set(ks) for ks in keys]
-        for c1, c2 in combinations(overlap, 2):
+        for c1, c2 in itertools.combinations(overlap, 2):
             overlap = c1 & c2
             if overlap:
-                raise ValueError(
-                    f"Found overlapping keys: `{self.names[list(overlap)]}`."
-                )
+                raise ValueError(f"Found overlapping keys: `{self.names[list(overlap)]}`.")
 
-        seen = set()
         names, colors, res = [], [], []
         for key in map(list, keys):
-            seen.update(self.names[key])
-            update_entries(key)
-
-        if len(lin_kind) == 1:
-            lin_kind = lin_kind[0]
-            keys = [i for i, n in enumerate(self.names) if n not in seen]
-
-            if lin_kind == Lin.OTHERS:
-                for key in keys:
-                    update_entries([key])
-            elif lin_kind == Lin.REST:
-                update_entries(keys)
-                if keys:
-                    names[-1] = str(lin_kind)
-            else:
-                raise NotImplementedError(
-                    f"Mixing `{lin_kind}` is not yet implemented."
-                )
-
-        res = np.stack(res, axis=-1)
-        return Lineage(res, names=names, colors=colors)
-
-    def __getitem__(self, item) -> "Lineage":
-        was_transposed = False
-        if self._is_transposed:
-            was_transposed = True
-            self = self.T
-            if isinstance(item, tuple):
-                item = item[::-1]
-
-        obj = self.__getitem(item)
+            if key:
+                res.append(self[rows, key].X.sum(1))
+                names.append(", ".join(self.names[key]))
+                colors.append(_compute_mean_color(self.colors[key]))
 
-        return obj.T if was_transposed else obj
+        return Lineage(np.stack(res, axis=-1), names=names, colors=colors)
 
     def __getitem(self, item):
         if isinstance(item, tuple):
             if len(item) > 2:
-                raise ValueError(
-                    f"Expected key to be of length `2`, found `{len(item)}`."
-                )
+                raise ValueError(f"Expected key to be of length `2`, found `{len(item)}`.")
 
             item = list(item)
             if item[0] is Ellipsis or item[0] is None:
                 item[0] = range(self.shape[0])
             if len(item) == 2 and (item[1] is Ellipsis or item[1] is None):
                 item[1] = range(self.shape[1])
             item = tuple(item)
 
         is_tuple_len_2 = (
             isinstance(item, tuple)
             and len(item) == 2
-            and isinstance(
-                item[0], (int, np.integer, range, slice, tuple, list, np.ndarray)
-            )
+            and isinstance(item[0], (int, np.integer, range, slice, tuple, list, np.ndarray))
         )
         if is_tuple_len_2:
             rows, col = item
-
             if isinstance(col, (int, np.integer, str)):
                 col = [col]
-
             try:
                 # slicing an array where row/col are like 2D indices
                 if 1 < len(col) == len(rows) and len(rows) == self.shape[0]:
                     col = self._maybe_convert_names(col, make_unique=False)
                     return Lineage(
                         # never remove this expand_dims - it's critical
                         np.expand_dims(self.X[rows, col], axis=-1),
                         names=["mixture"],
                         colors=["#000000"],
                     )
             except TypeError:  # because of range
                 pass
 
             if isinstance(col, (list, tuple, np.ndarray)):
-                if any(
-                    map(
-                        lambda i: isinstance(i, Lin)
-                        or (isinstance(i, str) and ("," in i or "or" in i)),
-                        col,
-                    )
-                ):
-                    return self._mixer(rows, col)
+                if any(isinstance(i, str) and "," in i for i in col):
+                    return self._mix_lineages(rows, col)
                 col = self._maybe_convert_names(col)
                 item = rows, col
         else:
             if isinstance(item, (int, np.integer, str)):
                 item = [item]
-
             col = range(len(self.names))
             if isinstance(item, (tuple, list, np.ndarray)):
-                if any(
-                    map(
-                        lambda i: isinstance(i, Lin)
-                        or (isinstance(i, str) and ("," in i or "or" in i)),
-                        item,
-                    )
-                ):
-                    return self._mixer(slice(None, None, None), item)
-                elif any(map(lambda i: isinstance(i, str), item)):
+                if any(isinstance(i, str) and "," in i for i in item):
+                    return self._mix_lineages(slice(None, None, None), item)
+                if any(isinstance(i, str) for i in item):
                     item = (slice(None, None, None), self._maybe_convert_names(item))
                     col = item[1]
 
         shape, row_order, col_order = None, None, None
-        if (
-            is_tuple_len_2
-            and not isinstance(item[0], slice)
-            and not isinstance(item[1], slice)
-        ):
-            item_0 = (
-                np.array(item[0]) if not isinstance(item[0], np.ndarray) else item[0]
-            )
-            item_1 = (
-                np.array(item[1]) if not isinstance(item[1], np.ndarray) else item[1]
-            )
+        if is_tuple_len_2 and not isinstance(item[0], slice) and not isinstance(item[1], slice):
+            item_0 = np.array(item[0]) if not isinstance(item[0], np.ndarray) else item[0]
+            item_1 = np.array(item[1]) if not isinstance(item[1], np.ndarray) else item[1]
             item_0 = _at_least_2d(item_0, -1)
             item_1 = _at_least_2d(item_1, 0)
 
+            # handle boolean indexing
             if item_1.dtype == bool:
                 if item_0.dtype != bool:
                     if not issubclass(item_0.dtype.type, np.integer):
                         raise TypeError(f"Invalid type `{item_0.dtype.type}`.")
                     row_order = (
-                        item_0[:, 0]
-                        if item_0.shape[0] == self.shape[0]
-                        else np.argsort(np.argsort(item_0[:, 0]))
+                        item_0[:, 0] if item_0.shape[0] == self.shape[0] else np.argsort(np.argsort(item_0[:, 0]))
                     )
                     item_0 = _at_least_2d(np.isin(np.arange(self.shape[0]), item_0), -1)
                 item = item_0 * item_1
                 shape = np.max(np.sum(item, axis=0)), np.max(np.sum(item, axis=1))
                 col = np.where(np.all(item_1, axis=0))[0]
             elif item_0.dtype == bool:
                 if item_1.dtype != bool:
                     if not issubclass(item_1.dtype.type, np.integer):
                         raise TypeError(f"Invalid type `{item_1.dtype.type}`.")
                     col_order = (
-                        item_1[0, :]
-                        if item_1.shape[1] == self.shape[1]
-                        else np.argsort(np.argsort(item_1[0, :]))
+                        item_1[0, :] if item_1.shape[1] == self.shape[1] else np.argsort(np.argsort(item_1[0, :]))
                     )
                     item_1 = _at_least_2d(np.isin(np.arange(self.shape[1]), item_1), 0)
 
                 item = item_0 * item_1
                 shape = np.max(np.sum(item, axis=0)), np.max(np.sum(item, axis=1))
                 col = np.where(np.all(item_1, axis=0))[0]
             else:
+                # defer to numpy
                 item = (item_0, item_1)
 
         obj = super().__getitem__(item)
 
-        if shape is not None:  # keep the resulting shape
+        # keep the resulting shape
+        if shape is not None:
             obj = obj.reshape(shape)
+        # correctly reorder
         if row_order is not None:
             obj = obj[row_order, :]
         if col_order is not None:
             obj = obj[:, col_order]
 
+        # correctly set names and colors
         if isinstance(obj, Lineage):
             obj._names = np.atleast_1d(self.names[col])
             obj._colors = np.atleast_1d(self.colors[col])
             if col_order is not None:
                 obj._names = obj._names[col_order]
                 obj._colors = obj._colors[col_order]
             obj._names_to_ixs = {name: i for i, name in enumerate(obj._names)}
 
         return obj
 
-    def __array_function__(self, func, types, args, kwargs):
-        if func not in _HANDLED_FUNCTIONS:
-            return NotImplemented
-        # Note: this allows subclasses that don't override
-        # __array_function__ to handle MyArray objects
-        if not all(issubclass(t, type(self)) for t in types):
-            return NotImplemented
-
-        return _HANDLED_FUNCTIONS[func](*args, **kwargs)
-
     @property
     def names(self) -> np.ndarray:
-        """Lineage names. Must be unique."""
+        """Lineage names."""
         return self._names
 
     @names.setter
-    def names(self, value: Iterable[str]):
+    def names(self, value: Iterable[str]) -> None:
         if not isinstance(value, Iterable):
             raise TypeError(_ERROR_NOT_ITERABLE.format("names", type(value).__name__))
 
-        value = [v if isinstance(v, str) else str(v) for v in value]
-        value = self._check_shape(value, _ERROR_WRONG_SIZE.format("names"))
+        value = [str(v) for v in value]
+        value = self._check_axis1_shape(value, _ERROR_WRONG_SIZE.format("names"))
 
         if len(set(value)) != len(value):
             raise ValueError(f"Not all lineage names are unique: `{value}`.")
 
         self._names = self._prepare_annotation(value)
         self._names_to_ixs = {name: ix for ix, name in enumerate(self.names)}
 
     @property
     def colors(self) -> np.ndarray:
         """Lineage colors."""
         return self._colors
 
     @colors.setter
-    def colors(self, value: Optional[Iterable[ColorLike]]):
+    def colors(self, value: Optional[Iterable[ColorLike]]) -> None:
         if value is None:
             value = _create_categorical_colors(self._n_lineages)
         elif not isinstance(value, Iterable):
             raise TypeError(_ERROR_NOT_ITERABLE.format("colors", type(value).__name__))
 
-        value = self._check_shape(value, _ERROR_WRONG_SIZE.format("colors"))
+        value = self._check_axis1_shape(value, _ERROR_WRONG_SIZE.format("colors"))
         self._colors = self._prepare_annotation(
             value,
-            checker=c.is_color_like,
-            transformer=c.to_hex,
+            checker=colors.is_color_like,
+            transformer=colors.to_hex,
             checker_msg="Value `{}` is not a valid color.",
         )
 
-    def _maybe_convert_names(
-        self,
-        names: Iterable[Union[int, str, bool]],
-        is_singleton: bool = False,
-        default: Optional[Union[int, str]] = None,
-        make_unique: bool = True,
-    ) -> Union[int, List[int], List[bool]]:
-        if all(map(lambda n: isinstance(n, (bool, np.bool_)), names)):
-            return list(names)
-        res = []
-        for name in names:
-            if isinstance(name, str):
-                if name in self._names_to_ixs:
-                    name = self._names_to_ixs[name]
-                elif default is not None:
-                    if isinstance(default, str):
-                        if default not in self._names_to_ixs:
-                            raise KeyError(
-                                f"Invalid lineage name: `{name}`. "
-                                f"Valid names are: `{list(self.names)}`."
-                            )
-                        name = self._names_to_ixs[default]
-                    else:
-                        name = default
-                else:
-                    raise KeyError(
-                        f"Invalid lineage name `{name}`. "
-                        f"Valid names are: `{list(self.names)}`."
-                    )
-            res.append(name)
-
-        if make_unique:
-            res = _unique_order_preserving(res)
-
-        return res[0] if is_singleton else res
-
-    def _check_shape(
-        self, array: Iterable[Union[str, ColorLike]], msg: str
-    ) -> List[Union[str, ColorLike]]:
-        array = list(array)
-        if len(array) != self._n_lineages:
-            raise ValueError(msg.format(self._n_lineages, len(array)))
-
-        return array
-
-    def _prepare_annotation(
-        self,
-        array: List[str],
-        checker: Optional[Callable] = None,
-        transformer: Optional[Callable] = None,
-        checker_msg: Optional[str] = None,
-    ) -> np.ndarray:
-        if checker:
-            assert checker_msg, "Please provide a message when `checker` is not `None`."
-            for v in array:
-                if not checker(v):
-                    raise ValueError(checker_msg.format(v))
-
-        if transformer is not None:
-            array = np.array([transformer(v) for v in array])
-
-        return np.array(array)
-
     @property
     def X(self) -> np.ndarray:
-        """Convert self to numpy array, losing names and colors."""
+        """Convert self to an array."""
         return np.array(self, copy=False)
 
     @property
     def T(self):
         """Transpose of self."""
         obj = self.transpose()
         obj._is_transposed = not self._is_transposed
         return obj
 
-    def view(self, dtype=None, type=None) -> "LineageView":
-        """Return a view of self."""
-        return LineageView(self)
-
-    def __repr__(self) -> str:
-        return f'{super().__repr__()[:-1]},\n  names([{", ".join(self.names)}]))'
-
-    def __str__(self):
-        return f'{super().__str__()}\n names=[{", ".join(self.names)}]'
-
     @property
-    def _fmt(self) -> Callable:
-        if np.issubdtype(self.dtype, float):
-            return "{:.06f}".format
-        return "{}".format
-
-    def _repr_html_(self) -> str:
-        def format_row(r):
-            rng = (
-                range(self.shape[1])
-                if not self._is_transposed
-                or (self._is_transposed and self.shape[1] <= _HTML_REPR_THRESH)
-                else list(range(_HT_CELLS))
-                + [...]
-                + list(range(self.shape[1] - _HT_CELLS - 1, self.shape[1] - 1))
-            )
-
-            cells = "".join(
-                f"<td style='text-align: right;'>" f"{self._fmt(self.X[r, c])}" f"</td>"
-                if isinstance(c, int)
-                else _DUMMY_CELL
-                for c in rng
-            )
-            return f"<tr>{(names[r] if self._is_transposed else '') + cells}</tr>"
-
-        def dummy_row():
-            values = "".join(_DUMMY_CELL for _ in range(self.shape[1]))
-            return f"<tr>{values}</tr>"
-
-        if self.names is None or self.colors is None:
-            raise RuntimeError(
-                f"Name or colors are `None`. This can happen when running `array.view({type(self).__name__}`."
-            )
-
-        if self.ndim != 2:
-            return repr(self)
-
-        styles = [
-            f"'background-color: {bg}; color: {fg}; text-align: center; word-wrap: break-word; max-width: 100px'"
-            for bg, fg in map(_get_bg_fg_colors, self.colors)
-        ]
-        names = [f"<th style={style}>{n}</th>" for n, style in zip(self.names, styles)]
-        header = f"<tr>{''.join(names)}</tr>"
-
-        if self.shape[0] > _HTML_REPR_THRESH:
-            body = "".join(format_row(i) for i in range(_HT_CELLS))
-            body += dummy_row()
-            body += "".join(
-                format_row(i)
-                for i in range(self.shape[0] - _HT_CELLS - 1, self.shape[0] - 1)
-            )
-        else:
-            body = "".join(format_row(i) for i in range(self.shape[0]))
-
-        cells = "cells" if self.shape[0] > 1 else "cell"
-        lineages = "lineages" if self.shape[1] > 1 else "lineage"
-        if self._is_transposed:
-            cells, lineages = lineages, cells
-        metadata = f"<p>{self.shape[0]} {cells} x {self.shape[1]} {lineages}</p>"
-
-        if self._is_transposed:
-            header = ""
-        return (
-            f"<div style='scoped' class='rendered_html'>"
-            f"<table class='dataframe'>{header}{body}</table>{metadata}"
-            f"</div>"
-        )
-
-    def __format__(self, format_spec):
-        if self.shape == (1, 1):
-            return format_spec.format(self.X[0, 0])
-        if self.shape == (1,):
-            return format_spec.format(self.X[0])
-        return NotImplemented
-
-    def __setstate__(self, state):
-        *state, names, colors, is_t = state
-        names = names[-1]
-        colors = colors[-1]
-
-        self._names = np.empty(names[1])
-        self._colors = np.empty(colors[1])
-
-        super().__setstate__(tuple(state))
-        self._names.__setstate__(tuple(names))
-        self._colors.__setstate__(tuple(colors))
-
-        self._is_transposed = is_t
-        self._n_lineages = len(self.names)
-        self._names_to_ixs = {name: ix for ix, name in enumerate(self.names)}
-
-    def __reduce__(self):
-        res = list(super().__reduce__())
-
-        names = self.names.__reduce__()
-        colors = self.colors.__reduce__()
-        res[-1] += (names, colors, self._is_transposed)
-
-        return tuple(res)
-
-    def copy(self, _="C") -> "Lineage":
-        """Return a copy of itself."""
-        obj = Lineage(
-            self.T if self._is_transposed else self,
-            names=np.array(self.names, copy=True, order=_ORDER),
-            colors=np.array(self.colors, copy=True, order=_ORDER),
-        )
-        return obj.T if self._is_transposed else obj
-
-    def __copy__(self):
-        return self.copy()
+    def nlin(self) -> int:
+        """Number of lineages."""
+        return self.shape[1]
 
     @d.get_full_description(base="lin_pd")
     @d.get_sections(base="lin_pd", sections=["Parameters", "Returns"])
     def priming_degree(
         self,
         method: Literal["kl_divergence", "entropy"] = "kl_divergence",
         early_cells: Optional[np.ndarray] = None,
     ) -> np.ndarray:
-        """
-        Compute the degree of lineage priming.
+        """Compute the degree of lineage priming.
 
-        It returns a score in `[0, 1]` where `0` stands for naive and `1` stands for committed.
+        It returns a score in :math:`[0, 1]` where :math:`0` stands for naive and :math:`1` stands for committed.
 
         Parameters
         ----------
         method
             The method used to compute the degree of lineage priming. Valid options are:
 
-                - `'kl_divergence'` - as in :cite:`velten:17`, computes KL-divergence between the fate probabilities of
-                  a cell and the average fate probabilities. Computation of average fate probabilities can be restricted
-                  to a set of user-defined ``early_cells``.
-                - `'entropy'` - as in :cite:`setty:19`, computes entropy over a cell's fate probabilities.
+            - ``'kl_divergence'`` - as in :cite:`velten:17`, computes KL-divergence between the fate probabilities of
+              a cell and the average fate probabilities. Computation of average fate probabilities can be restricted
+              to a set of user-defined ``early_cells``.
+            - ``'entropy'`` - as in :cite:`setty:19`, computes entropy over a cell's fate probabilities.
         early_cells
-            Cell IDs or a mask marking early cells. If `None`, use all cells.
+            Cell IDs or a mask marking early cells. If :obj:`None`, use all cells.
             Only used when ``method = 'kl_divergence'``.
 
         Returns
         -------
         The priming degree.
         """
-        early_cells = (
-            np.ones((len(self),), dtype=np.bool_)
-            if early_cells is None
-            else np.asarray(early_cells)
-        )
+        early_cells = np.ones((len(self),), dtype=np.bool_) if early_cells is None else np.asarray(early_cells)
         if not np.issubdtype(early_cells.dtype, np.bool_):
             early_cells = np.unique(early_cells)
 
         method = PrimingDegree(method)
         probs = self.X
         early_subset = probs[early_cells, :]
         if not len(early_subset):
             raise ValueError("No early cells have been specified.")
 
         with np.errstate(divide="ignore", invalid="ignore"):
             if method == PrimingDegree.KL_DIVERGENCE:
                 probs = np.nan_to_num(
-                    np.sum(
-                        probs * np.log2(probs / np.mean(early_subset, axis=0)), axis=1
-                    ),
+                    np.sum(probs * np.log2(probs / np.mean(early_subset, axis=0)), axis=1),
                     nan=1.0,
                     copy=False,
                 )
             elif method == PrimingDegree.ENTROPY:
-                probs = entropy(probs, axis=1)
+                probs = st.entropy(probs, axis=1)
                 probs = np.max(probs) - probs
             else:
                 raise NotImplementedError(f"Method `{method}` is not yet implemented")
 
             minn, maxx = np.min(probs), np.max(probs)
             return (probs - minn) / (maxx - minn)
 
     @d.dedent
     def plot_pie(
         self,
         reduction: Callable,
         title: Optional[str] = None,
         legend_loc: Optional[str] = "on data",
-        legend_kwargs: Mapping = MappingProxyType({}),
+        legend_kwargs: Mapping = types.MappingProxyType({}),
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[float] = None,
-        save: Optional[Union[Path, str]] = None,
-        **kwargs,
+        save: Optional[Union[pathlib.Path, str]] = None,
+        **kwargs: Any,
     ) -> None:
-        """
-        Plot a pie chart visualizing aggregated lineage probabilities.
+        """Plot a pie chart visualizing aggregated lineage probabilities.
 
         Parameters
         ----------
         reduction
             Function that will be applied lineage-wise.
         title
             Title of the figure.
         legend_loc
-            Location of the legend. If `None`, it is not shown.
+            Location of the legend. If :obj:`None`, it is not shown.
         legend_kwargs
-            Keyword arguments for :func:`matplotlib.axes.Axes.legend`.
+            Keyword arguments for :meth:`~matplotlib.axes.Axes.legend`.
         %(plotting)s
+        kwargs
+            Keyword arguments for :meth:`~matplotlib.axes.Axes.pie`.
 
         Returns
         -------
         %(just_plots)s
         """
+        from cellrank._utils._utils import save_fig
 
         if len(self.names) == 1:
             raise ValueError("Cannot plot pie chart for only 1 lineage.")
 
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
 
         if "autopct" not in kwargs:
             autopct_found = False
-            autopct = (
-                "{:.1f}%".format
-            )  # we don't really care, we don't shot the pct, but the value
+            autopct = "{:.1f}%".format  # we don't really care, we don't shot the pct, but the value
         else:
             autopct_found = True
             autopct = kwargs.pop("autopct")
 
         if title is None:
             title = reduction.__name__ if hasattr(reduction, "__name__") else None
 
@@ -902,90 +647,84 @@
         dist_measure: Literal[
             "cosine_sim", "wasserstein_dist", "kl_div", "js_div", "mutual_info", "equal"
         ] = DistanceMeasure.MUTUAL_INFO,
         normalize_weights: Literal["scale", "softmax"] = NormWeights.SOFTMAX,
         softmax_scale: float = 1,
         return_weights: bool = False,
     ) -> Union["Lineage", Tuple["Lineage", Optional[pd.DataFrame]]]:
-        """
-        Subset states and normalize them so that they again sum to 1.
+        """Subset states and normalize them so that they again sum to :math:`1`.
 
         Parameters
         ----------
         keys
             List of keys that define the states, to which this object will be reduced by projecting the values
             of the other states.
         mode
             Reduction mode to use. Valid options are:
 
-                - `{m.DIST!r}` - use a distance measure ``dist_measure`` to compute weights.
-                - `{m.SCALE!r}` - just rescale the values.
+            - ``{m.DIST!r}`` - use a distance measure ``dist_measure`` to compute weights.
+            - ``{m.SCALE!r}`` - just rescale the values.
         dist_measure
             Used to quantify similarity between query and reference states. Valid options are:
 
-                - `{dm.COSINE_SIM!r}` - cosine similarity.
-                - `{dm.WASSERSTEIN_DIST!r}` - Wasserstein distance.
-                - `{dm.KL_DIV!r}` - Kullback–Leibler divergence.
-                - `{dm.JS_DIV!r}` - Jensen–Shannon divergence.
-                - `{dm.MUTUAL_INFO!r}` - mutual information.
-                - `{dm.EQUAL!r}` - equally redistribute the mass among the rest.
+            - ``{dm.COSINE_SIM!r}`` - cosine similarity.
+            - ``{dm.WASSERSTEIN_DIST!r}`` - Wasserstein distance.
+            - ``{dm.KL_DIV!r}`` - Kullback–Leibler divergence.
+            - ``{dm.JS_DIV!r}`` - Jensen–Shannon divergence.
+            - ``{dm.MUTUAL_INFO!r}`` - mutual information.
+            - ``{dm.EQUAL!r}`` - equally redistribute the mass among the rest.
 
             Only use when ``mode = {m.DIST!r}``.
         normalize_weights
             How to row-normalize the weights. Valid options are:
 
-                - `{nw.SCALE!r}` - divide by the sum.
-                - `{nw.SOFTMAX!r}`- use a softmax.
+            - ``{nw.SCALE!r}`` - divide by the sum.
+            - ``{nw.SOFTMAX!r}``- use a softmax.
 
-            Only use when ``mode = {m.DIST!r}``.
+            Only used when ``mode = {m.DIST!r}``.
         softmax_scale
-            Scaling factor in the softmax, used for normalizing the weights to sum to `1`.
+            Scaling factor in the softmax, used for normalizing the weights to sum to :math:`1`.
         return_weights
-            If `True`, a :class:`pandas.DataFrame` of the weights used for the projection is also returned.
+            If `True`, a :class:`~pandas.DataFrame` of the weights used for the projection is also returned.
             If ``mode = {m.SCALE!r}``, the weights will be `None`.
 
         Returns
         -------
         The lineage object, reduced to the %(initial_or_terminal)s states.
         The weights used for the projection of shape ``(n_query, n_reference)``, if ``return_weights = True``.
         """
-
         mode = Reduction(mode)
         dist_measure = DistanceMeasure(dist_measure)
         normalize_weights = NormWeights(normalize_weights)
 
         if self._is_transposed:
             raise RuntimeError("This method works only on non-transposed lineages.")
 
         if not len(keys):
             raise ValueError("Unable to perform the reduction, no keys specified.")
 
         # check the lineage object
-        if not np.allclose(np.sum(self, axis=1).X, 1.0):
+        if not np.allclose(np.sum(self.X, axis=1), 1.0):
             raise ValueError("Memberships do not sum to one row-wise.")
 
         if len(keys) == 1:
             tmp = self[:, keys]
             return Lineage(
                 np.ones((self.shape[0], 1), dtype=self.dtype),
                 names=tmp.names,
                 colors=tmp.colors,
             )
 
         # check input parameters
         if return_weights and mode == Reduction.SCALE:
-            logg.warning(
-                f"If `mode={mode!r}`, no weights are computed. Returning `None`"
-            )
+            logg.warning(f"If `mode={mode!r}`, no weights are computed. Returning `None`")
 
         reference = self[:, keys]
-        rest = [
-            k for k in self.names if all(map(lambda rk: k not in rk, reference.names))
-        ]
-        if not len(rest):
+        rest = [k for k in self.names if all(k not in rk for rk in reference.names)]
+        if not rest:
             logg.warning(
                 "Unable to perform reduction because all keys have been selected. Returning combined object only"
             )
             return (reference.copy(), None) if return_weights else reference.copy()
 
         query = self[:, rest]
 
@@ -1002,168 +741,328 @@
             elif dist_measure == DistanceMeasure.JS_DIV:
                 weights = _js_div(reference.X, query.X)
             elif dist_measure == DistanceMeasure.MUTUAL_INFO:
                 weights = _mutual_info(reference.X, query.X)
             elif dist_measure == DistanceMeasure.EQUAL:
                 weights = _row_normalize(np.ones((query.shape[1], reference.shape[1])))
             else:
-                raise NotImplementedError(
-                    f"Distance measure `{dist_measure}` is not yet implemented."
-                )
+                raise NotImplementedError(f"Distance measure `{dist_measure}` is not yet implemented.")
 
             # make some checks on the weights
             if weights.shape != (query.shape[1], reference.shape[1]):
                 raise ValueError(
                     f"Expected weight matrix to be of shape `({query.shape[1]}, {reference.shape[1]})`, "
                     f"found `{weights.shape}`."
                 )
             if not np.isfinite(weights).all():
-                raise ValueError(
-                    "Weights matrix contains elements that are not finite."
-                )
+                raise ValueError("Weights matrix contains elements that are not finite.")
             if (weights < 0).any():
                 raise ValueError("Weights matrix contains negative elements.")
 
             if (weights == 0).any():
                 logg.warning("Weights matrix contains exact zeros.")
 
             # normalize the weights to row-sum to one
             if normalize_weights == NormWeights.SCALE:
                 weights_n = _row_normalize(weights)
             elif normalize_weights == NormWeights.SOFTMAX:
                 weights_n = _softmax(_row_normalize(weights), softmax_scale)
             else:
-                raise NotImplementedError(
-                    f"Normalization method `{normalize_weights}` is yet implemented."
-                )
+                raise NotImplementedError(f"Normalization method `{normalize_weights}` is yet implemented.")
 
             # check that the weights row-sum to one now
             if not np.allclose(weights_n.sum(1), 1.0):
                 raise ValueError("Weights do not sum to 1 row-wise.")
 
             # use the weights to re-distribute probability mass form query to reference
             for i, w in enumerate(weights_n):
                 reference += np.dot(query[:, i].X, w[None, :])
         else:
-            raise NotImplementedError(
-                f"Reduction mode `{mode}` is not yet implemented."
-            )
+            raise NotImplementedError(f"Reduction mode `{mode}` is not yet implemented.")
 
         # check that the lineages row-sum to one now
         if not np.allclose(reference.sum(1), 1.0):
             raise ValueError("Reduced lineage rows do not sum to 1.")
 
         # potentially create a weights-df and return everything
         if return_weights:
             if mode == Reduction.DIST:
                 return (
                     reference,
-                    pd.DataFrame(
-                        data=weights_n, columns=reference.names, index=query.names
-                    ),
+                    pd.DataFrame(data=weights_n, columns=reference.names, index=query.names),
                 )
             return reference, None
 
         return reference
 
     @classmethod
     @d.dedent
     @inject_docs(lk=LinKind)
     def from_adata(
         cls,
         adata: AnnData,
         backward: bool = False,
-        kind: Literal["macrostates", "term_states", "abs_probs"] = LinKind.ABS_PROBS,
+        estimator_backward: Optional[bool] = None,
+        kind: Literal["macrostates", "term_states", "fate_probs"] = LinKind.FATE_PROBS,
+        copy: bool = False,
     ) -> "Lineage":
-        """
-        Reconstruct :class:`cellrank.tl.Lineage` from :class:`anndata.AnnData`.
+        """Reconstruct the :class:`~cellrank.Lineage` object from :class:`~anndata.AnnData` object.
 
         Parameters
         ----------
         %(adata)s
         %(backward)s
+        estimator_backward
+            Key which helps to determine whether these states are initial or terminal.
         kind
             Which kind of object to reconstruct. Valid options are:
 
-                - `{lk.MACROSTATES!r}`- macrostates memberships from :class:`cellrank.tl.estimators.GPCCA`.
-                - `{lk.TERM_STATES!r}`- terminal states memberships from :class:`cellrank.tl.estimators.GPCCA`.
-                - `{lk.ABS_PROBS!r}`- the absorption probabilities.
+            - ``{lk.MACROSTATES!r}``- macrostates memberships from :class:`cellrank.estimators.GPCCA`.
+            - ``{lk.TERM_STATES!r}``- terminal states memberships from :class:`cellrank.estimators.GPCCA`.
+            - ``{lk.FATE_PROBS!r}``- fate probabilities.
+        copy
+            Whether to return a copy of the underlying array.
 
         Returns
         -------
         The reconstructed lineage object.
         """
         kind = LinKind(kind)
         if kind == LinKind.MACROSTATES:
             nkey = Key.obs.macrostates(backward)
             key = Key.obsm.memberships(nkey)
         elif kind == LinKind.TERM_STATES:
-            nkey = Key.obs.term_states(backward)
+            nkey = Key.obs.term_states(estim_bwd=estimator_backward, bwd=backward)
             key = Key.obsm.memberships(nkey)
-        elif kind == LinKind.ABS_PROBS:
-            nkey = Key.obs.term_states(backward)
-            key = Key.obsm.abs_probs(backward)
+        elif kind == LinKind.FATE_PROBS:
+            nkey = Key.obs.term_states(estim_bwd=estimator_backward, bwd=backward)
+            key = Key.obsm.fate_probs(backward)
         else:
             raise NotImplementedError(f"Lineage kind `{kind}` is not yet implemented.")
 
         ckey = Key.uns.colors(nkey)
 
-        data: Optional[Union[np.ndarray, Lineage]] = copy(adata.obsm.get(key, None))
-        if data is None:
+        if key not in adata.obsm:
             raise KeyError(f"Unable to find lineage data in `adata.obsm[{key!r}]`.")
+        data: Union[np.ndarray, Lineage] = adata.obsm[key]
+        if copy:
+            data = copy_.copy(data)
         if isinstance(data, Lineage):
             return data
         if data.ndim != 2:
             raise ValueError(f"Expected 2 dimensional data, found `{data.ndim}`.")
 
         states = adata.obs.get(nkey, None)
         if states is None:
-            logg.warning(
-                f"Unable to find states in `adata.obs[{nkey!r}]`. Using default names"
-            )
+            logg.warning(f"Unable to find states in `adata.obs[{nkey!r}]`. Using default names")
         elif not is_categorical_dtype(states):
             logg.warning(
                 f"Expected `adata.obs[{key!r}]` to be `categorical`, "
                 f"found `{infer_dtype(adata.obs[nkey])}`. Using default names"
             )
         else:
             states = list(states.cat.categories)
             if len(states) != data.shape[1]:
                 logg.warning(
-                    f"Expected to find `{data.shape[1]}` names, found `{len(states)}`. "
-                    f"Using default names"
+                    f"Expected to find `{data.shape[1]}` names, found `{len(states)}`. " f"Using default names"
                 )
         if states is None or len(states) != data.shape[1]:
             states = [str(i) for i in range(data.shape[1])]
 
         colors = adata.uns.get(ckey, None)
         if colors is None:
-            logg.warning(
-                f"Unable to find colors in `adata.uns[{ckey!r}]`. "
-                f"Using default colors"
-            )
+            logg.warning(f"Unable to find colors in `adata.uns[{ckey!r}]`. " f"Using default colors")
         elif len(colors) != data.shape[1]:
-            logg.warning(
-                f"Expected to find `{data.shape[1]}` colors, found `{len(colors)}`. "
-                f"Using default colors"
-            )
+            logg.warning(f"Expected to find `{data.shape[1]}` colors, found `{len(colors)}`. " f"Using default colors")
             colors = None
 
         return Lineage(data, names=states, colors=colors)
 
+    def view(self, dtype=None, type=None, *_, **__) -> "LineageView":
+        """Return a view of self."""
+        return LineageView(self)
+
+    def __repr__(self) -> str:
+        return f'{super().__repr__()[:-1]},\n  names([{", ".join(self.names)}]))'
+
+    def __str__(self):
+        return f'{super().__str__()}\n names=[{", ".join(self.names)}]'
+
+    @property
+    def _fmt(self) -> Callable[[Any], str]:
+        return "{:.06f}".format if np.issubdtype(self.dtype, float) else "{}".format
+
+    def _repr_html_(self) -> str:
+        def format_row(r):
+            rng = (
+                range(self.shape[1])
+                if not self._is_transposed or (self._is_transposed and self.shape[1] <= _HTML_REPR_THRESH)
+                else list(range(_HT_CELLS)) + [...] + list(range(self.shape[1] - _HT_CELLS - 1, self.shape[1] - 1))
+            )
+
+            cells = "".join(
+                f"<td style='text-align: right;'>" f"{self._fmt(self.X[r, c])}" f"</td>"
+                if isinstance(c, int)
+                else _DUMMY_CELL
+                for c in rng
+            )
+            return f"<tr>{(names[r] if self._is_transposed else '') + cells}</tr>"
+
+        def dummy_row() -> str:
+            values = "".join(_DUMMY_CELL for _ in range(self.shape[1]))
+            return f"<tr>{values}</tr>"
+
+        if self.names is None or self.colors is None:
+            raise RuntimeError(
+                f"Name or colors are `None`. This can happen when running `array.view({type(self).__name__}`."
+            )
+
+        if self.ndim != 2:
+            return repr(self)
+
+        styles = [
+            f"'background-color: {bg}; color: {fg}; text-align: center; word-wrap: break-word; max-width: 100px'"
+            for bg, fg in map(_get_bg_fg_colors, self.colors)
+        ]
+        names = [f"<th style={style}>{n}</th>" for n, style in zip(self.names, styles)]
+        header = f"<tr>{''.join(names)}</tr>"
+
+        if self.shape[0] > _HTML_REPR_THRESH:
+            body = "".join(format_row(i) for i in range(_HT_CELLS))
+            body += dummy_row()
+            body += "".join(format_row(i) for i in range(self.shape[0] - _HT_CELLS - 1, self.shape[0] - 1))
+        else:
+            body = "".join(format_row(i) for i in range(self.shape[0]))
+
+        cells = "cells" if self.shape[0] > 1 else "cell"
+        lineages = "lineages" if self.shape[1] > 1 else "lineage"
+        if self._is_transposed:
+            cells, lineages = lineages, cells
+        metadata = f"<p>{self.shape[0]} {cells} x {self.shape[1]} {lineages}</p>"
+
+        if self._is_transposed:
+            header = ""
+        return (
+            f"<div style='scoped' class='rendered_html'>"
+            f"<table class='dataframe'>{header}{body}</table>{metadata}"
+            f"</div>"
+        )
+
+    def __format__(self, format_spec):
+        if self.shape == (1, 1):
+            return format_spec.format(self.X[0, 0])
+        if self.shape == (1,):
+            return format_spec.format(self.X[0])
+        return NotImplemented
+
+    def __setstate__(self, state, *_, **__):
+        *state, names, colors, is_t = state
+        names = names[-1]
+        colors = colors[-1]
+
+        self._names = np.empty(names[1])
+        self._colors = np.empty(colors[1])
+
+        super().__setstate__(tuple(state))
+        self._names.__setstate__(tuple(names))
+        self._colors.__setstate__(tuple(colors))
+
+        self._is_transposed = is_t
+        self._n_lineages = len(self.names)
+        self._names_to_ixs = {name: ix for ix, name in enumerate(self.names)}
+
+    def __reduce__(self):
+        res = list(super().__reduce__())
+
+        names = self.names.__reduce__()
+        colors = self.colors.__reduce__()
+        res[-1] += (names, colors, self._is_transposed)
+
+        return tuple(res)
+
+    def copy(self, _="C") -> "Lineage":
+        """Return a copy of itself."""
+        obj = Lineage(
+            self.T if self._is_transposed else self,
+            names=np.array(self.names, copy=True, order=_ORDER),
+            colors=np.array(self.colors, copy=True, order=_ORDER),
+        )
+        return obj.T if self._is_transposed else obj
+
+    def __copy__(self):
+        return self.copy()
+
+    def _check_axis1_shape(self, array: Iterable[Union[str, ColorLike]], msg: str) -> List[Union[str, ColorLike]]:
+        """Check whether the size of the 1D array has the correct length."""
+        array = list(array)
+        if len(array) != self._n_lineages:
+            raise ValueError(msg.format(self._n_lineages, len(array)))
+
+        return array
+
+    def _maybe_convert_names(
+        self,
+        names: Iterable[Union[int, str, bool]],
+        is_singleton: bool = False,
+        default: Optional[Union[int, str]] = None,
+        make_unique: bool = True,
+    ) -> Union[int, List[int], List[bool]]:
+        """Convert string indices to their corresponding int indices."""
+        from cellrank._utils._utils import _unique_order_preserving
+
+        if all(isinstance(n, (bool, np.bool_)) for n in names):
+            return list(names)
+        res = []
+        for name in names:
+            if isinstance(name, str):
+                if name in self._names_to_ixs:
+                    name = self._names_to_ixs[name]
+                elif default is not None:
+                    if isinstance(default, str):
+                        if default not in self._names_to_ixs:
+                            raise KeyError(
+                                f"Invalid lineage name: `{name}`. " f"Valid names are: `{list(self.names)}`."
+                            )
+                        name = self._names_to_ixs[default]
+                    else:
+                        name = default
+                else:
+                    raise KeyError(f"Invalid lineage name `{name!r}`. Valid names are: `{list(self.names)}`.")
+            res.append(name)
+
+        if make_unique:
+            res = _unique_order_preserving(res)
+
+        return res[0] if is_singleton else res
+
+    @staticmethod
+    def _prepare_annotation(
+        array: List[str],
+        checker: Optional[Callable] = None,
+        transformer: Optional[Callable] = None,
+        checker_msg: Optional[str] = None,
+    ) -> np.ndarray:
+        if checker is not None:
+            assert checker_msg, "Please provide a message when `checker` is not `None`."
+            for v in array:
+                if not checker(v):
+                    raise ValueError(checker_msg.format(v))
+        if transformer is not None:
+            array = np.array([transformer(v) for v in array])
+
+        return np.array(array)
+
 
 class LineageView(Lineage):
-    """View of :class:`cellrank.tl.Lineage`."""
+    """View of :class:`~cellrank.Lineage`."""
 
     def __new__(cls, lineage: Lineage) -> "LineageView":
         """Create a LineageView."""
         if not isinstance(lineage, Lineage):
-            raise TypeError(
-                f"Cannot create a `{cls.__name__}` of `{type(lineage).__name__}`."
-            )
+            raise TypeError(f"Cannot create a `{cls.__name__}` of `{type(lineage).__name__}`.")
 
         view = np.array(lineage, copy=False).view(cls)
         view._owner = lineage
         view._names = lineage.names
         view._n_lineages = len(view.names)
         view._names_to_ixs = lineage._names_to_ixs
         view._colors = lineage.colors
@@ -1190,20 +1089,20 @@
         """Lineage colors."""
         return super().colors
 
     @colors.setter
     def colors(self, _):
         raise RuntimeError(f"Unable to set colors of `{type(self).__name__}`.")
 
-    def view(self, dtype=None, type=None) -> "LineageView":
+    def view(self, dtype=None, type=None, *_, **__) -> "LineageView":
         """Return self."""
         return self
 
     def copy(self, _="C") -> Lineage:
-        """Return a copy of itself."""
+        """Return a copy of self."""
         was_trasposed = False
         if self._is_transposed:
             self = self.T
             was_trasposed = True
 
         obj = Lineage(
             self,
@@ -1217,17 +1116,15 @@
     if a.shape[0] != b.shape[0]:
         raise ValueError("Lineage objects have unequal cell numbers")
 
     bool_a = (a == 0).any(axis=1)
     bool_b = (b == 0).any(axis=1)
     mask = ~np.logical_or(bool_a, bool_b)
 
-    logg.warning(
-        f"Removed {a.shape[0] - np.sum(mask)} rows because they contained zeros"
-    )
+    logg.warning(f"Removed {a.shape[0] - np.sum(mask)} rows because they contained zeros")
 
     return a[mask, :], b[mask, :]
 
 
 def _softmax(X, beta: float = 1):
     return np.exp(X * beta) / np.expand_dims(np.sum(np.exp(X * beta), axis=1), -1)
 
@@ -1242,18 +1139,16 @@
     from numpy.linalg import norm
 
     return X / norm(X, ord=norm_ord, axis=0)
 
 
 def _cosine_sim(reference, query):
     # the cosine similarity is symmetric
-
     # normalize these to have 2-norm 1
     reference_n, query_n = _col_normalize(reference, 2), _col_normalize(query, 2)
-
     return (reference_n.T @ query_n).T
 
 
 def _point_wise_distance(reference, query, distance):
     # utility function for all point-wise distances/divergences
     # take care of rows that contain zeros
     reference_no_zero, query_no_zero = _remove_zero_rows(reference, query)
@@ -1271,24 +1166,19 @@
             weights[i, j] = 1.0 / distance(q_d, r_d)
 
     return weights
 
 
 def _wasserstein_dist(reference, query):
     # the wasserstein distance is symmetric
-    from scipy.stats import wasserstein_distance
-
-    return _point_wise_distance(reference, query, wasserstein_distance)
+    return _point_wise_distance(reference, query, st.wasserstein_distance)
 
 
 def _kl_div(reference, query):
-    # the KL divergence is not symmetric
-    from scipy.stats import entropy
-
-    return _point_wise_distance(reference, query, entropy)
+    return _point_wise_distance(reference, query, st.entropy)
 
 
 def _js_div(reference, query):
     # the js divergence is symmetric
     from scipy.spatial.distance import jensenshannon
 
     return _point_wise_distance(reference, query, jensenshannon)
@@ -1299,7 +1189,23 @@
     from sklearn.feature_selection import mutual_info_regression
 
     weights = np.zeros((query.shape[1], reference.shape[1]))
     for i, target in enumerate(query.T):
         weights[i, :] = mutual_info_regression(reference, target)
 
     return weights
+
+
+_SPEC = IOSpec("array", "0.2.0")
+
+
+@_REGISTRY.register_write(H5Group, Lineage, _SPEC)
+@_REGISTRY.register_write(H5Group, LineageView, _SPEC)
+@_REGISTRY.register_write(ZarrGroup, Lineage, _SPEC)
+@_REGISTRY.register_write(ZarrGroup, LineageView, _SPEC)
+def _write_lineage(
+    f: Any,
+    k: str,
+    elem: Union[Lineage, LineageView],
+    dataset_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
+) -> None:
+    write_basic(f, k, elem=elem.X, dataset_kwargs=dataset_kwargs)
```

### Comparing `cellrank-1.5.1/cellrank/tl/_linear_solver.py` & `cellrank-2.0.0/src/cellrank/_utils/_linear_solver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,92 +1,78 @@
-"""Module containing anything related to linear solvers."""
-from typing import List, Tuple, Union, TypeVar, Optional
+import functools
+from typing import List, Optional, Tuple, TypeVar, Union
 
-from functools import singledispatch
+import numpy as np
+import scipy.sparse as sp
+from scipy.linalg import solve
 
 from cellrank import logging as logg
-from cellrank.tl._enum import _DEFAULT_BACKEND
-from cellrank.ul._utils import _get_n_cores
-from cellrank.ul._parallelize import parallelize
+from cellrank._utils._enum import DEFAULT_BACKEND
+from cellrank._utils._parallelize import _get_n_cores, parallelize
 
-import numpy as np
-from scipy.linalg import solve
-from scipy.sparse import eye as speye
-from scipy.sparse import (
-    issparse,
-    spmatrix,
-    csc_matrix,
-    csr_matrix,
-    isspmatrix_csc,
-    isspmatrix_csr,
-)
-from scipy.sparse.linalg import gmres, lgmres, gcrotmk, bicgstab
+__all__ = ["_solve_lin_system", "_is_petsc_slepc_available"]
 
 _DEFAULT_SOLVER = "gmres"
 _PETSC_ERROR_MSG_SHOWN = False
 _PETSC_ERROR_MSG = (
     "Unable to import petsc4py. "
     "For installation, please refer to: https://petsc4py.readthedocs.io/en/stable/install.html.\n"
     "Defaulting to `{!r}` solver."
 )
 _AVAIL_ITER_SOLVERS = {
-    "gmres": gmres,
-    "lgmres": lgmres,
-    "bicgstab": bicgstab,
-    "gcrotmk": gcrotmk,
+    "gmres": sp.linalg.gmres,
+    "lgmres": sp.linalg.lgmres,
+    "bicgstab": sp.linalg.bicgstab,
+    "gcrotmk": sp.linalg.gcrotmk,
 }
 
 LinSolver = TypeVar("LinSolver")
 PETScMat = TypeVar("PETScMat")
 Queue = TypeVar("Queue")
 
 
-def _create_petsc_matrix(
-    mat: Union[np.ndarray, spmatrix], as_dense: bool = False
-) -> PETScMat:
-    """
-    Create a PETSc matrix from :mod:`numpy` or :mod:`scipy.sparse` matrix.
+def _create_petsc_matrix(mat: Union[np.ndarray, sp.spmatrix], as_dense: bool = False) -> PETScMat:
+    """Create a PETSc matrix from :mod:`numpy` or :mod:`scipy.sparse` matrix.
 
     Parameters
     ----------
     mat
         The matrix to convert.
     as_dense
         Only used when ``mat`` is a sparse matrix. If `True`, create `'seqdense'` matrix,
         otherwise `'seqaij'` matrix.
 
     Returns
     -------
     The converted matrix.
     """
-
     # TODO(michalk8): for some solvers, we need to set the diagonal entries explicitly, even if they are zeros
     # see: https://lists.mcs.anl.gov/mailman/htdig/petsc-users/2014-October/023212.html
 
     from petsc4py import PETSc
 
-    if issparse(mat) and as_dense:
+    if sp.issparse(mat) and as_dense:
         mat = mat.toarray()
 
     A = PETSc.Mat().create()
-    if issparse(mat):
-        if not isspmatrix_csr(mat):
-            mat = csr_matrix(mat)
+    if sp.issparse(mat):
+        if not sp.isspmatrix_csr(mat):
+            mat = sp.csr_matrix(mat)
         A.createAIJ(size=mat.shape, csr=(mat.indptr, mat.indices, mat.data))
     else:
         A.createDense(mat.shape, array=mat)
 
     A.assemblyBegin()
     A.assemblyEnd()
 
     return A
 
 
 def _create_solver(
-    mat_a: Union[np.ndarray, spmatrix],
+    mat_a: Union[np.ndarray, sp.spmatrix],
     solver: Optional[str],
     preconditioner: Optional[str],
     tol: float,
 ) -> Tuple["petsc4py.PETSc.KSP", "petsc4py.PETSc.Vec", "petsc4py.PETScVec"]:  # noqa
     """
     Create a linear system solver.
 
@@ -101,15 +87,14 @@
     tol
         The relative convergence tolerance, relative decrease in the (possibly preconditioned) residual norm .
 
     Returns
     -------
     Triple containing the solver, vector ``x`` and vector ``b`` in ``A * x = b``.
     """
-
     from petsc4py import PETSc
 
     A = _create_petsc_matrix(mat_a)
 
     ksp = PETSc.KSP().create()
     ksp.setTolerances(rtol=tol)
     ksp.setType(solver if solver is not None else PETSc.KSP.Type.GMRES)
@@ -129,55 +114,53 @@
     ksp.setFromOptions()
 
     x, b = A.getVecs()
 
     return ksp, x, b
 
 
-@singledispatch
+@functools.singledispatch
 def _solve_many_sparse_problems_petsc(
-    mat_b: csc_matrix,
-    _mat_a: Union[np.ndarray, spmatrix],
+    mat_b: sp.csc_matrix,
+    _mat_a: Union[np.ndarray, sp.spmatrix],
     _solver: Optional[str] = None,
     _preconditioner: Optional[str] = None,
     _tol: float = 1e-5,
     _queue: Optional[Queue] = None,
 ) -> Tuple[np.ndarray, int]:
     raise NotImplementedError(f"Not implemented for type `{type(mat_b).__name__!r}`.")
 
 
 @_solve_many_sparse_problems_petsc.register(np.ndarray)
 def _(
     mat_b: np.ndarray,
-    mat_a: Union[np.ndarray, spmatrix],
+    mat_a: Union[np.ndarray, sp.spmatrix],
     solver: Optional[str] = None,
     preconditioner: Optional[str] = None,
     tol: float = 1e-5,
     _queue: Optional[Queue] = None,
 ) -> Tuple[np.ndarray, int]:
     if mat_b.ndim not in (1, 2) or (mat_b.ndim == 2 and mat_b.shape[1] != 1):
-        raise ValueError(
-            f"Expected either a vector or a matrix with `1` column, got `{mat_b.shape}`."
-        )
+        raise ValueError(f"Expected either a vector or a matrix with `1` column, got `{mat_b.shape}`.")
 
     if solver == "direct":  # this can sometimes happen
         solver = None
 
     ksp, x, b = _create_solver(mat_a, solver, preconditioner=preconditioner, tol=tol)
     b.setArray(mat_b.squeeze())
 
     ksp.solve(b, x)
 
     return np.atleast_1d(x.getArray().copy().squeeze()), int(ksp.converged)
 
 
-@_solve_many_sparse_problems_petsc.register(csc_matrix)
+@_solve_many_sparse_problems_petsc.register(sp.csc_matrix)
 def _(
-    mat_b: csc_matrix,
-    mat_a: Union[np.ndarray, spmatrix],
+    mat_b: sp.csc_matrix,
+    mat_a: Union[np.ndarray, sp.spmatrix],
     solver: Optional[str],
     preconditioner: Optional[str],
     tol: float,
     queue: Queue,
 ) -> Tuple[np.ndarray, int]:
     ksp, x, b = _create_solver(mat_a, solver, preconditioner=preconditioner, tol=tol)
     xs, converged = [], 0
@@ -199,22 +182,21 @@
     if queue is not None:
         queue.put(None)
 
     return np.stack(xs, axis=1), converged
 
 
 def _solve_many_sparse_problems(
-    mat_b: spmatrix,
-    mat_a: spmatrix,
+    mat_b: sp.spmatrix,
+    mat_a: sp.spmatrix,
     solver: LinSolver,
     tol: float,
     queue: Queue,
 ) -> Tuple[np.ndarray, int]:
-    """
-    Solve ``mat_a * x = mat_b`` efficiently using an iterative solver.
+    """Solve ``mat_a * x = mat_b`` efficiently using an iterative solver.
 
     This is a utility function which is optimized for the case of ``mat_a`` and ``mat_b`` being sparse,
     and columns in ``mat_b`` being related. In that case, we can treat each column of ``mat_b`` as a
     separate linear problem and solve that efficiently using iterative solvers that exploit sparsity.
 
     Parameters
     ----------
@@ -232,18 +214,17 @@
     Returns
     -------
     Matrix of shape `n x m`. Each column in the resulting matrix corresponds to the solution
     of one of the sub-problems defined via columns in ``mat_b``.
 
     Number of converged solutions.
     """
-
     # initialise solution list and info list
     x_list, n_converged = [], 0
-    kwargs = {} if solver is not gmres else {"atol": "legacy"}  # get rid of the warning
+    kwargs = {} if solver is not sp.linalg.gmres else {"atol": "legacy"}  # get rid of the warning
 
     for b in mat_b:
         # actually call the solver for the current sub-problem
         x, info = solver(mat_a, b.toarray().flatten(), tol=tol, x0=None, **kwargs)
 
         # append solution and info
         x_list.append(np.atleast_1d(x))
@@ -255,16 +236,16 @@
     if queue is not None:
         queue.put(None)
 
     return np.stack(x_list, axis=1), n_converged
 
 
 def _petsc_direct_solve(
-    mat_a: Union[np.ndarray, spmatrix],
-    mat_b: Optional[Union[spmatrix, np.ndarray]] = None,
+    mat_a: Union[np.ndarray, sp.spmatrix],
+    mat_b: Optional[Union[sp.spmatrix, np.ndarray]] = None,
     tol: float = 1e-5,
     **kwargs,
 ) -> np.ndarray:
     from petsc4py import PETSc
 
     if mat_b is None:
         if mat_a.shape[0] != mat_a.shape[1]:
@@ -278,20 +259,18 @@
 
         start, end = B.getOwnershipRange()
         for i in range(start, end):
             B[i, i] = 1
         B.assemble()
     else:
         if mat_b.ndim == 1 or (mat_b.ndim == 2 and mat_b.shape[1] == 1):
-            if issparse(mat_b):
+            if sp.issparse(mat_b):
                 mat_b = mat_b.toarray()
 
-            res, converged = _solve_many_sparse_problems_petsc(
-                mat_b, mat_a=mat_a, tol=tol, **kwargs
-            )
+            res, converged = _solve_many_sparse_problems_petsc(mat_b, mat_a=mat_a, tol=tol, **kwargs)
             if not converged:
                 logg.warning(
                     f"The solution for system "
                     f"`A{list(mat_a.shape)} * x[{mat_b.shape[0]}] = b[{mat_b.shape[0]}]` "
                     f"did not converge"
                 )
 
@@ -335,27 +314,26 @@
             f"did not converge"
         )
 
     return res
 
 
 def _solve_lin_system(
-    mat_a: Union[np.ndarray, spmatrix],
-    mat_b: Union[np.ndarray, spmatrix],
+    mat_a: Union[np.ndarray, sp.spmatrix],
+    mat_b: Union[np.ndarray, sp.spmatrix],
     solver: str = _DEFAULT_SOLVER,
     use_petsc: bool = False,
     preconditioner: Optional[str] = None,
     n_jobs: Optional[int] = None,
-    backend: str = _DEFAULT_BACKEND,
+    backend: str = DEFAULT_BACKEND,
     tol: float = 1e-5,
     use_eye: bool = False,
     show_progress_bar: bool = True,
 ) -> np.ndarray:
-    """
-    Solve ``mat_a * x = mat_b`` efficiently using either iterative or direct methods.
+    """Solve ``mat_a * x = mat_b`` efficiently using either iterative or direct methods.
 
     This is a utility function which is optimized for the case of ``mat_a`` and ``mat_b`` being sparse,
     and columns in ``mat_b`` being related. In that case, we can treat each column of ``mat_b`` as a
     separate linear problem and solve that efficiently using iterative solvers that exploit sparsity.
 
     If the columns of ``mat_b`` are related, we can use the solution of the previous problem as an
     initial guess for the next problem. Further, we parallelize the individual problems for each
@@ -390,68 +368,59 @@
         The relative convergence tolerance, relative decrease in the (possibly preconditioned) residual norm .
     use_eye
         Solve ``(I - mat_a) * x = mat_b`` instead.
     show_progress_bar
         Whether to show progress bar when the solver isn't a direct one.
 
     Returns
-    --------
+    -------
     Matrix of shape `n x m`. Each column corresponds to the solution of one of the sub-problems
     defined via columns in ``mat_b``.
     """
 
-    def extractor(
-        res_converged: List[Tuple[np.ndarray, int]]
-    ) -> Tuple[np.ndarray, int]:
+    def extractor(res_converged: List[Tuple[np.ndarray, int]]) -> Tuple[np.ndarray, int]:
         res, converged = zip(*res_converged)
         return np.hstack(res), sum(converged)
 
     n_jobs = _get_n_cores(n_jobs, n_jobs=None)
 
-    if use_petsc:
-        try:
-            from petsc4py import PETSc
-        except ImportError:
-            global _PETSC_ERROR_MSG_SHOWN
-            if not _PETSC_ERROR_MSG_SHOWN:
-                _PETSC_ERROR_MSG_SHOWN = True
-                logg.warning(_PETSC_ERROR_MSG.format(_DEFAULT_SOLVER))
-            solver = _DEFAULT_SOLVER
-            use_petsc = False
+    if use_petsc and not _is_petsc_slepc_available():
+        global _PETSC_ERROR_MSG_SHOWN
+        if not _PETSC_ERROR_MSG_SHOWN:
+            _PETSC_ERROR_MSG_SHOWN = True
+            logg.warning(_PETSC_ERROR_MSG.format(_DEFAULT_SOLVER))
+        solver = _DEFAULT_SOLVER
+        use_petsc = False
 
     if use_eye:
-        mat_a = (
-            speye(mat_a.shape[0]) if issparse(mat_a) else np.eye(mat_a.shape[0])
-        ) - mat_a
+        mat_a = (sp.eye(mat_a.shape[0]) if sp.issparse(mat_a) else np.eye(mat_a.shape[0])) - mat_a
 
     if solver == "direct":
         if use_petsc:
             logg.debug("Solving the linear system directly using `PETSc`")
-            return _petsc_direct_solve(
-                mat_a, mat_b, solver=solver, preconditioner=preconditioner, tol=tol
-            )
+            return _petsc_direct_solve(mat_a, mat_b, solver=solver, preconditioner=preconditioner, tol=tol)
 
-        if issparse(mat_a):
+        if sp.issparse(mat_a):
             logg.debug("Densifying `A` for `scipy` direct solver")
             mat_a = mat_a.toarray()
-        if issparse(mat_b):
+        if sp.issparse(mat_b):
             logg.debug("Densifying `B` for `scipy` direct solver")
             mat_b = mat_b.toarray()
 
         logg.debug("Solving the linear system directly using `scipy`")
 
         return solve(mat_a, mat_b)
 
     if use_petsc:
-        if not isspmatrix_csr(mat_a):
-            mat_a = csr_matrix(mat_a)
+        if not sp.isspmatrix_csr(mat_a):
+            mat_a = sp.csr_matrix(mat_a)
 
         mat_b = mat_b.T
-        if not isspmatrix_csc(mat_b):
-            mat_b = csc_matrix(mat_b)
+        if not sp.isspmatrix_csc(mat_b):
+            mat_b = sp.csc_matrix(mat_b)
 
         # as_array causes an issue, because it's called like this np.array([(NxM), (NxK), ....]
         # in the end, we want array of shape Nx(M + K + ...) - this is ensured by the extractor
         logg.debug(
             f"Solving the linear system using `PETSc` solver `{('gmres' if solver is None else solver)!r}` "
             f"on `{n_jobs}` core(s) with {'no' if preconditioner is None else preconditioner} preconditioner and "
             f"`tol={tol}`"
@@ -463,22 +432,22 @@
             n_jobs=n_jobs,
             backend=backend,
             as_array=False,
             extractor=extractor,
             show_progress_bar=show_progress_bar,
         )(mat_a, solver=solver, preconditioner=preconditioner, tol=tol)
     elif solver in _AVAIL_ITER_SOLVERS:
-        if not issparse(mat_a):
+        if not sp.issparse(mat_a):
             logg.debug("Sparsifying `A` for iterative solver")
-            mat_a = csr_matrix(mat_a)
+            mat_a = sp.csr_matrix(mat_a)
 
         mat_b = mat_b.T
-        if not issparse(mat_b):
+        if not sp.issparse(mat_b):
             logg.debug("Sparsifying `B` for iterative solver")
-            mat_b = csr_matrix(mat_b)
+            mat_b = sp.csr_matrix(mat_b)
 
         logg.debug(
             f"Solving the linear system using `scipy` solver `{solver!r}` on `{n_jobs} cores(s)` with `tol={tol}`"
         )
 
         mat_x, n_converged = parallelize(
             _solve_many_sparse_problems,
@@ -493,7 +462,17 @@
     else:
         raise ValueError(f"Invalid solver `{solver!r}`.")
 
     if n_converged != mat_b.shape[0]:
         logg.warning(f"`{mat_b.shape[0] - n_converged}` solution(s) did not converge")
 
     return mat_x
+
+
+def _is_petsc_slepc_available() -> bool:
+    try:
+        import petsc4py  # noqa
+        import slepc4py  # noqa
+
+        return True
+    except ImportError:
+        return False
```

### Comparing `cellrank-1.5.1/cellrank/tl/_mixins/_anndata.py` & `cellrank-2.0.0/src/cellrank/kernels/mixins/_anndata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,70 @@
+import abc
 from typing import Any, Optional
 
-from abc import ABC, abstractmethod
-
 from anndata import AnnData
-from cellrank.ul._docs import d
+
+from cellrank._utils._docs import d
+
+__all__ = ["AnnDataMixin"]
 
 
-class AnnDataMixin(ABC):
-    """Mixin that allows for serialization from/to :class:`anndata.AnnData`."""
+class AnnDataMixin(abc.ABC):
+    """Mixin that allows for serialization from/to :class:`~anndata.AnnData`."""
 
-    @abstractmethod
+    @abc.abstractmethod
     @d.dedent
     def _read_from_adata(self, adata: AnnData, **kwargs: Any) -> bool:
-        """
-        Populate attributes of self from :class:`anndata.AnnData`.
+        """Populate attributes from :class:`~anndata.AnnData`.
 
         Parameters
         ----------
         %(adata)s
         kwargs
             Additional keyword arguments.
 
         Returns
         -------
-        `True` if the deserialization was successful, otherwise `False`.
+        :obj:`True` if the de-serialization was successful, otherwise :obj:`False`.
         """
         return True
 
     @property
-    @abstractmethod
+    @abc.abstractmethod
     def adata(self) -> AnnData:
         """Annotated data object."""
 
     @adata.setter
-    @abstractmethod
+    @abc.abstractmethod
     def adata(self, adata: Optional[AnnData]) -> None:
         ...
 
-    @abstractmethod
+    @abc.abstractmethod
     def __len__(self) -> int:
         ...
 
-    @abstractmethod
+    @abc.abstractmethod
     @d.get_full_description(base="to_adata")
     def to_adata(self, **kwargs: Any) -> AnnData:
-        """Serialize self to :class:`anndata.Anndata`."""
+        """Serialize self to :class:`~anndata.Anndata`."""
 
     @classmethod
     @d.get_full_description(base="from_adata")
     @d.get_sections(base="from_adata", sections=["Returns"])
     @d.dedent
     def from_adata(cls, adata: AnnData, **kwargs: Any) -> "AnnDataMixin":
-        """
-        Deserialize self from :class:`anndata.AnnData`.
+        """De-serialize self from :class:`~anndata.AnnData`.
 
         Parameters
         ----------
         %(adata)s
         kwargs
-            Additional keyword arguments.
+            Additional keyword arguments for initialization.
 
         Returns
         -------
-        The deserialized object.
+        The de-serialized object.
         """
         obj = cls(adata, **kwargs)
         obj._read_from_adata(adata)
 
         return obj
```

### Comparing `cellrank-1.5.1/cellrank/tl/_mixins/_io.py` & `cellrank-2.0.0/src/cellrank/kernels/mixins/_io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,136 +1,111 @@
-from typing import Any, Tuple, Union, Optional
-from typing_extensions import Protocol
-
+import contextlib
+import pathlib
 import pickle
-from pathlib import Path
-from contextlib import contextmanager
+from typing import Optional, Protocol, Tuple, Union
 
 from anndata import AnnData
+
 from cellrank import logging as logg
 
+__all__ = ["IOMixin"]
+
 
-class IOMixinProtocol(Protocol):  # noqa: D101
+class IOMixinProtocol(Protocol):
     @property
-    def shape(self) -> Tuple[int, ...]:  # noqa: D102
+    def shape(self) -> Tuple[int, ...]:
         ...
 
     @property
-    def adata(self) -> AnnData:  # noqa: D102
+    def adata(self) -> AnnData:
         ...
 
     @adata.setter
     def adata(self, adata: AnnData) -> None:
         ...
 
 
 class IOMixin:
     """Mixin that allows for serialization from/to files using :mod:`pickle`."""
 
-    def __init__(self, **kwargs: Any):
-        super().__init__(**kwargs)
-
     @property
-    @contextmanager
+    @contextlib.contextmanager
     def _remove_adata(self) -> None:
         """Temporarily remove :attr:`adata`, if present."""
         adata = getattr(self, "adata", None)
 
         try:
             if adata is not None:
                 self.adata = None
             yield
         finally:
             if adata is not None:
                 self.adata = adata
 
     def write(
         self,
-        fname: Union[str, Path],
+        fname: Union[str, pathlib.Path],
         write_adata: bool = True,
-        ext: Optional[str] = "pickle",
     ) -> None:
-        """
-        Serialize self to a file.
+        """Serialize self to a file using :mod:`pickle`.
 
         Parameters
         ----------
         fname
-            Filename where to save the object.
+            Path where to save the object.
         write_adata
-            Whether to save :attr:`adata` object or not, if present.
-        ext
-            Filename extension to use. If `None`, don't append any extension.
+            Whether to save :attr:`adata` object.
 
         Returns
         -------
-        Nothing, just writes itself to a file using :mod:`pickle`.
+        Nothing, just writes itself to a file.
         """
-
-        fname = str(fname)
-        if ext is not None:
-            if not ext.startswith("."):
-                ext = "." + ext
-            if not fname.endswith(ext):
-                fname += ext
-
         logg.info(f"Writing `{self}` to `{fname}`")
 
         if write_adata:
             with open(fname, "wb") as fout:
                 pickle.dump(self, fout)
-            return
-
-        with self._remove_adata:
-            with open(fname, "wb") as fout:
+        else:
+            with self._remove_adata, open(fname, "wb") as fout:
                 pickle.dump(self, fout)
 
     @staticmethod
-    def read(
-        fname: Union[str, Path], adata: Optional[AnnData] = None, copy: bool = False
-    ) -> "IOMixin":
-        """
-        Deserialize self from a file.
+    def read(fname: Union[str, pathlib.Path], adata: Optional[AnnData] = None, copy: bool = False) -> "IOMixin":
+        """De-serialize self from a file.
 
         Parameters
         ----------
         fname
-            Filename from which to read the object.
+            Path from which to read the object.
         adata
-            :class:`anndata.AnnData` object to assign to the saved object.
+            :class:`~anndata.AnnData` object to assign to the saved object.
             Only used when the saved object has :attr:`adata` and it was saved without it.
         copy
-            Whether to copy ``adata`` before assigning it or not. If ``adata`` is a view, it is always copied.
+            Whether to copy ``adata`` before assigning it. If ``adata`` is a view, it is always copied.
 
         Returns
         -------
-        The deserialized object.
+        The de-serialized object.
         """
-
         with open(fname, "rb") as fin:
             obj: IOMixinProtocol = pickle.load(fin)
 
         if hasattr(obj, "adata"):
             if isinstance(obj.adata, AnnData):
                 if adata is not None:
-                    logg.warning(
-                        "Ignoring supplied `adata` object because it is already present"
-                    )
+                    logg.warning("Ignoring supplied `adata` object because it is already present")
                 return obj
 
             if not isinstance(adata, AnnData):
                 raise TypeError(
-                    "This object was saved without its `adata` object. "
-                    "Please supply one as `adata=...`."
+                    "This object was saved without its `adata` object. " "Please supply one as `adata=...`."
                 )
 
             if obj.shape[0] != len(adata):
-                raise ValueError(
-                    f"Expected `adata` to be of length `{len(adata)}`, found `{obj.shape[0]}`."
-                )
+                raise ValueError(f"Expected `adata` to be of length `{len(adata)}`, found `{obj.shape[0]}`.")
             if copy or adata.is_view:
                 adata = adata.copy()
 
             obj.adata = adata
             return obj
 
         return obj
```

### Comparing `cellrank-1.5.1/cellrank/tl/_mixins/_kernel.py` & `cellrank-2.0.0/src/cellrank/estimators/mixins/_kernel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Tuple, Union, TypeVar, Optional
+from typing import Any, Optional, Tuple, TypeVar, Union
 
-from abc import ABC
+import numpy as np
+import scipy.sparse as sp
 
 from anndata import AnnData
 
-import numpy as np
-from scipy.sparse import spmatrix
+__all__ = ["KernelMixin"]
 
-KernelExpression = TypeVar("KernelExpression")
+KernelExpression = TypeVar("KernelExpression", bound="KernelMixin")
 
 
-class KernelMixin(ABC):
+class KernelMixin:
     """Mixin that exposes various properties of :class:`cellrank.kernels.KernelExpression`."""
 
     def __init__(self, kernel: "KernelExpression", **kwargs: Any):
         super().__init__(**kwargs)
         self._kernel = kernel
         self._n_obs = self.kernel.adata.n_obs
 
@@ -37,15 +37,15 @@
     def adata(self, adata: Optional[AnnData]) -> None:
         self.kernel.adata = adata
 
     def __len__(self) -> int:
         return self._n_obs
 
     @property
-    def transition_matrix(self) -> Union[np.ndarray, spmatrix]:
-        """Transition matrix of :attr:`kernel`."""
+    def transition_matrix(self) -> Union[np.ndarray, sp.spmatrix]:
+        """Transition matrix of the :attr:`kernel`."""
         return self.kernel.transition_matrix
 
     @property
     def backward(self) -> bool:
-        """Direction of :attr:`kernel`."""
+        """Direction of the :attr:`kernel`."""
         return self.kernel.backward
```

### Comparing `cellrank-1.5.1/cellrank/tl/_utils.py` & `cellrank-2.0.0/src/cellrank/_utils/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,239 +1,242 @@
+import contextlib
+import functools
+import inspect
+import itertools
+import os
+import types
+import warnings
 from typing import (
     Any,
-    Dict,
-    List,
-    Tuple,
-    Union,
-    TypeVar,
     Callable,
+    Dict,
     Hashable,
     Iterable,
+    List,
+    Literal,
     Optional,
     Sequence,
+    Tuple,
+    TypeVar,
+    Union,
 )
-from typing_extensions import Literal
 
-import os
 import wrapt
-import warnings
-from itertools import tee, product, combinations
+
+import numpy as np
+import pandas as pd
+import scipy.sparse as sp
+import scipy.stats as st
+from pandas.api.types import infer_dtype, is_categorical_dtype
+from sklearn.cluster import KMeans
 from statsmodels.stats.multitest import multipletests
 
+from matplotlib import colors
+
 import scanpy as sc
 from anndata import AnnData
+from anndata.utils import make_index_unique
+
 from cellrank import logging as logg
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d
-from cellrank.ul._utils import _get_neighs, _has_neighs, _get_neighs_params
-from cellrank.tl._colors import (
+from cellrank._utils._colors import (
     _compute_mean_color,
     _convert_to_hex_colors,
     _insert_categorical_colors,
 )
-from cellrank.ul._parallelize import parallelize
-from cellrank.tl._linear_solver import _solve_lin_system
-from cellrank.tl.kernels._utils import np_std, np_mean, _filter_kwargs
-
-import numpy as np
-import pandas as pd
-from pandas import Series
-from scipy.stats import norm
-from numpy.linalg import norm as d_norm
-from scipy.sparse import eye as speye
-from scipy.sparse import diags, issparse, spmatrix, csr_matrix, isspmatrix_csr
-from sklearn.cluster import KMeans
-from pandas.api.types import infer_dtype, is_bool_dtype, is_categorical_dtype
-from scipy.sparse.linalg import norm as sparse_norm
-
-import matplotlib.colors as mcolors
+from cellrank._utils._docs import d
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._linear_solver import _solve_lin_system
 
 ColorLike = TypeVar("ColorLike")
 GPCCA = TypeVar("GPCCA")
 CFLARE = TypeVar("CFLARE")
 DiGraph = TypeVar("DiGraph")
 
 EPS = np.finfo(np.float64).eps
 
 
-class TestMethod(ModeEnum):  # noqa
-    FISCHER = "fischer"
+class TestMethod(ModeEnum):
+    FISHER = "fisher"
     PERM_TEST = "perm_test"
 
 
 class RandomKeys:
-    """
-    Create random keys inside an :class:`anndata.AnnData` object.
+    """Create random keys inside an :class:`~anndata.AnnData` object.
 
     Parameters
     ----------
     adata
         Annotated data object.
     n
         Number of keys, If `None`, create just 1 keys.
     where
         Attribute of ``adata``. If `'obs'`, also clean up `'{key}_colors'` for each generated key.
+    seed
+        Random seed.
     """
 
-    def __init__(self, adata: AnnData, n: Optional[int] = None, where: str = "obs"):
+    def __init__(self, adata: AnnData, n: Optional[int] = None, where: str = "obs", seed: int = 0):
         self._adata = adata
         self._where = where
         self._n = n or 1
+        self._seed = seed
         self._keys = []
 
     def _generate_random_keys(self):
-        def generator():
-            return f"RNG_COL_{np.random.randint(2 ** 16)}"
-
+        rng = np.random.default_rng(self._seed)
         where = getattr(self._adata, self._where)
         names, seen = [], set(where.keys())
 
         while len(names) != self._n:
-            name = generator()
+            name = f"RNG_COL_{rng.integers(0, 2 ** 32 - 1)}"
             if name not in seen:
                 seen.add(name)
                 names.append(name)
 
         return names
 
     def __enter__(self):
         self._keys = self._generate_random_keys()
         return self._keys
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         for key in self._keys:
-            try:
-                getattr(self._adata, self._where).drop(
-                    key, axis="columns", inplace=True
-                )
-            except KeyError:
-                pass
+            with contextlib.suppress(KeyError):
+                getattr(self._adata, self._where).drop(key, axis="columns", inplace=True)
+
             if self._where == "obs":
-                try:
+                with contextlib.suppress(KeyError):
                     del self._adata.uns[f"{key}_colors"]
-                except KeyError:
-                    pass
+
+
+def _filter_kwargs(_fn: Callable, **kwargs: Any) -> dict:
+    """Filter keyword arguments.
+
+    Parameters
+    ----------
+    _fn
+        Function for which to filter keyword arguments.
+    kwargs
+        Keyword arguments to filter
+
+    Returns
+    -------
+    dict
+        Filtered keyword arguments for the given function.
+    """
+    sig = inspect.signature(_fn).parameters
+    return {k: v for k, v in kwargs.items() if k in sig}
 
 
 def _pairwise(iterable: Iterable) -> zip:
     """Return pairs of elements from an iterable."""
-    a, b = tee(iterable)
+    a, b = itertools.tee(iterable)
     next(b, None)
     return zip(a, b)
 
 
 def _min_max_scale(x: np.ndarray) -> np.ndarray:
-    """
-    Scale a 1D array to 0-1 range.
+    """Scale a 1D array to 0-1 range.
 
     Parameters
     ----------
     x
         Array to be scaled.
 
     Returns
     -------
-        The scaled array.
+    The scaled array.
     """
     minn, maxx = np.nanmin(x), np.nanmax(x)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", RuntimeWarning)
         return (x - minn) / (maxx - minn)
 
 
 def _process_series(
-    series: pd.Series, keys: Optional[List[str]], colors: Optional[np.array] = None
+    series: pd.Series, keys: Optional[List[str]], cols: Optional[np.array] = None
 ) -> Union[pd.Series, Tuple[pd.Series, List[str]]]:
-    """
-    Process :class:`pandas.Series` categorical objects.
+    """Process :class:`~pandas.Series` of categorical objects.
 
     Categories in ``series`` are combined/removed according to ``keys``,
     the same transformation is applied to the corresponding colors.
 
     Parameters
     ----------
     series
-        Input data, must be a pd.series of categorical type.
+        Input categorical data.
     keys
         Keys could be e.g. `['cat_1, cat_2', 'cat_4']`. If originally,
         there were 4 categories in `series`, then this would combine the first
         and the second and remove the third. The same would be done to `colors`,
         i.e. the first and second color would be merged (average color), while
         the third would be removed.
-    colors
+    cols
         List of colors which aligns with the order of the categories.
 
     Returns
     -------
-    :class:`pandas.Series`
-        Categorical updated annotation. Each cell is assigned to either
-        `NaN` or one of updated approximate recurrent classes.
-    list
-        Color list processed according to keys.
+    - Categorical updated annotation. Each cell is assigned to either
+      `NaN` or one of updated approximate recurrent classes.
+    - Color list processed according to keys.
     """
-
     # determine whether we want to process colors as well
-    process_colors = colors is not None
+    process_colors = cols is not None
+
+    # assert dtype of the series
+    if not is_categorical_dtype(series):
+        raise TypeError(f"Series must be `categorical`, found `{infer_dtype(series)}`.")
 
     # if keys is None, just return
     if keys is None:
         if process_colors:
-            return series, colors
+            return series, cols
         return series
 
-    # assert dtype of the series
-    if not is_categorical_dtype(series):
-        raise TypeError(f"Series must be `categorical`, found `{infer_dtype(series)}`.")
-
     # initialize a copy of the series object
     series_in = series.copy()
     if process_colors:
-        colors_in = np.array(colors.copy())
+        colors_in = np.array(cols.copy())
         if len(colors_in) != len(series_in.cat.categories):
             raise ValueError(
                 f"Length of colors ({len(colors_in)}) does not match length of "
                 f"categories ({len(series_in.cat.categories)})."
             )
-        if not all(mcolors.is_color_like(c) for c in colors_in):
+        if not all(colors.is_color_like(c) for c in colors_in):
             raise ValueError("Not all colors are color-like.")
 
     # define a set of keys
-    keys_ = {
-        tuple(sorted({key.strip(" ") for key in rc.strip(" ,").split(",")}))
-        for rc in keys
-    }
+    keys_ = {tuple(sorted({key.strip(" ") for key in rc.strip(" ,").split(",")})) for rc in keys}
 
     # check that the keys are unique
     overlap = [set(ks) for ks in keys_]
-    for c1, c2 in combinations(overlap, 2):
+    for c1, c2 in itertools.combinations(overlap, 2):
         overlap = c1 & c2
         if overlap:
             raise ValueError(f"Found overlapping keys: `{list(overlap)}`.")
 
     # check the `keys` are all proper categories
     remaining_cat = [b for a in keys_ for b in a]
     if not np.all(np.in1d(remaining_cat, series_in.cat.categories)):
-        raise ValueError(
-            "Not all keys are proper categories. Check for spelling mistakes in `keys`."
-        )
+        raise ValueError("Not all keys are proper categories. Check for spelling mistakes in `keys`.")
 
     # remove cats and colors according to keys
     n_remaining = len(remaining_cat)
     removed_cat = list(set(series_in.cat.categories) - set(remaining_cat))
     if process_colors:
         mask = np.in1d(series_in.cat.categories, remaining_cat)
         colors_temp = colors_in[mask].copy()
     series_temp = series_in.cat.remove_categories(removed_cat)
 
     # loop over all indiv. or combined rc's
     colors_mod = {}
     for cat in keys_:
         # if there are more than two keys in this category, combine them
         if len(cat) > 1:
-            new_cat_name = " or ".join(cat)
+            new_cat_name = ", ".join(cat)
             mask = np.repeat(False, len(series_temp))
             for key in cat:
                 mask = np.logical_or(mask, series_temp == key)
                 remaining_cat.remove(key)
             series_temp = series_temp.cat.add_categories(new_cat_name)
             remaining_cat.append(new_cat_name)
             series_temp[mask] = new_cat_name
@@ -249,43 +252,36 @@
 
     # Since we have just appended colors at the end, we must now delete the unused ones
     series_temp = series_temp.cat.remove_unused_categories()
     series_temp = series_temp.cat.reorder_categories(remaining_cat)
 
     if process_colors:
         # original colors can still be present, convert to hex
-        colors_temp = _convert_to_hex_colors(
-            [colors_mod[c] for c in series_temp.cat.categories]
-        )
+        colors_temp = _convert_to_hex_colors([colors_mod[c] for c in series_temp.cat.categories])
         return series_temp, colors_temp
 
     return series_temp
 
 
-def _complex_warning(
-    X: np.array, use: Union[list, int, tuple, range], use_imag: bool = False
-) -> np.ndarray:
-    """
-    Check for imaginary components in columns of X specified by ``use``.
+def _complex_warning(X: np.array, use: Union[list, int, tuple, range], use_imag: bool = False) -> np.ndarray:
+    """Check for imaginary components in columns of X specified by ``use``.
 
     Parameters
     ----------
     X
         Matrix containing the eigenvectors.
     use
         Selection of columns of `X`.
     use_imag
         For eigenvectors that are complex, use real or imaginary part.
 
     Returns
     -------
-    class:`numpy.ndarray`
-        An array containing either only real eigenvectors or also complex ones.
+    An array containing either only real eigenvectors or also complex ones.
     """
-
     complex_mask = np.sum(X.imag != 0, axis=0) > 0
     complex_ixs = np.array(use)[np.where(complex_mask)[0]]
     complex_key = "imaginary" if use_imag else "real"
     if len(complex_ixs) > 0:
         logg.warning(
             f"The eigenvectors with indices `{list(complex_ixs)}` have an imaginary part. "
             f"Showing their {complex_key} part"
@@ -294,33 +290,33 @@
     if use_imag:
         X_[:, complex_mask] = X.imag[:, complex_mask]
 
     return X_
 
 
 def _mat_mat_corr_sparse(
-    X: csr_matrix,
+    X: sp.csr_matrix,
     Y: np.ndarray,
 ) -> np.ndarray:
     n = X.shape[1]
 
     X_bar = np.reshape(np.array(X.mean(axis=1)), (-1, 1))
-    X_std = np.reshape(
-        np.sqrt(np.array(X.power(2).mean(axis=1)) - (X_bar ** 2)), (-1, 1)
-    )
+    X_std = np.reshape(np.sqrt(np.array(X.power(2).mean(axis=1)) - (X_bar**2)), (-1, 1))
 
     y_bar = np.reshape(np.mean(Y, axis=0), (1, -1))
     y_std = np.reshape(np.std(Y, axis=0), (1, -1))
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore", RuntimeWarning)
         return (X @ Y - (n * X_bar * y_bar)) / ((n - 1) * X_std * y_std)
 
 
 def _mat_mat_corr_dense(X: np.ndarray, Y: np.ndarray) -> np.ndarray:
+    from cellrank.kernels._utils import np_mean, np_std
+
     n = X.shape[1]
 
     X_bar = np.reshape(np_mean(X, axis=1), (-1, 1))
     X_std = np.reshape(np_std(X, axis=1), (-1, 1))
 
     y_bar = np.reshape(np_mean(Y, axis=0), (1, -1))
     y_std = np.reshape(np_std(Y, axis=0), (1, -1))
@@ -329,25 +325,25 @@
         warnings.simplefilter("ignore", RuntimeWarning)
         return (X @ Y - (n * X_bar * y_bar)) / ((n - 1) * X_std * y_std)
 
 
 def _perm_test(
     ixs: np.ndarray,
     corr: np.ndarray,
-    X: Union[np.ndarray, spmatrix],
+    X: Union[np.ndarray, sp.spmatrix],
     Y: np.ndarray,
     seed: Optional[int] = None,
     queue=None,
 ) -> Tuple[np.ndarray, np.ndarray]:
     rs = np.random.RandomState(None if seed is None else seed + ixs[0])
     cell_ixs = np.arange(X.shape[1])
     pvals = np.zeros_like(corr, dtype=np.float64)
     corr_bs = np.zeros((len(ixs), X.shape[0], Y.shape[1]))  # perms x genes x lineages
 
-    mmc = _mat_mat_corr_sparse if issparse(X) else _mat_mat_corr_dense
+    mmc = _mat_mat_corr_sparse if sp.issparse(X) else _mat_mat_corr_dense
 
     for i, _ in enumerate(ixs):
         rs.shuffle(cell_ixs)
         corr_i = mmc(X, Y[cell_ixs, :])
         pvals += np.abs(corr_i) >= np.abs(corr)
 
         bootstrap_ixs = rs.choice(cell_ixs, replace=True, size=len(cell_ixs))
@@ -361,160 +357,163 @@
 
     return pvals, corr_bs
 
 
 @d.get_sections(base="correlation_test", sections=["Returns"])
 @d.dedent
 def _correlation_test(
-    X: Union[np.ndarray, spmatrix],
+    X: Union[np.ndarray, sp.spmatrix],
     Y: "Lineage",  # noqa: F821
     gene_names: Sequence[str],
-    method: TestMethod = TestMethod.FISCHER,
+    method: TestMethod = TestMethod.FISHER,
     confidence_level: float = 0.95,
     n_perms: Optional[int] = None,
     seed: Optional[int] = None,
     **kwargs: Any,
 ) -> pd.DataFrame:
-    """
-    Perform a statistical test.
+    """Perform a statistical test.
 
     Return NaN for genes which don't vary across cells.
 
     Parameters
     ----------
     X
         Array or sparse matrix of shape ``(n_cells, n_genes)`` containing the expression.
     Y
-        Array of shape ``(n_cells, n_lineages)`` containing the absorption probabilities.
+        Array of shape ``(n_cells, n_lineages)`` containing the fate probabilities.
     gene_names
         Sequence of shape ``(n_genes,)`` containing the gene names.
     method
         Method for p-value calculation.
     confidence_level
-        Confidence level for the confidence interval calculation. Must be in `[0, 1]`.
+        Confidence level for the confidence interval calculation. Must be in :math:`[0, 1]`.
     n_perms
         Number of permutations if ``method = 'perm_test'``.
     seed
         Random seed if ``method = 'perm_test'``.
     %(parallel)s
 
     Returns
     -------
     Dataframe of shape ``(n_genes, n_lineages * 5)`` containing the following columns, one for each lineage:
 
-        - ``{lineage}_corr`` - correlation between the gene expression and absorption probabilities.
-        - ``{lineage}_pval`` - calculated p-values for double-sided test.
-        - ``{lineage}_qval`` - corrected p-values using Benjamini-Hochberg method at level `0.05`.
-        - ``{lineage}_ci_low`` - lower bound of the ``confidence_level`` correlation confidence interval.
-        - ``{lineage}_ci_high`` - upper bound of the ``confidence_level`` correlation confidence interval.
+    - ``'{lineage}_corr'`` - correlation between the gene expression and fate probabilities.
+    - ``'{lineage}_pval'`` - calculated p-values for double-sided test.
+    - ``'{lineage}_qval'`` - corrected p-values using Benjamini-Hochberg method at level `0.05`.
+    - ``'{lineage}_ci_low'`` - lower bound of the ``confidence_level`` correlation confidence interval.
+    - ``'{lineage}_ci_high'`` - upper bound of the ``confidence_level`` correlation confidence interval.
     """
-
     corr, pvals, ci_low, ci_high = _correlation_test_helper(
         X.T,
         Y.X,
         method=method,
         n_perms=n_perms,
         seed=seed,
         confidence_level=confidence_level,
         **kwargs,
     )
-    invalid = np.sum((corr < -1) | (corr > 1))
-    if invalid:
-        raise ValueError(f"Found `{invalid}` correlations that are not in `[0, 1]`.")
+    invalid = (corr < -1) | (corr > 1)
+    if np.any(invalid):
+        logg.warning(
+            f"Found `{np.sum(invalid)}` correlation(s) that are not in `[0, 1]`. "
+            f"This usually happens when gene expression is constant across all cells. "
+            f"Setting to `NaN`"
+        )
+        corr[invalid] = np.nan
+        pvals[invalid] = np.nan
+        ci_low[invalid] = np.nan
+        ci_high[invalid] = np.nan
 
     res = pd.DataFrame(corr, index=gene_names, columns=[f"{c}_corr" for c in Y.names])
     for idx, c in enumerate(Y.names):
-        res[f"{c}_pval"] = pvals[:, idx]
-        res[f"{c}_qval"] = multipletests(pvals[:, idx], alpha=0.05, method="fdr_bh")[1]
+        p = pvals[:, idx]
+        valid_mask = ~np.isnan(p)
+
+        res[f"{c}_pval"] = p
+        res[f"{c}_qval"] = np.nan
+        if np.any(valid_mask):
+            res.loc[gene_names[valid_mask], f"{c}_qval"] = multipletests(p[valid_mask], alpha=0.05, method="fdr_bh")[1]
         res[f"{c}_ci_low"] = ci_low[:, idx]
         res[f"{c}_ci_high"] = ci_high[:, idx]
 
     # fmt: off
     res = res[[f"{c}_{stat}" for c in Y.names for stat in ("corr", "pval", "qval", "ci_low", "ci_high")]]
     return res.sort_values(by=[f"{c}_corr" for c in Y.names], ascending=False)
     # fmt: on
 
 
 def _correlation_test_helper(
-    X: Union[np.ndarray, spmatrix],
+    X: Union[np.ndarray, sp.spmatrix],
     Y: np.ndarray,
-    method: TestMethod = TestMethod.FISCHER,
+    method: TestMethod = TestMethod.FISHER,
     n_perms: Optional[int] = None,
     seed: Optional[int] = None,
     confidence_level: float = 0.95,
-    **kwargs,
+    **kwargs: Any,
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, np.ndarray]:
-    """
-    Compute the correlation between rows in matrix ``X`` columns of matrix ``Y``.
+    """Compute the correlation between rows in matrix ``X`` columns of matrix ``Y``.
 
     Parameters
     ----------
     X
         Array or matrix of `(M, N)` elements.
     Y
         Array of `(N, K)` elements.
     method
         Method for p-value calculation.
     n_perms
         Number of permutations if ``method='perm_test'``.
     seed
-        Random seed if ``method='perm_test'``.
+        Random seed if ``method = 'perm_test'``.
     confidence_level
         Confidence level for the confidence interval calculation. Must be in `[0, 1]`.
     kwargs
-        Keyword arguments for :func:`cellrank.ul._parallelize.parallelize`.
+        Keyword arguments for :func:`cellrank._utils._parallelize.parallelize`.
 
     Returns
     -------
         Correlations, p-values, corrected p-values, lower and upper bound of 95% confidence interval.
         Each array if of shape ``(n_genes, n_lineages)``.
     """
+    from cellrank._utils._parallelize import parallelize
 
-    def perm_test_extractor(
-        res: Sequence[Tuple[np.ndarray, np.ndarray]]
-    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    def perm_test_extractor(res: Sequence[Tuple[np.ndarray, np.ndarray]]) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         pvals, corr_bs = zip(*res)
         pvals = np.sum(pvals, axis=0) / float(n_perms)
 
         corr_bs = np.concatenate(corr_bs, axis=0)
-        corr_ci_low, corr_ci_high = np.quantile(corr_bs, q=ql, axis=0), np.quantile(
-            corr_bs, q=qh, axis=0
-        )
+        corr_ci_low, corr_ci_high = np.quantile(corr_bs, q=ql, axis=0), np.quantile(corr_bs, q=qh, axis=0)
 
         return pvals, corr_ci_low, corr_ci_high
 
     if not (0 <= confidence_level <= 1):
-        raise ValueError(
-            f"Expected `confidence_level` to be in interval `[0, 1]`, found `{confidence_level}`."
-        )
+        raise ValueError(f"Expected `confidence_level` to be in interval `[0, 1]`, found `{confidence_level}`.")
 
     n = X.shape[1]  # genes x cells
     ql = 1 - confidence_level - (1 - confidence_level) / 2.0
     qh = confidence_level + (1 - confidence_level) / 2.0
 
-    if issparse(X) and not isspmatrix_csr(X):
-        X = csr_matrix(X)
+    if sp.issparse(X) and not sp.isspmatrix_csr(X):
+        X = sp.csr_matrix(X)
 
-    corr = _mat_mat_corr_sparse(X, Y) if issparse(X) else _mat_mat_corr_dense(X, Y)
+    corr = _mat_mat_corr_sparse(X, Y) if sp.issparse(X) else _mat_mat_corr_dense(X, Y)
 
-    if method == TestMethod.FISCHER:
+    if method == TestMethod.FISHER:
         # see: https://en.wikipedia.org/wiki/Pearson_correlation_coefficient#Using_the_Fisher_transformation
         mean, se = np.arctanh(corr), 1.0 / np.sqrt(n - 3)
         z_score = (np.arctanh(corr) - np.arctanh(0)) * np.sqrt(n - 3)
 
-        z = norm.ppf(qh)
+        z = st.norm.ppf(qh)
         corr_ci_low = np.tanh(mean - z * se)
         corr_ci_high = np.tanh(mean + z * se)
-        pvals = 2 * norm.cdf(-np.abs(z_score))
+        pvals = 2 * st.norm.cdf(-np.abs(z_score))
 
     elif method == TestMethod.PERM_TEST:
         if not isinstance(n_perms, int):
-            raise TypeError(
-                f"Expected `n_perms` to be an integer, found `{type(n_perms).__name__!r}`."
-            )
+            raise TypeError(f"Expected `n_perms` to be an integer, found `{type(n_perms).__name__}`.")
         if n_perms <= 0:
             raise ValueError(f"Expcted `n_perms` to be positive, found `{n_perms}`.")
 
         pvals, corr_ci_low, corr_ci_high = parallelize(
             _perm_test,
             np.arange(n_perms),
             as_array=False,
@@ -525,35 +524,18 @@
 
     else:
         raise NotImplementedError(method)
 
     return corr, pvals, corr_ci_low, corr_ci_high
 
 
-def _make_cat(
-    labels: List[List[Any]], n_states: int, state_names: Sequence[str]
-) -> Series:
-    """Get categorical from list of lists."""
-
-    labels_new = np.repeat(np.nan, n_states)
-    for i, c in enumerate(labels):
-        labels_new[c] = i
-    labels_new = Series(labels_new, index=state_names, dtype="category")
-    labels_new.cat.categories = labels_new.cat.categories.astype("int")
-
-    return labels_new
-
-
-def _filter_cells(distances: spmatrix, rc_labels: Series, n_matches_min: int) -> Series:
+def _filter_cells(distances: sp.spmatrix, rc_labels: pd.Series, n_matches_min: int) -> pd.Series:
     """Filter out some cells that look like transient states based on their neighbors."""
-
     if not is_categorical_dtype(rc_labels):
-        raise TypeError(
-            f"Expected `categories` be `categorical`, found `{infer_dtype(rc_labels)}`."
-        )
+        raise TypeError(f"Expected `categories` be `categorical`, found `{infer_dtype(rc_labels)}`.")
 
     # retrieve knn graph
     rows, cols = distances.nonzero()
     cls = rc_labels.cat.categories
     freqs_orig = np.array([np.sum(rc_labels == cl) for cl in cls])
 
     # loop over cells and check whether they have neighbors from the same class
@@ -575,22 +557,21 @@
             "increasing 'n_neighbors_filtering'. This filters out too many cells"
         )
 
     return rc_labels
 
 
 def _cluster_X(
-    X: Union[np.ndarray, spmatrix],
+    X: Union[np.ndarray, sp.spmatrix],
     n_clusters: int,
     method: Literal["leiden", "kmeans"] = "leiden",
     n_neighbors: int = 20,
     resolution: float = 1.0,
 ) -> List[Any]:
-    """
-    Cluster the rows of the matrix X.
+    """Cluster the rows of ``X``.
 
     Parameters
     ----------
     X
         Matrix of shape ``n_samples x n_features``.
     n_clusters
         Number of clusters to use.
@@ -599,304 +580,265 @@
     n_neighbors
         If using a community-detection based clustering algorithm, number of neighbors for KNN construction.
     resolution
         Resolution parameter for `'leiden'` clustering.
 
     Returns
     -------
-    :class:`list`
-        List of cluster labels of length `n_samples`.
+    List of cluster labels of length `n_samples`.
     """
     if X.shape[0] == 1:
-        # sc.tl.leiden issue
+        # leiden issue
         return [0]
 
     if method == "kmeans":
         kmeans = KMeans(n_clusters=n_clusters).fit(X)
         labels = kmeans.labels_
     elif method == "leiden":
         adata_dummy = sc.AnnData(X=X)
         sc.pp.neighbors(adata_dummy, use_rep="X", n_neighbors=n_neighbors)
         sc.tl.leiden(adata_dummy, resolution=resolution)
         labels = adata_dummy.obs[method]
     else:
-        raise NotImplementedError(
-            f"Invalid method `{method}`. Valid options are `kmeans` or `leiden`."
-        )
+        raise NotImplementedError(f"Invalid method `{method}`. Valid options are `kmeans` or `leiden`.")
 
     return list(labels)
 
 
 def _eigengap(evals: np.ndarray, alpha: float) -> int:
-    """
-    Compute the eigengap among the top eigenvalues of a matrix.
+    """Compute the eigengap among the top eigenvalues of a matrix.
 
     Parameters
     ----------
     evals
         Sorted array of real numbers. If complex, take their real part.
     alpha
         Determines how much weight is given to the deviation of an eigenvalue from one.
 
     Returns
     -------
-    int
-        Number of eigenvectors to be used.
+    Number of eigenvectors to be used.
     """
-
     if np.iscomplexobj(evals):
         evals = evals.real
     evals = np.sort(evals)[::-1]  # they could be ordered by LM, not LR
 
     gap, eps = evals[:-1] - evals[1:], (1 - evals)[:-1]
     J = gap - alpha * eps
 
     return int(np.argmax(J))
 
 
 def _partition(
-    conn: Union[DiGraph, np.ndarray, spmatrix], sort: bool = True
+    conn: Union[DiGraph, np.ndarray, sp.spmatrix], sort: bool = True
 ) -> Tuple[List[List[Any]], List[List[Any]]]:
-    """
-    Partition a directed graph into its transient and recurrent classes.
+    """Partition a directed graph into its transient and recurrent classes.
 
     In a directed graph *G*, node *j* is accessible from node *i* if there exists a path from *i* to *j*.
     If *i* is accessible from *j* and the converse holds as well, then *i* and *j* communicate.
     Communication forms and equivalence relation on directed graphs, so every directed graph can be uniquely partitioned
     into its communication classes (also called strongly connected components).
 
     If *G* describes the state space of a Markov chain, then communication classes are often
     characterized as either recurrent or transient. Intuitively, once the process enters a recurrent class, it will
     never leave it again.
 
     Parameters
     ----------
     conn
-        Directed graph to _partition.
+        Directed graph to partition.
 
     Returns
     -------
-    :class:`list`, :class:`list`
-        Recurrent and transient classes, respectively.
+    Recurrent and transient classes, respectively.
     """
-
     import networkx as nx
 
     start = logg.debug("Partitioning the graph into current and transient classes")
 
     def partition(g):
         yield from (
             (
                 (sorted(scc) if sort else scc),
-                all((not nx.has_path(g, s, t) for s, t in product(scc, g.nodes - scc))),
+                all((not nx.has_path(g, s, t) for s, t in itertools.product(scc, g.nodes - scc))),
             )
             for scc in nx.strongly_connected_components(g)
         )
 
     def maybe_sort(iterable):
-        return (
-            sorted(iterable, key=lambda x: (-len(x), x[0]))
-            if sort
-            else list(map(list, iterable))
-        )
+        return sorted(iterable, key=lambda x: (-len(x), x[0])) if sort else list(map(list, iterable))
 
-    rec_classes, trans_classes = tee(
+    rec_classes, trans_classes = itertools.tee(
         partition(nx.DiGraph(conn) if not isinstance(conn, nx.DiGraph) else conn), 2
     )
 
     rec_classes = (node for node, is_rec in rec_classes if is_rec)
     trans_classes = (node for node, is_rec in trans_classes if not is_rec)
 
     logg.debug("    Finish", time=start)
 
     return maybe_sort(rec_classes), maybe_sort(trans_classes)
 
 
-def _connected(c: Union[spmatrix, np.ndarray]) -> bool:
-    """Check whether the undirected graph encoded by c is connected."""
-
+def _connected(c: Union[sp.spmatrix, np.ndarray]) -> bool:
+    """Check whether the undirected graph is connected."""
     import networkx as nx
 
-    G = nx.from_scipy_sparse_matrix(c) if issparse(c) else nx.from_numpy_array(c)
+    if sp.issparse(c):
+        try:
+            G = nx.from_scipy_sparse_array(c)
+        except AttributeError:
+            # bwd compatibility for `networkx <2.7`
+            G = nx.from_scipy_sparse_matrix(c)
+    else:
+        G = nx.from_numpy_array(c)
 
     return nx.is_connected(G)
 
 
-def _irreducible(d: Union[spmatrix, np.ndarray]) -> bool:
-    """Check whether the unirected graph encoded by d is irreducible."""
-
+def _irreducible(d: Union[sp.spmatrix, np.ndarray]) -> bool:
+    """Check whether the undirected graph encoded by d is irreducible."""
     import networkx as nx
 
-    start = logg.debug("Checking the transition matrix for irreducibility")
-
     G = nx.DiGraph(d) if not isinstance(d, nx.DiGraph) else d
-
     try:
         it = iter(nx.strongly_connected_components(G))
         _ = next(it)
         _ = next(it)
-        is_irreducible = False
+        return False
     except StopIteration:
-        is_irreducible = True
-
-    if not is_irreducible:
-        logg.warning("Transition matrix is not irreducible", time=start)
-    else:
-        logg.debug("Transition matrix is irreducible", time=start)
-
-    return is_irreducible
+        return True
 
 
 def _symmetric(
-    matrix: Union[spmatrix, np.ndarray],
+    matrix: Union[sp.spmatrix, np.ndarray],
     ord: str = "fro",
     eps: float = 1e-4,
     only_check_sparsity_pattern: bool = False,
 ) -> bool:
     """Check whether the graph encoded by `matrix` is symmetric."""
     if only_check_sparsity_pattern:
-        if issparse(matrix):
+        if sp.issparse(matrix):
             return len(((matrix != 0) - (matrix != 0).T).data) == 0
         return ((matrix != 0) == (matrix != 0).T).all()
 
-    if issparse(matrix):
-        return sparse_norm((matrix - matrix.T), ord=ord) < eps
-    return d_norm((matrix - matrix.T), ord=ord) < eps
+    if sp.issparse(matrix):
+        return sp.linalg.norm((matrix - matrix.T), ord=ord) < eps
+    return np.linalg.norm((matrix - matrix.T), ord=ord) < eps
 
 
 def _normalize(
-    X: Union[np.ndarray, spmatrix],
-) -> Union[np.ndarray, spmatrix]:
-    """
-    Row-normalizes an array to sum to 1.
+    X: Union[np.ndarray, sp.spmatrix],
+) -> Union[np.ndarray, sp.spmatrix]:
+    """Row-normalizes an array to sum to :math:`1`.
 
     Parameters
     ----------
     X
         Array to be normalized.
 
     Returns
     -------
     :class:`numpy.ndarray` or :class:`scipy.sparse.spmatrix`
         The normalized array.
     """
-
     with np.errstate(divide="ignore"):
-        if issparse(X):
-            return X.multiply(csr_matrix(1.0 / np.abs(X).sum(1)))
+        if sp.issparse(X):
+            return X.multiply(sp.csr_matrix(1.0 / np.abs(X).sum(1)))
         X = np.array(X)
         return X / (X.sum(1)[:, None])
 
 
 def _get_connectivities(
     adata: AnnData, mode: str = "connectivities", n_neighbors: Optional[int] = None
-) -> Optional[spmatrix]:
+) -> Optional[sp.spmatrix]:
     # utility function, copied from scvelo
     if _has_neighs(adata):
         C = _get_neighs(adata, mode)
-        if (
-            n_neighbors is not None
-            and n_neighbors <= _get_neighs_params(adata)["n_neighbors"]
-        ):
+        if n_neighbors is not None and n_neighbors <= _get_neighs_params(adata)["n_neighbors"]:
             C = (
                 _select_connectivities(C, n_neighbors)
                 if mode == "connectivities"
                 else _select_distances(C, n_neighbors)
             )
 
         return C.tocsr().astype(np.float32)
 
 
-def _select_connectivities(
-    connectivities: spmatrix, n_neighbors: Optional[int] = None
-) -> spmatrix:
+def _select_connectivities(connectivities: sp.spmatrix, n_neighbors: Optional[int] = None) -> sp.spmatrix:
     # utility function, copied from scvelo
     C = connectivities.copy()
-    n_counts = (C > 0).sum(1).A1 if issparse(C) else (C > 0).sum(1)
-    n_neighbors = (
-        n_counts.min() if n_neighbors is None else min(n_counts.min(), n_neighbors)
-    )
+    n_counts = (C > 0).sum(1).A1 if sp.issparse(C) else (C > 0).sum(1)
+    n_neighbors = n_counts.min() if n_neighbors is None else min(n_counts.min(), n_neighbors)
     rows = np.where(n_counts > n_neighbors)[0]
     cumsum_neighs = np.insert(n_counts.cumsum(), 0, 0)
     dat = C.data
 
     for row in rows:
         n0, n1 = cumsum_neighs[row], cumsum_neighs[row + 1]
         rm_idx = n0 + dat[n0:n1].argsort()[::-1][n_neighbors:]
         dat[rm_idx] = 0
     C.eliminate_zeros()
 
     return C
 
 
-def _select_distances(dist, n_neighbors: Optional[int] = None) -> spmatrix:
-    # utility funtion, copied from scvelo
+def _select_distances(dist, n_neighbors: Optional[int] = None) -> sp.spmatrix:
+    # utility function, copied from scvelo
     D = dist.copy()
-    n_counts = (D > 0).sum(1).A1 if issparse(D) else (D > 0).sum(1)
-    n_neighbors = (
-        n_counts.min() if n_neighbors is None else min(n_counts.min(), n_neighbors)
-    )
+    n_counts = (D > 0).sum(1).A1 if sp.issparse(D) else (D > 0).sum(1)
+    n_neighbors = n_counts.min() if n_neighbors is None else min(n_counts.min(), n_neighbors)
     rows = np.where(n_counts > n_neighbors)[0]
     cumsum_neighs = np.insert(n_counts.cumsum(), 0, 0)
     dat = D.data
 
     for row in rows:
         n0, n1 = cumsum_neighs[row], cumsum_neighs[row + 1]
         rm_idx = n0 + dat[n0:n1].argsort()[n_neighbors:]
         dat[rm_idx] = 0
     D.eliminate_zeros()
 
     return D
 
 
 def _maybe_create_dir(dirpath: Union[str, os.PathLike]) -> None:
-    """
-    Try creating a directory if it does not already exist.
+    """Try creating a directory if it does not already exist.
 
     Parameters
     ----------
     dirpath
         Path of the directory to create.
 
     Returns
     -------
-    None
-        Nothing, just creates a directory if it doesn't exist.
+    Nothing, just creates a directory if it doesn't exist.
     """
-
     if not os.path.exists(dirpath) or not os.path.isdir(dirpath):
-        try:
+        with contextlib.suppress(OSError):
             os.makedirs(dirpath, exist_ok=True)
-        except OSError:
-            pass
 
 
-def save_fig(
-    fig, path: Union[str, os.PathLike], make_dir: bool = True, ext: str = "png"
-) -> None:
-    """
-    Save a plot.
+def save_fig(fig, path: Union[str, os.PathLike], make_dir: bool = True, ext: str = "png") -> None:
+    """Save a plot.
 
     Parameters
     ----------
-    fig: :class:`matplotlib.figure.Figure`
+    fig
         Figure to save.
-    path:
+    path
         Path where to save the figure. If path is relative, save it under ``cellrank.settings.figdir``.
-    make_dir:
+    make_dir
         Whether to try making the directory if it does not exist.
-    ext:
+    ext
         Extension to use.
 
     Returns
     -------
-    None
-        Just saves the plot.
+    Just saves the plot.
     """
-
     from cellrank import settings
 
     if os.path.splitext(path)[1] == "":
         path = f"{path}.{ext}"
 
     if not os.path.isabs(path):
         path = os.path.join(settings.figdir, path)
@@ -907,31 +849,28 @@
     logg.debug(f"Saving figure to `{path!r}`")
 
     fig.savefig(path, bbox_inches="tight", transparent=True)
 
 
 def _convert_to_categorical_series(
     term_states: Dict[Union[int, str], Sequence[Union[int, str]]], cell_names: List[str]
-) -> Series:
-    """
-    Convert a mapping of terminal states to cells to a :class:`pandas.Series`.
+) -> pd.Series:
+    """Convert a mapping of terminal states to cells to a :class:`~pandas.Series`.
 
     Parameters
     ----------
     term_states
         Terminal states in the following format: `{'state_0': ['cell_0', 'cell_1', ...], ...}`.
     cell_names
-        List of valid cell names, usually taken from ``adata.obs_names``.
+        List of valid cell names, usually taken from :attr:`~anndata.AnnData.obs_names`.
 
     Returns
     -------
-    :class:`pandas.Series`
-        Categorical series where `NaN` mark cells which do not belong to any recurrent class.
+    Categorical series where `NaN` mark cells which do not belong to any recurrent class.
     """
-
     cnames = set(cell_names)
     mapper, expected_size = {}, 0
     for ts, cells in term_states.items():
         if not len(cells):
             logg.warning(f"No cells selected for category `{ts!r}`. Skipping")
             continue
         cells = [c if isinstance(c, str) else cell_names[c] for c in cells]
@@ -943,15 +882,15 @@
 
     if len(mapper) != expected_size:
         raise ValueError(
             "All terminal states are being converted to strings, ensure "
             "that there are no conflicting keys, such as `0` and `'0'`."
         )
 
-    term_states = Series([np.nan] * len(cell_names), index=cell_names)
+    term_states = pd.Series([np.nan] * len(cell_names), index=cell_names)
     for ts, cells in mapper.items():
         term_states[cells] = ts
 
     term_states = term_states.astype("category")
     if not len(term_states.cat.categories):
         raise ValueError("No categories have been selected.")
 
@@ -961,16 +900,15 @@
 def _merge_categorical_series(
     old: pd.Series,
     new: pd.Series,
     colors_old: Union[List[ColorLike], np.ndarray, Dict[Any, ColorLike]] = None,
     colors_new: Union[List[ColorLike], np.ndarray, Dict[Any, ColorLike]] = None,
     color_overwrite: bool = False,
 ) -> Optional[Union[pd.Series, Tuple[pd.Series, np.ndarray]]]:
-    """
-    Update categorical :class:`pandas.Series.` with new information.
+    """Update categorical :class:`~pandas.Series` with new information.
 
     It **can never remove** old categories, only add to the existing ones.
     Optionally, new colors can be created or merged.
 
     Parameters
     ----------
     old
@@ -982,68 +920,54 @@
     colors_new
         Colors associated with new categories.
     color_overwrite
         If `True`, overwrite the old colors with new ones for overlapping categories.
 
     Returns
     -------
-    :class:`pandas.Series`
-        Returns the modified approximate recurrent classes and if ``colors_old`` and ``colors_new`` are both `None`.
-    :class:`pandas.Series`, :class:`numpy.ndarray`
-        If any of ``colors_old``, ``colors_new`` contain the new colors.
+    - Returns the modified approximate recurrent classes and if ``colors_old`` and ``colors_new`` are both `None`.
+    - If any of ``colors_old``, ``colors_new`` contain the new colors.
     """
 
     def get_color_mapper(
         series: pd.Series,
-        colors: Union[List[ColorLike], np.ndarray, Dict[Any, ColorLike]],
+        cols: Union[List[ColorLike], np.ndarray, Dict[Any, ColorLike]],
     ):
-        if len(series.cat.categories) != len(colors):
-            raise ValueError(
-                f"Series ({len(series.cat.categories)}) and colors ({len(colors_new)}) differ in length."
-            )
+        if len(series.cat.categories) != len(cols):
+            raise ValueError(f"Series ({len(series.cat.categories)}) and colors ({len(colors_new)}) differ in length.")
 
-        if isinstance(colors, dict):
-            if set(series.cat.categories) != set(colors.keys()):
-                raise ValueError(
-                    "Color mapper and series' categories don't share the keys."
-                )
+        if isinstance(cols, dict):
+            if set(series.cat.categories) != set(cols.keys()):
+                raise ValueError("Color mapper and series' categories don't share the keys.")
         else:
-            colors = dict(zip(series.cat.categories, colors))
+            cols = dict(zip(series.cat.categories, cols))
 
-        for color in colors.values():
-            if not mcolors.is_color_like(color):
+        for color in cols.values():
+            if not colors.is_color_like(color):
                 raise ValueError(f"Color `{color}` is not color-like.")
 
-        return colors
+        return cols
 
     if not is_categorical_dtype(old):
-        raise TypeError(
-            f"Expected old approx. recurrent classes to be categorical, found "
-            f"`{infer_dtype(old)}`."
-        )
+        raise TypeError(f"Expected old approx. recurrent classes to be categorical, found " f"`{infer_dtype(old)}`.")
 
     if not is_categorical_dtype(new):
-        raise TypeError(
-            f"Expected new approx. recurrent classes to be categorical, found "
-            f"`{infer_dtype(new)}`."
-        )
+        raise TypeError(f"Expected new approx. recurrent classes to be categorical, found " f"`{infer_dtype(new)}`.")
 
     if (old.index != new.index).any():
         raise ValueError("Index for old and new approx. recurrent classes differ.")
 
     old, new = old.copy(), new.copy()
     mask = ~new.isna()
     if np.sum(mask) == 0:
         return old
 
     old_cats = old.cat.categories
     new_cats = new.cat.categories
-    cats_to_add = (
-        pd.CategoricalIndex(new.loc[mask]).remove_unused_categories().categories
-    )
+    cats_to_add = pd.CategoricalIndex(new.loc[mask]).remove_unused_categories().categories
 
     if not colors_old and colors_new:
         colors_old = _insert_categorical_colors(
             list(colors_new.values()) if isinstance(colors_new, dict) else colors_new,
             len(old_cats),
         )
     if not colors_new and colors_old:
@@ -1063,70 +987,47 @@
 
     old.loc[mask] = new.loc[mask]
     old = old.cat.remove_unused_categories()
 
     if not colors_old and not colors_new:
         return old
 
-    colors_merged = (
-        {**colors_old, **colors_new}
-        if color_overwrite
-        else {**colors_new, **colors_old}
-    )
+    colors_merged = {**colors_old, **colors_new} if color_overwrite else {**colors_new, **colors_old}
     colors_merged = np.array([colors_merged[c] for c in old.cat.categories])
 
     return old, colors_merged
 
 
 def _unique_order_preserving(iterable: Iterable[Hashable]) -> List[Hashable]:
     """Remove items from an iterable while preserving the order."""
     seen = set()
     return [i for i in iterable if i not in seen and not seen.add(i)]
 
 
-def _convert_lineage_name(names: str) -> Tuple[str, ...]:
-    sep = "or" if "or" in names else ","
-    return tuple(
-        sorted({name.strip(" ") for name in names.strip(f" {sep}").split(sep)})
-    )
-
-
-def _info_if_obs_keys_categorical_present(
-    adata: AnnData, keys: Iterable[str], msg_fmt: str, warn_once: bool = True
-) -> None:
-    for key in keys:
-        if key in adata.obs.keys() and is_categorical_dtype(adata.obs[key]):
-            logg.info(msg_fmt.format(key))
-            if warn_once:
-                break
-
-
 def _one_hot(n, cat: Optional[int] = None) -> np.ndarray:
     """
     One-hot encode cat to a vector of length n.
 
     If cat is `None`, return a vector of zeros.
     """
-
     out = np.zeros(n, dtype=bool)
     if cat is not None:
         out[cat] = True
 
     return out
 
 
 def _fuzzy_to_discrete(
     a_fuzzy: np.array,
     n_most_likely: int = 10,
     remove_overlap: bool = True,
     raise_threshold: Optional[float] = 0.2,
     check_row_sums: bool = True,
 ) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    Map fuzzy clustering to discrete clustering.
+    """Map fuzzy clustering to discrete clustering.
 
     Given a fuzzy clustering of `n_samples` samples represented by a matrix ``a_fuzzy`` of shape
     `(n_samples x n_clusters)` where rows sum to one and indicate cluster membership to each of
     the `c_clusters` clusters, we compute an assignment of a subset of samples to clusters such
     that each cluster is represented by its ``n_most_likely`` most likely samples. In case a sample
     is assigned more than once, it can either be removed (``remove_overlap=True``) or it can be
     assigned to the cluster it most likely belongs to (``remove_overlap=False``). In case this
@@ -1154,248 +1055,187 @@
         exception. Set to `None` if you only want to raise if there is an empty cluster.
     check_row_sums
         Check whether rows in `a_fuzzy` sum to one. The one situation where we don't do this is when
         we have selected a couple of main states and we don't want to re-distribute probability mass.
 
     Returns
     -------
-    :class:`numpy.ndarray`m :class:`numpy.ndarray`
-        Boolean matrix of the same shape as `a_fuzzy`, assigning a subset of the samples to clusters and
-        an rray of clusters with less than `n_most_likely` samples assigned, respectively.
+    Boolean matrix of the same shape as `a_fuzzy`, assigning a subset of the samples to clusters and
+    an array of clusters with less than `n_most_likely` samples assigned, respectively.
     """
-
     # check the inputs
     n_samples, n_clusters = a_fuzzy.shape
     if not isinstance(a_fuzzy, np.ndarray):
-        raise TypeError(
-            f"Expected `a_fuzzy` to be of type `numpy.ndarray`, got `{type(a_fuzzy).__name__!r}`."
-        )
+        raise TypeError(f"Expected `a_fuzzy` to be of type `numpy.ndarray`, got `{type(a_fuzzy).__name__}`.")
     a_fuzzy = np.asarray(a_fuzzy)  # convert to array from lineage classs, don't copy
-    if check_row_sums:
-        if n_clusters != 1 and not np.allclose(
-            a_fuzzy.sum(1), 1, rtol=1e6 * EPS, atol=1e6 * EPS
-        ):
-            raise ValueError("Rows in `a_fuzzy` do not sum to `1`.")
+    if check_row_sums and n_clusters != 1 and not np.allclose(a_fuzzy.sum(1), 1, rtol=1e6 * EPS, atol=1e6 * EPS):
+        raise ValueError("Rows in `a_fuzzy` do not sum to `1`.")
     if n_most_likely > int(n_samples / n_clusters):
         raise ValueError(
             f"You've selected `{n_most_likely}` cells, please decrease this to at most "
             f"`{int(n_samples / n_clusters)}` cells for your dataset."
         )
 
     # initialise
-    n_raise = (
-        1
-        if raise_threshold is None
-        else np.max([int(raise_threshold * n_most_likely), 1])
-    )
+    n_raise = 1 if raise_threshold is None else np.max([int(raise_threshold * n_most_likely), 1])
     logg.debug(f"Raising an exception if there are less than `{n_raise}` cells.")
 
     # initially select `n_most_likely` samples per cluster
     sample_assignment = {
         cl: fuzzy_assignment.argpartition(-n_most_likely)[-n_most_likely:]
         for cl, fuzzy_assignment in enumerate(a_fuzzy.T)
     }
 
     # create the one-hot encoded discrete clustering
-    a_discrete = np.zeros(
-        a_fuzzy.shape, dtype=bool
-    )  # don't use `zeros_like` - it also copies the dtype
+    a_discrete = np.zeros(a_fuzzy.shape, dtype=bool)  # don't use `zeros_like` - it also copies the dtype
     for ix in range(n_clusters):
         a_discrete[sample_assignment[ix], ix] = True
 
     # handle samples assigned to more than one cluster
     critical_samples = np.where(a_discrete.sum(1) > 1)[0]
     for sample_ix in critical_samples:
         if remove_overlap:
             a_discrete[sample_ix, :] = _one_hot(n_clusters)
         else:
             candidate_ixs = np.where(a_discrete[sample_ix, :])[0]
-            most_likely_ix = candidate_ixs[
-                np.argmax(a_fuzzy[sample_ix, list(a_discrete[sample_ix, :])])
-            ]
+            most_likely_ix = candidate_ixs[np.argmax(a_fuzzy[sample_ix, list(a_discrete[sample_ix, :])])]
             a_discrete[sample_ix, :] = _one_hot(n_clusters, most_likely_ix)
 
     # check how many samples this left for each cluster
     n_samples_per_cluster = a_discrete.sum(0)
-    if raise_threshold is not None:
-        if (n_samples_per_cluster < n_raise).any():
-            min_samples = np.min(n_samples_per_cluster)
-            raise ValueError(
-                f"Discretizing leads to a cluster with `{min_samples}` samples, less than the threshold which is "
-                f"`{n_raise}` samples. Consider recomputing the fuzzy clustering."
-            )
+    if raise_threshold is not None and (n_samples_per_cluster < n_raise).any():
+        min_samples = np.min(n_samples_per_cluster)
+        raise ValueError(
+            f"Discretizing leads to a cluster with `{min_samples}` samples, less than the threshold which is "
+            f"`{n_raise}` samples. Consider recomputing the fuzzy clustering."
+        )
     if (n_samples_per_cluster > n_most_likely).any():
         raise ValueError("Assigned more samples than requested.")
     critical_clusters = np.where(n_samples_per_cluster < n_most_likely)[0]
 
     return a_discrete, critical_clusters
 
 
 def _series_from_one_hot_matrix(
     membership: np.array,
     index: Optional[Iterable] = None,
     names: Optional[Iterable] = None,
 ) -> pd.Series:
-    """
-    Create a pandas Series based on a one-hot encoded matrix.
+    """Create a pandas Series based on a one-hot encoded matrix.
 
     Parameters
     ----------
     membership
         One-hot encoded membership matrix, of shape `(n_samples x n_clusters)` i.e. a `1` in position `i, j`
         signifies that sample `i` belongs to cluster `j`.
     index
         Index for the Series. Careful, if this is not given, categories are removed when writing to AnnData.
 
     Returns
     -------
-    :class:`pandas.Series`
-        Series, indicating cluster membership for each sample. The data type of the categories is :class:`str`
-        and samples that belong to no cluster are assigned `NaN`.
+    Series, indicating cluster membership for each sample. The data type of the categories is :class:`str`
+    and samples that belong to no cluster are assigned `NaN`.
     """
     n_samples, n_clusters = membership.shape
     if not isinstance(membership, np.ndarray):
-        raise TypeError(
-            f"Expected `membership` to be of type `numpy.ndarray`, found `{type(membership).__name__!r}`."
-        )
-    membership = np.asarray(
-        membership
-    )  # change the type in case a lineage object was passed.
+        raise TypeError(f"Expected `membership` to be of type `numpy.ndarray`, found `{type(membership).__name__}`.")
+    membership = np.asarray(membership)  # change the type in case a lineage object was passed.
     if membership.dtype != bool:
-        raise TypeError(
-            f"Expected `membership`'s elements to be boolean, found `{membership.dtype.name!r}`."
-        )
+        raise TypeError(f"Expected `membership`'s elements to be boolean, found `{membership.dtype.name!r}`.")
 
     if not np.all(membership.sum(axis=1) <= 1):
         raise ValueError("Not all items are one-hot encoded or empty.")
     if (membership.sum(0) == 0).any():
         logg.warning(f"Detected {np.sum((membership.sum(0) == 0))} empty categories")
 
     if index is None:
         index = range(n_samples)
     if names is not None:
         if len(names) != n_clusters:
-            raise ValueError(
-                f"Shape mismatch, length of `names` is `{len(names)}`, but `n_clusters={n_clusters}`."
-            )
+            raise ValueError(f"Shape mismatch, length of `names` is `{len(names)}`, but `n_clusters={n_clusters}`.")
     else:
         names = np.arange(n_clusters).astype("str")
 
     target_series = pd.Series(index=index, dtype="category")
     for vec, name in zip(membership.T, names):
         target_series = target_series.cat.add_categories(name)
         target_series[np.where(vec)[0]] = name
 
     return target_series
 
 
 def _get_cat_and_null_indices(
-    cat_series: Series,
+    cat_series: pd.Series,
 ) -> Tuple[np.ndarray, np.ndarray, Dict[Any, np.ndarray]]:
-    """
-    Given a categorical :class:`pandas.Series`, get the indices corresponding to categories and `NaNs`.
+    """Given a categorical :class:`~pandas.Series`, get the indices corresponding to categories and `NaNs`.
 
     Parameters
     ----------
     cat_series
         Series that contains categorical annotations.
 
     Returns
     -------
-    :class: `numpy.ndarray`
-        Array containing the indices of elements corresponding to categories in ``cat_series``.
-    :class: `numpy.ndarray`
-        Array containing the indices of elements corresponding to NaNs in ``cat_series``.
-    :class:`dict`
-        Dict containing categories of ``cat_series`` as keys and an array of corresponding indices as values.
+    - Array containing the indices of elements corresponding to categories in ``cat_series``.
+    - Array containing the indices of elements corresponding to NaNs in ``cat_series``.
+    - Dict containing categories of ``cat_series`` as keys and an array of corresponding indices as values.
     """
-
     # check the dtype
     if cat_series.dtype != "category":
-        raise TypeError(
-            f"Expected `cat_series` to be categorical, found `{cat_series.dtype.name!r}`."
-        )
+        raise TypeError(f"Expected `cat_series` to be categorical, found `{cat_series.dtype.name!r}`.")
 
     # define a dict that has category names as keys and arrays of indices as values
-    lookup_dict = {
-        cat: np.where(cat_series == cat)[0] for cat in cat_series.cat.categories
-    }
+    lookup_dict = {cat: np.where(cat_series == cat)[0] for cat in cat_series.cat.categories}
     all_indices = np.arange(len(cat_series))
 
     # collect all category indices
     cat_indices = np.concatenate(list(lookup_dict.values()))
 
     # collect all null indices (the ones where we have NaN in `cat_series`)
     null_indices = np.array(list(set(all_indices) - set(cat_indices)))
 
     # check that null indices and cat indices are unique
-    assert (
-        np.unique(cat_indices, return_counts=True)[1] == 1
-    ).all(), "Cat indices are not unique."
-    assert (
-        np.unique(null_indices, return_counts=True)[1] == 1
-    ).all(), "Null indices are not unique."
+    assert (np.unique(cat_indices, return_counts=True)[1] == 1).all(), "Cat indices are not unique."
+    assert (np.unique(null_indices, return_counts=True)[1] == 1).all(), "Null indices are not unique."
 
     # check that there is no overlap
-    assert (
-        len(set(cat_indices).intersection(set(null_indices))) == 0
-    ), "Cat and null indices overlap."
+    assert len(set(cat_indices).intersection(set(null_indices))) == 0, "Cat and null indices overlap."
 
     # check that their untion is the set of all indices
-    assert set(cat_indices).union(set(null_indices)) == set(
-        all_indices
-    ), "Some indices got lost on the way."
+    assert set(cat_indices).union(set(null_indices)) == set(all_indices), "Some indices got lost on the way."
 
     return cat_indices, null_indices, lookup_dict
 
 
-def _check_estimator_type(estimator: Any) -> None:
-    # prevents cyclic import
-    from cellrank.tl.estimators._base_estimator import BaseEstimator
-
-    if not isinstance(estimator, type):
-        raise TypeError(
-            f"Expected estimator to be a class, found `{type(estimator).__name__!r}`."
-        )
-
-    if not issubclass(estimator, BaseEstimator):
-        raise TypeError(
-            f"Expected estimator to be a subclass of `cellrank.tl.estimators.BaseEstimator`, "
-            f"found `{type(estimator).__name__!r}`."
-        )
-
-
 def _calculate_absorption_time_moments(
-    Q: Union[np.ndarray, spmatrix],
+    Q: Union[np.ndarray, sp.spmatrix],
     trans_indices: np.ndarray,
     n: int,
     calculate_variance: bool = False,
-    **kwargs,
+    **kwargs: Any,
 ) -> Tuple[np.ndarray, Optional[np.ndarray]]:
-    """
-    Calculate the mean time until absorption and optionally its variance.
+    """Calculate the mean time until absorption and optionally its variance.
 
     Parameters
     ----------
     Q
         Transient-transient submatrix of the transition matrix.
     trans_indices
         Transient indices.
     n
         Number of states of the full transition matrix.
     calculate_variance
         Whether to calculate also the variance of time to absorption, not only mean.
     kwargs
-        Keyword arguments for :func:`cellrank.tl._lin_solver._solver_lin_system`.
+        Keyword arguments for :func:`cellrank._utils._linear_solver._solver_lin_system`.
 
     Returns
     -------
-        Mean time until absorption and optionally its variance, based on ``calculate_variance``.
+    Mean time until absorption and optionally its variance, based on ``calculate_variance``.
     """
-
     n_jobs = kwargs.pop("n_jobs", None)
     solve_kwargs = _filter_kwargs(_solve_lin_system, **kwargs)
 
     logg.debug("Calculating mean time to absorption to any absorbing state")
     m = _solve_lin_system(
         Q,
         np.ones((Q.shape[0],), dtype=np.float32),
@@ -1404,43 +1244,41 @@
         **solve_kwargs,
     ).squeeze()
     mean = np.zeros(n, dtype=np.float32)
     var = None
     mean[trans_indices] = m
 
     if calculate_variance:
-        logg.debug(
-            "Calculating variance of mean time to absorption to any absorbing state"
-        )
+        logg.debug("Calculating variance of mean time to absorption to any absorbing state")
 
-        I = speye(Q.shape[0]) if issparse(Q) else np.eye(Q.shape[0])  # noqa
+        I = sp.eye(Q.shape[0]) if sp.issparse(Q) else np.eye(Q.shape[0])
         A_t = (I + Q).T
         B_t = (I - Q).T
 
         logg.debug("Solving equation (1/2)")
         X = _solve_lin_system(A_t, B_t, n_jobs=n_jobs, **kwargs).T
-        y = m - X @ (m ** 2)
+        y = m - X @ (m**2)
 
         logg.debug("Solving equation (2/2)")
         v = _solve_lin_system(X, y, use_eye=False, n_jobs=1, **solve_kwargs).squeeze()
         assert np.all(v >= 0), f"Encountered negative variance: `{v[v < 0]}`."
 
         var = np.zeros(n, dtype=np.float32)
         var[trans_indices] = v
 
     return mean, var
 
 
 def _calculate_lineage_absorption_time_means(
-    Q: csr_matrix,
-    R: csr_matrix,
+    Q: sp.csr_matrix,
+    R: sp.csr_matrix,
     trans_indices: np.ndarray,
     ixs: Dict[str, np.ndarray],
-    lineages: Dict[Sequence[str], str],
     index: pd.Index,
+    calculate_variance: bool = False,
     **kwargs: Any,
 ) -> pd.DataFrame:
     """
     Calculate the mean time until absorption and optionally its variance for specific lineages or their combinations.
 
     Parameters
     ----------
@@ -1450,196 +1288,299 @@
         Transient-recurrent submatrix of the transition matrix.
     trans_indices
         Transient indices.
     n
         Number of states of the full transition matrix.
     ixs
         Mapping of names of absorbing states and their indices in the full transition matrix.
-    lineages
-        Lineages for which to calculate the mean time until absorption moments.
+    calculate_variance
+        Whether to calculate variance of the mean time to absorption.
     kwargs
-        Keyword arguments for :func:`cellrank.tl._lin_solver._solver_lin_system`.
+        Keyword arguments for :func:`cellrank._utils._linear_solver._solver_lin_system`.
 
     Returns
     -------
-    :class:`pandas.DataFrame`
-        A :class:`pandas.DataFrame. with means and optionally variances of
-        mean time to absorption for each lineage in ``lineages``.
-
-        Uses more efficient implementation if compute the time for all lineages.
+    A dataframe with means and optionally variances of the time to absorption for each lineage in ``ixs``.
+    Uses more efficient implementation if compute the time for all lineages.
     """
     n = len(index)
     res = pd.DataFrame(index=index)
 
-    if len(lineages) == 1 and set(next(iter(lineages.keys()))) == set(ixs.keys()):
+    if len(ixs) == 1:
         # use faster implementation in this case
         name = ", ".join(ixs.keys())
-        res[f"{name} mean"], var = _calculate_absorption_time_moments(
+        res[f"{name}_mean"], var = _calculate_absorption_time_moments(
             Q,
             trans_indices,
             n,
-            calculate_variance=next(iter(lineages.values())) == "var",
+            calculate_variance=calculate_variance,
             **kwargs,
         )
         if var is not None:
-            res[f"{name} var"] = var
+            res[f"{name}_var"] = var
 
         return res
 
-    res = pd.DataFrame()
-    tmp_ixs, cnt = {}, 0
-    for k, ix in ixs.items():
-        # get the indices to B matrix
-        tmp_ixs[k] = np.arange(cnt, cnt + len(ix), dtype=np.int32)
-        cnt += len(ix)
-
-    I = speye(Q.shape[0]) if issparse(Q) else np.eye(Q.shape)  # noqa
+    I = sp.eye(Q.shape[0]) if sp.issparse(Q) else np.eye(Q.shape)
     N_inv = I - Q
 
     logg.debug("Solving equation for `B`")
     B = _solve_lin_system(Q, R, use_eye=True, **kwargs)
 
     no_jobs_kwargs = kwargs.copy()
     _ = no_jobs_kwargs.pop("n_jobs", None)
 
-    for lns, moment in lineages.items():
-        name = ", ".join(lns)
-        ix = np.concatenate([ixs[ln] for ln in lns])
-
-        D_j = diags(np.sum(B[:, np.concatenate([tmp_ixs[ln] for ln in lns])], axis=1))
+    for i, (lineage, indices) in enumerate(ixs.items()):
+        D_j = sp.diags(B[:, i])  # use `i`, since `B` is already aggregated
         D_j_inv = D_j.copy()
         D_j_inv.data = 1.0 / D_j.data
 
-        logg.debug(f"Calculating mean time to absorption to `{name!r}`")
-        m = _solve_lin_system(
-            D_j_inv @ N_inv @ D_j, np.ones(Q.shape[0]), **kwargs
-        ).squeeze()
-
-        mean = np.empty(n, dtype=np.float64)
-        mean[:] = np.inf
-        mean[ix] = 0
-        mean[trans_indices] = m
+        # fmt: off
+        logg.debug(f"Calculating mean time to absorption to `{lineage!r}`")
+        m = _solve_lin_system(D_j_inv @ N_inv @ D_j, np.ones(Q.shape[0]), **kwargs).squeeze()
+        # fmt: on
 
-        res[f"{name} mean"] = mean
+        mean = np.full(n, fill_value=np.inf, dtype=np.float64)
+        mean[indices] = 0
+        mean[trans_indices] = m
+        res[f"{lineage}_mean"] = mean
 
-        if moment == "var":
-            logg.debug(f"Calculating variance of mean time to absorption to `{name!r}`")
+        if calculate_variance:
+            # fmt: off
+            logg.debug(f"Calculating variance of the mean time to absorption to `{lineage!r}`")
 
-            logg.debug("Solving equation (1/2)")
             X = _solve_lin_system(D_j + Q @ D_j, N_inv @ D_j, use_eye=False, **kwargs)
-            y = m - X @ (m ** 2)
+            y = m - X @ (m**2)
 
-            logg.debug("Solving equation (2/2)")
-            v = _solve_lin_system(
-                X, y, use_eye=False, n_jobs=1, **no_jobs_kwargs
-            ).squeeze()
+            v = _solve_lin_system(X, y, use_eye=False, n_jobs=1, **no_jobs_kwargs).squeeze()
             assert np.all(v >= 0), f"Encountered negative variance: `{v[v < 0]}`."
 
             var = np.full(n, fill_value=np.nan, dtype=np.float64)
-            var[ix] = 0
+            var[indices] = 0
             var[trans_indices] = v
+            res[f"{lineage}_var"] = var
+            # fmt: on
+    return res
+
+
+def _check_collection(
+    adata: AnnData,
+    needles: Iterable[str],
+    attr_name: str,
+    key_name: str = "Gene",
+    use_raw: bool = False,
+    raise_exc: bool = True,
+) -> List[str]:
+    """Check if given collection contains all the keys.
+
+    Parameters
+    ----------
+    adata
+        Annotated data object.
+    needles
+        Keys to check.
+    attr_name
+        Attribute of ``adata`` where the needles are stored.
+    key_name
+        Pretty name of the key which will be displayed when error is found.
+    use_raw
+        Whether to access :attr:`anndata.AnnData.raw` or just ``adata``.
+
+    Returns
+    -------
+    Nothing, but raises and :class:`KeyError` if one of the needles is not found.
+    """
+    adata_name = "adata"
 
-            res[f"{name} var"] = var
+    if use_raw and adata.raw is None:
+        logg.warning("Argument `use_raw` was set to `True`, but no `raw` attribute is found. Ignoring")
+        use_raw = False
+    if use_raw:
+        adata_name = "adata.raw"
+        adata = adata.raw
+
+    haystack, res = getattr(adata, attr_name), []
+    for needle in needles:
+        if needle not in haystack:
+            if raise_exc:
+                raise KeyError(f"{key_name} `{needle}` not found in `{adata_name}.{attr_name}`.")
+        else:
+            res.append(needle)
 
     return res
 
 
-def _create_initial_terminal_annotations(
-    adata: AnnData,
-    terminal_key: str = "terminal_states",
-    initial_key: str = "initial_states",
-    terminal_prefix: Optional[str] = "terminal",
-    initial_prefix: Optional[str] = "initial",
-    key_added: Optional[str] = "initial_terminal",
-) -> None:
-    """
-    Create categorical annotations of both initial and terminal states.
-
-    This is a utility function for creating a categorical :class:`pandas.Series` object which combines
-    the information about initial and terminal states. The :class:`pandas.Series` is written directly
-    to the :class:`anndata.AnnData`object. This can for example be used to create a scatter plot in :mod:`scvelo`.
+def _minmax(data: np.ndarray, perc: Optional[Tuple[float, float]] = None) -> Tuple[float, float]:
+    """Return minimum and maximum value of the data.
+
+    Parameters
+    ----------
+    data
+        Values for which to return the minimum and maximum.
+    perc
+        If not `None`, clip the values by the percentiles before getting the result.
+
+    Returns
+    -------
+    Minimum and maximum values, respectively.
+    """
+    if perc is not None:
+        data = np.clip(data, *np.percentile(data, sorted(perc)))
+
+    return float(np.nanmin(data)), float(np.nanmax(data))
+
+
+def _modify_neigh_key(key: Optional[str]) -> str:
+    if key in (None, "connectivities", "distances"):
+        return "neighbors"
+
+    if key.endswith("_connectivities"):
+        key = key[:-15]
+    elif key.endswith("_distances"):
+        key = key[:-10]
+
+    return key
+
+
+def _get_neighs(adata: AnnData, mode: str = "distances", key: Optional[str] = None) -> Union[np.ndarray, sp.spmatrix]:
+    if key is None:
+        res = _read_graph_data(adata, mode)  # legacy behavior
+    else:
+        try:
+            res = _read_graph_data(adata, key)
+            assert isinstance(res, (np.ndarray, sp.spmatrix))
+        except (KeyError, AssertionError):
+            res = _read_graph_data(adata, f"{_modify_neigh_key(key)}_{mode}")
+
+    if not isinstance(res, (np.ndarray, sp.spmatrix)):
+        raise TypeError(f"Expected to find `numpy.ndarray` or `scipy.sparse.spmatrix`, found `{type(res)}`.")
+
+    return res
+
+
+def _has_neighs(adata: AnnData, key: Optional[str] = None) -> bool:
+    return _modify_neigh_key(key) in adata.uns
+
+
+def _get_neighs_params(adata: AnnData, key: str = "neighbors") -> Dict[str, Any]:
+    return adata.uns.get(key, {}).get("params", {})
+
+
+def _read_graph_data(adata: AnnData, key: str) -> Union[np.ndarray, sp.spmatrix]:
+    """Read graph data from :class:`~anndata.AnnData`.
 
     Parameters
     ----------
     adata
-        AnnData object to write to ``.obs[key_added]``.
-    terminal_key
-        Key from ``adata.obs`` where terminal states have been saved.
-    initial_key
-        Key from ``adata.obs`` where initial states have been saved.
-    terminal_prefix
-        Forward direction prefix used in the annotations.
-    initial_prefix
-        Backward direction prefix used in the annotations.
-    key_added
-        Key added to ``adata.obs``.
+        Annotated data object.
+    key
+        Key in :attr:`~anndata.AnnData.obsp`.
 
     Returns
     -------
-    None
-        Nothing, just writes to ``adata``.
-    """
-
-    # get both Series objects
-    cats_final, colors_final = (
-        adata.obs[terminal_key],
-        adata.uns[f"{terminal_key}_colors"],
-    )
-    cats_root, colors_root = adata.obs[initial_key], adata.uns[f"{initial_key}_colors"]
+    The graph data.
+    """
+    if key in adata.obsp:
+        return adata.obsp[key]
 
-    # merge
-    cats_merged, colors_merged = _merge_categorical_series(
-        cats_final,
-        cats_root,
-        colors_old=list(colors_final),
-        colors_new=list(colors_root),
-    )
+    raise KeyError(f"Unable to find data in `adata.obsp[{key!r}]`.")
 
-    # adjust the names
-    final_names = cats_final.cat.categories
-    final_labels = [
-        f"{terminal_prefix if key in final_names else initial_prefix}: {key}"
-        for key in cats_merged.cat.categories
-    ]
-    cats_merged = cats_merged.cat.rename_categories(final_labels)
-
-    # write to AnnData
-    adata.obs[key_added] = cats_merged
-    adata.uns[f"{key_added}_colors"] = colors_merged
 
+def valuedispatch(func):
+    """Dispatch a function based on the first value."""
+    registry = {}
 
-def _maybe_subset_hvgs(
-    adata: AnnData, use_highly_variable: Optional[Union[bool, str]]
-) -> AnnData:
-    if use_highly_variable in (None, False):
-        return adata
-    key = "highly_variable" if use_highly_variable is True else use_highly_variable
-
-    if key not in adata.var.keys():
-        logg.warning(f"Unable to find HVGs in `adata.var[{key!r}]`. Using all genes")
-        return adata
+    def dispatch(value):
+        return registry.get(value, func)
 
-    if not is_bool_dtype(adata.var[key]):
-        logg.warning(
-            f"Expected `adata.var[{key!r}]` to be of bool dtype, "
-            f"found `{infer_dtype(adata.var[key])}`. Using all genes"
-        )
-        return adata
+    def register(value, func=None):
+        if func is None:
+            return lambda f: register(value, f)
+        registry[value] = func
+        return func
 
-    logg.info(f"Using `{np.sum(adata.var[key])}` HVGs from `adata.var[{key!r}]`")
-    return adata[:, adata.var[key]]
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        return dispatch(args[0])(*args[1:], **kwargs)
 
+    wrapper.register = register
+    wrapper.dispatch = dispatch
+    wrapper.registry = types.MappingProxyType(registry)
 
-def _deprecate(*, version: str) -> Callable:
-    @wrapt.decorator
-    def wrapper(wrapped: Callable, instance: Any, args: Any, kwargs: Any) -> Any:
-        with warnings.catch_warnings():
-            warnings.simplefilter("always", DeprecationWarning)
-            warnings.warn(
-                f"`cellrank.tl.{wrapped.__name__}` will be removed in version `{version}`. "
-                f"Please use the `cellrank.kernels` or `cellrank.estimators` interface instead.",
-                stacklevel=2,
-                category=DeprecationWarning,
-            )
-        return wrapped(*args, **kwargs)
+    functools.update_wrapper(wrapper, func)
 
     return wrapper
+
+
+def _densify_squeeze(x: Union[sp.spmatrix, np.ndarray], dtype=np.float32) -> np.ndarray:
+    if sp.issparse(x):
+        x = x.toarray()
+    # use np.array instead of asarray to create a copy
+    x = np.array(x, dtype=dtype)
+    if x.ndim == 2 and x.shape[1] == 1:
+        x = np.squeeze(x, axis=1)
+
+    return x
+
+
+@contextlib.contextmanager
+@d.dedent
+def _gene_symbols_ctx(
+    adata: AnnData,
+    *,
+    key: Optional[str] = None,
+    use_raw: bool = False,
+    make_unique: bool = False,
+) -> AnnData:
+    """Set gene names from a column in :attr:`~anndata.AnnData.var`.
+
+    Parameters
+    ----------
+    %(adata)s
+    key
+        Key in :attr:`~anndata.AnnData.var` where the gene symbols are stored. If `None`, this operation is a no-op.
+    use_raw
+        Whether to change the gene names in :attr:`~anndata.AnnData.raw`.
+    make_unique
+        Whether to make the newly assigned gene names unique.
+
+    Yields
+    ------
+    The same ``adata`` with modified :attr:`~anndata.AnnData.var_names`, depending on the ``use_raw``.
+    """
+
+    def key_present() -> bool:
+        if use_raw:
+            if adata.raw is None:
+                raise AttributeError("No `.raw` attribute found. Try specifying `use_raw=False`.")
+            return key in adata.raw.var
+        return key in adata.var
+
+    if key is None:
+        yield adata
+    elif not key_present():
+        raise KeyError(f"Unable to find gene symbols in `adata.{'raw.' if use_raw else ''}var[{key!r}]`.")
+    else:
+        adata_orig = adata
+        if use_raw:
+            adata = adata.raw
+
+        var_names = adata.var_names.copy()
+        try:
+            # TODO(michalk8): doesn't update varm (niche)
+            adata.var.index = make_index_unique(adata.var[key]) if make_unique else adata.var[key]
+            yield adata_orig
+        finally:
+            # in principle we assume the callee doesn't change the index
+            # otherwise, would need to check whether it has been changed and add an option to determine what to do
+            adata.var.index = var_names
+
+
+@wrapt.decorator
+def _genesymbols(wrapped: Callable[..., Any], instance: Any, args: Any, kwargs: Any) -> Any:
+    with _gene_symbols_ctx(
+        args[0],
+        key=kwargs.pop("gene_symbols", None),
+        make_unique=True,
+        use_raw=kwargs.get("use_raw", False),
+    ):
+        return wrapped(*args, **kwargs)
```

### Comparing `cellrank-1.5.1/cellrank/tl/estimators/_base_estimator.py` & `cellrank-2.0.0/src/cellrank/estimators/_base_estimator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,128 +1,146 @@
-from typing import Any, Dict, List, Tuple, Union, Mapping, Callable, Optional, Sequence
-from typing_extensions import Literal
+import abc
+import contextlib
+import copy as copy_
+import inspect
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Sequence,
+    Tuple,
+    Union,
+)
 
-from abc import ABC, abstractmethod
-from copy import copy as copy_
-from copy import deepcopy
-from inspect import Parameter, signature, getmembers, currentframe
-from contextlib import contextmanager
+import numpy as np
+import pandas as pd
+import scipy.sparse as sp
 
 from anndata import AnnData
-from cellrank._key import Key
-from cellrank.ul._docs import d
-from cellrank.tl._mixins import IOMixin, KernelMixin, AnnDataMixin
-from cellrank.tl.kernels import PrecomputedKernel
-from cellrank.tl._lineage import Lineage
-from cellrank.tl.kernels._base_kernel import Kernel, KernelExpression
 
-import numpy as np
-import pandas as pd
-from scipy.sparse import spmatrix, csr_matrix
+from cellrank._utils._docs import d
+from cellrank._utils._key import Key
+from cellrank._utils._lineage import Lineage
+from cellrank.estimators.mixins import KernelMixin
+from cellrank.kernels import PrecomputedKernel
+from cellrank.kernels._base_kernel import KernelExpression
+from cellrank.kernels.mixins import AnnDataMixin, IOMixin
 
-Attr_t = (
-    Literal["X", "raw", "layers", "obs", "var", "obsm", "varm", "obsp", "varp", "uns"],
-)
+__all__ = ["BaseEstimator"]
+
+Attr_t = (Literal["X", "raw", "layers", "obs", "var", "obsm", "varm", "obsp", "varp", "uns"],)
 
 
 @d.get_sections(base="base_estimator", sections=["Parameters"])
-class BaseEstimator(IOMixin, KernelMixin, AnnDataMixin, ABC):
-    """
-    Base class for all estimators.
+class BaseEstimator(IOMixin, KernelMixin, AnnDataMixin, abc.ABC):
+    """Base class for all estimators.
 
     Parameters
     ----------
-    obj
-        Can be one of the following:
+    object
+        Can be one of the following types:
 
-            - :class:`cellrank.tl.kernels.Kernel` - kernel object.
-            - :class:`anndata.AnnData` - annotated data object containing transition matrix in
-              :attr:`anndata.AnnData.obsp`.
-            - :class:`numpy.ndarray` - row-normalized sparse transition matrix.
-            - :class:`scipy.sparse.spmatrix` - row-normalized sparse transition matrix.
-    obsp_key
-        Key in :attr:`anndata.AnnData.obsp` where the transition matrix is stored.
-        Only used when ``obj`` is an :class:`anndata.AnnData` object.
+        - :class:`~anndata.AnnData` - annotated data object.
+        - :class:`~scipy.sparse.spmatrix`, :class:`~numpy.ndarray` - row-normalized transition matrix.
+        - :class:`~cellrank.kernels.KernelExpression` - kernel expression.
+        - :class:`str` - key in :attr:`~anndata.AnnData.obsp` where the transition matrix is stored and
+          ``adata`` must be provided in this case.
+        - :class:`bool` - directionality of the transition matrix that will be used to infer its storage location.
+          If :obj:`None`, the directionality will be determined automatically and
+          ``adata`` must be provided in this case.
+    kwargs
+        Keyword arguments for the :class:`~cellrank.kernels.PrecomputedKernel`.
     """
 
     def __init__(
         self,
-        obj: Union[AnnData, np.ndarray, spmatrix, KernelExpression],
-        obsp_key: Optional[str] = None,
+        object: Union[str, bool, np.ndarray, sp.spmatrix, AnnData, KernelExpression],
+        **kwargs: Any,
     ):
-        if isinstance(obj, Kernel):
-            if obj._transition_matrix is None:
-                raise ValueError(
-                    "Compute transition matrix first as `.compute_transition_matrix()`."
-                )
-            kernel = obj
-        elif isinstance(obj, KernelExpression):
-            # this will fail if not all kernels have transition matrix computed
-            kernel = obj.compute_transition_matrix()
-        elif isinstance(obj, (np.ndarray, spmatrix)):
-            kernel = PrecomputedKernel(obj)
-        elif isinstance(obj, AnnData):
-            if obsp_key is None:
-                raise ValueError(
-                    "Specify `obsp_key=...` when supplying an `AnnData` object."
-                )
-            elif obsp_key not in obj.obsp:
-                raise KeyError(
-                    f"Unable to find transition matrix in `adata.obsp[{obsp_key!r}]`."
-                )
-            kernel = PrecomputedKernel(obsp_key, adata=obj)
+        if isinstance(object, KernelExpression):
+            if object.transition_matrix is None:
+                raise RuntimeError("Compute transition matrix first as `.compute_transition_matrix()`.")
         else:
-            raise TypeError(
-                f"Expected an object of type `KernelExpression`, `numpy.ndarray`, `scipy.sparse.spmatrix` "
-                f"or `anndata.AnnData`, got `{type(obj).__name__}`."
-            )
-
-        super().__init__(kernel=kernel)
+            object = PrecomputedKernel(object, copy=False, **kwargs)
+        super().__init__(kernel=object)
 
         self._params: Dict[str, Any] = {}
         self._shadow_adata = AnnData(
-            X=csr_matrix(self.adata.shape, dtype=self.adata.X.dtype),
+            X=sp.csr_matrix(self.adata.shape, dtype=self.adata.X.dtype),
             obs=self.adata.obs[[]].copy(),
             var=self.adata.var[[]].copy(),
             raw=None if self.adata.raw is None else self.adata.raw.to_adata(),
         )
 
     def __init_subclass__(cls, **kwargs: Any):
         super().__init_subclass__()
 
+    @abc.abstractmethod
+    def fit(self, *args: Any, **kwargs: Any) -> "BaseEstimator":
+        """Fit the estimator.
+
+        Parameters
+        ----------
+        args
+            Positional arguments.
+        kwargs
+            Keyword arguments.
+
+        Returns
+        -------
+        Self.
+        """
+
+    @abc.abstractmethod
+    def predict(self, *args: Any, **kwargs: Any) -> "BaseEstimator":
+        """Run the prediction.
+
+        Parameters
+        ----------
+        args
+            Positional arguments.
+        kwargs
+            Keyword arguments.
+
+        Returns
+        -------
+        Self.
+        """
+
     def _set(
         self,
         attr: Optional[str] = None,
         obj: Optional[Union[pd.DataFrame, Mapping[str, Any]]] = None,
         key: Optional[str] = None,
-        value: Optional[
-            Union[np.ndarray, pd.Series, pd.DataFrame, Lineage, AnnData, Dict[str, Any]]
-        ] = None,
+        value: Optional[Union[np.ndarray, pd.Series, pd.DataFrame, Lineage, AnnData, Dict[str, Any]]] = None,
         copy: bool = True,
         shadow_only: bool = False,
     ) -> None:
-        """
-        Set an attribute and optionally update ``obj[{key}]``.
+        """Set an attribute and optionally update ``obj['{key}']``.
 
         Parameters
         ----------
         attr
-            Attribute to set. Only updated when we're not in the shadow. If `None`, don't update anything.
+            Attribute to set. Only updated when we're not in the shadow. If :obj:`None`, don't update anything.
             See :attr:`_in_shadow` and ``obj`` for more information.
         obj
-            Object which to update with ``value`` alongside the ``attr`.
+            Object which to update with ``value`` alongside the ``attr``.
             Usually, an attribute of :attr:`adata` is passed here.
         key
             Key in ``obj`` to update with ``value``. Only used when ``obj != None``.
         value
-            Value to set. If `None` and ``key != None``, it removes the values under ``obj[key]``, if present.
+            Value to set. If :obj:`None` and ``key != None``, it removes the values under ``obj['{key}']``, if present.
         copy
             Whether to copy the ``value`` before setting it in ``obj``.
         shadow_only
-            Whether or not to update the ``obj`` if we are not in the shadow.
+            Whether to update the ``obj`` if we are not in the shadow.
 
         Returns
         -------
         Nothing, just optionally updates ``attr`` and/or ``obj[{key}]``.
 
         Raises
         ------
@@ -138,87 +156,81 @@
                 return
 
         if obj is None:
             return
 
         if key is not None:
             if value is None:
-                try:
+                with contextlib.suppress(KeyError):
                     del obj[key]
-                except KeyError:
-                    pass
+
             else:
-                obj[key] = copy_(value) if copy else value
+                obj[key] = copy_.copy(value) if copy else value
 
     def _get(
         self,
-        attr: str,
+        *,
         obj: Union[pd.DataFrame, Mapping[str, Any]],
         key: str,
-        where: Optional[Literal["obs", "obsm", "var", "varm", "uns"]] = None,
+        shadow_attr: Optional[Literal["obs", "obsm", "var", "varm", "uns"]] = None,
         dtype: Optional[Union[type, Tuple[type, ...]]] = None,
         copy: bool = True,
         allow_missing: bool = False,
-    ) -> None:
-        """
-        Get data from an object and set an attribute.
+    ) -> Any:
+        """Get data from an object and set an attribute.
 
         Parameters
         ----------
-        attr
-            Attribute to set.
         obj
             Object from which to extract the data.
         key
             Key in ``obj`` where the data is stored.
-        where
-            Attribute of :attr:`_shadow_adata` where to save the extracted data. If `None`, don't update it.
+        shadow_attr
+            Attribute of :attr:`_shadow_adata` where to save the extracted data. If :obj:`None`, don't update it.
         dtype
             Valid type(s) of the extracted data.
         copy
-            Copy the data before setting the ``attr``.
+            Copy the data before setting the ``self_attr``.
         allow_missing
-            Whether or not to allow ``key`` to be missing in ``obj``.
+            Whether to allow ``key`` to be missing in ``obj``.
 
         Returns
         -------
-        Nothing, just updates ``attr`` with the extracted values and optionally :attr:`_shadow_adata`.
+        The extracted values and optionally updates :attr:`_shadow_adata` ``.{shadow_attr}``.
 
         Raises
         ------
         AttributeError
             If ``attr`` doesn't exist.
         TypeError
             If ``dtype != None`` and the extracted values are not instances of ``dtype``.
         KeyError
             If ``allow_missing = False`` and ``key`` was not found in ``obj``.
         """
-        if not hasattr(self, attr):
-            raise AttributeError(attr)
+        if shadow_attr is not None and not hasattr(self._shadow_adata, shadow_attr):
+            raise AttributeError(shadow_attr)
 
         try:
             data = obj[key]
             if dtype is not None and not isinstance(data, dtype):
-                raise TypeError(
-                    f"Expected `.{attr}` to be of type `{dtype}`, found `{type(data).__name__}`."
-                )
+                raise TypeError(f"Expected object to be of type `{dtype}`, found `{type(data).__name__}`.")
             if copy:
-                data = copy_(data)
-            setattr(self, attr, data)
-            if where is not None:
-                getattr(self._shadow_adata, where)[key] = data
+                data = copy_.copy(data)
+            if shadow_attr is not None:
+                getattr(self._shadow_adata, shadow_attr)[key] = data
+            return data
         except KeyError:
             if not allow_missing:
                 raise
+            return None
 
     @property
-    @contextmanager
+    @contextlib.contextmanager
     def _shadow(self) -> None:
-        """
-        Temporarily set :attr:`adata` to :attr:`_shadow_adata`.
+        """Temporarily set :attr:`adata` to :attr:`_shadow_adata`.
 
         Used to construct the serialization object in :meth:`to_adata`.
         """
         if self._in_shadow:
             yield
         else:
             adata = self.adata
@@ -235,49 +247,46 @@
 
     def _create_params(
         self,
         locs: Optional[Mapping[str, Any]] = None,
         func: Optional[Callable] = None,
         remove: Sequence[str] = (),
     ) -> Dict[str, Any]:
-        """
-        Create parameters of interest from a function call.
+        """Create parameters of interest from a function call.
 
         Parameters
         ----------
         locs
             Environment from which to get the parameters. If `None`, get the caller's environment.
         func
-            Function of interest. If `None`, use the caller.
+            Function of interest. If :obj:`None`, use the caller.
         remove
             Keys in ``locs`` which should not be included in the result.
 
         Returns
         -------
         The parameters as a :class:`dict`.
 
         Notes
         -----
         *args/**kwargs are always ignored and the values in ``locs`` are not copied.
         """
-        frame = currentframe()
+        frame = inspect.currentframe()
         try:
             if locs is None:
                 locs = frame.f_back.f_locals
-            if func is None or True:
+            if func is None:
                 name = frame.f_back.f_code.co_name
-                func = dict(getmembers(self)).get(name, None)
+                func = dict(inspect.getmembers(self)).get(name, None)
             if not callable(func):
-                raise TypeError(
-                    f"Expected `func` to be `callable`, found `{type(func).__name__}`."
-                )
+                raise TypeError(f"Expected `func` to be `callable`, found `{type(func).__name__}`.")
 
             params = {}
-            for name, param in signature(func).parameters.items():
-                if param.kind in (Parameter.VAR_POSITIONAL, Parameter.VAR_KEYWORD):
+            for name, param in inspect.signature(func).parameters.items():
+                if param.kind in (inspect.Parameter.VAR_POSITIONAL, inspect.Parameter.VAR_KEYWORD):
                     continue
                 if name in remove:
                     continue
                 if name in locs:
                     params[name] = locs[name]
 
             return params
@@ -286,62 +295,56 @@
             return {}
         except TypeError:
             return {}
         finally:
             del frame
 
     def _read_params(self, key: str) -> Dict[str, Any]:
-        """
-        Read ``key`` from estimator params in :attr:`adata`.
+        """Read ``key`` from estimator params in :attr:`adata`.
 
         Usually called in :meth:`_read_adata` during :meth:`from_adata`.
         """
         ekey = Key.uns.estimator(self.backward) + "_params"
         return dict(self.adata.uns.get(ekey, {}).get(key, {}))
 
     @d.dedent
     def to_adata(
         self,
         keep: Union[Literal["all"], Sequence[Attr_t]] = ("X", "raw"),
         *,
         copy: Union[bool, Sequence[Attr_t]] = True,
     ) -> AnnData:
-        """
-        %(to_adata.full_desc)s
+        """%(to_adata.full_desc)s
 
         Parameters
         ----------
         keep
             Which attributes to keep from the underlying :attr:`adata`. Valid options are:
 
-                - `'all'` - keep all attributes specified in the signature.
-                - :class:`typing.Sequence` - keep only subset of these attributes.
-                - :class:`dict` - the keys correspond the attribute names and values to a subset of keys
-                  which to keep from this attribute. If the values are specified either as `True` or `'all'`,
-                  everything from this attribute will be kept.
+            - ``'all'`` - keep all attributes specified in the signature.
+            - :class:`~typing.Sequence` - keep only subset of these attributes.
+            - :class:`dict` - the keys correspond the attribute names and values to a subset of keys
+              which to keep from this attribute. If the values are specified either as :obj:`True` or ``'all'``,
+              everything from this attribute will be kept.
         copy
-            Whether to copy the data. Can be specified on per-attribute basis. Useful for attributes that store arrays.
-            Attributes not specified here will not be copied.
+            Whether to copy the data. Can be specified on per-attribute basis.
+            Useful for attributes that are array-like.
 
         Returns
         -------
-        %(adata)s
+        Annotated data object.
         """  # noqa: D400
 
         def handle_attribute(attr: Attr_t, keys: List[str], *, copy: bool) -> None:
             try:
                 if attr == "X":
-                    adata.X = deepcopy(self.adata.X) if copy else self.adata.X
+                    adata.X = copy_.deepcopy(self.adata.X) if copy else self.adata.X
                     return
                 if attr == "raw":
-                    adata.raw = (
-                        self.adata.raw.to_adata()
-                        if self.adata.raw is not None
-                        else None
-                    )
+                    adata.raw = self.adata.raw.to_adata() if self.adata.raw is not None else None
                     return
 
                 old = getattr(self.adata, attr)
                 new = getattr(adata, attr)
                 if keys == ["all"]:
                     keys = list(old.keys())
 
@@ -350,39 +353,37 @@
                     old = old[keys]
                     # avoid duplicates
                     old = old[old.columns.difference(new.columns)]
                     setattr(adata, attr, pd.merge(new, old, how="inner", left_index=True, right_index=True, copy=copy))
                 elif isinstance(new, Mapping):
                     old = {k: old[k] for k in keys}
                     # old has preference, since it's user supplied
-                    setattr(adata, attr, {**new, **(deepcopy(old) if copy else old)})
+                    setattr(adata, attr, {**new, **(copy_.deepcopy(old) if copy else old)})
                 else:
                     raise TypeError(f"Expected `adata.{attr}` to be either `Mapping` or `pandas. DataFrame`, "
                                     f"found `{type(new).__name__}`.")
                 # fmt: on
             except KeyError:
                 missing = sorted(k for k in keys if k not in old)
-                raise KeyError(
-                    f"Unable to find key(s) `{missing}` in `adata.{attr}`."
-                ) from None
+                raise KeyError(f"Unable to find key(s) `{missing}` in `adata.{attr}`.") from None
 
         adata = self._shadow_adata.copy()
         _adata = self.adata
         try:
             # kernel and estimator share the adata
             self.adata = adata
             self.kernel.write_to_adata()
         finally:
             self.adata = _adata
         key = Key.uns.estimator(self.backward) + "_params"
-        adata.uns[key] = deepcopy(self.params)
+        adata.uns[key] = copy_.deepcopy(self.params)
 
         # fmt: off
         if isinstance(keep, str):
-            if keep == 'all':
+            if keep == "all":
                 keep = ["X", "raw", "layers", "obs", "var", "obsm", "varm", "obsp", "varp", "uns"]
             else:
                 keep = [keep]
         if not isinstance(keep, Mapping):
             keep = {attr: True for attr in keep}
         if isinstance(copy, bool):
             copy = {attr: copy for attr in keep}
@@ -402,93 +403,60 @@
             handle_attribute(attr, keys=list(keys), copy=copy.get(attr, False))
 
         return adata
 
     @classmethod
     @d.dedent
     def from_adata(cls, adata: AnnData, obsp_key: str) -> "BaseEstimator":
-        """
-        %(from_adata.full_desc)s
+        """%(from_adata.full_desc)s
 
         Parameters
         ----------
         %(adata)s
         obsp_key
-            Key in :attr:`anndata.AnnData.obsp` where the transition matrix is stored.
+            Key in :attr:`~anndata.AnnData.obsp` where the transition matrix is stored.
 
         Returns
         -------
         %(from_adata.returns)s
         """  # noqa: D400
         return super().from_adata(adata, obsp_key=obsp_key)
 
     @d.dedent
     def copy(self, *, deep: bool = False) -> "BaseEstimator":
-        """
-        Return a copy of self.
+        """Return a copy of self.
 
         Parameters
         ----------
         deep
-            Whether to return a deep copy or not. If `True`, this also copies the :attr:`adata`.
+            Whether to return a deep copy or not. If :obj:`True`, this also copies the :attr:`adata`.
 
         Returns
         -------
         A copy of self.
         """
-        k = deepcopy(self.kernel) if deep else copy_(self.kernel)
+        k = copy_.deepcopy(self.kernel) if deep else copy_.copy(self.kernel)
         res = type(self)(k)
         for k, v in self.__dict__.items():
             if isinstance(v, Mapping):
-                res.__dict__[k] = deepcopy(v)
+                res.__dict__[k] = copy_.deepcopy(v)
             elif k != "_kernel":
-                res.__dict__[k] = deepcopy(v) if deep else copy_(v)
+                res.__dict__[k] = copy_.deepcopy(v) if deep else copy_.copy(v)
 
         return res
 
     def __copy__(self) -> "BaseEstimator":
         return self.copy(deep=False)
 
+    def _format_params(self) -> str:
+        return f"kernel={self.kernel!s}"
+
     def __repr__(self) -> str:
-        return f"{self.__class__.__name__}[n={len(self)}, kernel={repr(self.kernel)}]"
+        return f"{self.__class__.__name__}[{self._format_params()}]"
 
     def __str__(self) -> str:
-        return f"{self.__class__.__name__}[n={len(self)}, kernel={str(self.kernel)}]"
+        return repr(self)
 
     @property
     def params(self) -> Dict[str, Any]:
         """Estimator parameters."""
         return self._params
-
-    @abstractmethod
-    def fit(self, *args: Any, **kwargs: Any) -> "BaseEstimator":
-        """
-        Fit an estimator.
-
-        Parameters
-        ----------
-        args
-            Positional arguments.
-        kwargs
-            Keyword arguments.
-
-        Returns
-        -------
-        Self.
-        """
-
-    @abstractmethod
-    def predict(self, *args: Any, **kwargs: Any) -> None:
-        """
-        Run a prediction.
-
-        Parameters
-        ----------
-        args
-            Positional arguments.
-        kwargs
-            Keyword arguments.
-
-        Returns
-        -------
-        Nothing.
-        """
```

### Comparing `cellrank-1.5.1/cellrank/tl/estimators/mixins/_absorption_probabilities.py` & `cellrank-2.0.0/src/cellrank/estimators/mixins/_lineage_drivers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,511 +1,583 @@
-from typing import Any, Dict, Tuple, Union, Mapping, Optional, Sequence
-from typing_extensions import Literal
+import contextlib
+import pathlib
+import types
+from typing import Any, Dict, Literal, Mapping, Optional, Sequence, Tuple, Union
 
-from types import MappingProxyType
-
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import _DEFAULT_BACKEND, Backend_t
-from cellrank.ul._docs import d
-from cellrank.tl._utils import (
-    _pairwise,
-    _process_series,
-    _get_cat_and_null_indices,
-    _calculate_lineage_absorption_time_means,
-)
-from cellrank.tl._lineage import Lineage
-from cellrank.tl._linear_solver import _solve_lin_system
-from cellrank.tl.estimators._utils import SafeGetter
-from cellrank.tl.estimators.mixins._utils import (
-    BaseProtocol,
-    logger,
-    shadow,
-    register_plotter,
-)
+import scvelo as scv
 
 import numpy as np
 import pandas as pd
-from scipy.sparse import issparse, spmatrix
-from pandas.api.types import infer_dtype, is_categorical_dtype
 
+import matplotlib.pyplot as plt
+from matplotlib import patheffects, rc_context
+from matplotlib.axes import Axes
+from matplotlib.patches import ArrowStyle
 
-class AbsProbsProtocol(BaseProtocol):  # noqa: D101
-    _term_states_colors: np.ndarray
+import scanpy as sc
+from anndata import AnnData, Raw
 
-    @property
-    def transition_matrix(self) -> Union[np.ndarray, spmatrix]:  # noqa: D102
-        ...
-
-    @property
-    def terminal_states(self) -> pd.Series:  # noqa: D102
-        ...
+from cellrank import logging as logg
+from cellrank._utils._colors import _create_categorical_colors
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._key import Key
+from cellrank._utils._lineage import Lineage
+from cellrank._utils._utils import RandomKeys, TestMethod, _correlation_test, save_fig
+from cellrank.estimators.mixins._fate_probabilities import FateProbsMixin
+from cellrank.estimators.mixins._utils import BaseProtocol, SafeGetter, logger, shadow
 
-    @property
-    def absorption_probabilities(self) -> Optional[Lineage]:  # noqa: D102
-        ...
+__all__ = ["LinDriversMixin"]
 
-    @property
-    def absorption_times(self) -> Optional[pd.DataFrame]:  # noqa: D102
-        ...
 
-    @property
-    def priming_degree(self) -> Optional[pd.Series]:  # noqa: D102
-        ...
-
-    def __len__(self) -> int:
-        ...
-
-    def _compute_absorption_probabilities(
+class LinDriversProtocol(BaseProtocol):
+    def _write_lineage_drivers(
         self,
-        q: Union[np.ndarray, spmatrix],
-        s: Union[np.ndarray, spmatrix],
-        trans_indices: np.ndarray,
-        term_states: np.ndim,
-        solver: str,
-        use_petsc: bool,
-        n_jobs: Optional[int],
-        backend: str,
-        tol: float,
-        show_progress_bar: bool,
-        preconditioner: str,
-    ) -> np.ndarray:
+        drivers: Optional[pd.DataFrame],
+        use_raw: bool,
+        params: Mapping[str, Any] = types.MappingProxyType({}),
+    ) -> None:
         ...
 
-    def _ensure_lineage_object(self, attr: str, **kwargs: Any) -> None:
+    @property
+    def eigendecomposition(self) -> Dict[str, Any]:
         ...
 
-    def _write_absorption_probabilities(
-        self,
-        abs_probs: Optional[Lineage],
-        abs_times: Optional[pd.DataFrame],
-    ) -> str:
+    @property
+    def fate_probabilities(self) -> Optional[Lineage]:
         ...
 
-    def _write_lineage_priming(
-        self,
-        priming_degree: Optional[pd.Series],
-    ) -> str:
+    @property
+    def lineage_drivers(self) -> Optional[pd.DataFrame]:
         ...
 
 
-def _normalize_abs_times(
-    keys: Sequence[str], time_to_absorption: Any = None
-) -> Dict[Tuple[str, ...], Literal["mean", "var"]]:
-    if time_to_absorption is None:
-        return {}
-
-    if isinstance(time_to_absorption, (str, tuple)):
-        time_to_absorption = [time_to_absorption]
-    if not isinstance(time_to_absorption, dict):
-        time_to_absorption = {ln: "mean" for ln in time_to_absorption}
-
-    res = {}
-    for ln, moment in time_to_absorption.items():
-        if moment not in ("mean", "var"):
-            raise ValueError(
-                f"Moment must be either `'mean'` or `'var'`, found `{moment!r}` in `{ln}`."
-            )
-
-        seen = set()
-        if isinstance(ln, str):
-            ln = tuple(keys) if ln == "all" else (ln,)
-        sorted_ln = tuple(sorted(ln))  # preserve the user order
-
-        if sorted_ln not in seen:
-            seen.add(sorted_ln)
-            for lin in ln:
-                if lin not in keys:
-                    raise ValueError(
-                        f"Invalid absorbing state `{lin!r}` in `{ln}`. "
-                        f"Valid options are `{list(keys)}`."
-                    )
-            res[tuple(ln)] = moment
-
-    return res
-
-
-class AbsProbsMixin:
-    """Mixin that supports computation of absorption probabilities and mean times to absorption."""
+class LinDriversMixin(FateProbsMixin):
+    """Mixin that computes potential driver genes for lineages."""
 
     def __init__(self, **kwargs: Any):
         super().__init__(**kwargs)
+        self._lineage_drivers: Optional[pd.DataFrame] = None
 
-        self._absorption_probabilities: Optional[Lineage] = None
-        self._absorption_times: Optional[pd.DataFrame] = None
-        self._priming_degree: Optional[pd.Series] = None
-
-    @property
-    @d.get_summary(base="abs_probs")
-    def absorption_probabilities(self) -> Optional[Lineage]:
-        """Absorption probabilities.
-
-        Informally, given a (finite, discrete) Markov chain with a set of transient states :math:`T` and
-        a set of absorbing states :math:`A`, the absorption probability for cell :math:`i` from :math:`T`
-        to reach cell :math:`j` from :math:`R` is the probability that a random walk initialized in :math:`i`
-        will reach absorbing state :math:`j`.
-
-        In our context, states correspond to cells, in particular, absorbing states correspond to cells in terminal
-        states.
-        """
-        return self._absorption_probabilities
-
-    @property
-    @d.get_summary(base="abs_times")
-    def absorption_times(self) -> Optional[pd.DataFrame]:
-        """Mean and variance of the time until absorption.
-
-        Related to conditional mean first passage times. Corresponds to the expectation of the time until absorption,
-        depending on initialization, and the variance.
-        """
-        return self._absorption_times
-
-    @property
-    @d.get_summary(base="priming_degree")
-    def priming_degree(self) -> Optional[pd.Series]:
-        """Priming degree.
-
-        Given a cell :math:`i` and a set of terminal states, this quantifies how committed vs. naive cell :math:`i` is,
-        i.e. its degree of pluripotency. Low values correspond to naive cells (high degree of pluripotency), high values
-        correspond to committed cells (low degree of pluripotency).
-        """
-        return self._priming_degree
-
+    @d.get_full_description(base="lineage_drivers")
+    @d.get_sections(base="lineage_drivers", sections=["Parameters", "Returns"])
     @d.dedent
-    def compute_absorption_probabilities(
-        self: AbsProbsProtocol,
-        keys: Optional[Sequence[str]] = None,
-        solver: Union[
-            str, Literal["direct", "gmres", "lgmres", "bicgstab", "gcrotmk"]
-        ] = "gmres",
-        use_petsc: bool = True,
-        time_to_absorption: Optional[
-            Union[
-                Literal["all"],
-                Sequence[Union[str, Sequence[str]]],
-                Dict[Union[str, Sequence[str]], Literal["mean", "var"]],
-            ]
-        ] = None,
-        n_jobs: Optional[int] = None,
-        backend: Backend_t = _DEFAULT_BACKEND,
-        show_progress_bar: bool = True,
-        tol: float = 1e-6,
-        preconditioner: Optional[str] = None,
-    ) -> None:
-        """
-        Compute absorption probabilities.
+    @inject_docs(tm=TestMethod)
+    def compute_lineage_drivers(
+        self: LinDriversProtocol,
+        lineages: Optional[Union[str, Sequence]] = None,
+        method: Literal["fisher", "perm_test"] = TestMethod.FISHER,
+        cluster_key: Optional[str] = None,
+        clusters: Optional[Union[str, Sequence]] = None,
+        layer: Optional[str] = None,
+        use_raw: bool = False,
+        confidence_level: float = 0.95,
+        n_perms: int = 1000,
+        seed: Optional[int] = None,
+        **kwargs: Any,
+    ) -> pd.DataFrame:
+        """Compute driver genes per lineage.
 
-        For each cell, this computes the probability of being absorbed in any of the :attr:`terminal_states`. In
-        particular, this corresponds to the probability that a random walk initialized in transient cell :math:`i`
-        will reach any cell from a fixed transient state before reaching a cell from any other transient state.
+        Correlates gene expression with lineage probabilities, for a given lineage and set of clusters.
+        Often, it makes sense to restrict this to a set of clusters which are relevant for the specified lineages.
 
         Parameters
         ----------
-        keys
-            Terminal states for which to compute the absorption probabilities.
-            If `None`, use all states defined in :attr:`terminal_states`.
-        solver
-            Solver to use for the linear problem. Options are `'direct', 'gmres', 'lgmres', 'bicgstab' or 'gcrotmk'`
-            when ``use_petsc = False`` or one of :class:`petsc4py.PETSc.KPS.Type` otherwise.
-
-            Information on the :mod:`scipy` iterative solvers can be found in :func:`scipy.sparse.linalg` or for
-            :mod:`petsc4py` solver `here <https://petsc.org/release/overview/linear_solve_table/>`__.
-        use_petsc
-            Whether to use solvers from :mod:`petsc4py` or :mod:`scipy`. Recommended for large problems.
-            If no installation is found, defaults to :func:`scipy.sparse.linalg.gmres`.
-        time_to_absorption
-            Whether to compute mean time to absorption and its variance to specific absorbing states.
-
-            If a :class:`dict`, can be specified as ``{{'Alpha': 'var', ...}}`` to also compute variance.
-            In case when states are a :class:`tuple`, time to absorption will be computed to the subset of these states,
-            such as ``[('Alpha', 'Beta'), ...]`` or ``{{('Alpha', 'Beta'): 'mean', ...}}``.
-            Can be specified as ``'all'`` to compute it to any absorbing state in ``keys``, which is more efficient
-            than listing all absorbing states explicitly.
-
-            It might be beneficial to disable the progress bar as ``show_progress_bar = False`` because of many solves.
-        n_jobs
-            Number of parallel jobs to use when using an iterative solver.
-        backend
-            Which backend to use for multiprocessing. See :class:`joblib.Parallel` for valid options.
-        show_progress_bar
-            Whether to show progress bar. Only used when ``solver != 'direct'``.
-        tol
-            Convergence tolerance for the iterative solver. The default is fine for most cases, only consider
-            decreasing this for severely ill-conditioned matrices.
-        preconditioner
-            Preconditioner to use, only available when ``use_petsc = True``. For valid options, see
-            `here <https://petsc.org/release/docs/manual/ksp/?highlight=pctype#preconditioners>`__.
-            We recommend the `'ilu'` preconditioner for badly conditioned problems.
+        lineages
+            Lineage names from :attr:`fate_probabilities`. If :obj:`None`, use all lineages.
+        method
+            Mode to use when calculating p-values and confidence intervals. Valid options are:
+
+            - ``{tm.FISHER!r}`` - Fisher transformation :cite:`fisher:21`.
+            - ``{tm.PERM_TEST!r}`` - permutation test.
+        cluster_key
+            Key in :attr:`~anndata.AnnData.obs` to obtain cluster annotations. These are considered for ``clusters``.
+        clusters
+            Restrict the correlations to these clusters.
+        layer
+            Key from :attr:`~anndata.AnnData.layers` from which to get the expression.
+            If :obj:`None` or `'X'`, use :attr:`~anndata.AnnData.X`.
+        use_raw
+            Whether to use :attr:`~anndata.AnnData.raw` to correlate gene expression.
+        confidence_level
+            Confidence level for the confidence interval calculation. Must be in interval :math:`[0, 1]`.
+        n_perms
+            Number of permutations to use when ``method = {tm.PERM_TEST!r}``.
+        seed
+            Random seed when ``method = {tm.PERM_TEST!r}``.
+        %(parallel)s
+        kwargs
+            Keyword for the correlation test.
 
         Returns
         -------
-        Nothing, just updates the following fields:
+        %(correlation_test.returns)s Also updates the following field:
 
-            - :attr:`absorption_probabilities` - %(abs_probs.summary)s
-            - :attr:`absorption_times` - %(abs_times.summary)s Only if ``time_to_absorption`` is specified.
+        - :attr:`lineage_drivers` - the same :class:`pandas.DataFrame` as described above.
         """
-        if self.terminal_states is None:
-            raise RuntimeError(
-                "Compute terminal states first as `.compute_terminal_states()`."
+        # check that lineage probs have been computed
+        method = TestMethod(method)
+        fate_probs = self.fate_probabilities
+        if fate_probs is None:
+            raise RuntimeError("Compute `.fate_probabilities` first as `.compute_fate_probabilities()`.")
+
+        if fate_probs.shape[1] == 1:
+            logg.warning("There is only 1 lineage present. Using stationary distribution instead")
+            stat_dist = self.eigendecomposition.get("stationary_dist", None)
+            if stat_dist is None:
+                raise RuntimeError("No stationary distribution found in `.eigendecomposition['stationary_dist']`.")
+            fate_probs = Lineage(
+                stat_dist,
+                names=fate_probs.names,
+                colors=fate_probs.colors,
             )
-        if keys is not None:
-            keys = sorted(set(keys))
 
-        start = logg.info("Computing absorption probabilities")
-
-        # get the transition matrix
-        if not issparse(self.transition_matrix):
-            logg.warning(
-                "Attempting to solve a potentially large linear system with dense transition matrix"
-            )
+        # check all lin_keys exist in self.lin_names
+        if isinstance(lineages, str):
+            lineages = [lineages]
+        if lineages is not None:
+            _ = fate_probs[lineages]
+        else:
+            lineages = fate_probs.names
+        lineages = list(lineages)
+
+        if not len(lineages):
+            raise ValueError("No lineages have been selected.")
+
+        # use `cluster_key` and clusters to subset the data
+        if clusters is not None:
+            if cluster_key not in self.adata.obs.keys():
+                raise KeyError(f"Unable to find clusters in `adata.obs[{cluster_key!r}]`.")
+            if isinstance(clusters, str):
+                clusters = [clusters]
+
+            all_clusters = np.array(self.adata.obs[cluster_key].cat.categories)
+            cluster_mask = np.array([name not in all_clusters for name in clusters])
+
+            if any(cluster_mask):
+                raise KeyError(
+                    f"Clusters `{list(np.array(clusters)[cluster_mask])}` not found in "
+                    f"`adata.obs[{cluster_key!r}]`."
+                )
+            subset_mask = np.in1d(self.adata.obs[cluster_key], clusters)
+            adata_comp = self.adata[subset_mask]
+            lin_probs = fate_probs[subset_mask, :]
+        else:
+            adata_comp = self.adata
+            lin_probs = fate_probs
+
+        # check that the layer exists, and that use raw is only used with layer X
+        if layer in (None, "X"):
+            if use_raw and self.adata.raw is None:
+                logg.warning("No raw attribute set. Using `.X` instead")
+                use_raw = False
+            data = adata_comp.raw.X if use_raw else adata_comp.X
+            var_names = adata_comp.raw.var_names if use_raw else adata_comp.var_names
+        else:
+            if layer not in self.adata.layers:
+                raise KeyError(f"Layer `{layer!r}` not found in `adata.layers`.")
+            if use_raw:
+                logg.warning("If `use_raw=True`, layer must be `None`.")
+                use_raw = False
+            data = adata_comp.layers[layer]
+            var_names = adata_comp.var_names
+
+        start = logg.debug(
+            f"Computing correlations for lineages `{sorted(lineages)}` restricted to clusters `{clusters}` in "
+            f"layer `{'X' if layer is None else layer}` with `use_raw={use_raw}`"
+        )
 
-        # process the current annotations according to `keys`
-        term_states, colors = _process_series(
-            series=self.terminal_states, keys=keys, colors=self._term_states_colors
+        lin_probs = lin_probs[lineages]
+        drivers = _correlation_test(
+            data,
+            lin_probs,
+            gene_names=var_names,
+            method=method,
+            n_perms=n_perms,
+            seed=seed,
+            confidence_level=confidence_level,
+            **kwargs,
         )
-        # warn in case only one state is left
-        keys = list(term_states.cat.categories)
-        if len(keys) == 1:
-            logg.warning(
-                "There is only `1` terminal state, all cells will have probability `1` of going there"
-            )
+        params = self._create_params()
+        self._write_lineage_drivers(drivers.loc[var_names], use_raw=use_raw, params=params, time=start)
 
-        # get indices corresponding to recurrent and transient states
-        rec_indices, trans_indices, lookup_dict = _get_cat_and_null_indices(term_states)
-        if not len(trans_indices):
-            raise RuntimeError("Markov chain is irreducible.")
-
-        # create Q (restriction transient-transient), S (restriction transient-recurrent)
-        q = self.transition_matrix[trans_indices, :][:, trans_indices]
-        s = self.transition_matrix[trans_indices, :][:, rec_indices]
+        return drivers
 
-        # take individual solutions and piece them together to get absorption probabilities towards the classes
-        # fmt: off
-        macro_ix_helper = np.cumsum([0] + [len(indices) for indices in lookup_dict.values()])
-        s = np.concatenate([s[:, np.arange(a, b)].sum(axis=1) for a, b in _pairwise(macro_ix_helper)], axis=1)
-        # fmt: on
+    @d.get_sections(base="plot_lineage_drivers", sections=["Parameters"])
+    @d.dedent
+    def plot_lineage_drivers(
+        self: LinDriversProtocol,
+        lineage: str,
+        n_genes: int = 8,
+        use_raw: bool = False,
+        ascending: bool = False,
+        ncols: Optional[int] = None,
+        title_fmt: str = "{gene} qval={qval:.4e}",
+        figsize: Optional[Tuple[float, float]] = None,
+        dpi: Optional[int] = None,
+        save: Optional[Union[str, pathlib.Path]] = None,
+        **kwargs: Any,
+    ) -> None:
+        """Plot lineage drivers.
+
+        Parameters
+        ----------
+        lineage
+            Lineage for which to plot the driver genes.
+        n_genes
+            Top most correlated genes to plot.
+        use_raw
+            Whether to access data in :attr:`~anndata.AnnData.raw` or not.
+        ascending
+            Whether to sort the genes in ascending order.
+        ncols
+            Number of columns.
+        title_fmt
+            Title format. Can include ``{gene}``, ``{pval}``, ``{qval}`` or ``{corr}``, which will be substituted
+            with the actual values.
+        %(plotting)s
+        kwargs
+            Keyword arguments for :func:`~scvelo.pl.scatter`.
+
+        Returns
+        -------
+        %(just_plots)s
+        """
 
-        abs_probs = self._compute_absorption_probabilities(
-            q,
-            s,
-            trans_indices=trans_indices,
-            term_states=term_states,
-            solver=solver,
-            use_petsc=use_petsc,
-            n_jobs=n_jobs,
-            backend=backend,
-            tol=tol,
-            show_progress_bar=show_progress_bar,
-            preconditioner=preconditioner,
+        def prepare_format(
+            gene: str,
+            *,
+            pval: Optional[float],
+            qval: Optional[float],
+            corr: Optional[float],
+        ) -> Dict[str, Any]:
+            kwargs: Dict[str, Optional[Union[str, float]]] = {}
+            if "{gene" in title_fmt:
+                kwargs["gene"] = gene
+            if "{pval" in title_fmt:
+                kwargs["pval"] = float(pval) if pval is not None else np.nan
+            if "{qval" in title_fmt:
+                kwargs["qval"] = float(qval) if qval is not None else np.nan
+            if "{corr" in title_fmt:
+                kwargs["corr"] = float(corr) if corr is not None else np.nan
+
+            return kwargs
+
+        lin_drivers = self.lineage_drivers
+        if lin_drivers is None:
+            raise RuntimeError("Compute `.lineage_drivers` first as `.compute_lineage_drivers()`.")
+
+        key = f"{lineage}_corr"
+        if key not in lin_drivers:
+            raise KeyError(f"Lineage `{key!r}` not found in `{list(lin_drivers.columns)}`.")
+
+        if n_genes <= 0:
+            raise ValueError(f"Expected `n_genes` to be positive, found `{n_genes}`.")
+
+        _ = kwargs.pop("save", None)
+        genes = lin_drivers.sort_values(by=key, ascending=ascending).head(n_genes)
+
+        ncols = 4 if ncols is None else ncols
+        nrows = int(np.ceil(len(genes) / ncols))
+
+        fig, axes = plt.subplots(
+            ncols=ncols,
+            nrows=nrows,
+            dpi=dpi,
+            figsize=(ncols * 6, nrows * 4) if figsize is None else figsize,
         )
-        abs_probs = Lineage(abs_probs, names=keys, colors=colors)
+        axes = np.ravel([axes])
 
-        abs_times = None
-        if time_to_absorption is not None:
-            lineages = _normalize_abs_times(keys, time_to_absorption=time_to_absorption)
-            abs_times = _calculate_lineage_absorption_time_means(
-                q,
-                s,
-                trans_indices=trans_indices,
-                ixs=lookup_dict,
-                lineages=lineages,
-                solver=solver,
-                use_petsc=use_petsc,
-                n_jobs=n_jobs,
-                backend=backend,
-                tol=tol,
-                show_progress_bar=show_progress_bar,
-                preconditioner=preconditioner,
-                index=self.adata.obs_names,
+        _i = 0
+        for _i, (gene, ax) in enumerate(zip(genes.index, axes)):
+            data = genes.loc[gene]
+            scv.pl.scatter(
+                self.adata,
+                color=gene,
+                ncols=ncols,
+                use_raw=use_raw,
+                ax=ax,
+                show=False,
+                title=title_fmt.format(
+                    **prepare_format(
+                        gene,
+                        pval=data.get(f"{lineage}_pval", None),
+                        qval=data.get(f"{lineage}_qval", None),
+                        corr=data.get(f"{lineage}_corr", None),
+                    )
+                ),
+                **kwargs,
             )
 
-        params = self._create_params(
-            remove=["use_petsc", "n_jobs", "backend", "show_progress_bar"]
-        )
-        self._write_absorption_probabilities(
-            abs_probs, abs_times, params=params, time=start
-        )
+        for j in range(_i + 1, len(axes)):
+            axes[j].remove()
+
+        if save is not None:
+            save_fig(fig, save)
 
     @d.dedent
-    def compute_lineage_priming(
-        self: AbsProbsProtocol,
-        method: Literal["kl_divergence", "entropy"] = "kl_divergence",
-        early_cells: Optional[Union[Mapping[str, Sequence[str]], Sequence[str]]] = None,
-    ) -> pd.Series:
-        """
-        %(lin_pd.full_desc)s
+    def plot_lineage_drivers_correlation(
+        self: LinDriversProtocol,
+        lineage_x: str,
+        lineage_y: str,
+        color: Optional[str] = None,
+        gene_sets: Optional[Dict[str, Sequence[str]]] = None,
+        gene_sets_colors: Optional[Sequence[str]] = None,
+        use_raw: bool = False,
+        cmap: str = "RdYlBu_r",
+        fontsize: int = 12,
+        adjust_text: bool = False,
+        legend_loc: Optional[str] = "best",
+        figsize: Optional[Tuple[float, float]] = (4, 4),
+        dpi: Optional[int] = None,
+        save: Optional[Union[str, pathlib.Path]] = None,
+        show: bool = True,
+        **kwargs: Any,
+    ) -> Optional[Axes]:
+        """Show scatter plot of gene-correlations between two lineages.
+
+        Optionally, a :class:`dict` of gene names can be passed to highlight in the plot.
 
         Parameters
         ----------
-        %(lin_pd.parameters)s
-            If a :class:`dict`, the key specifies a cluster key in :attr:`anndata.AnnData.obs` and the values
-            specify cluster labels containing early cells.
+        lineage_x
+            Name of the lineage on the x-axis.
+        lineage_y
+            Name of the lineage on the y-axis.
+        color
+            Key in :attr:`~anndata.AnnData.var` or :attr:`~anndata.AnnData.varm`, preferring for the former.
+        gene_sets
+            Gene sets annotations of the form ``{'gene_set_name': ['gene_1', 'gene_2'], ...}``.
+        gene_sets_colors
+            List of colors where each entry corresponds to a gene set from ``genes_sets``.
+            If `None` and keys in ``gene_sets`` correspond to lineage names, use the lineage colors.
+            Otherwise, use default colors.
+        use_raw
+            Whether to access :attr:`~anndata.AnnData.raw` or not.
+        cmap
+            Colormap to use.
+        fontsize
+            Size of the text when plotting ``gene_sets``.
+        adjust_text
+            Whether to automatically adjust text in order to reduce overlap.
+        legend_loc
+            Position of the legend. If :obj:`None`, don't show the legend. Only used when ``gene_sets != None``.
+        %(plotting)s
+        show
+            If :obj:`False`, return the :class:`~matplotlib.axes.Axes` object.
+        kwargs
+            Keyword arguments for :func:`~scanpy.pl.scatter`.
 
         Returns
         -------
-        %(lin_pd.returns)s
+        If ``show = True``, nothing, just plots, otherwise returns the axes object.
+        Optionally saves it based on ``save``.
+
+        Notes
+        -----
+        This plot is based on the following
+        `notebook <https://github.com/theislab/gastrulation_analysis/blob/main/6_cellrank.ipynb>`_ by *Maren Büttner*.
+        """
+        from cellrank.pl._utils import _position_legend
 
-        Also updates the following field:
+        if use_raw and self.adata.raw is None:
+            logg.warning("No raw attribute set. Setting `use_raw=False`")
+            use_raw = False
+        adata = self.adata.raw if use_raw else self.adata
+        dkey = Key.varm.lineage_drivers(self.backward)
+        # this makes a useless copy, wish there was another way
+        if isinstance(adata, Raw):
+            adata = adata.to_adata()
 
-            - :attr:`priming_degree` - %(priming_degree.summary)s
-        """  # noqa: D400
-        abs_probs = self.absorption_probabilities
-        if abs_probs is None:
+        if color is not None:
+            if not isinstance(color, str):
+                raise TypeError(
+                    "Expected `color` to be either of type `str` or `None`, " f"found `{type(color).__name__}`."
+                )
+            if color not in adata.var and color not in adata.varm[dkey]:
+                raise KeyError(
+                    f"Unable to find key `{color!r}` in `adata{'.raw' if use_raw else ''}.var` "
+                    f"or `adata.{'.raw' if use_raw else ''}varm[{dkey!r}]`."
+                )
+
+        # silent assumption: `.compute_lineage_drivers()` always writes to AnnData
+        key1, key2 = f"{lineage_x}_corr", f"{lineage_y}_corr"
+        if key1 not in adata.varm[dkey] or key2 not in adata.varm[dkey]:
+            haystack = "adata.raw.varm" if use_raw else "adata.varm"
             raise RuntimeError(
-                "Compute absorption probabilities first as `.compute_absorption_probabilities()`."
+                f"Unable to find correlations in `{haystack}[{key1!r}]` or `{haystack}[{key2!r}]`."
+                f"Compute `.lineage_drivers` first as "
+                f"`.compute_lineage_drivers([{lineage_x!r}, {lineage_y!r}], use_raw={use_raw})`."
+            )
+        # produce the actual scatter plot
+        ctx = {"figure.figsize": figsize, "figure.dpi": dpi}
+        for key in list(ctx.keys()):
+            if ctx[key] is None:
+                del ctx[key]
+        with rc_context(ctx), RandomKeys(adata, n=3, where="var") as keys:
+            adata.var[keys[0]] = adata.varm[dkey][key1]
+            adata.var[keys[1]] = adata.varm[dkey][key2]
+            if color is not None:
+                if color in adata.var:
+                    ckey = color
+                else:
+                    adata.var[keys[2]] = adata.varm[dkey][color]
+                    ckey = keys[2]
+
+            ax = sc.pl.scatter(
+                adata,
+                x=keys[0],
+                y=keys[1],
+                color_map=cmap,
+                use_raw=False,
+                show=False,
+                color=None if color is None else ckey,
+                **kwargs,
             )
-        if isinstance(early_cells, dict):
-            if len(early_cells) != 1:
+
+            # add some lines to highlight the origin
+            xmin, xmax = np.nanmin(adata.var[keys[0]]), np.nanmax(adata.var[keys[0]])
+            ymin, ymax = np.nanmin(adata.var[keys[1]]), np.nanmax(adata.var[keys[1]])
+            ax.hlines(0, xmin=xmin, xmax=xmax, color="grey", alpha=0.5, zorder=-1)
+            ax.vlines(0, ymin=ymin, ymax=ymax, color="grey", alpha=0.5, zorder=-1)
+
+        fig = ax.figure
+        ax.set_xlabel(key1)
+        ax.set_ylabel(key2)
+        ax.set_title(color)
+
+        # annotate the passed set of genes
+        if gene_sets is not None:
+            if gene_sets_colors is None:
+                try:
+                    # fmt: off
+                    sets = list(gene_sets.keys())
+                    gene_sets_colors = self.fate_probabilities[sets].colors
+                    # fmt: on
+                except KeyError:
+                    logg.warning("Unable to determine gene sets colors from lineages. Using default colors")
+                    gene_sets_colors = _create_categorical_colors(len(gene_sets))
+            if len(gene_sets_colors) != len(gene_sets):
                 raise ValueError(
-                    f"Expected a dictionary with only 1 key, found `{len(early_cells)}`."
+                    f"Expected `gene_sets_colors` to be of length `{len(gene_sets)}`, "
+                    f"found `{len(gene_sets_colors)}`."
                 )
-            key = next(iter(early_cells.keys()))
-            if key not in self.adata.obs:
-                raise KeyError(f"Unable to find clusters in `adata.obs[{key!r}]`.")
-            if not is_categorical_dtype(self.adata.obs[key]):
-                raise TypeError(
-                    f"Expected `adata.obs[{key!r}]` to be categorical, "
-                    f"found `{infer_dtype(self.adata.obs[key])}`."
-                )
-            early_cells = self.adata.obs[key].isin(early_cells[key])
-        elif early_cells is not None:
-            early_cells = np.asarray(early_cells)
-            if not np.issubdtype(early_cells.dtype, np.bool_):
-                early_cells = np.isin(self.adata.obs_names, early_cells)
 
-        values = pd.Series(
-            abs_probs.priming_degree(method, early_cells), index=self.adata.obs_names
-        )
-        self._write_lineage_priming(values)
+            path_effect = [
+                patheffects.Stroke(linewidth=2, foreground="w", alpha=0.8),
+                patheffects.Normal(),
+            ]
+            annots = []
+            for (key, values), color in zip(gene_sets.items(), gene_sets_colors):
+                arrowprops = (
+                    {
+                        "arrowstyle": ArrowStyle.CurveFilledB(head_width=0.1, head_length=0.2),
+                        "fc": color,
+                        "ec": color,
+                    }
+                    if adjust_text
+                    else None
+                )
+                values = set(values) & set(adata.var_names)
+                for value in values:
+                    x = adata.varm[dkey].loc[value, key1]
+                    y = adata.varm[dkey].loc[value, key2]
+
+                    annot = ax.annotate(
+                        value,
+                        xy=(x, y),
+                        va="top",
+                        ha="left",
+                        path_effects=path_effect,
+                        arrowprops=arrowprops,
+                        size=fontsize,
+                        c=color,
+                    )
+                    annots.append(annot)
+                if values:
+                    ax.scatter([], [], color=color, label=key)
+
+            if adjust_text:
+                try:
+                    import adjustText
+
+                    start = logg.info("Adjusting text position")
+                    adjustText.adjust_text(
+                        annots,
+                        # https://github.com/theislab/cellrank/issues/1033
+                        x=np.array(adata.varm[dkey][key1], copy=True),
+                        y=np.array(adata.varm[dkey][key2], copy=True),
+                        ax=ax,
+                    )
+                    logg.info("    Finish", time=start)
+                except ImportError:
+                    logg.error("Please install `adjustText` first as `pip install adjustText`")
+            if len(annots) and legend_loc not in (None, "none"):
+                _position_legend(ax, legend_loc=legend_loc)
 
-        return values
+        if save is not None:
+            save_fig(fig, path=save)
 
-    def _compute_absorption_probabilities(
-        self: AbsProbsProtocol,
-        q: Union[np.ndarray, spmatrix],
-        s: Union[np.ndarray, spmatrix],
-        trans_indices: np.ndarray,
-        term_states: np.ndim,
-        solver: str,
-        use_petsc: bool,
-        n_jobs: Optional[int],
-        backend: str,
-        tol: float,
-        show_progress_bar: bool,
-        preconditioner: str,
-    ) -> np.ndarray:
-        _abs_classes = _solve_lin_system(
-            q,
-            s,
-            solver=solver,
-            use_petsc=use_petsc,
-            n_jobs=n_jobs,
-            backend=backend,
-            tol=tol,
-            use_eye=True,
-            show_progress_bar=show_progress_bar,
-            preconditioner=preconditioner,
-        )
-        abs_classes = np.zeros(
-            shape=(len(self), len(term_states.cat.categories)), dtype=np.float64
-        )
-        for col, rec_class in enumerate(term_states.cat.categories):
-            rec_indices = np.where(term_states == rec_class)[0]
-            abs_classes[trans_indices, col] = _abs_classes[:, col]
-            abs_classes[rec_indices, col] = 1.0
-
-        mask = abs_classes >= 0
-        if not np.all(mask):
-            raise ValueError(
-                f"`{np.sum(~mask)}` value(s) are negative. Try decreasing the tolerance as `tol=...`, "
-                f"specifying a preconditioner as `preconditioner=...` or "
-                f"use a direct solver as `solver='direct'` if the matrix is small."
-            )
-        mask = np.isclose(abs_classes.sum(1), 1.0, rtol=1e-3)
-        if not np.all(mask):
-            raise ValueError(
-                f"`{np.sum(~mask)}` value(s) do not sum to 1 (rtol=1e-3). Try decreasing the tolerance as `tol=...`, "
-                f"specifying a preconditioner as `preconditioner=...` or "
-                f"use a direct solver as `solver='direct'` if the matrix is small."
-            )
-
-        return abs_classes
+        if not show:
+            return ax
 
     @logger
     @shadow
-    def _write_absorption_probabilities(
-        self: AbsProbsProtocol,
-        abs_probs: Optional[Lineage],
-        abs_times: Optional[pd.DataFrame],
-        params: Mapping[str, Any] = MappingProxyType({}),
+    def _write_fate_probabilities(
+        self: LinDriversProtocol,
+        fate_probs: Optional[Lineage],
+        params: Mapping[str, Any] = types.MappingProxyType({}),
     ) -> str:
-        # fmt: off
-        key1 = Key.obsm.abs_probs(self.backward)
-        self._set("_absorption_probabilities", self.adata.obsm, key=key1, value=abs_probs)
-        key2 = Key.obsm.abs_times(self.backward)
-        self._set("_absorption_times", self.adata.obsm, key=key2, value=abs_times)
-        self._write_lineage_priming(None, log=False)
-        self.params[key1] = dict(params)
-        # fmt: on
-
-        if abs_times is None:
-            return (
-                f"Adding `adata.obsm[{key1!r}]`\n"
-                f"       `.absorption_probabilities`\n"
-                f"    Finish"
-            )
-        return (
-            f"Adding `adata.obsm[{key1!r}]`\n"
-            f"       `adata.obsm[{key2!r}]`\n"
-            f"       `.absorption_probabilities`\n"
-            f"       `.absorption_times`\n"
-            f"    Finish"
-        )
+        self._write_lineage_drivers(None, use_raw=False, log=False)
+        with contextlib.suppress(AttributeError):
+            self._write_lineage_drivers(None, use_raw=True, log=False)
 
-    def _ensure_lineage_object(
-        self: AbsProbsProtocol, attr: str, **kwargs: Any
-    ) -> None:
-        if isinstance(getattr(self, attr), np.ndarray):
-            try:
-                setattr(
-                    self,
-                    attr,
-                    Lineage.from_adata(self.adata, backward=self.backward, **kwargs),
-                )
-            except Exception as e:  # noqa: B902
-                raise RuntimeError(
-                    f"Unable to reconstruct `.absorption_probabilities`. Reason: `{e}`."
-                ) from None
+        return super()._write_fate_probabilities(fate_probs, params=params, log=False)
 
     @logger
     @shadow
-    def _write_lineage_priming(
-        self: AbsProbsProtocol, priming_degree: Optional[pd.Series]
+    def _write_lineage_drivers(
+        self: LinDriversProtocol,
+        drivers: Optional[pd.DataFrame],
+        use_raw: bool,
+        params: Mapping[str, Any] = types.MappingProxyType({}),
     ) -> str:
-        self._priming_degree = priming_degree
-        key = Key.obs.priming_degree(self.backward)
-        self._set("_priming_degree", self.adata.obs, key=key, value=priming_degree)
-
-        return f"Adding `adata.obs[{key!r}]`\n       `.priming_degree`\n    Finish"
-
-    def _read_absorption_probabilities(
-        self: AbsProbsProtocol, anndata: AnnData
-    ) -> bool:
         # fmt: off
-        with SafeGetter(self, allowed=KeyError) as sg:
-            key1 = Key.obsm.abs_probs(self.backward)
-            self._get("_absorption_probabilities", self.adata.obsm, key=key1, where="obsm", dtype=(np.ndarray, Lineage))
-            self._ensure_lineage_object("_absorption_probabilities", kind="abs_probs")
-            key = Key.obsm.abs_times(self.backward)
-            self._get("_absorption_times", self.adata.obsm, key=key, where="obsm", dtype=pd.DataFrame,
-                      allow_missing=True)
-            key = Key.obs.priming_degree(self.backward)
-            self._get("_priming_degree", self.adata.obs, key=key, where="obs", dtype=pd.Series, allow_missing=True)
-            self.params[key1] = self._read_params(key1)
+        key = Key.varm.lineage_drivers(self.backward)
+        self._set("_lineage_drivers", self.adata.raw.varm if use_raw else self.adata.varm, key=key, value=drivers)
+        self.params[key] = dict(params)
         # fmt: on
 
+        return f"Adding `adata.{'raw.' if use_raw else ''}varm[{key!r}]`\n" f"       `.lineage_drivers`\n" "    Finish"
+
+    def _read_fate_probabilities(self: LinDriversProtocol, adata: AnnData) -> bool:
+        ok = super()._read_fate_probabilities(adata)
+        if not ok:
+            return False
+
+        key = Key.varm.lineage_drivers(self.backward)
+        with SafeGetter(self, allowed=(KeyError, AttributeError)) as sg:
+            self.params[key] = self._read_params(key)
+            if self.params[key].get("use_raw", False):
+                self._lineage_drivers = self._get(
+                    obj=self.adata.raw.varm,
+                    key=key,
+                    shadow_attr="varm",
+                    dtype=pd.DataFrame,
+                )
+            else:
+                self._lineage_drivers = self._get(obj=self.adata.varm, key=key, shadow_attr="varm", dtype=pd.DataFrame)
+
         return sg.ok
 
-    plot_absorption_probabilities = register_plotter(
-        continuous="absorption_probabilities"
-    )
+    @property
+    @d.dedent
+    def lineage_drivers(self) -> Optional[pd.DataFrame]:
+        """Potential lineage drivers.
+
+        Computes Pearson correlation of each gene with fate probabilities for every terminal state. High Pearson
+        correlation indicates potential lineage drivers. Also computes p-values and confidence intervals.
+
+        Returns
+        -------
+        %(correlation_test.returns)s
+        """
+        return self._lineage_drivers
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cellrank-1.5.1/cellrank/tl/estimators/mixins/decomposition/_eigen.py` & `cellrank-2.0.0/src/cellrank/estimators/mixins/decomposition/_eigen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,79 @@
-from typing import Any, Dict, Tuple, Union, Mapping, Optional
-from typing_extensions import Literal
+import pathlib
+import types
+from typing import Any, Dict, Literal, Mapping, Optional, Tuple, Union
 
-from types import MappingProxyType
-from pathlib import Path
+import numpy as np
+import scipy.sparse as sp
+
+import matplotlib.pyplot as plt
+from matplotlib.ticker import FormatStrFormatter, MultipleLocator
 
 from anndata import AnnData
-from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.ul._docs import d
-from cellrank.tl._utils import save_fig, _eigengap
-from cellrank.tl.estimators._utils import SafeGetter
-from cellrank.tl.estimators.mixins._utils import BaseProtocol, logger, shadow
 
-import numpy as np
-from scipy.sparse import issparse, spmatrix
-from scipy.sparse.linalg import eigs
+from cellrank import logging as logg
+from cellrank._utils._docs import d
+from cellrank._utils._key import Key
+from cellrank._utils._utils import _eigengap, save_fig
+from cellrank.estimators.mixins._utils import BaseProtocol, SafeGetter, logger, shadow
 
-import matplotlib.pyplot as plt
-from matplotlib.ticker import MultipleLocator, FormatStrFormatter
+__all__ = ["EigenMixin"]
 
 EPS = np.finfo(np.float64).eps
 
 
-class EigenProtocol(BaseProtocol):  # noqa: D101
+class EigenProtocol(BaseProtocol):
     @property
-    def transition_matrix(self) -> Union[np.ndarray, spmatrix]:  # noqa: D102
+    def transition_matrix(self) -> Union[np.ndarray, sp.spmatrix]:
         ...
 
     def _write_eigendecomposition(
-        self, decomp: Dict[str, Any], params: Mapping[str, Any] = MappingProxyType({})
+        self, decomp: Dict[str, Any], params: Mapping[str, Any] = types.MappingProxyType({})
     ) -> str:
         ...
 
 
 class EigenMixin:
     """Mixin that computes Schur decomposition."""
 
     def __init__(self, **kwargs: Any):
         super().__init__(**kwargs)
-
         self._eigendecomposition = None
 
     @property
     @d.get_summary(base="eigen")
     def eigendecomposition(self) -> Optional[Dict[str, Any]]:
-        """Eigendecomposition of :attr:`transition_matrix`.
+        """Eigendecomposition of the :attr:`transition_matrix`.
 
         For non-symmetric real matrices, left and right eigenvectors will in general be different and complex. We
         compute both left and right eigenvectors.
 
         Returns
         -------
         A dictionary with the following keys:
 
-            - `'D'` - the eigenvalues.
-            - `'eigengap'` - the eigengap.
-            - `'params'` - parameters used for the computation.
-            - `'V_l'` - left eigenvectors (optional).
-            - `'V_r'` - right eigenvectors (optional).
-            - `'stationary_dist'` - stationary distribution of :attr:`transition_matrix`, if present.
+        - ``'D'`` - the eigenvalues.
+        - ``'eigengap'`` - the `eigengap <https://en.wikipedia.org/wiki/Eigengap>`__.
+        - ``'params'`` - parameters used for the computation.
+        - ``'V_l'`` - left eigenvectors (optional).
+        - ``'V_r'`` - right eigenvectors (optional).
+        - ``'stationary_dist'`` - stationary distribution of the :attr:`transition_matrix`, if present.
         """
         return self._eigendecomposition
 
     @d.dedent
     def compute_eigendecomposition(
         self: EigenProtocol,
         k: int = 20,
         which: Literal["LR", "LM"] = "LR",
         alpha: float = 1.0,
         only_evals: bool = False,
         ncv: Optional[int] = None,
-    ) -> None:
-        """
-        Compute eigendecomposition of :attr:`transition_matrix`.
+    ) -> "EigenMixin":
+        """Compute eigendecomposition of the :attr:`transition_matrix`.
 
         Uses a sparse implementation, if possible, and only computes the top :math:`k` eigenvectors
         to speed up the computation. Computes both left and right eigenvectors.
 
         Parameters
         ----------
         k
@@ -85,42 +82,40 @@
         only_evals
             Whether to compute only eigenvalues.
         ncv
             Number of Lanczos vectors generated.
 
         Returns
         -------
-        Nothing, just updates the following field:
+        Self and updates the following fields:
 
-            - :attr:`eigendecomposition` - %(eigen.summary)s
+        - :attr:`eigendecomposition` - %(eigen.summary)s
         """
 
         def get_top_k_evals() -> np.ndarray:
             return D[np.flip(np.argsort(D.real))][:k]
 
         start = logg.info("Computing eigendecomposition of the transition matrix")
 
-        if issparse(self.transition_matrix):
+        if sp.issparse(self.transition_matrix):
             logg.debug(f"Computing top `{k}` eigenvalues of a sparse matrix")
-            D, V_l = eigs(self.transition_matrix.T, k=k, which=which, ncv=ncv)
+            D, V_l = sp.linalg.eigs(self.transition_matrix.T, k=k, which=which, ncv=ncv)
             if only_evals:
                 self._write_eigendecomposition(
                     {
                         "D": get_top_k_evals(),
                         "eigengap": _eigengap(get_top_k_evals().real, alpha),
                         "params": {"which": which, "k": k, "alpha": alpha},
                     },
                     time=start,
                 )
                 return
-            _, V_r = eigs(self.transition_matrix, k=k, which=which, ncv=ncv)
+            _, V_r = sp.linalg.eigs(self.transition_matrix, k=k, which=which, ncv=ncv)
         else:
-            logg.warning(
-                "This transition matrix is not sparse, computing full eigendecomposition"
-            )
+            logg.warning("This transition matrix is not sparse, computing full eigendecomposition")
             D, V_l = np.linalg.eig(self.transition_matrix.T)
             if only_evals:
                 self._write_eigendecomposition(
                     {
                         "D": get_top_k_evals(),
                         "eigengap": _eigengap(D.real, alpha),
                         "params": {"which": which, "k": k, "alpha": alpha},
@@ -146,69 +141,68 @@
                 "V_l": V_l,
                 "V_r": V_r,
                 "eigengap": e_gap,
                 "params": {"which": which, "k": k, "alpha": alpha},
             },
             time=start,
         )
+        return self
 
     @d.dedent
     def plot_spectrum(
         self,
         n: Optional[int] = None,
-        real_only: bool = False,
+        real_only: Optional[bool] = None,
         show_eigengap: bool = True,
         show_all_xticks: bool = True,
         legend_loc: Optional[str] = None,
         title: Optional[str] = None,
         marker: str = ".",
         figsize: Optional[Tuple[float, float]] = (5, 5),
         dpi: int = 100,
-        save: Optional[Union[str, Path]] = None,
+        save: Optional[Union[str, pathlib.Path]] = None,
         **kwargs: Any,
     ) -> None:
-        """
-        Plot the top eigenvalues in real or complex plane.
+        """Plot the top eigenvalues in a real or a complex plane.
 
         Parameters
         ----------
         n
-            Number of eigenvalues to show. If `None`, show all that have been computed.
+            Number of eigenvalues to show. If :obj:`None`, show all that have been computed.
         real_only
             Whether to plot only the real part of the spectrum.
+            If :obj:`None`, plot real spectrum if no complex eigenvalues are present.
         show_eigengap
-            When ``real_only = True``, this determines whether to show the inferred eigengap as
-            a dotted line.
+            When ``real_only = True``, this determines whether to show the inferred eigengap as a dotted line.
         show_all_xticks
             When ``real_only = True``, this determines whether to show the indices of all eigenvalues on the x-axis.
         legend_loc
             Location parameter for the legend.
         title
             Title of the figure.
         marker
-            Marker symbol used, valid options can be found in :mod:`matplotlib.markers`.
+            Marker symbol used, valid options can be found in :mod:`~matplotlib.markers`.
         %(plotting)s
         kwargs
-            Keyword arguments for :func:`matplotlib.pyplot.scatter`.
+            Keyword arguments for :meth:`~matplotlib.axes.Axes.scatter`.
 
         Returns
         -------
         %(just_plots)s
         """
-
         eig = self.eigendecomposition
         if eig is None:
-            raise RuntimeError(
-                "Compute eigendecomposition first as `.compute_eigendecomposition()`."
-            )
+            raise RuntimeError("Compute eigendecomposition first as `.compute_eigendecomposition()`.")
 
         if n is None:
             n = len(eig["D"])
         if n <= 0:
             raise ValueError(f"Expected `n` to be > 0, found `{n}`.")
+        if real_only is None:
+            real_only = np.any(np.iscomplex(eig["D"][:n]))
 
         if real_only:
             fig = self._plot_real_spectrum(
                 n,
                 show_eigengap=show_eigengap,
                 show_all_xticks=show_all_xticks,
                 dpi=dpi,
@@ -237,17 +231,17 @@
         n: int,
         dpi: int = 100,
         figsize: Optional[Tuple[float, float]] = None,
         legend_loc: Optional[str] = None,
         title: Optional[str] = None,
         marker: str = ".",
         **kwargs: Any,
-    ):
+    ) -> plt.Figure:
         # define a function to make the data limits rectangular
-        def adapt_range(min_, max_, range_):
+        def adapt_range(min_: float, max_: float, range_: float) -> Tuple[float, float]:
             return (
                 min_ + (max_ - min_) / 2 - range_ / 2,
                 min_ + (max_ - min_) / 2 + range_ / 2,
             )
 
         eig = self.eigendecomposition
         D, params = eig["D"][:n], eig["params"]
@@ -294,16 +288,16 @@
         show_eigengap: bool = True,
         show_all_xticks: bool = True,
         dpi: int = 100,
         figsize: Optional[Tuple[float, float]] = None,
         legend_loc: Optional[str] = None,
         title: Optional[str] = None,
         marker: str = ".",
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> plt.Figure:
         eig = self.eigendecomposition
         D, params = eig["D"][:n], eig["params"]
 
         D_real, D_imag = D.real, D.imag
         ixs = np.arange(len(D))
         mask = D_imag == 0
 
@@ -329,14 +323,15 @@
         # add dashed line for the eigengap, ticks, labels, title and legend
         if show_eigengap and eig["eigengap"] < n:
             ax.axvline(eig["eigengap"], label="eigengap", ls="--", lw=2, c="k")
 
         ax.set_xlabel("index")
         if show_all_xticks:
             ax.set_xticks(np.arange(len(D)))
+            ax.set_xticklabels(np.arange(1, len(D) + 1))
         else:
             ax.xaxis.set_major_locator(MultipleLocator(2.0))
             ax.xaxis.set_major_formatter(FormatStrFormatter("%d"))
 
         ax.set_ylabel(r"Re($\lambda_i$)")
 
         key = "real part" if params["which"] == "LR" else "magnitude"
@@ -350,31 +345,29 @@
         return fig
 
     @logger
     @shadow
     def _write_eigendecomposition(
         self: EigenProtocol,
         decomp: Dict[str, Any],
-        params: Mapping[str, Any] = MappingProxyType({}),
+        params: Mapping[str, Any] = types.MappingProxyType({}),
     ) -> str:
         key = Key.uns.eigen(self.backward)
         self._set("_eigendecomposition", self.adata.uns, key=key, value=decomp)
         params = params or decomp.get("params", {})
         self.params[key] = dict(params)
 
-        return (
-            f"Adding `adata.uns[{key!r}]`\n"
-            f"       `.eigendecomposition`\n"
-            "    Finish"
-        )
+        return f"Adding `adata.uns[{key!r}]`\n" f"       `.eigendecomposition`\n" "    Finish"
 
-    def _read_eigendecomposition(
-        self: EigenProtocol, adata: AnnData, allow_missing: bool = True
-    ) -> bool:
-        # fmt: off
+    def _read_eigendecomposition(self: EigenProtocol, adata: AnnData, allow_missing: bool = True) -> bool:
         key = Key.uns.eigen(self.backward)
         with SafeGetter(self, allowed=KeyError) as sg:
-            self._get("_eigendecomposition", adata.uns, key=key, where="uns", dtype=dict, allow_missing=allow_missing)
+            self._eigendecomposition = self._get(
+                obj=adata.uns,
+                key=key,
+                shadow_attr="uns",
+                dtype=dict,
+                allow_missing=allow_missing,
+            )
             self.params[key] = self._read_params(key)
-        # fmt: on
 
         return sg.ok
```

### Comparing `cellrank-1.5.1/cellrank/tl/estimators/mixins/decomposition/_schur.py` & `cellrank-2.0.0/src/cellrank/estimators/mixins/decomposition/_schur.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,62 @@
-from typing import Any, Dict, Tuple, Union, Mapping, Optional
-from typing_extensions import Literal
+import contextlib
+import io
+import pathlib
+import types
+from typing import Any, Dict, Literal, Mapping, Optional, Tuple, Union
 
-from types import MappingProxyType
-from pathlib import Path
 from pygpcca import GPCCA
 from pygpcca._sorted_schur import _check_conj_split
 
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.ul._docs import d
-from cellrank.tl._utils import save_fig, _eigengap
-from cellrank.tl.estimators._utils import SafeGetter
-from cellrank.tl.estimators.mixins._utils import BaseProtocol, logger, shadow
-
 import numpy as np
-from scipy.sparse import issparse, spmatrix
+import scipy.sparse as sp
 
 import matplotlib.pyplot as plt
-from seaborn import heatmap
+import seaborn as sns
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
+from anndata import AnnData
+
+from cellrank import logging as logg
+from cellrank._utils._docs import d
+from cellrank._utils._key import Key
+from cellrank._utils._utils import _eigengap, save_fig
+from cellrank.estimators.mixins._utils import BaseProtocol, SafeGetter, logger, shadow
+
+__all__ = ["SchurMixin"]
+
 EPS = np.finfo(np.float64).eps
 
 
-class SchurProtocol(BaseProtocol):  # noqa: D101
-    def transition_matrix(self) -> Union[np.ndarray, spmatrix]:  # noqa: D102
+class SchurProtocol(BaseProtocol):
+    _gpcca: Optional[GPCCA] = None
+    _invalid_n_states: Optional[np.ndarray] = None
+
+    schur_vectors: Optional[np.ndarray] = None
+    _schur_matrix: Optional[np.ndarray] = None
+    _eigendecomposition: Optional[Dict[str, Any]] = None
+
+    def transition_matrix(self) -> Union[np.ndarray, sp.spmatrix]:
         ...
 
     def _write_schur_decomposition(
         self,
         decomp: Dict[str, Any],
         vectors: np.ndarray,
         matrix: np.ndarray,
-        params: Mapping[str, Any] = MappingProxyType({}),
+        params: Mapping[str, Any] = types.MappingProxyType({}),
     ) -> str:
         ...
 
 
 class SchurMixin:
     """Mixin that computes Schur decomposition."""
 
     def __init__(self, **kwargs: Any):
         super().__init__(**kwargs)
-
         self._gpcca: Optional[GPCCA] = None
         self._invalid_n_states: Optional[np.ndarray] = None
 
         self._schur_vectors: Optional[np.ndarray] = None
         self._schur_matrix: Optional[np.ndarray] = None
         self._eigendecomposition: Optional[Dict[str, Any]] = None
 
@@ -57,14 +66,15 @@
     def schur_vectors(self) -> Optional[np.ndarray]:
         """Real Schur vectors of the transition matrix.
 
         The real Schur decomposition is a generalization of the Eigendecomposition and can be computed for any
         real-valued, square matrix :math:`A`. It is given by :math:`A = Q R Q^T`, where :math:`Q` contains the
         real Schur vectors and :math:`R` is the Schur matrix. :math:`Q` is orthogonal and :math:`R` is quasi-upper
         triangular with 1x1 and 2x2 blocks on the diagonal.
+
         If PETSc and SLEPc are installed, only the leading Schur vectors are computed.
         """
         return self._schur_vectors
 
     @property
     @d.get_summary(base="schur_matrix")
     @d.dedent
@@ -74,119 +84,113 @@
         %(schur_vectors.summary_ext)s
         """
         return self._schur_matrix
 
     @property
     @d.get_summary(base="eigen")
     def eigendecomposition(self) -> Optional[Dict[str, Any]]:
-        """Eigendecomposition of :attr:`transition_matrix`.
+        """Eigendecomposition of the :attr:`transition_matrix`.
 
-        For non-symmetric real matrices, left and right eigenvectors will in general be different and complex. We
-        compute both left and right eigenvectors.
+        For non-symmetric real matrices, left and right eigenvectors will in general be different and complex.
+        We compute both left and right eigenvectors.
 
         Returns
         -------
         A dictionary with the following keys:
 
-            - `'D'` - the eigenvalues.
-            - `'eigengap'` - the eigengap.
-            - `'params'` - parameters used for the computation.
-            - `'V_l'` - left eigenvectors (optional).
-            - `'V_r'` - right eigenvectors (optional).
-            - `'stationary_dist'` - stationary distribution of :attr:`transition_matrix`, if present.
+        - ``'D'`` - the eigenvalues.
+        - ``'eigengap'`` - the `eigengap <https://en.wikipedia.org/wiki/Eigengap>`__.
+        - ``'params'`` - parameters used for the computation.
+        - ``'V_l'`` - left eigenvectors (optional).
+        - ``'V_r'`` - right eigenvectors (optional).
+        - ``'stationary_dist'`` - stationary distribution of the :attr:`transition_matrix`, if present.
         """
         return self._eigendecomposition
 
     @d.dedent
     def compute_schur(
         self: SchurProtocol,
-        n_components: int = 10,
+        n_components: int = 20,
         initial_distribution: Optional[np.ndarray] = None,
         method: Literal["krylov", "brandts"] = "krylov",
         which: Literal["LR", "LM"] = "LR",
         alpha: float = 1.0,
-    ):
-        """
-        Compute Schur decomposition.
+        verbose: Optional[bool] = None,
+    ) -> "SchurMixin":
+        """Compute the Schur decomposition.
 
         Parameters
         ----------
         n_components
             Number of Schur vectors to compute.
         initial_distribution
-            Input distribution over all cells. If `None`, uniform distribution is used.
+            Input distribution over all cells. If :obj:`None`, uniform distribution is used.
         method
             Method for calculating the Schur vectors. Valid options are:
 
-                - `'krylov'` - an iterative procedure that computes a partial, sorted Schur decomposition for
-                  large, sparse matrices.
-                - `'brandts'` - full sorted Schur decomposition of a dense matrix.
+            - ``'krylov'`` - an iterative procedure that computes a partial, sorted Schur decomposition for
+              large, sparse matrices.
+            - ``'brandts'`` - full sorted Schur decomposition of a dense matrix.
 
-            For benefits of each method, see :class:`pygpcca.GPCCA`.
+            For benefits of each method, see :class:`~pygpcca.GPCCA`.
         %(eigen)s
+        verbose
+            Whether to print extra information when computing the Schur decomposition.
+            If :obj:`None`, it's disabled when ``method = 'krylov'``.
 
         Returns
         -------
-        Nothing, just updates the following fields:
+        Self and just updates the following fields:
 
-            - :attr:`schur_vectors` - %(schur_vectors.summary)s
-            - :attr:`schur_matrix` -  %(schur_matrix.summary)s
-            - :attr:`eigendecomposition` - %(eigen.summary)s
+        - :attr:`schur_vectors` - %(schur_vectors.summary)s
+        - :attr:`schur_matrix` -  %(schur_matrix.summary)s
+        - :attr:`eigendecomposition` - %(eigen.summary)s
         """
+        from cellrank._utils._linear_solver import _is_petsc_slepc_available
+
         if n_components < 2:
             logg.warning(
-                f"Number of Schur vectors `>=2`, but only `{n_components}` "
-                f"were requested. Using `n_components=2`"
+                f"Number of Schur vectors `>=2`, but only `{n_components}` " f"were requested. Using `n_components=2`"
             )
             n_components = 2
 
         if method not in ("brandts", "krylov"):
-            raise ValueError(
-                f"Invalid method `{method!r}`. Valid options are:`'brandts'` or `'krylov'`."
-            )
+            raise ValueError(f"Invalid method `{method!r}`. Valid options are:`'brandts'` or `'krylov'`.")
 
-        try:
-            import petsc4py
-            import slepc4py
-        except ImportError:
+        if not _is_petsc_slepc_available():
             method = "brandts"
-            logg.warning(
-                f"Unable to import `petsc4py` or `slepc4py`. Using `method={method!r}`"
-            )
+            logg.warning(f"Unable to import `petsc4py` or `slepc4py`. Using `method={method!r}`")
+        if verbose is None:
+            verbose = method == "brandts"
 
         tmat = self.transition_matrix
-        if method == "brandts" and issparse(self.transition_matrix):
+        if method == "brandts" and sp.issparse(self.transition_matrix):
             logg.warning("For `method='brandts'`, dense matrix is required. Densifying")
             tmat = tmat.A
 
         self._gpcca = GPCCA(tmat, eta=initial_distribution, z=which, method=method)
         start = logg.info("Computing Schur decomposition")
 
-        try:
-            self._gpcca._do_schur_helper(n_components)
-        except ValueError as e:
-            if "will split complex conjugate eigenvalues" not in str(e):
-                raise
-            logg.warning(
-                f"Using `{n_components}` components would split a block of complex conjugate eigenvalues. "
-                f"Using `n_components={n_components + 1}`"
-            )
-            self._gpcca._do_schur_helper(n_components + 1)
+        with (contextlib.nullcontext if verbose else contextlib.redirect_stdout)(io.StringIO()):
+            try:
+                self._gpcca._do_schur_helper(n_components)
+            except ValueError as e:
+                if "will split complex conjugate eigenvalues" not in str(e):
+                    raise
+                logg.warning(
+                    f"Using `{n_components}` components would split a block of complex conjugate eigenvalues. "
+                    f"Using `n_components={n_components + 1}`"
+                )
+                self._gpcca._do_schur_helper(n_components + 1)
 
         self._invalid_n_states = np.array(
-            [
-                i
-                for i in range(2, len(self._gpcca._p_eigenvalues))
-                if _check_conj_split(self._gpcca._p_eigenvalues[:i])
-            ]
+            [i for i in range(2, len(self._gpcca._p_eigenvalues)) if _check_conj_split(self._gpcca._p_eigenvalues[:i])]
         )
         if len(self._invalid_n_states):
-            logg.info(
-                f"When computing macrostates, choose a number of states NOT in `{list(self._invalid_n_states)}`"
-            )
+            logg.info(f"When computing macrostates, choose a number of states NOT in `{list(self._invalid_n_states)}`")
 
         self._write_schur_decomposition(
             {
                 "D": self._gpcca._p_eigenvalues,
                 "eigengap": _eigengap(self._gpcca._p_eigenvalues, alpha),
                 "params": {
                     "which": which,
@@ -195,64 +199,62 @@
                 },
             },
             vectors=self._gpcca._p_X,
             matrix=self._gpcca._p_R,
             params=self._create_params(),
             time=start,
         )
+        return self
 
     @d.dedent
     def plot_schur_matrix(
         self,
         title: Optional[str] = "schur matrix",
         cmap: str = "viridis",
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[float] = 80,
-        save: Optional[Union[str, Path]] = None,
+        save: Optional[Union[str, pathlib.Path]] = None,
         **kwargs: Any,
-    ):
-        """
-        Plot the Schur matrix.
+    ) -> None:
+        """Plot the Schur matrix.
 
         Parameters
         ----------
         title
             Title of the figure.
         cmap
             Colormap to use.
         %(plotting)s
         kwargs
-            Keyword arguments for :func:`seaborn.heatmap`.
+            Keyword arguments for :func:`~seaborn.heatmap`.
 
         Returns
         -------
         %(just_plots)s
         """
         schur_matrix = self.schur_matrix
         if schur_matrix is None:
             raise RuntimeError("Compute Schur matrix first as `.compute_schur()`.")
 
-        fig, ax = plt.subplots(
-            figsize=schur_matrix.shape if figsize is None else figsize, dpi=dpi
-        )
+        fig, ax = plt.subplots(figsize=schur_matrix.shape if figsize is None else figsize, dpi=dpi)
 
         divider = make_axes_locatable(ax)  # square=True make the colorbar a bit bigger
         cbar_ax = divider.append_axes("right", size="2%", pad=0.1)
 
         mask = np.zeros_like(schur_matrix, dtype=np.bool_)
         mask[np.tril_indices_from(mask, k=-1)] = True
         mask[~np.isclose(schur_matrix, 0.0)] = False
 
         vmin, vmax = (
             np.min(schur_matrix[~mask]),
             np.max(schur_matrix[~mask]),
         )
 
         kwargs["fmt"] = kwargs.get("fmt", "0.2f")
-        heatmap(
+        sns.heatmap(
             data=schur_matrix,
             cmap=cmap,
             square=True,
             annot=True,
             vmin=vmin,
             vmax=vmax,
             cbar_ax=cbar_ax,
@@ -271,15 +273,15 @@
     @logger
     @shadow
     def _write_schur_decomposition(
         self: SchurProtocol,
         decomp: Dict[str, Any],
         vectors: np.ndarray,
         matrix: np.ndarray,
-        params: Mapping[str, Any] = MappingProxyType({}),
+        params: Mapping[str, Any] = types.MappingProxyType({}),
     ) -> str:
         key = Key.uns.schur_matrix(self.backward)
         self._set("_schur_matrix", self.adata.uns, key=key, value=matrix)
         key = Key.obsm.schur_vectors(self.backward)
         self._set("_schur_vectors", self.adata.obsm, key=key, value=vectors)
         key = Key.uns.eigen(self.backward)
         self._set("_eigendecomposition", self.adata.uns, key=key, value=decomp)
@@ -289,25 +291,37 @@
             f"Adding `adata.uns[{key!r}]`\n"
             f"       `.schur_vectors`\n"
             f"       `.schur_matrix`\n"
             f"       `.eigendecomposition`\n"
             "    Finish"
         )
 
-    def _read_schur_decomposition(
-        self: SchurProtocol, adata: AnnData, allow_missing: bool = True
-    ) -> bool:
-        # fmt: off
+    def _read_schur_decomposition(self: SchurProtocol, adata: AnnData, allow_missing: bool = True) -> bool:
         key = Key.uns.eigen(self.backward)
         with SafeGetter(self, allowed=KeyError) as sg:
-            self._get("_eigendecomposition", adata.uns, key=key, where="uns", dtype=dict, allow_missing=allow_missing)
+            self._eigendecomposition = self._get(
+                obj=adata.uns,
+                key=key,
+                shadow_attr="uns",
+                dtype=dict,
+                allow_missing=allow_missing,
+            )
             key = Key.obsm.schur_vectors(self.backward)
-            self._get("_schur_vectors", self.adata.obsm, key=key, where="obsm", dtype=np.ndarray,
-                      allow_missing=allow_missing)
+            self._schur_vectors = self._get(
+                obj=self.adata.obsm,
+                key=key,
+                shadow_attr="obsm",
+                dtype=np.ndarray,
+                allow_missing=allow_missing,
+            )
             key = Key.uns.schur_matrix(self.backward)
-            self._get("_schur_matrix", self.adata.uns, key=key, where="uns", dtype=np.ndarray,
-                      allow_missing=allow_missing)
+            self._schur_matrix = self._get(
+                obj=self.adata.uns,
+                key=key,
+                shadow_attr="uns",
+                dtype=np.ndarray,
+                allow_missing=allow_missing,
+            )
             key = f"schur_decomposition_{Key.backward(self.backward)}"
             self.params[key] = self._read_params(key)
-        # fmt: on
 
         return sg.ok
```

### Comparing `cellrank-1.5.1/cellrank/tl/estimators/terminal_states/_cflare.py` & `cellrank-2.0.0/src/cellrank/estimators/terminal_states/_cflare.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,146 +1,141 @@
-from typing import Any, Dict, List, Union, Optional, Sequence
-from typing_extensions import Literal
+from typing import Any, Dict, List, Literal, Optional, Sequence, Union
+
+import numpy as np
+import pandas as pd
+import scipy.stats as st
 
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank.ul._docs import d
-from cellrank.tl._utils import (
+from cellrank._utils._docs import d
+from cellrank._utils._utils import (
     _cluster_X,
-    _filter_cells,
     _complex_warning,
+    _filter_cells,
     _get_connectivities,
 )
-from cellrank.tl.kernels._utils import _get_basis
-from cellrank.tl.estimators.mixins import EigenMixin, LinDriversMixin
-from cellrank.tl.estimators.terminal_states._term_states_estimator import (
+from cellrank.estimators.mixins import EigenMixin, LinDriversMixin
+from cellrank.estimators.terminal_states._term_states_estimator import (
     TermStatesEstimator,
 )
+from cellrank.kernels._utils import _get_basis
 
-import numpy as np
-import pandas as pd
-from scipy.stats import zscore
+__all__ = ["CFLARE"]
 
 
 @d.dedent
 class CFLARE(TermStatesEstimator, LinDriversMixin, EigenMixin):
-    """
-    Compute the initial/terminal states of a Markov chain via spectral heuristics.
+    """Clustering and filtering of left and right eigenvectors (CFLARE).
 
-    This estimator uses the left eigenvectors of the transition matrix to filter to a set of recurrent cells
-    and the right eigenvectors to cluster this set of cells into discrete groups.
+    This estimator computes initial and terminal states, as well as fate probabilities.
+    It uses the left eigenvectors of the transition matrix to filter to a set of (approximately)
+    recurrent cells and the right eigenvectors to cluster this set of cells into discrete groups.
+    CFLARE exists mostly for legacy reasons, we recommend using the :class:`cellrank.estimators.GPCCA`
+    estimator, which is mathematically more principled.
 
     Parameters
     ----------
     %(base_estimator.parameters)s
     """
 
     @d.dedent
     def fit(self, k: int = 20, **kwargs: Any) -> "TermStatesEstimator":
-        """
-        Prepare self for terminal states prediction.
+        """Prepare self for terminal states prediction.
 
         Parameters
         ----------
         k
             Number of eigenvectors to compute.
         kwargs
             Keyword arguments for :meth:`compute_eigendecomposition`.
 
         Returns
         -------
-        Self and modifies the following field:
+        Returns self and updates the following fields:
 
-            - :attr:`eigendecomposition` - %(eigen.summary)s
+        - :attr:`eigendecomposition` - %(eigen.summary)s
         """
-        self.compute_eigendecomposition(k=k, only_evals=False, **kwargs)
-        return self
+        return self.compute_eigendecomposition(k=k, only_evals=False, **kwargs)
 
     @d.dedent
     def predict(
         self,
         use: Optional[Union[int, Sequence[int]]] = None,
         percentile: Optional[int] = 98,
-        method: Literal["leiden", "means"] = "leiden",
+        method: Literal["leiden", "kmeans"] = "leiden",
         cluster_key: Optional[str] = None,
         n_clusters_kmeans: Optional[int] = None,
         n_neighbors: int = 20,
         resolution: float = 0.1,
         n_matches_min: int = 0,
         n_neighbors_filtering: int = 15,
         basis: Optional[str] = None,
         n_comps: int = 5,
         scale: Optional[bool] = None,
-    ) -> None:
-        """
-        Find approximate recurrent classes of the Markov chain.
+    ) -> "CFLARE":
+        """Find approximate recurrent classes of the Markov chain.
 
-        Filter to obtain recurrent states in left eigenvectors.
-        Cluster to obtain approximate recurrent classes in right eigenvectors.
+        Filter to obtain recurrent states from left eigenvectors.
+        Cluster to obtain approximate recurrent classes from right eigenvectors.
 
         Parameters
         ----------
         use
             Which or how many first eigenvectors to use as features for filtering and clustering.
-            If `None`, use the *eigengap* statistic.
+            If :obj:`None`, use the *eigengap* statistic.
         percentile
             Threshold used for filtering out cells which are most likely transient states. Cells which are in the
             lower ``percentile`` percent of each eigenvector will be removed from the data matrix.
         method
             Method to be used for clustering. Valid option are:
 
-                - `'kmeans'` - :class:`sklearn.cluster.KMeans`.
-                - `'leiden'` - :func:`scanpy.tl.leiden`.
+            - ``'kmeans'`` - :class:`~sklearn.cluster.KMeans`.
+            - ``'leiden'`` - :func:`~scanpy.tl.leiden`.
         cluster_key
-            Key in :attr:`anndata.AnnData.obs` in order to associate names and colors with :attr:`terminal_states`.
+            Key in :attr:`~anndata.AnnData.obs` in order to associate names and colors with :attr:`terminal_states`.
         n_clusters_kmeans
-            If `None`, this is set to ``use + 1``.
+            Number of clusters when ``method = 'kmeans'``. If :obj:`None`, this is set to ``use + 1``.
         n_neighbors
-            Number of neighbors in a KNN graph. This is the :math:`K` parameter for that,
+            Number of neighbors in a kNN graph. This is the :math:`K` parameter for that,
             the number of neighbors for each cell. Only used when ``method = 'leiden'``.
         resolution
-            Resolution parameter for :func:`scanpy.tl.leiden`. Should be chosen relatively small.
+            Resolution parameter for :func:`~scanpy.tl.leiden`. Should be chosen relatively small.
         n_matches_min
             Filters out cells which don't have at least ``n_matches_min`` neighbors from the same category.
             This filters out some cells which are transient but have been misassigned.
         n_neighbors_filtering
             Parameter for filtering cells. Cells are filtered out if they don't have at least ``n_matches_min``
-            neighbors among their ``n_neighbors_filtering`` nearest cells.
+            neighbors among the ``n_neighbors_filtering`` nearest cells.
         basis
-            Key from :attr:`anndata.AnnData.obsm` as additional features for clustering.
+            Key from :attr:`~anndata.AnnData.obsm` as additional features for clustering.
             If `None`, use only the right eigenvectors.
         n_comps
-            Number of embedding components to be use when ``basis != None``.
+            Number of embedding components to be used when ``basis != None``.
         scale
-            Scale the values to z-scores. If `None`, scale the values if ``basis != None``.
+            Scale the values to z-scores. If :obj:`None`, scale the values if ``basis != None``.
 
         Returns
         -------
-        Nothing, just updates the following fields:
+        Returns self and just updates the following fields:
 
-            - :attr:`terminal_states` - %(tse_term_states.summary)s
-            - :attr:`terminal_states_probabilities` - %(tse_term_states_probs.summary)s
+        - :attr:`terminal_states` - %(tse_term_states.summary)s
+        - :attr:`terminal_states_probabilities` - %(tse_term_states_probs.summary)s
         """
 
-        def convert_use(
-            use: Optional[Union[int, Sequence[int], np.ndarray]]
-        ) -> List[int]:
+        def convert_use(use: Optional[Union[int, Sequence[int], np.ndarray]]) -> List[int]:
             if method not in ["kmeans", "leiden"]:
-                raise ValueError(
-                    f"Invalid method `{method!r}`. Valid options are `leiden` or `kmeans`."
-                )
+                raise ValueError(f"Invalid method `{method!r}`. Valid options are `leiden` or `kmeans`.")
 
             if use is None:
                 use = eig["eigengap"] + 1  # add one b/c indexing starts at 0
             if isinstance(use, int):
                 use = list(range(use))
             elif not isinstance(use, (np.ndarray, Sequence)):
-                raise TypeError(
-                    f"Expected `use` to be `int` or a `Sequence`, found `{type(use).__name__}`."
-                )
+                raise TypeError(f"Expected `use` to be `int` or a `Sequence`, found `{type(use).__name__}`.")
             use = list(use)
 
             if not use:
                 raise ValueError("No eigenvectors have been selected.")
 
             muse, mevecs = max(use), max(eig["V_l"].shape[1], eig["V_r"].shape[1])
             if muse >= mevecs:
@@ -149,17 +144,15 @@
                     f"Use `.compute_eigendecomposition(k={muse})` to recompute the eigendecomposition."
                 )
 
             return use
 
         eig = self.eigendecomposition
         if eig is None:
-            raise RuntimeError(
-                "Compute eigendecomposition first as `.compute_eigendecomposition()`."
-            )
+            raise RuntimeError("Compute eigendecomposition first as `.compute_eigendecomposition()`.")
         use = convert_use(use)
 
         start = logg.info("Computing terminal states")
         # we check for complex values only in the left, that's okay because the complex pattern
         # will be identical for left and right
         V_l, V_r = eig["V_l"][:, use], eig["V_r"].real[:, use]
         V_l = _complex_warning(V_l, use, use_imag=False)
@@ -171,25 +164,23 @@
         else:
             X = V_r
 
         # filter out cells which are in the lowest q percentile in abs value in each eigenvector
         if percentile is not None:
             logg.debug("Filtering out cells according to percentile")
             if not (0 <= percentile <= 100):
-                raise ValueError(
-                    f"Expected `percentile` to be in interval `[0, 100]`, found `{percentile}`."
-                )
+                raise ValueError(f"Expected `percentile` to be in interval `[0, 100]`, found `{percentile}`.")
             cutoffs = np.percentile(np.abs(V_l), percentile, axis=0)
             ixs = np.any(cutoffs <= np.abs(V_l), axis=1)
             X = X[ixs, :]
 
         if scale is None:
             scale = basis is not None
         if scale:
-            X = zscore(X, axis=0)
+            X = st.zscore(X, axis=0)
 
         # cluster X
         if method == "kmeans" and n_clusters_kmeans is None:
             n_clusters_kmeans = len(use) + (percentile is None)
             if X.shape[0] < n_clusters_kmeans:
                 raise ValueError(
                     f"Filtering resulted in only {X.shape[0]} cell(s), insufficient to cluster into "
@@ -211,32 +202,30 @@
             labels = np.repeat(None, len(self))
             labels[ixs] = clusters
         else:
             labels = clusters
         labels = pd.Series(labels, index=self.adata.obs_names, dtype="category")
         labels = labels.cat.rename_categories({c: str(c) for c in labels.cat.categories})
 
-        # filtering to get rid of some of the left over transient states
+        # filtering to get rid of some of the leftover transient states
         if n_matches_min > 0:
             logg.debug(f"Filtering according to `n_matches_min={n_matches_min}`")
             distances = _get_connectivities(self.adata, mode="distances", n_neighbors=n_neighbors_filtering)
             labels = _filter_cells(distances, rc_labels=labels, n_matches_min=n_matches_min)
         # fmt: on
 
-        self.set_terminal_states(
-            labels=labels,
+        return self.set_terminal_states(
+            states=labels,
             cluster_key=cluster_key,
             probs=self._compute_term_states_probs(eig, use),
             params=self._create_params(),
             time=start,
         )
 
-    def _compute_term_states_probs(
-        self, eig: Dict[str, Any], use: List[int]
-    ) -> pd.Series:
+    def _compute_term_states_probs(self, eig: Dict[str, Any], use: List[int]) -> pd.Series:
         # get the truncated eigendecomposition
         V, evals = eig["V_l"].real[:, use], eig["D"].real[use]
 
         # shift and scale
         V_pos = np.abs(V)
         V_shifted = V_pos - np.min(V_pos, axis=0)
         V_scaled = V_shifted / np.max(V_shifted, axis=0)
@@ -252,12 +241,9 @@
         c = np.sum(V_eigs, axis=1)
         c /= np.max(c)
 
         return pd.Series(c, index=self.adata.obs_names)
 
     def _read_from_adata(self, adata: AnnData, **kwargs: Any) -> bool:
         ok = super()._read_from_adata(adata, **kwargs)
-        return (
-            ok
-            and self._read_eigendecomposition(adata, allow_missing=False)
-            and self._read_absorption_probabilities(adata)
-        )
+        ok = ok and self._read_eigendecomposition(adata, allow_missing=False)
+        return ok and self._read_fate_probabilities(adata) and self._read_absorption_times(adata)
```

### Comparing `cellrank-1.5.1/cellrank/tl/estimators/terminal_states/_gpcca.py` & `cellrank-2.0.0/src/cellrank/estimators/terminal_states/_gpcca.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,128 @@
-from typing import Any, Dict, Tuple, Union, Mapping, Optional, Sequence
-from typing_extensions import Literal
+import datetime
+import enum
+import pathlib
+import types
+from typing import Any, Dict, Literal, Mapping, Optional, Sequence, Tuple, Union
 
-from enum import auto
-from types import MappingProxyType
-from pathlib import Path
-from datetime import datetime
+import numpy as np
+import pandas as pd
+import scipy.sparse as sp
+from pandas.api.types import infer_dtype, is_categorical_dtype
+
+import matplotlib.pyplot as plt
+from matplotlib.axes import Axes
+from matplotlib.colorbar import ColorbarBase
+from matplotlib.colors import ListedColormap, Normalize
+from matplotlib.ticker import StrMethodFormatter
 
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d
-from cellrank.tl._utils import (
-    save_fig,
+from cellrank._utils._colors import _create_categorical_colors, _get_black_or_white
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._key import Key
+from cellrank._utils._lineage import Lineage
+from cellrank._utils._utils import (
     _eigengap,
     _fuzzy_to_discrete,
     _series_from_one_hot_matrix,
+    save_fig,
 )
-from cellrank.tl._colors import _get_black_or_white, _create_categorical_colors
-from cellrank.tl._lineage import Lineage
-from cellrank.tl.estimators._utils import SafeGetter
-from cellrank.tl.estimators.mixins import EigenMixin, SchurMixin, LinDriversMixin
-from cellrank.tl.kernels._base_kernel import KernelExpression
-from cellrank.tl.estimators.mixins._utils import logger, shadow, register_plotter
-from cellrank.tl.estimators.terminal_states._term_states_estimator import (
+from cellrank.estimators.mixins import EigenMixin, LinDriversMixin, SchurMixin
+from cellrank.estimators.mixins._utils import SafeGetter, StatesHolder, logger, shadow
+from cellrank.estimators.terminal_states._term_states_estimator import (
     TermStatesEstimator,
 )
+from cellrank.kernels._base_kernel import KernelExpression
 
-import numpy as np
-import pandas as pd
-from scipy.sparse import spmatrix
-from pandas.api.types import infer_dtype, is_categorical_dtype
+__all__ = ["GPCCA"]
 
-import matplotlib.pyplot as plt
-from matplotlib.axes import Axes
-from matplotlib.colors import Normalize, ListedColormap
-from matplotlib.ticker import StrMethodFormatter
-from matplotlib.colorbar import ColorbarBase
+
+class TermStatesMethod(ModeEnum):
+    EIGENGAP = enum.auto()
+    EIGENGAP_COARSE = enum.auto()
+    TOP_N = enum.auto()
+    STABILITY = enum.auto()
 
 
-class TermStatesMethod(ModeEnum):  # noqa: D101
-    EIGENGAP = auto()
-    EIGENGAP_COARSE = auto()
-    TOP_N = auto()
-    STABILITY = auto()
+class CoarseTOrder(ModeEnum):
+    STABILITY = enum.auto()  # diagonal
+    INCOMING = enum.auto()
+    OUTGOING = enum.auto()
+    STAT_DIST = enum.auto()
 
 
 @d.dedent
 class GPCCA(TermStatesEstimator, LinDriversMixin, SchurMixin, EigenMixin):
-    """
-    Generalized Perron Cluster Cluster Analysis :cite:`reuter:18` as implemented in \
-    `pyGPCCA <https://pygpcca.readthedocs.io/en/latest/>`_.
+    """Generalized Perron Cluster Cluster Analysis (GPCCA) :cite:`reuter:18,reuter:19`.
 
-    Coarse-grains a discrete Markov chain into a set of macrostates and computes coarse-grained transition probabilities
-    among the macrostates. Each macrostate corresponds to an area of the state space, i.e. to a subset of cells. The
-    assignment is soft, i.e. each cell is assigned to every macrostate with a certain weight, where weights sum to
-    one per cell. Macrostates are computed by maximizing the 'crispness' which can be thought of as a measure for
-    minimal overlap between macrostates in a certain inner-product sense. Once the macrostates have been computed,
-    we project the large transition matrix onto a coarse-grained transition matrix among the macrostates via
-    a Galerkin projection. This projection is based on invariant subspaces of the original transition matrix which
-    are obtained using the real Schur decomposition :cite:`reuter:18`.
+    .. seealso::
+        - See :doc:`../../../notebooks/tutorials/estimators/600_initial_terminal` on how to compute the
+          :attr:`initial <initial_states>` and :attr:`terminal <terminal_states>` states.
+        - See :doc:`../../../notebooks/tutorials/estimators/700_fate_probabilities` on how to compute the
+          :attr:`fate_probabilities` and :attr:`lineage_drivers`.
+
+    This is our main and recommended estimator implemented in `pyGPCCA <https://pygpcca.readthedocs.io/en/latest/>`_ .
+    Use it to compute macrostates, automatically and semi-automatically classify these as initial, intermediate and
+    terminal states, compute fate probabilities towards macrostates, uncover driver genes, and much more. To compute and
+    classify macrostates, we run the GPCCA algorithm under the hood, which returns a soft assignment of cells
+    to macrostates, as well as a coarse-grained transition matrix among the set of macrostates
+    :cite:`reuter:18,reuter:19`. This estimator allows you to inject prior knowledge where available
+    to guide the identification of initial, intermediate and terminal states.
 
     Parameters
     ----------
     %(base_estimator.parameters)s
     """
 
     def __init__(
         self,
-        obj: Union[AnnData, np.ndarray, spmatrix, KernelExpression],
-        obsp_key: Optional[str] = None,
+        object: Union[str, bool, np.ndarray, sp.spmatrix, AnnData, KernelExpression],
         **kwargs: Any,
     ):
-        super().__init__(obj=obj, obsp_key=obsp_key, **kwargs)
-
+        super().__init__(object=object, **kwargs)
+        self._macrostates = StatesHolder()
         self._coarse_init_dist: Optional[pd.Series] = None
         self._coarse_stat_dist: Optional[pd.Series] = None
         self._coarse_tmat: Optional[pd.DataFrame] = None
 
-        self._macrostates: Optional[pd.Series] = None
-        self._macrostates_memberships: Optional[Lineage] = None
-        self._macrostates_colors: Optional[np.ndarray] = None
-
-        self._term_states_memberships: Optional[Lineage] = None
-
     @property
     @d.get_summary(base="gpcca_macro")
     def macrostates(self) -> Optional[pd.Series]:
         """Macrostates of the transition matrix."""
-        return self._macrostates
+        return self._macrostates.assignment
 
     @property
     @d.get_summary(base="gpcca_macro_memberships")
     def macrostates_memberships(self) -> Optional[Lineage]:
-        """Macrostate membership matrix.
+        """Macrostate memberships.
 
         Soft assignment of microstates (cells) to macrostates.
         """
-        return self._macrostates_memberships
+        return self._macrostates.memberships
+
+    @property
+    @d.get_summary(base="gpcca_init_states_memberships")
+    def initial_states_memberships(self) -> Optional[Lineage]:
+        """Initial states memberships.
+
+        Soft assignment of cells to initial states.
+        """
+        return self._init_states.memberships
 
     @property
     @d.get_summary(base="gpcca_term_states_memberships")
     def terminal_states_memberships(self) -> Optional[Lineage]:
-        """Terminal state membership matrix.
+        """Terminal states memberships.
 
         Soft assignment of cells to terminal states.
         """
-        return self._term_states_memberships
+        return self._term_states.memberships
 
     @property
     @d.get_summary(base="gpcca_coarse_init")
     def coarse_initial_distribution(self) -> Optional[pd.Series]:
         """Coarse-grained initial distribution."""
         return self._coarse_init_dist
 
@@ -130,50 +142,49 @@
     @d.dedent
     def compute_macrostates(
         self,
         n_states: Optional[Union[int, Sequence[int]]] = None,
         n_cells: Optional[int] = 30,
         cluster_key: Optional[str] = None,
         **kwargs: Any,
-    ) -> None:
-        """
-        Compute the macrostates.
+    ) -> "GPCCA":
+        """Compute the macrostates.
 
         Parameters
         ----------
         n_states
-            Number of macrostates. If a :class:`typing.Sequence`, use the *minChi* criterion :cite:`reuter:18`.
-            If `None`, use the *eigengap* heuristic.
+            Number of macrostates to compute. If a :class:`~typing.Sequence`, use the *minChi*
+            criterion :cite:`reuter:18`. If :obj:`None`, use the `eigengap <https://en.wikipedia.org/wiki/Eigengap>`__
+            heuristic.
         %(n_cells)s
         cluster_key
             If a key to cluster labels is given, names and colors of the states will be associated with the clusters.
         kwargs
             Keyword arguments for :meth:`compute_schur`.
 
         Returns
         -------
-        Nothing, just updates the following fields:
+        Returns self and updates the following fields:
 
-            - :attr:`macrostates` - %(gpcca_macro.summary)s
-            - :attr:`macrostates_memberships` - %(gpcca_macro_memberships.summary)s
-            - :attr:`coarse_T` - %(gpcca_coarse_tmat.summary)s
-            - :attr:`coarse_initial_distribution` - %(gpcca_coarse_init.summary)s
-            - :attr:`coarse_stationary_distribution` - %(gpcca_coarse_stat.summary)s
-            - :attr:`schur_vectors` - %(schur_vectors.summary)s
-            - :attr:`schur_matrix` - %(schur_matrix.summary)s
-            - :attr:`eigendecomposition` - %(eigen.summary)s
+        - :attr:`macrostates` - %(gpcca_macro.summary)s
+        - :attr:`macrostates_memberships` - %(gpcca_macro_memberships.summary)s
+        - :attr:`coarse_T` - %(gpcca_coarse_tmat.summary)s
+        - :attr:`coarse_initial_distribution` - %(gpcca_coarse_init.summary)s
+        - :attr:`coarse_stationary_distribution` - %(gpcca_coarse_stat.summary)s
+        - :attr:`schur_vectors` - %(schur_vectors.summary)s
+        - :attr:`schur_matrix` - %(schur_matrix.summary)s
+        - :attr:`eigendecomposition` - %(eigen.summary)s
         """
-
         n_states = self._n_states(n_states)
         if n_states == 1:
             self._compute_one_macrostate(
                 n_cells=n_cells,
                 cluster_key=cluster_key,
             )
-            return
+            return self
 
         if self._gpcca is None or kwargs:
             self.compute_schur(n_states, **kwargs)
         n_states = self._validate_n_states(n_states)
 
         if self._gpcca._p_X.shape[1] < n_states:
             # precomputed X
@@ -200,205 +211,330 @@
         self._set_macrostates(
             memberships=self._gpcca.memberships,
             n_cells=n_cells,
             cluster_key=cluster_key,
             params=self._create_params(),
             time=start,
         )
+        return self
+
+    def predict(self, *args: Any, **kwargs: Any) -> "GPCCA":
+        """Alias for :meth:`predict_terminal_states`.
+
+        Parameters
+        ----------
+        args
+            Positional arguments.
+        kwargs
+            Keyword arguments.
+
+        Returns
+        -------
+        Same as :meth:`predict_terminal_states`.
+        """
+        return self.predict_terminal_states(*args, **kwargs)
 
     @d.dedent
-    def predict(
+    def predict_terminal_states(
         self,
-        method: Literal[
-            "stability", "top_n", "eigengap", "eigengap_coarse"
-        ] = TermStatesMethod.STABILITY,
+        method: Literal["stability", "top_n", "eigengap", "eigengap_coarse"] = TermStatesMethod.STABILITY,
         n_cells: int = 30,
         alpha: Optional[float] = 1,
         stability_threshold: float = 0.96,
         n_states: Optional[int] = None,
-    ) -> None:
-        """
-        Automatically select terminal states from macrostates.
+        allow_overlap: bool = False,
+    ) -> "GPCCA":
+        """Automatically select terminal states from macrostates.
 
         Parameters
         ----------
         method
             How to select the terminal states. Valid option are:
 
-                - `'eigengap'` - select the number of states based on the *eigengap* of :attr:`transition_matrix`.
-                - `'eigengap_coarse'` - select the number of states based on the *eigengap* of the diagonal
-                  of :attr:`coarse_T`.
-                - `'top_n'` - select top ``n_states`` based on the probability of the diagonal of :attr:`coarse_T`.
-                - `'stability'` - select states which have a stability >= ``stability_threshold``.
-                  The stability is given by the diagonal elements of :attr:`coarse_T`.
+            - ``'eigengap'`` - select the number of states based on the
+              `eigengap <https://en.wikipedia.org/wiki/Eigengap>`__ of :attr:`transition_matrix`.
+            - ``'eigengap_coarse'`` - select the number of states based on the *eigengap* of the diagonal
+              of :attr:`coarse_T`.
+            - ``'top_n'`` - select top ``n_states`` based on the probability of the diagonal of :attr:`coarse_T`.
+            - ``'stability'`` - select states which have a stability >= ``stability_threshold``.
+              The stability is given by the diagonal elements of :attr:`coarse_T`.
         %(n_cells)s
         alpha
             Weight given to the deviation of an eigenvalue from one.
             Only used when ``method = 'eigengap'`` or ``method = 'eigengap_coarse'``.
         stability_threshold
             Threshold used when ``method = 'stability'``.
         n_states
             Number of states used when ``method = 'top_n'``.
+        %(allow_overlap)s
 
         Returns
         -------
-        Nothing, just updates the following fields:
+        Returns self and updates the following fields:
 
-            - :attr:`terminal_states` - %(tse_term_states.summary)s
-            - :attr:`terminal_states_memberships` - %(gpcca_term_states_memberships.summary)s
-            - :attr:`terminal_states_probabilities` - %(tse_term_states_probs.summary)s
+        - :attr:`terminal_states` - %(tse_term_states.summary)s
+        - :attr:`terminal_states_probabilities` - %(tse_term_states_probs.summary)s
+        - :attr:`terminal_states_memberships` - %(gpcca_term_states_memberships.summary)s
         """
         if self.macrostates is None:
             raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
 
-        # fmt: off
-        if len(self._macrostates.cat.categories) == 1:
-            logg.warning("Found only one macrostate. Making it the single terminal state")
-            self.set_terminal_states_from_macrostates(None, n_cells=n_cells, params=self._create_params())
-            return
+        if len(self.macrostates.cat.categories) == 1:
+            logg.warning("Found only one macrostate, making it the singular terminal state")
+            return self.set_terminal_states(
+                states=None,
+                n_cells=n_cells,
+                allow_overlap=allow_overlap,
+                params=self._create_params(),
+            )
 
         method = TermStatesMethod(method)
         eig = self.eigendecomposition
         coarse_T = self.coarse_T
 
+        # fmt: off
         if method == TermStatesMethod.EIGENGAP:
             if eig is None:
                 raise RuntimeError("Compute eigendecomposition first as `.compute_eigendecomposition()`.")
             n_states = _eigengap(eig["D"], alpha=alpha) + 1
         elif method == TermStatesMethod.EIGENGAP_COARSE:
             if coarse_T is None:
                 raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
             n_states = _eigengap(np.sort(np.diag(coarse_T)[::-1]), alpha=alpha)
         elif method == TermStatesMethod.TOP_N:
             if n_states is None:
                 raise ValueError("Expected `n_states != None` for `method='top_n'`.")
-            elif n_states <= 0:
+            if n_states <= 0:
                 raise ValueError(f"Expected `n_states` to be positive, found `{n_states}`.")
         elif method == TermStatesMethod.STABILITY:
             if stability_threshold is None:
                 raise ValueError("Expected `stability_threshold != None` for `method='stability'`.")
             stability = pd.Series(np.diag(coarse_T), index=coarse_T.columns)
             names = stability[stability.values >= stability_threshold].index
-            self.set_terminal_states_from_macrostates(names, n_cells=n_cells, params=self._create_params())
-            return
+            return self.set_terminal_states(
+                names,
+                n_cells=n_cells,
+                allow_overlap=allow_overlap,
+                params=self._create_params()
+            )
         else:
             raise NotImplementedError(f"Method `{method}` is not yet implemented.")
         # fmt: on
 
         names = coarse_T.columns[np.argsort(np.diag(coarse_T))][-n_states:]
-        self.set_terminal_states_from_macrostates(
-            names, n_cells=n_cells, params=self._create_params()
+        return self.set_terminal_states(
+            names,
+            n_cells=n_cells,
+            allow_overlap=allow_overlap,
+            params=self._create_params(),
         )
 
-        return
+    @d.dedent
+    def predict_initial_states(self, n_states: int = 1, n_cells: int = 30, allow_overlap: bool = False) -> "GPCCA":
+        """Compute initial states from macrostates using :attr:`coarse_stationary_distribution`.
+
+        Parameters
+        ----------
+        n_states
+            Number of initial states.
+        %(n_cells)s
+        %(allow_overlap)s
+
+        Returns
+        -------
+        Returns self and updates the following fields:
+
+        - :attr:`initial_states` - %(tse_init_states.summary)s
+        - :attr:`initial_states_probabilities` - %(tse_init_states_probs.summary)s
+        - :attr:`initial_states_memberships` - %(gpcca_init_states_memberships.summary)s
+        """
+        if n_states <= 0:
+            raise ValueError(f"Expected `n_states` to be positive, found `{n_states}`.")
+        if n_cells <= 0:
+            raise ValueError(f"Expected `n_cells` to be positive, found `{n_cells}`.")
+
+        probs = self.macrostates_memberships
+        if probs is None:
+            raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
+        if n_states > probs.shape[1]:
+            raise ValueError(
+                f"Requested `{n_states}` initial states, but only `{probs.shape[1]}` macrostates have been computed."
+            )
+
+        if probs.shape[1] == 1:
+            return self.set_initial_states(states=None, n_cells=n_cells, allow_overlap=allow_overlap)
+
+        stat_dist = self.coarse_stationary_distribution
+        if stat_dist is None:
+            raise RuntimeError("No coarse-grained stationary distribution found.")
+
+        states = list(stat_dist[np.argsort(stat_dist)][:n_states].index)
+        return self.set_initial_states(states, n_cells=n_cells, allow_overlap=allow_overlap)
 
     @d.dedent
-    def set_terminal_states_from_macrostates(
+    def set_terminal_states(
         self,
-        names: Optional[Union[str, Sequence[str], Mapping[str, str]]] = None,
+        states: Optional[Union[str, Sequence[str], Dict[str, Sequence[str]], pd.Series]] = None,
         n_cells: int = 30,
+        allow_overlap: bool = False,
+        cluster_key: Optional[str] = None,
         **kwargs: Any,
-    ) -> None:
-        """
-        Manually select terminal states from macrostates.
+    ) -> "GPCCA":
+        """Set the :attr:`terminal_states`.
 
         Parameters
         ----------
-        names
-            Names of the macrostates to be marked as terminal. Multiple states can be combined using `','`,
-            such as ``["Alpha, Beta", "Epsilon"]``.  If a :class:`dict`, keys correspond to the names
-            of the macrostates and the values to the new names.  If `None`, select all macrostates.
+        states
+            Which states to select. Valid options are:
+
+            - :class:`str`, :class:`~typing.Sequence` - subset of :attr:`macrostates`. Multiple states can be
+              combined using ``','``, such as ``['Alpha, Beta', 'Epsilon']``.
+            - :class:`dict` - keys correspond to terminal states and values to cell IDs in
+              :attr:`~anndata.AnnData.obs_names`.
+            - :class:`~pandas.Series` - categorical series where each category corresponds to a macrostate.
+              `NaN` values mark cells that should not be marked as :attr:`terminal_states`.
+            - :obj:`None` - select all :attr:`macrostates`.
         %(n_cells)s
+        %(allow_overlap)s
+        cluster_key
+            Key in :attr:`~anndata.AnnData.obs` to associate names and colors with :attr:`terminal_states`.
+            Each state will be given the name and color corresponding to the cluster it mostly overlaps with.
+            Only used when ``states`` is a :class:`dict` or :class:`~pandas.Series`.
+        kwargs
+            Additional keyword arguments.
 
         Returns
         -------
-        Nothing, just updates the following fields:
+        Returns self and updates the following fields:
 
-            - :attr:`terminal_states` - %(tse_term_states.summary)s
-            - :attr:`terminal_states_probabilities` - %(tse_term_states_probs.summary)s
-            - :attr:`terminal_states_probabilities_memberships` - %(gpcca_term_states_memberships.summary)s
+        - :attr:`terminal_states` - %(tse_term_states.summary)s
+        - :attr:`terminal_states_probabilities` - %(tse_term_states_probs.summary)s
+        - :attr:`terminal_states_memberships` - %(gpcca_term_states_memberships.summary)s
         """
+        if isinstance(states, (dict, pd.Series)):
+            return super().set_terminal_states(states, cluster_key=cluster_key, allow_overlap=allow_overlap, **kwargs)
+
         if n_cells <= 0:
             raise ValueError(f"Expected `n_cells` to be positive, found `{n_cells}`.")
 
         memberships = self.macrostates_memberships
         if memberships is None:
             raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
 
-        rename = True
-        if names is None:
-            names = memberships.names
-            rename = False
-        if isinstance(names, str):
-            names = [names]
-            rename = False
-        if not isinstance(names, dict):
-            names = {n: n for n in names}
-            rename = False
-        if not len(names):
+        if states is None:
+            states = memberships.names
+        elif isinstance(states, str):
+            states = [states]
+        if not len(states):  # unset the states
             raise ValueError("No macrostates have been selected.")
 
-        # we do this also here because if `rename_terminal_states` fails
-        # invalid states would've been written to this object and nothing to adata
-        names = {str(k): str(v) for k, v in names.items()}
-        names_after_renaming = {names.get(n, n) for n in memberships.names}
-        if len(names_after_renaming) != memberships.shape[1]:
-            raise ValueError(
-                f"After renaming, terminal state names will no longer be unique: `{names_after_renaming}`."
-            )
-
-        # this also checks that the names are correct before renaming
         is_singleton = memberships.shape[1] == 1
-        memberships = memberships[list(names.keys())].copy()
+        memberships = memberships[list(states)].copy()
 
         states = self._create_states(memberships, n_cells=n_cells, check_row_sums=False)
         if is_singleton:
-            colors = self._macrostates_colors.copy()
+            colors = self._macrostates.colors.copy()
             probs = memberships.X.squeeze() / memberships.X.max()
         else:
             colors = memberships[list(states.cat.categories)].colors
-            probs = (memberships.X / memberships.X.max(0)).max(1)
+            probs = (memberships.X / memberships.X.max(axis=0)).max(axis=1)
         probs = pd.Series(probs, index=self.adata.obs_names)
 
-        self._write_terminal_states(
-            states, colors, probs, memberships, params=kwargs.pop("params", {})
+        self._write_states(
+            "terminal",
+            states=states,
+            colors=colors,
+            probs=probs,
+            memberships=memberships,
+            params=kwargs.pop("params", {}),
+            allow_overlap=allow_overlap,
+            **kwargs,
         )
-        if rename:
-            # TODO(michalk8): in a future PR, remove this behavior in Lineage
-            # access lineage renames join states, e.g. 'Alpha, Beta' becomes 'Alpha or Beta' + whitespace stripping
-            self.rename_terminal_states(
-                dict(zip(self.terminal_states.cat.categories, names.values()))
-            )
+        return self
 
     @d.dedent
-    def rename_terminal_states(self, new_names: Mapping[str, str]) -> None:
-        """
-        %(tse_rename_term_states.full_desc)s
+    def set_initial_states(
+        self,
+        states: Optional[Union[str, Sequence[str], Dict[str, Sequence[str]], pd.Series]] = None,
+        n_cells: int = 30,
+        allow_overlap: bool = False,
+        cluster_key: Optional[str] = None,
+        **kwargs: Any,
+    ) -> "GPCCA":
+        """Set the :attr:`initial_states`.
 
         Parameters
         ----------
-        %(tse_rename_term_states.parameters)s
+        states
+            Which states to select. Valid options are:
+
+            - :class:`str`, :class:`~typing.Sequence` - subset of :attr:`macrostates`. Multiple states can be
+              combined using ``','``, such as ``['Alpha, Beta', 'Epsilon']``.
+            - :class:`dict` - keys correspond to initial states and values to cell IDs in
+              :attr:`~anndata.AnnData.obs_names`.
+            - :class:`~pandas.Series` - categorical series where each category corresponds to a macrostate.
+              `NaN` values mark cells that should not be marked as :attr:`initial_states`.
+            - :obj:`None` - select all :attr:`macrostates`.
+        %(n_cells)s
+        %(allow_overlap)s
+        cluster_key
+            Key in :attr:`~anndata.AnnData.obs` to associate names and colors with :attr:`initial_states`.
+            Each state will be given the name and color corresponding to the cluster it mostly overlaps with.
+            Only used when ``states`` is a :class:`dict` or :class:`~pandas.Series`.
+        kwargs
+            Additional keyword arguments.
 
         Returns
         -------
-        %(tse_rename_term_states.returns)s
-            - :attr:`terminal_states_memberships` - %(gpcca_term_states_memberships.summary)s
-        """  # noqa: D400
-        term_states_memberships = self.terminal_states_memberships
-        super().rename_terminal_states(new_names)
+        Returns self and updates the following fields:
 
-        # fmt: off
-        new_names = {str(k): str(v) for k, v in new_names.items()}
-        term_states_memberships.names = [new_names.get(n, n) for n in term_states_memberships.names]
-        self._set("_term_states_memberships", value=term_states_memberships, shadow_only=True)
-        # fmt: on
+        - :attr:`initial_states` - %(tse_init_states.summary)s
+        - :attr:`initial_states_probabilities` - %(tse_init_states_probs.summary)s
+        - :attr:`initial_states_memberships` - %(gpcca_init_states_memberships.summary)s
+        """
+        if isinstance(states, (pd.Series, dict)):
+            return super().set_initial_states(states, cluster_key=cluster_key, allow_overlap=allow_overlap, **kwargs)
+
+        if n_cells <= 0:
+            raise ValueError(f"Expected `n_cells` to be positive, found `{n_cells}`.")
 
-        with self._shadow:
-            key = Key.obsm.memberships(Key.obs.macrostates(self.backward))
-            self._set(obj=self.adata.obsm, key=key, value=term_states_memberships)
+        memberships = self.macrostates_memberships
+        if memberships is None:
+            raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
+
+        if states is None:
+            states = memberships.names
+        elif isinstance(states, str):
+            states = [states]
+        if not len(states):  # unset the states
+            raise ValueError("No macrostates have been selected.")
+
+        is_singleton = memberships.shape[1] == 1
+        memberships = memberships[list(states)].copy()
+
+        states = self._create_states(memberships, n_cells=n_cells, check_row_sums=False)
+        if is_singleton:
+            colors = self._macrostates.colors.copy()
+            probs = memberships.X.squeeze() / memberships.X.max()
+        else:
+            colors = memberships[list(states.cat.categories)].colors
+            probs = (memberships.X / memberships.X.max(axis=0)).max(axis=1)
+        probs = pd.Series(probs, index=self.adata.obs_names)
+
+        self._write_states(
+            "initial",
+            states=states,
+            colors=colors,
+            probs=probs,
+            memberships=memberships,
+            params=kwargs.pop("params", {}),
+            allow_overlap=allow_overlap,
+            **kwargs,
+        )
+        return self
 
     @d.dedent
     def fit(
         self,
         n_states: Optional[Union[int, Sequence[int]]] = None,
         n_cells: Optional[int] = 30,
         cluster_key: Optional[str] = None,
@@ -414,70 +550,117 @@
         Returns
         -------
         %(gpcca_compute_macro.returns)s
         """
         if n_states is None:
             self.compute_eigendecomposition()
             n_states = self.eigendecomposition["eigengap"] + 1
-        if isinstance(n_states, int) and n_states == 1:
+        elif isinstance(n_states, int) and n_states == 1:
             self.compute_eigendecomposition()
 
-        self.compute_macrostates(n_states=n_states, cluster_key=cluster_key, **kwargs)
-
-        return self
+        n = n_states if isinstance(n_states, int) else max(n_states)
+        # call explicitly since `compute_macrostates` doesn't handle the case
+        # when `minChi` is used for `n_states` and `self._gpcca` is uninitialized
+        _ = self.compute_schur(n, **kwargs)
+        return self.compute_macrostates(n_states=n_states, cluster_key=cluster_key, n_cells=n_cells)
 
     @d.dedent
+    @inject_docs(o=CoarseTOrder)
     def plot_coarse_T(
         self,
         show_stationary_dist: bool = True,
         show_initial_dist: bool = False,
+        order: Optional[Literal["stability", "incoming", "outgoing", "stat_dist"]] = "stability",
         cmap: Union[str, ListedColormap] = "viridis",
         xtick_rotation: float = 45,
         annotate: bool = True,
         show_cbar: bool = True,
         title: Optional[str] = None,
         figsize: Tuple[float, float] = (8, 8),
         dpi: int = 80,
-        save: Optional[Union[Path, str]] = None,
-        text_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        save: Optional[Union[str, pathlib.Path]] = None,
+        text_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         **kwargs: Any,
     ) -> None:
-        """
-        Plot the coarse-grained transition matrix between macrostates.
+        """Plot the coarse-grained transition matrix.
 
         Parameters
         ----------
         show_stationary_dist
-            Whether to show :attr:`coarse_stationary_distribution`, if present.
+            Whether to show the :attr:`coarse_stationary_distribution`, if present.
         show_initial_dist
-            Whether to show :attr:`coarse_initial_distribution`.
+            Whether to show the :attr:`coarse_initial_distribution`.
+        order
+            How to order the coarse-grained transition matrix. Valid options are:
+
+            - ``{o.STABILITY!r}`` - order by the values on the diagonal.
+            - ``{o.INCOMING!r}`` - order by the incoming mass, excluding the diagonal.
+            - ``{o.OUTGOING!r}`` - order by the outgoing mass, excluding the diagonal.
+            - ``{o.STAT_DIST!r}`` - order by coarse stationary distribution. If not present, use ``{o.STABILITY!r}``.
         cmap
             Colormap to use.
         xtick_rotation
             Rotation of ticks on the x-axis.
         annotate
             Whether to display the text on each cell.
         show_cbar
-            Whether to show colorbar.
+            Whether to show the colorbar.
         title
             Title of the figure.
         %(plotting)s
         text_kwargs
-            Keyword arguments for :func:`matplotlib.pyplot.text`.
+            Keyword arguments for :meth:`~matplotlib.axes.Axes.text`.
         kwargs
-            Keyword arguments for :func:`matplotlib.pyplot.imshow`.
+            Keyword arguments for :meth:`~matplotlib.axes.Axes.imshow`.
 
         Returns
         -------
         %(just_plots)s
         """
 
-        def stylize_dist(
-            ax: Axes, data: np.ndarray, xticks_labels: Sequence[str] = ()
-        ) -> None:
+        def order_matrix(
+            order: Optional[CoarseTOrder],
+        ) -> Tuple[pd.DataFrame, Optional[pd.Series], Optional[pd.Series]]:
+            coarse_T = self.coarse_T
+            init_d = self.coarse_initial_distribution
+            stat_d = self.coarse_stationary_distribution
+
+            if order is None:
+                return coarse_T, init_d, stat_d
+
+            order = CoarseTOrder(order)
+            if order == CoarseTOrder.STAT_DIST and stat_d is None:
+                order = CoarseTOrder.STABILITY
+                logg.warning(
+                    f"Unable to order by `{CoarseTOrder.STAT_DIST}`, no coarse stationary distribution. "
+                    f"Using `order={order}`"
+                )
+
+            if order == CoarseTOrder.INCOMING:
+                values = (coarse_T.sum(0) - np.diag(coarse_T)).argsort(kind="stable")
+                names = values.index[values]
+            elif order == CoarseTOrder.OUTGOING:
+                values = (coarse_T.sum(1) - np.diag(coarse_T)).argsort(kind="stable")
+                names = values.index[values]
+            elif order == CoarseTOrder.STABILITY:
+                names = coarse_T.index[np.argsort(np.diag(coarse_T), kind="stable")]
+            elif order == CoarseTOrder.STAT_DIST:
+                names = stat_d.index[stat_d.argsort(kind="stable")]
+            else:
+                raise NotImplementedError(f"Order `{order}` is not yet implemented.")
+
+            coarse_T = coarse_T.loc[names][names]
+            if init_d is not None:
+                init_d = init_d[names]
+            if stat_d is not None:
+                stat_d = stat_d[names]
+
+            return coarse_T, init_d, stat_d
+
+        def stylize_dist(ax: Axes, data: np.ndarray, xticks_labels: Sequence[str] = ()) -> None:
             _ = ax.imshow(data, aspect="auto", cmap=cmap, norm=norm)
             for spine in ax.spines.values():
                 spine.set_visible(False)
 
             if xticks_labels is not None:
                 ax.set_xticks(np.arange(data.shape[1]))
                 ax.set_xticklabels(xticks_labels)
@@ -485,17 +668,15 @@
                     ax.get_xticklabels(),
                     rotation=xtick_rotation,
                     ha="right",
                     rotation_mode="anchor",
                 )
             else:
                 ax.set_xticks([])
-                ax.tick_params(
-                    which="both", top=False, right=False, bottom=False, left=False
-                )
+                ax.tick_params(which="both", top=False, right=False, bottom=False, left=False)
 
             ax.set_yticks([])
 
         def annotate_heatmap(im, valfmt: str = "{x:.2f}") -> None:
             # modified from matplotlib's site
 
             data = im.get_array()
@@ -511,15 +692,15 @@
             texts = []
             for i in range(data.shape[0]):
                 for j in range(data.shape[1]):
                     kw.update(color=_get_black_or_white(im.norm(data[i, j]), cmap))
                     text = im.axes.text(j, i, valfmt(data[i, j], None), **kw)
                     texts.append(text)
 
-        def annotate_dist_ax(ax, data: np.ndarray, valfmt: str = "{x:.2f}"):
+        def annotate_dist_ax(ax: Axes, data: np.ndarray, valfmt: str = "{x:.2f}") -> None:
             if ax is None:
                 return
 
             if isinstance(valfmt, str):
                 valfmt = StrMethodFormatter(valfmt)
 
             kw = {"ha": "center", "va": "center"}
@@ -530,23 +711,20 @@
                 ax.text(
                     i,
                     0,
                     valfmt(val, None),
                     **kw,
                 )
 
-        coarse_T = self.coarse_T
-        coarse_init_d = self.coarse_initial_distribution
-        coarse_stat_d = self.coarse_stationary_distribution
-
-        if coarse_T is None:
+        if self.coarse_T is None:
             raise RuntimeError(
                 "Compute coarse-grained transition matrix first as `.compute_macrostates()` with `n_states > 1`."
             )
 
+        coarse_T, coarse_init_d, coarse_stat_d = order_matrix(order)
         if show_stationary_dist and coarse_stat_d is None:
             logg.warning("Coarse stationary distribution is `None`, ignoring")
             show_stationary_dist = False
         if show_initial_dist and coarse_init_d is None:
             logg.warning("Coarse initial distribution is `None`, ignoring")
             show_initial_dist = False
 
@@ -572,15 +750,15 @@
         if isinstance(cmap, str):
             cmap = plt.get_cmap(cmap)
 
         ax = fig.add_subplot(gs[0, 0])
         cax = fig.add_subplot(gs[:1, -1]) if show_cbar else None
         init_ax, stat_ax = None, None
 
-        labels = list(self.coarse_T.columns)
+        labels = list(coarse_T.columns)
 
         tmp = coarse_T
         if show_initial_dist:
             tmp = np.c_[tmp, coarse_stat_d]
         if show_initial_dist:
             tmp = np.c_[tmp, coarse_init_d]
 
@@ -595,17 +773,15 @@
                 xticks_labels=labels if not show_initial_dist else None,
             )
             stat_ax.yaxis.set_label_position("right")
             stat_ax.set_ylabel("stationary dist", rotation=0, ha="left", va="center")
 
         if show_initial_dist:
             init_ax = fig.add_subplot(gs[show_stationary_dist + show_initial_dist, 0])
-            stylize_dist(
-                init_ax, np.array(coarse_init_d).reshape(1, -1), xticks_labels=labels
-            )
+            stylize_dist(init_ax, np.array(coarse_init_d).reshape(1, -1), xticks_labels=labels)
 
             init_ax.yaxis.set_label_position("right")
             init_ax.set_ylabel("initial dist", rotation=0, ha="left", va="center")
 
         im = ax.imshow(coarse_T, aspect="auto", cmap=cmap, norm=norm, **kwargs)
         ax.set_title("coarse-grained transition matrix" if title is None else title)
 
@@ -662,67 +838,63 @@
         key: str,
         width: float = 0.8,
         title: Optional[str] = None,
         labelrot: float = 45,
         legend_loc: Optional[str] = "upper right out",
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[int] = None,
-        save: Optional[Union[str, Path]] = None,
+        save: Optional[Union[str, pathlib.Path]] = None,
         show: bool = True,
     ) -> Optional[Axes]:
-        """
-        Plot stacked histogram of macrostates over categorical annotations.
+        """Plot histogram of macrostates over categorical annotations.
 
         Parameters
         ----------
         %(adata)s
         key
-            Key from :attr:`anndata.AnnData.obs` containing categorical annotations.
+            Key from :attr:`~anndata.AnnData.obs` containing categorical annotations.
         width
-            Bar width in `[0, 1]`.
+            Bar width in :math:`[0, 1]`.
         title
-            Title of the figure. If `None`, create one automatically.
+            Title of the figure. If :obj:`None`, create one automatically.
         labelrot
             Rotation of labels on x-axis.
         legend_loc
-            Position of the legend. If `None`, don't show legend.
+            Position of the legend. If :obj:`None`, don't show the legend.
         %(plotting)s
         show
-            If `False`, return :class:`matplotlib.pyplot.Axes`.
+            If `False`, return the :class:`~matplotlib.axes.Axes` object.
 
         Returns
         -------
-        The axes object, if ``show = False``.
-        %(just_plots)s
+        If ``show = True``, nothing, just plots, otherwise returns the axes object.
+        Optionally saves it based on ``save``.
         """
         from cellrank.pl._utils import _position_legend
 
         macrostates = self.macrostates
         if macrostates is None:
             raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
         if key not in self.adata.obs:
             raise KeyError(f"Data not found in `adata.obs[{key!r}]`.")
         if not is_categorical_dtype(self.adata.obs[key]):
             raise TypeError(
-                f"Expected `adata.obs[{key!r}]` to be `categorical`, "
-                f"found `{infer_dtype(self.adata.obs[key])}`."
+                f"Expected `adata.obs[{key!r}]` to be `categorical`, " f"found `{infer_dtype(self.adata.obs[key])}`."
             )
 
         mask = ~macrostates.isnull()
         df = (
             pd.DataFrame({"macrostates": macrostates, key: self.adata.obs[key]})[mask]
             .groupby([key, "macrostates"])
             .size()
         )
         try:
             cats_colors = self.adata.uns[f"{key}_colors"]
         except KeyError:
-            cats_colors = _create_categorical_colors(
-                len(self.adata.obs[key].cat.categories)
-            )
+            cats_colors = _create_categorical_colors(len(self.adata.obs[key].cat.categories))
         cat_color_mapper = dict(zip(self.adata.obs[key].cat.categories, cats_colors))
         x_indices = np.arange(len(macrostates.cat.categories))
         bottom = np.zeros_like(x_indices, dtype=np.float32)
 
         width = min(1, max(0, width))
         fig, ax = plt.subplots(figsize=figsize, dpi=dpi, tight_layout=True)
         for cat, color in cat_color_mapper.items():
@@ -848,19 +1020,15 @@
         self,
         n_cells: Optional[int],
         cluster_key: Optional[str],
     ) -> None:
         start = logg.info("For 1 macrostate, stationary distribution is computed")
 
         eig = self.eigendecomposition
-        if (
-            eig is not None
-            and "stationary_dist" in eig
-            and eig["params"]["which"] == "LR"
-        ):
+        if eig is not None and "stationary_dist" in eig and eig["params"]["which"] == "LR":
             stationary_dist = eig["stationary_dist"]
         else:
             self.compute_eigendecomposition(only_evals=False, which="LR")
             stationary_dist = self.eigendecomposition["stationary_dist"]
 
         self._set_macrostates(
             memberships=stationary_dist[:, None],
@@ -873,119 +1041,126 @@
     @d.dedent
     def _set_macrostates(
         self,
         memberships: np.ndarray,
         n_cells: Optional[int] = 30,
         cluster_key: str = "clusters",
         check_row_sums: bool = True,
-        time: Optional[datetime] = None,
-        params: Dict[str, Any] = MappingProxyType({}),
+        time: Optional[datetime.datetime] = None,
+        params: Dict[str, Any] = types.MappingProxyType({}),
     ) -> None:
-        """
-        Map fuzzy clustering to pre-computed annotations to get names and colors.
+        """Map fuzzy clustering to pre-computed annotations to get names and colors.
 
         Given the fuzzy clustering, we would like to select the most likely cells from each state and use these to
         give each state a name and a color by comparing with pre-computed, categorical cluster annotations.
 
         Parameters
         ----------
         memberships
             Fuzzy clustering.
         %(n_cells)s
         cluster_key
-            Key from :attr:`anndata.AnnData.obs` to get reference cluster annotations.
+            Key from :attr:`~anndata.AnnData.obs` to get reference cluster annotations.
         check_row_sums
-            Check whether rows in `memberships` sum to `1`.
+            Check whether rows in `memberships` sum to :math:`1`.
         time
             Start time of macrostates computation.
         params
             Parameters used in macrostates computation.
 
         Returns
         -------
-        Nothing, just updates the field as described in :meth:`compute_macrostates`.
+        Nothing, just updates the fields as described in :meth:`compute_macrostates`.
         """
-
         if n_cells is None:
             # fmt: off
             logg.debug("Setting the macrostates using macrostate assignment")
             assignment = pd.Series(np.argmax(memberships, axis=1).astype(str), dtype="category")
             # sometimes, a category can be missing
             assignment = assignment.cat.reorder_categories([str(i) for i in range(memberships.shape[1])])
-            not_enough_cells = []
             # fmt: on
         else:
             logg.debug("Setting the macrostates using macrostates memberships")
 
             # select the most likely cells from each macrostate
             assignment, not_enough_cells = self._create_states(
                 memberships,
                 n_cells=n_cells,
                 check_row_sums=check_row_sums,
                 return_not_enough_cells=True,
             )
 
         # remove previous fields
-        self._write_terminal_states(None, None, None, None, log=False)
-
         # fmt: off
+        self._write_states("initial", states=None, colors=None, probs=None, memberships=None, log=False)
+        self._write_states("terminal", states=None, colors=None, probs=None, memberships=None, log=False)
+
         assignment, colors = self._set_categorical_labels(assignment, cluster_key=cluster_key)
         memberships = Lineage(memberships, names=list(assignment.cat.categories), colors=colors)
         # fmt: on
 
-        groups = pd.DataFrame(assignment).groupby(0).size()
+        groups = assignment.value_counts()
         groups = groups[groups != n_cells].to_dict()
         if len(groups):
             logg.warning(
-                f"The following terminal states have different number "
-                f"of cells than requested ({n_cells}): {groups}"
+                f"The following terminal states have different number " f"of cells than requested ({n_cells}): {groups}"
             )
 
         self._write_macrostates(
-            assignment, colors, memberships, time=time, params=params
+            macrostates=assignment,
+            colors=colors,
+            memberships=memberships,
+            time=time,
+            params=params,
         )
 
     @logger
     @shadow
     def _write_macrostates(
         self,
         macrostates: pd.Series,
         colors: np.ndarray,
         memberships: Lineage,
-        params: Dict[str, Any] = MappingProxyType({}),
+        params: Dict[str, Any] = types.MappingProxyType({}),
     ) -> str:
         # fmt: off
-        names = list(macrostates.cat.categories)
-
         key = Key.obs.macrostates(self.backward)
-        self._set("_macrostates", obj=self.adata.obs, key=key, value=macrostates, shadow_only=True)
+        self._set(obj=self.adata.obs, key=key, value=macrostates)
         ckey = Key.uns.colors(key)
-        self._set("_macrostates_colors", obj=self.adata.uns, key=ckey, value=colors, shadow_only=True)
+        self._set(obj=self.adata.uns, key=ckey, value=colors)
         mkey = Key.obsm.memberships(key)
-        self._set("_macrostates_memberships", obj=self.adata.obsm, key=mkey, value=memberships, shadow_only=True)
+        self._set(obj=self.adata.obsm, key=mkey, value=memberships)
+        self._macrostates = self._macrostates.set(assignment=macrostates, colors=colors, memberships=memberships)
         self.params[key] = dict(params)
 
+        names = list(macrostates.cat.categories)
         if len(names) > 1:
             # not using stationary distribution
             g = self._gpcca
             tmat = pd.DataFrame(g.coarse_grained_transition_matrix, index=names, columns=names)
             init_dist = pd.Series(g.coarse_grained_input_distribution, index=names)
-            stat_dist = pd.Series(g.coarse_grained_stationary_probability, index=names)
-            dists = pd.DataFrame({"coarse_init_dist": init_dist})
+            if g.coarse_grained_stationary_probability is None:
+                stat_dist = None
+            else:
+                stat_dist = pd.Series(g.coarse_grained_stationary_probability, index=names)
+            dists = pd.DataFrame({"coarse_init_dist": init_dist}, index=names)
             if stat_dist is not None:
-                dists["coarse_stat_dist"] = pd.Series(stat_dist, index=names)
+                dists["coarse_stat_dist"] = stat_dist
 
             key = Key.obsm.schur_vectors(self.backward)
             self._set("_schur_vectors", obj=self.adata.obsm, key=key, value=g._p_X, shadow_only=True)
             key = Key.uns.schur_matrix(self.backward)
             self._set("_schur_matrix", obj=self.adata.uns, key=key, value=g._p_R, shadow_only=True)
             self._set("_coarse_tmat", value=tmat, shadow_only=True)
             self._set("_coarse_init_dist", value=init_dist, shadow_only=True)
             self._set("_coarse_stat_dist", value=stat_dist, shadow_only=True)
-            self._set(obj=self.adata.uns, key=Key.uns.coarse(self.backward), value=AnnData(tmat, obs=dists))
+            self._set(
+                obj=self.adata.uns, key=Key.uns.coarse(self.backward),
+                value=AnnData(tmat, obs=dists, dtype=float)
+            )
         else:
             for attr in ["_schur_vectors", "_schur_matrix", "_coarse_tmat", "_coarse_init_dist", "_coarse_stat_dist"]:
                 self._set(attr, value=None, shadow_only=True)
             self._set(obj=self.adata.uns, key=Key.uns.coarse(self.backward), value=None)
         # fmt: on
 
         return (
@@ -998,194 +1173,100 @@
             "       `.schur_matrix`\n"
             "       `.eigendecomposition`\n"
             "    Finish"
         )
 
     @logger
     @shadow
-    def _write_terminal_states(
+    def _write_states(
         self,
+        which: Literal["initial", "terminal"],
         states: Optional[pd.Series],
         colors: Optional[np.ndarray],
         probs: Optional[pd.Series] = None,
         memberships: Optional[Lineage] = None,
-        params: Dict[str, Any] = MappingProxyType({}),
+        params: Dict[str, Any] = types.MappingProxyType({}),
+        allow_overlap: bool = False,
     ) -> str:
+        msg = super()._write_states(
+            which,
+            states=states,
+            colors=colors,
+            probs=probs,
+            params=params,
+            allow_overlap=allow_overlap,
+            log=False,
+        )
         # fmt: off
-        msg = super()._write_terminal_states(states, colors, probs, params=params, log=False)
         msg = "\n".join(msg.split("\n")[:-1])
-        msg += "\n       `.terminal_states_memberships\n    Finish`"
+        msg += f"\n       `.{which}_states_memberships\n    Finish`"
 
-        self._write_absorption_probabilities(None, None, log=False)
-        key = Key.obsm.memberships(Key.obs.term_states(self.backward))
-        self._set("_term_states_memberships", obj=self.adata.obsm, key=key, value=memberships)
+        self._write_fate_probabilities(None, log=False)
+        # TODO(michalk8): CFLARE doesn't remove the downstream properties
+        self._write_absorption_times(None, log=False)
+
+        backward = which == "initial"
+        key = Key.obsm.memberships(Key.obs.term_states(self.backward, bwd=backward))
+        self._set(obj=self.adata.obsm, key=key, value=memberships)
+        if backward:
+            self._init_states = self._init_states.set(memberships=memberships)
+        else:
+            self._term_states = self._term_states.set(memberships=memberships)
         # fmt: on
 
         return msg
 
     def _read_from_adata(self, adata: AnnData, **kwargs: Any) -> bool:
+        # design choice: no need to eigen/Schur-decomposition
         _ = self._read_eigendecomposition(adata, allow_missing=True)
-        # TODO(michalk8): reintroduce in 2.0
         ok = self._read_schur_decomposition(adata, allow_missing=True)
         if not ok:
             return False
 
         # fmt: off
         with SafeGetter(self, allowed=KeyError) as sg:
             key = Key.obs.macrostates(self.backward)
             # TODO(michalk8): in the future, be more stringent and ensure the categories match the macro memberships
-            self._get("_macrostates", self.adata.obs, key=key, where="obs", dtype=pd.Series)
+            assignment = self._get(obj=adata.obs, key=key, shadow_attr="obs", dtype=pd.Series)
             ckey = Key.uns.colors(key)
-            self._get("_macrostates_colors", self.adata.uns, key=ckey, where="uns", dtype=(list, tuple, np.ndarray))
+            colors = self._get(obj=adata.uns, key=ckey, shadow_attr="uns", dtype=(list, tuple, np.ndarray))
             mkey = Key.obsm.memberships(key)
-            self._get("_macrostates_memberships", self.adata.obsm, key=mkey, where="obsm", dtype=(Lineage, np.ndarray))
-            self._ensure_lineage_object("_macrostates_memberships", kind="macrostates")
-
-            self._macrostates_colors = self.macrostates_memberships.colors.copy()
+            memberships = self._get(obj=adata.obsm, key=mkey, shadow_attr="obsm", dtype=(Lineage, np.ndarray))
+            memberships = self._ensure_lineage_object(memberships, backward=self.backward, kind="macrostates")
+            self._macrostates = StatesHolder(assignment=assignment, colors=colors, memberships=memberships)
             self.params[key] = self._read_params(key)
 
-            # TODO(michalk8): allow missing?
-            tmat: AnnData = self.adata.uns[Key.uns.coarse(self.backward)]
+            tmat = adata.uns[Key.uns.coarse(self.backward)].copy()
             if not isinstance(tmat, AnnData):
-                raise TypeError(f"Expected coarse-grained transition matrix to be stored "
-                                f"as `anndata.AnnData`, found `{type(tmat).__name__}`.")
-            tmat = tmat.copy()
-            names = tmat.obs_names
+                raise TypeError(
+                    f"Expected coarse-grained transition matrix to be stored "
+                    f"as `AnnData`, found `{type(tmat).__name__}`."
+                )
 
-            self._coarse_tmat = pd.DataFrame(tmat.X, index=names, columns=names)
+            self._coarse_tmat = pd.DataFrame(tmat.X, index=tmat.obs_names, columns=tmat.obs_names)
             self._coarse_init_dist = tmat.obs["coarse_init_dist"]
             self._coarse_stat_dist = tmat.obs.get("coarse_stat_dist", None)
 
             self._set(obj=self._shadow_adata.uns, key=Key.uns.coarse(self.backward), value=tmat)
 
-        # TODO(michalk8): reintroduce this in 2.0 - this is done for high-level plotting of init/term states only
-        # if not sg.ok:
-        #    return False
+        if not sg.ok:
+            return False
 
         if not super()._read_from_adata(adata, **kwargs):
             return False
 
-        with SafeGetter(self, allowed=KeyError) as sg:
-            key = Key.obsm.memberships(Key.obs.term_states(self.backward))
-            self._get("_term_states_memberships", self.adata.obsm, key=key, where="obsm", dtype=(np.ndarray, Lineage))
-            self._ensure_lineage_object("_term_states_memberships", kind="term_states")
+        # status is based on `backward=False` by design
+        for backward in [True, False]:
+            with SafeGetter(self, allowed=KeyError) as sg:
+                key = Key.obsm.memberships(Key.obs.term_states(self.backward, bwd=backward))
+                memberships = self._get(obj=adata.obsm, key=key, shadow_attr="obsm", dtype=(np.ndarray, Lineage))
+                memberships = self._ensure_lineage_object(memberships, backward=backward, kind="term_states")
+                if backward:
+                    self._init_states = self._init_states.set(memberships=memberships)
+                else:
+                    self._term_states = self._term_states.set(memberships=memberships)
+                self._set(obj=self._shadow_adata.obsm, key=key, value=memberships)
         # fmt: on
 
-        return sg.ok and self._read_absorption_probabilities(adata)
-
-    plot_macrostates = register_plotter(
-        discrete="macrostates", continuous="macrostates_memberships"
-    )
-    plot_terminal_states = register_plotter(
-        discrete="terminal_states", continuous="terminal_states_memberships"
-    )
-
-    @d.dedent
-    def _compute_initial_states(self, n_states: int = 1, n_cells: int = 30) -> None:
-        """
-        Compute initial states from macrostates using :attr:`coarse_stationary_distribution`.
-
-        Parameters
-        ----------
-        n_states
-            Number of initial states.
-        %(n_cells)s
-
-        Returns
-        -------
-        %(set_initial_states_from_macrostates.returns)s
-        """
-
-        if n_states <= 0:
-            raise ValueError(f"Expected `n_states` to be positive, found `{n_states}`.")
-
-        if n_cells <= 0:
-            raise ValueError(f"Expected `n_cells` to be positive, found `{n_cells}`.")
-
-        probs = self.macrostates_memberships
-        if probs is None:
-            raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
-
-        if n_states > probs.shape[1]:
-            raise ValueError(
-                f"Requested `{n_states}` initial states, but only `{probs.shape[1]}` macrostates have been computed."
-            )
-
-        if probs.shape[1] == 1:
-            self._set_initial_states_from_macrostates(n_cells=n_cells)
-            return
-
-        stat_dist = self.coarse_stationary_distribution
-        if stat_dist is None:
-            raise RuntimeError("No coarse-grained stationary distribution found.")
-
-        self._set_initial_states_from_macrostates(
-            stat_dist[np.argsort(stat_dist)][:n_states].index, n_cells=n_cells
-        )
-
-    @d.get_sections(base="set_initial_states_from_macrostates", sections=["Returns"])
-    @d.dedent
-    def _set_initial_states_from_macrostates(
-        self,
-        names: Optional[Union[str, Sequence[str]]] = None,
-        n_cells: int = 30,
-    ) -> None:
-        """
-        Manually select initial states from macrostates.
-
-        Note that no check is performed to ensure initial and terminal states are distinct.
-
-        Parameters
-        ----------
-        names
-            Names of the macrostates to be marked as initial states. Multiple states can be combined using `','`,
-            such as `["Alpha, Beta", "Epsilon"]`.
-        %(n_cells)s
-
-        Returns
-        -------
-        Nothing, just modifies :attr:`anndata.AnnData.obs`. The actual keys depend of :attr:`backward`.
-        """
-
-        if not isinstance(n_cells, int):
-            raise TypeError(
-                f"Expected `n_cells` to be of type `int`, found `{type(n_cells).__name__}`."
-            )
-
-        if n_cells <= 0:
-            raise ValueError(f"Expected `n_cells` to be positive, found `{n_cells}`.")
-
-        probs = self.macrostates_memberships
-        if probs is None:
-            raise RuntimeError("Compute macrostates first as `.compute_macrostates()`.")
-        elif probs.shape[1] == 1:
-            categorical = self._create_states(probs, n_cells=n_cells)
-            scaled = probs / probs.max()
-        else:
-            if names is None:
-                names = probs.names
-            if isinstance(names, str):
-                names = [names]
-
-            probs = probs[list(names)]
-            categorical = self._create_states(probs, n_cells=n_cells)
-            probs /= probs.max(0)
-
-            # compute the aggregated probability of being a initial/terminal state (no matter which)
-            scaled = probs.X.max(1)
-
-        self._write_initial_states(membership=probs, probs=scaled, cats=categorical)
-
-    def _write_initial_states(
-        self, membership: Lineage, probs: pd.Series, cats: pd.Series, time=None
-    ) -> None:
-        key = Key.obs.term_states(not self.backward)
-
-        self.adata.obs[key] = cats
-        self.adata.obs[Key.obs.probs(key)] = probs
-
-        self.adata.uns[Key.uns.colors(key)] = membership.colors
-
-        logg.info(
-            f"Adding `adata.obs[{key!r}]`\n       `adata.obs[{Key.uns.colors(key)!r}]`\n",
-            time=time,
-        )
+        fate_prob_ok = self._read_fate_probabilities(adata)
+        abs_time_ok = self._read_absorption_times(adata)
+        return sg.ok and fate_prob_ok and abs_time_ok
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_base_kernel.py` & `cellrank-2.0.0/src/cellrank/models/_base_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1384 +1,1420 @@
-"""Kernel module."""
-from typing import (
-    Any,
-    Dict,
-    List,
-    Type,
-    Tuple,
-    Union,
-    Callable,
-    Iterable,
-    Optional,
-    Sequence,
-)
-
+import abc
+import collections
+import copy
+import enum
+import re
 import warnings
-from abc import ABC, abstractmethod
-from copy import copy
-from pathlib import Path
-from functools import reduce
+from typing import Any, Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
-import scvelo as scv
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank.ul._docs import d, inject_docs
-from cellrank.tl._utils import (
-    save_fig,
-    _connected,
-    _normalize,
-    _symmetric,
-    _get_neighs,
-    _irreducible,
-)
-from scvelo.plotting.utils import default_size, plot_outline
-from cellrank.tl._mixins._io import IOMixin
-from cellrank.tl.kernels._utils import _get_basis, _filter_kwargs
-from cellrank.tl.kernels._tmat_flow import FlowPlotter
-from cellrank.tl.kernels._random_walk import RandomWalk
+import wrapt
 
 import numpy as np
-from scipy.sparse import spdiags, issparse, spmatrix, csr_matrix, isspmatrix_csr
-from pandas.api.types import infer_dtype, is_numeric_dtype
-from pandas.core.dtypes.common import is_categorical_dtype
+import scipy.sparse as sp
+from pandas.api.types import infer_dtype, is_categorical_dtype, is_numeric_dtype
+from scipy.ndimage import convolve
 
+import matplotlib as mpl
 import matplotlib.pyplot as plt
-from matplotlib.colors import LinearSegmentedColormap, to_hex
-from matplotlib.collections import LineCollection
+from matplotlib import cm, colors
+from mpl_toolkits.axes_grid1 import make_axes_locatable
 
-_ERROR_DIRECTION_MSG = "Can only combine kernels that have the same direction."
-_ERROR_EMPTY_CACHE_MSG = (
-    "Fatal error: tried to used cached values, but the cache was empty."
-)
-_ERROR_CONF_ADAPT = (
-    "Confidence adaptive operator is only supported for kernels, found type `{!r}`."
-)
-_ERROR_VAR_NOT_FOUND = "Variances not found in kernel `{!r}`."
-
-_LOG_USING_CACHE = "Using cached transition matrix"
-
-_RTOL = 1e-12
-_n_dec = 2
-_dtype = np.float64
-_cond_num_tolerance = 1e-15
-Indices_t = Optional[
-    Union[Sequence[str], Dict[str, Union[str, Sequence[str], Tuple[float, float]]]]
-]
+from anndata import AnnData
+from scanpy.plotting._utils import add_colors_for_categorical_sample_annotation
 
+from cellrank import logging as logg
+from cellrank._utils._docs import d
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._lineage import Lineage
+from cellrank._utils._utils import _densify_squeeze, _minmax, save_fig, valuedispatch
+from cellrank.kernels.mixins import IOMixin
+
+__all__ = ["BaseModel"]
+
+_dup_spaces = re.compile(r" +")  # used on repr for underlying model's repr
+ArrayLike = Union[np.ndarray, sp.spmatrix, List, Tuple]
+
+
+class UnknownModelError(RuntimeError):
+    pass
+
+
+class FailedReturnType(ModeEnum):
+    PREPARE = enum.auto()
+    FIT = enum.auto()
+    PREDICT = enum.auto()
+    CONFIDENCE_INTERVAL = enum.auto()
+    DEFAULT_CONFIDENCE_INTERVAL = enum.auto()
+    PLOT = enum.auto()
+
+
+class ColorType(ModeEnum):
+    CONT = enum.auto()
+    CAT = enum.auto()
+    STR = enum.auto()
+
+
+def _handle_exception(return_type: FailedReturnType, func: Callable) -> Callable:
+    def handle(*, exception_handler: Callable):
+        @wrapt.decorator
+        def wrapper(wrapped, instance, args, kwargs):
+            try:
+                if isinstance(instance, FailedModel):
+                    instance.reraise()
+                return wrapped(*args, **kwargs)
+            except Exception as e:  # noqa: BLE001
+                return exception_handler(instance, e, *args, **kwargs)
+
+        return wrapper
+
+    def array_output(instance: "BaseModel", exc: BaseException, *_args, **kwargs) -> np.ndarray:
+        if not instance._is_bulk:
+            raise exc from None
+
+        if kwargs.get("x_test", None) is not None:
+            n_obs = kwargs["x_test"].shape[0]
+        elif instance.x_test is not None:
+            n_obs = instance.x_test.shape[0]
+        else:
+            n_obs = 200
 
-class KernelExpression(IOMixin, ABC):
-    """Base class for all kernels and kernel expressions."""
+        return np.full((n_obs, array_shape), np.nan, dtype=instance._dtype)
 
-    def __init__(
-        self,
-        op_name: Optional[str] = None,
-        backward: bool = False,
-        compute_cond_num: bool = False,
-    ):
-        self._op_name = op_name
-        self._transition_matrix = None
-        self._backward = backward
-        self._compute_cond_num = compute_cond_num
-        self._cond_num = None
-        self._params = {}
-        self._normalize = True
-        self._parent = None
+    def model_output(instance: "BaseModel", exc: BaseException, *_args, **_kwargs) -> "FailedModel":
+        if not isinstance(instance, FailedModel):
+            instance = FailedModel(instance, exc=exc)
+        if not instance._is_bulk:
+            instance.reraise()
+
+        return instance
+
+    def no_output(instance: "BaseModel", exc: BaseException, *_args, **_kwargs) -> None:
+        if not instance._is_bulk:
+            raise exc from None
+
+    @valuedispatch
+    def wrapper(mode: FailedReturnType, *_args, **_kwargs):
+        raise NotImplementedError(mode)
+
+    @wrapper.register(FailedReturnType.PREPARE)
+    @wrapper.register(FailedReturnType.FIT)
+    def _(func: Callable) -> Callable:
+        return handle(exception_handler=model_output)(func)
+
+    @wrapper.register(FailedReturnType.PREDICT)
+    @wrapper.register(FailedReturnType.CONFIDENCE_INTERVAL)
+    @wrapper.register(FailedReturnType.DEFAULT_CONFIDENCE_INTERVAL)
+    def _(func: Callable) -> Callable:
+        return handle(exception_handler=array_output)(func)
+
+    @wrapper.register(FailedReturnType.PLOT)
+    def _(func: Callable):
+        return handle(exception_handler=no_output)(func)
+
+    return_type = FailedReturnType(return_type)
+    array_shape = 1 + (
+        return_type
+        in (
+            FailedReturnType.CONFIDENCE_INTERVAL,
+            FailedReturnType.DEFAULT_CONFIDENCE_INTERVAL,
+        )
+    )
 
-    def __init_subclass__(cls, **kwargs: Any):
-        super().__init_subclass__()
+    return wrapper(return_type, func)
 
-    @property
-    def condition_number(self) -> Optional[int]:
-        """Condition number of the transition matrix."""
-        return self._cond_num
 
-    @property
-    def transition_matrix(self) -> Union[np.ndarray, spmatrix]:
-        """
-        Return row-normalized transition matrix.
+class BaseModelMeta(abc.ABCMeta):
+    """Metaclass for all base models."""
+
+    def __new__(cls, clsname: str, superclasses: Tuple[type, ...], attributedict: Dict[str, Any]):
+        """Create a new instance.
 
-        If not present, it is computed iff all underlying kernels have been initialized.
+        Parameters
+        ----------
+        clsname
+            Name of class to be constructed.
+        superclasses
+            List of superclasses.
+        attributedict
+            Dictionary of attributes.
         """
+        obj = super().__new__(cls, clsname, superclasses, attributedict)
+        for fun_name in list(FailedReturnType):
+            setattr(
+                obj,
+                fun_name,
+                _handle_exception(FailedReturnType(fun_name), getattr(obj, fun_name)),
+            )
+
+        return obj
+
 
-        if self._parent is None and self._transition_matrix is None:
-            self.compute_transition_matrix()
+@d.get_sections(base="base_model", sections=["Parameters"])
+@d.dedent
+class BaseModel(IOMixin, abc.ABC, metaclass=BaseModelMeta):
+    """Base class for all model classes.
+
+    Parameters
+    ----------
+    %(adata)s
+    model
+        The underlying model that is used for fitting and prediction.
+    """
 
-        return self._transition_matrix
+    _dtype = np.float64
 
+    def __init__(
+        self,
+        adata: Optional[AnnData],
+        model: Any,
+    ):
+        if not isinstance(adata, AnnData) and not isinstance(self, FittedModel):
+            # FittedModel doesn't need it
+            raise TypeError(f"Expected `adata` to be of type `anndata.AnnData`, found `{type(adata).__name__}`.")
+        super().__init__()
+
+        self._adata = adata
+        self._n_obs = 0 if adata is None else adata.n_obs
+        self._model = model
+        self._gene = None
+        self._use_raw = False
+        self._data_key = None
+        self._lineage = None
+        self._prepared = False
+
+        self._obs_names = None
+        self._is_bulk = False
+
+        self._x_all = None
+        self._y_all = None
+        self._w_all = None
+
+        self._x = None
+        self._y = None
+        self._w = None
+
+        self._x_test = None
+        self._y_test = None
+        self._x_hat = None
+        self._y_hat = None
+
+        self._conf_int = None
+
+    @d.get_summary(base="base_model_prepared")
     @property
-    def backward(self) -> bool:
-        """Direction of the process."""
-        return self._backward
+    def prepared(self):
+        """Whether the model is prepared for fitting."""
+        return self._prepared
 
     @property
-    @abstractmethod
+    @d.dedent
     def adata(self) -> AnnData:
         """Annotated data object."""
+        return self._adata
 
     @adata.setter
-    @abstractmethod
-    def adata(self, value: AnnData) -> None:
-        pass
+    def adata(self, adata: Optional[AnnData]) -> None:
+        self._adata = adata
 
     @property
-    @abstractmethod
-    def shape(self) -> Tuple[int, int]:
-        """`(n_cells, n_cells)`."""
+    def shape(self) -> Tuple[int]:
+        """Number of cells in :attr:`adata`."""
+        return (self._n_obs,)
 
     @property
-    def params(self) -> Dict[str, Any]:
-        """Parameters which are used to compute the transition matrix."""
-        if len(self.kernels) == 1:
-            return self._params
-        # we need some identifier
-        return {f"{repr(k)}:{i}": k.params for i, k in enumerate(self.kernels)}
-
-    def _format_params(self):
-        return ", ".join(
-            f"{k}={round(v, _n_dec) if isinstance(v, float) else v}"
-            for k, v in self.params.items()
-        )
+    def model(self) -> Any:
+        """Underlying model."""
+        return self._model
 
-    @transition_matrix.setter
-    def transition_matrix(self, value: Union[np.ndarray, spmatrix]) -> None:
-        """
-        Set a new value of the transition matrix.
+    @property
+    @d.get_summary(base="base_model_x_all")
+    def x_all(self) -> np.ndarray:
+        """Unfiltered independent variables of shape ``(n_cells, 1)``."""
+        return self._x_all
 
-        Parameters
-        ----------
-        value
-            The new transition matrix. If the expression has no parent, the matrix is normalized, if needed.
+    @property
+    @d.get_summary(base="base_model_y_all")
+    def y_all(self) -> np.ndarray:
+        """Unfiltered dependent variables of shape ``(n_cells, 1)``."""
+        return self._y_all
 
-        Returns
-        -------
-        None
-            Nothing, just updates the :attr:`transition_matrix` and optionally normalizes it.
-        """
-        should_norm = ~np.isclose(value.sum(1), 1.0, rtol=_RTOL).all()
+    @property
+    @d.get_summary(base="base_model_w_all")
+    def w_all(self) -> np.ndarray:
+        """Unfiltered weights of shape ``(n_cells,)``."""
+        return self._w_all
 
-        if self._parent is None:
-            self._transition_matrix = _normalize(value) if should_norm else value
-        else:
-            # it's AND, not OR, because of combinations
-            self._transition_matrix = (
-                _normalize(value) if self._normalize and should_norm else value
-            )
+    @property
+    @d.get_summary(base="base_model_x")
+    def x(self) -> np.ndarray:
+        """Filtered independent variables of shape ``(n_filtered_cells, 1)`` used for fitting."""
+        return self._x
 
-    @abstractmethod
-    def compute_transition_matrix(
-        self, *args: Any, **kwargs: Any
-    ) -> "KernelExpression":
-        """
-        Compute a transition matrix.
+    @property
+    @d.get_summary(base="base_model_y")
+    def y(self) -> np.ndarray:
+        """Filtered dependent variables of shape ``(n_filtered_cells, 1)`` used for fitting."""
+        return self._y
 
-        Parameters
-        ----------
-        args
-            Positional arguments.
-        kwargs
-            Keyword arguments.
+    @property
+    @d.get_summary(base="base_model_w")
+    def w(self) -> np.ndarray:
+        """Filtered weights of shape ``(n_filtered_cells,)`` used for fitting."""
+        return self._w
 
-        Returns
-        -------
-        :class:`cellrank.tl.kernels.KernelExpression`
-            Self.
-        """
+    @property
+    @d.get_summary(base="base_model_x_test")
+    def x_test(self) -> np.ndarray:
+        """Independent variables of shape ``(n_samples, 1)`` used for prediction."""
+        return self._x_test
+
+    @property
+    @d.get_summary(base="base_model_y_test")
+    def y_test(self) -> np.ndarray:
+        """Prediction values of shape ``(n_samples,)`` for :attr:`x_test`."""
+        return self._y_test
+
+    @property
+    @d.get_summary(base="base_model_x_hat")
+    def x_hat(self) -> np.ndarray:
+        """Filtered independent variables used when calculating default confidence interval, usually same as :attr:`x`."""  # noqa: E501
+        return self._x_hat
 
-    @d.get_sections(base="write_to_adata", sections=["Parameters"])
-    @inject_docs()  # get rid of {{}}
+    @property
+    @d.get_summary(base="base_model_y_hat")
+    def y_hat(self) -> np.ndarray:
+        """Filtered dependent variables used when calculating default confidence interval, usually same as :attr:`y`."""
+        return self._y_hat
+
+    @property
+    @d.get_summary(base="base_model_conf_int")
+    def conf_int(self) -> np.ndarray:
+        """Array of shape ``(n_samples, 2)`` containing the lower and upper bound of the confidence interval."""
+        return self._conf_int
+
+    @d.get_sections(base="base_model_prepare", sections=["Parameters", "Returns"])
+    @d.get_full_description(base="base_model_prepare")
     @d.dedent
-    def write_to_adata(self, key: Optional[str] = None) -> None:
-        """
-        Write the transition matrix and parameters used for computation to the underlying :attr:`adata` object.
+    def prepare(
+        self,
+        gene: str,
+        lineage: Optional[str],
+        time_key: str,
+        backward: bool = False,
+        time_range: Optional[Union[float, Tuple[float, float]]] = None,
+        data_key: Optional[str] = "X",
+        use_raw: bool = False,
+        threshold: Optional[float] = None,
+        weight_threshold: Union[float, Tuple[float, float]] = (0.01, 0.01),
+        filter_cells: Optional[float] = None,
+        n_test_points: int = 200,
+    ) -> "BaseModel":
+        """Prepare the model to be ready for fitting.
 
         Parameters
         ----------
-        key
-            Key used when writing transition matrix to :attr:`adata`. If `None`, determine the key automatically.
+        gene
+            Gene in :attr:`~anndata.AnnData.var_names`.
+        lineage
+            Name of the lineage. If :obj:`None`, all weights will be set to :math:`1`.
+        time_key
+            Key in :attr:`~anndata.AnnData.obs` where the pseudotime is stored.
+        %(backward)s
+        %(time_range)s
+        data_key
+            Key in :attr:`~anndata.AnnData.layers` or ``'X'`` for :attr:`~anndata.AnnData.X`.
+            If ``use_raw = True``, it's always set to ``'X'``.
+        use_raw
+            Whether to access :attr:`~anndata.AnnData.raw`.
+        threshold
+            Consider only cells with weights > ``threshold`` when estimating the test endpoint.
+            If :obj:`None`, use the median of the weights.
+        weight_threshold
+            Set all weights below ``weight_threshold`` to ``weight_threshold`` if a :class:`float`,
+            or to the second value, if a :class:`tuple`.
+        filter_cells
+            Filter out all cells with expression values lower than this threshold.
+        n_test_points
+            Number of test points. If :obj:`None`, use the original points based on ``threshold``.
 
         Returns
         -------
-        None
-            %(write_to_adata)s
-        """
-        from cellrank._key import Key
+        Nothing, just updates the following fields:
 
-        if self._transition_matrix is None:
-            raise ValueError(
-                "Compute transition matrix first as `.compute_transition_matrix()`."
-            )
+        - :attr:`x` - %(base_model_x.summary)s
+        - :attr:`y` - %(base_model_y.summary)s
+        - :attr:`w` - %(base_model_w.summary)s
+        - :attr:`x_all` - %(base_model_x_all.summary)s
+        - :attr:`y_all` - %(base_model_y_all.summary)s
+        - :attr:`w_all` - %(base_model_w_all.summary)s
+        - :attr:`x_test` - %(base_model_x_test.summary)s
+        - :attr:`prepared` - %(base_model_prepared.summary)s
+        """
+        if use_raw:
+            if self.adata.raw is None:
+                raise AttributeError("AnnData object has no attribute `.raw`.")
+            if data_key != "X":
+                data_key = "X"
+        self._use_raw = use_raw
+
+        if data_key not in ["X", "obs", None] + list(self.adata.layers.keys()):
+            raise KeyError(
+                f"Data key must be a key of `adata.layers`: `{list(self.adata.layers.keys())}`, "
+                f"`adata.X` or `adata.obs`."
+            )
+
+        probs = Lineage.from_adata(self.adata, backward=backward)
+        if lineage is not None:
+            probs = probs[lineage]
+
+        if time_key not in self.adata.obs:
+            raise KeyError(f"Time key `{time_key!r}` not found in `adata.obs`.")
+
+        if data_key == "obs":
+            if gene not in self.adata.obs:
+                raise KeyError(f"Unable to find data in `adata.obs[{gene!r}]`.")
+        else:
+            if use_raw and gene not in self.adata.raw.var_names:
+                raise KeyError(f"Gene `{gene!r}` not found in `adata.raw.var_names`.")
+            if not use_raw and gene not in self.adata.var_names:
+                raise KeyError(f"Gene `{gene!r}` not found in `adata.var_names`.")
 
-        key = Key.uns.kernel(self.backward, key=key)
-        # retain the embedding info
-        self.adata.uns[f"{key}_params"] = {
-            **self.adata.uns.get(f"{key}_params", {}),
-            **{"params": self.params},
-        }
-        self.adata.obsp[key] = self.transition_matrix
-
-    @abstractmethod
-    def copy(self) -> "KernelExpression":
-        """Return a copy of itself. Note that the underlying :attr:`adata` object is not copied."""
-
-    def _maybe_compute_cond_num(self) -> None:
-        """Optionally compute condition number."""
-        if self._compute_cond_num and self._cond_num is None:
-            logg.debug("Computing condition number")
-            self._cond_num = np.linalg.cond(
-                self._transition_matrix.toarray()
-                if issparse(self._transition_matrix)
-                else self._transition_matrix
+        if not isinstance(time_range, (type(None), float, int, tuple)):
+            raise TypeError(
+                f"Expected time range to be either `None`, "
+                f"`float` or `tuple`, found `{type(time_range).__name__!r}`."
             )
-            if self._cond_num > _cond_num_tolerance:
-                logg.warning(
-                    f"Transition matrix may be ill-conditioned, its condition number is `{self._cond_num:.2e}`"
+        if isinstance(time_range, tuple):
+            if len(time_range) != 2:
+                raise ValueError(f"Expected time range to be a `tuple` of length `2`, found `{len(time_range)}`.")
+            if not isinstance(time_range[0], (float, int, type(None))) or not isinstance(
+                time_range[1], (float, int, type(None))
+            ):
+                raise TypeError(
+                    f"Expected values in time ranges be of types `float` or `int` or `None`, "
+                    f"got `{type(time_range[0]).__name__!r}` and `{type(time_range[1]).__name__!r}`."
                 )
-            else:
-                logg.info(f"Condition number is `{self._cond_num:.2e}`")
+            val_start, val_end = time_range
+        elif time_range is None:
+            val_start, val_end = None, None
+        else:
+            val_start, val_end = None, time_range
 
-    def _reuse_cache(
-        self, expected_params: Dict[str, Any], *, time: Optional[Any] = None
-    ) -> bool:
-        if expected_params == self._params:
-            assert self.transition_matrix is not None, _ERROR_EMPTY_CACHE_MSG
-            logg.debug(_LOG_USING_CACHE)
-            logg.info("    Finish", time=time)
-            return True
+        if isinstance(weight_threshold, (int, float)):
+            weight_threshold = (weight_threshold, weight_threshold)
+        if len(weight_threshold) != 2:
+            raise ValueError(f"Expected `weight_threshold` to be of size `2`, found `{len(weight_threshold)}`.")
+
+        self._obs_names = self.adata.obs_names.values[:]
+
+        x = np.array(self.adata.obs[time_key]).astype(self._dtype)
+
+        adata = self.adata.raw.to_adata() if use_raw else self.adata
+        gene_ix = np.where(adata.var_names == gene)[0]
+
+        if data_key in ("X", None):
+            y = adata.X[:, gene_ix]
+            self._data_key = None
+        elif data_key == "obs":
+            y = adata.obs[gene].values
+            # don't set data_key, it's just when `cell_color = ...`
+        elif data_key in adata.layers:
+            y = adata.layers[data_key][:, gene_ix]
+            self._data_key = data_key
+        else:
+            raise NotImplementedError(f"Data key `{data_key!r}` is not implemented.")
 
-        self._params = expected_params
-        return False
+        if lineage is not None:
+            weight_threshold, val = weight_threshold
+            w = _densify_squeeze(probs.X, self._dtype)
+            w[w < weight_threshold] = val
+        else:
+            w = np.ones(len(x), dtype=self._dtype)
 
-    @abstractmethod
-    def _get_kernels(self) -> Iterable["Kernel"]:
-        pass
+        if use_raw:
+            correct_ixs = np.isin(self.adata.obs_names, adata.obs_names)
+            x = x[correct_ixs]
+            y = y[correct_ixs]
+            w = w[correct_ixs]
+            self._obs_names = self._obs_names[correct_ixs]
+
+        del adata
+
+        self._x_all, self._y_all, self._w_all = (
+            _densify_squeeze(x, self._dtype)[:, np.newaxis],
+            _densify_squeeze(y, self._dtype)[:, np.newaxis],
+            w,
+        )
+        x, y, w = self.x_all[:], self.y_all[:], self.w_all[:]
 
-    @property
-    def kernels(self) -> List["Kernel"]:
-        """Get the kernels of the kernel expression, except for constants."""
-        return list(set(self._get_kernels()))
+        # sanity checks
+        if self._x_all.shape[0] != self._y_all.shape[0]:
+            raise ValueError(
+                f"Independent variable's first dimension ({self._x_all.shape[0]}) "
+                f"differs from dependent variable's first dimension ({self._y_all.shape[0]})."
+            )
+        if self._x_all.shape[0] != self._w_all.shape[0]:
+            raise ValueError(
+                f"Independent variable's first dimension ({self._x_all.shape[0]}) "
+                f"differs from weights' first dimension ({self._w_all.shape[0]})."
+            )
 
-    def compute_projection(
-        self,
-        basis: str = "umap",
-        key_added: Optional[str] = None,
-        copy: bool = False,
-    ) -> Optional[np.ndarray]:
-        """
-        Compute a projection of the transition matrix in the embedding.
+        x, ixs = np.unique(x, return_index=True)  # GAMR (mgcv) needs unique
+        y = y[ixs]
+        w = w[ixs]
+
+        ixs = np.argsort(x)
+        x, y, w = x[ixs], y[ixs], w[ixs]
+        self._obs_names = self._obs_names[ixs]
+
+        if np.allclose(w, w[0]):
+            # degenerate case
+            val_start = w[0] - 1
+            val_end = w[0] + 1
+
+        if val_start is None:
+            val_start = np.min(x)
+        if val_end is None:
+            if threshold is None:
+                threshold = np.nanmedian(w)
+            # use `>=` because weights can all be 1
+            w_test = w[w >= threshold]
+            n_window = n_test_points // 20
+            tmp = convolve(w_test, np.ones(n_window) / n_window, mode="nearest")
+            val_end = x[w >= threshold][-1 if lineage is None else np.nanargmax(tmp)]
+
+        if val_start > val_end:
+            val_start, val_end = val_end, val_start
+        val_start, val_end = (max(val_start, np.min(x)), min(val_end, np.max(x)))
+
+        fil = (x >= val_start) & (x <= val_end)
+        x_test = np.linspace(val_start, val_end, n_test_points) if n_test_points is not None else x[fil]
+        x, y, w = x[fil], y[fil], w[fil]
+        self._obs_names = self._obs_names[fil]
+
+        if filter_cells is not None:
+            tmp = y.squeeze()
+            fil = (tmp >= filter_cells) & (~np.isclose(tmp, filter_cells).astype(bool))
+            x, y, w = x[fil], y[fil], w[fil]
+            self._obs_names = self._obs_names[fil]
+
+        self._x, self._y, self._w = (
+            self._reshape_and_retype(x),
+            self._reshape_and_retype(y),
+            self._reshape_and_retype(w).squeeze(-1),
+        )
+        self._x_test = self._reshape_and_retype(x_test)
+        self._y_test = None
+        self._x_hat = None
+        self._y_hat = None
+        self._conf_int = None
+
+        if self.x.shape[0] == 0:
+            raise RuntimeError("Unable to proceed, no values to fit.")
+
+        if len({self.x.shape[0], self.y.shape[0], self.w.shape[0]}) != 1:
+            raise RuntimeError(
+                f"Values have different shapes: `{self.x.shape[0]}`, `{self.y.shape[0]}`, `{self.w.shape[0]}`."
+            )
+
+        self._gene = gene
+        self._lineage = lineage
+        self._prepared = True
 
-        Projections can only be calculated for kNN based kernels. The projected matrix
-        can be then visualized as::
+        return self
 
-            scvelo.pl.velocity_embedding(adata, vkey='T_fwd', basis='umap')
+    @abc.abstractmethod
+    @d.get_sections(base="base_model_fit", sections=["Parameters"])
+    @d.get_full_description(base="base_model_fit")
+    def fit(
+        self,
+        x: Optional[np.ndarray] = None,
+        y: Optional[np.ndarray] = None,
+        w: Optional[np.ndarray] = None,
+        **kwargs: Any,
+    ) -> "BaseModel":
+        """Fit the model.
 
         Parameters
         ----------
-        basis
-            Basis in :attr:`anndata.AnnData.obsm` for which to compute the projection.
-        key_added
-            If not `None` and ``copy = False``, save the result to :attr:`anndata.AnnData.obsm` ``['{key_added}']``.
-            Otherwise, save the result to `'T_fwd_{basis}'` or `T_bwd_{basis}`, depending on the direction.
-        copy
-            Whether to return the projection or modify :attr:`adata` inplace.
+        x
+            Independent variables, array of shape ``(n_samples, 1)``. If :obj:`None`, use :attr:`x`.
+        y
+            Dependent variables, array of shape ``(n_samples, 1)``. If :obj:`None`, use :attr:`y`.
+        w
+            Optional weights of :attr:`x`, array of shape ``(n_samples,)``. If :obj:`None`, use :attr:`w`.
+        kwargs
+            Keyword arguments for underlying :attr:`model`'s fitting function.
 
         Returns
         -------
-        If ``copy=True``, the projection array of shape `(n_cells, n_components)`.
-        Otherwise, it modifies :attr:`anndata.AnnData.obsm` with a key based on ``key_added``.
+        Fits the :attr:`model` and returns self.
         """
-        # modified from: https://github.com/theislab/scvelo/blob/master/scvelo/tools/velocity_embedding.py
-        from cellrank._key import Key
-        from scvelo.tools.velocity_embedding import quiver_autoscale
-
-        if self._transition_matrix is None:
-            raise RuntimeError(
-                "Compute transition matrix first as `.compute_transition_matrix()`."
-            )
-
-        for kernel in self.kernels:
-            if kernel._conn is None:
-                raise AttributeError(
-                    f"{kernel!r} is not a kNN based kernel. The embedding projection "
-                    "only works for kNN based kernels."
-                )
+        if not self.prepared:
+            raise RuntimeError("The model has not been prepared yet, call `.prepare()` first.")
 
-        start = logg.info(f"Projecting transition matrix onto `{basis}`")
-        emb = _get_basis(self.adata, basis)
-        T_emb = np.empty_like(emb)
+        self._check("_x", x)
+        self._check("_y", y)
+        self._check("_w", w, ndim=1)
+
+        if self._x.shape != self._y.shape:
+            raise ValueError(f"Inputs and targets differ in shape: `{self._x.shape}` vs. `{self._y.shape}`.")
+        if self._y.shape[0] != self._w.shape[0]:
+            raise ValueError(f"Inputs and weights differ in shape: `{self._y.shape[0]}` vs. `{self._w.shape[0]}`.")
 
-        conn = self.kernels[0]._conn
-
-        with warnings.catch_warnings():
-            warnings.simplefilter("ignore")
-            for row_id, row in enumerate(self.transition_matrix):
-                conn_idxs = conn[row_id, :].indices
-
-                dX = emb[conn_idxs] - emb[row_id, None]
-
-                if np.any(np.isnan(dX)):
-                    T_emb[row_id, :] = np.nan
-                else:
-                    probs = row[:, conn_idxs]
-                    if issparse(probs):
-                        probs = probs.A.squeeze()
-
-                    dX /= np.linalg.norm(dX, axis=1)[:, None]
-                    dX = np.nan_to_num(dX)
-                    T_emb[row_id, :] = probs.dot(dX) - dX.sum(0) / dX.shape[0]
-
-        T_emb /= 3 * quiver_autoscale(np.nan_to_num(emb), T_emb)
-
-        if copy:
-            return T_emb
-
-        key = Key.uns.kernel(self.backward, key=key_added)
-        ukey = f"{key}_params"
-
-        embs = self.adata.uns.get(ukey, {}).get("embeddings", [])
-        if basis not in embs:
-            embs = list(embs) + [basis]
-            self.adata.uns[ukey] = self.adata.uns.get(ukey, {})
-            self.adata.uns[ukey]["embeddings"] = embs
-
-        key = key + "_" + basis
-        logg.info(
-            f"Adding `adata.obsm[{key!r}]`\n    Finish",
-            time=start,
-        )
-        self.adata.obsm[key] = T_emb
+        return self
 
+    @abc.abstractmethod
+    @d.get_sections(base="base_model_predict", sections=["Parameters", "Returns"])
+    @d.get_full_description(base="base_model_predict")
     @d.dedent
-    def plot_random_walks(
+    def predict(
         self,
-        n_sims: int,
-        max_iter: Union[int, float] = 0.25,
-        seed: Optional[int] = None,
-        successive_hits: int = 0,
-        start_ixs: Indices_t = None,
-        stop_ixs: Indices_t = None,
-        basis: str = "umap",
-        cmap: Union[str, LinearSegmentedColormap] = "gnuplot",
-        linewidth: float = 1.0,
-        linealpha: float = 0.3,
-        ixs_legend_loc: Optional[str] = None,
-        n_jobs: Optional[int] = None,
-        backend: str = "loky",
-        show_progress_bar: bool = True,
-        figsize: Optional[Tuple[float, float]] = None,
-        dpi: Optional[int] = None,
-        save: Optional[Union[str, Path]] = None,
+        x_test: Optional[np.ndarray] = None,
+        key_added: Optional[str] = "_x_test",
         **kwargs: Any,
-    ) -> None:
+    ) -> np.ndarray:
+        """Run the prediction.
+
+        Parameters
+        ----------
+        x_test
+            Array of shape ``(n_samples,)`` used for prediction. If :obj:`None`, use :attr:`x_test`.
+        key_added
+            Attribute name where to save the :attr:`x_test` for later use. If :obj:`None`, don't save it.
+        kwargs
+            Keyword arguments for underlying :attr:`model`'s prediction method.
+
+        Returns
+        -------
+        Returns and updates the following fields:
+
+        - :attr:`y_test` - %(base_model_y_test.summary)s
         """
-        Plot random walks in an embedding.
 
-        This method simulates random walks on the Markov chain defined though the corresponding transition matrix. The
-        method is intended to give qualitative rather than quantitative insights into the transition matrix. Random
-        walks are simulated by iteratively choosing the next cell based on the current cell's transition probabilities.
+    @abc.abstractmethod
+    @d.get_sections(base="base_model_ci", sections=["Parameters", "Returns"])
+    @d.get_summary(base="base_model_ci")
+    @d.get_full_description(base="base_model_ci")
+    @d.dedent
+    def confidence_interval(self, x_test: Optional[np.ndarray] = None, **kwargs) -> np.ndarray:
+        """Calculate the confidence interval.
+
+        Use :meth:`default_confidence_interval` function if underlying :attr:`model` has no method
+        for confidence interval calculation.
 
         Parameters
         ----------
-        n_sims
-            Number of random walks to simulate.
-        %(rw_sim.parameters)s
-        start_ixs
-            Cells from which to sample the starting points. If `None`, use all cells.
-            %(rw_ixs)s
-            For example ``{'dpt_pseudotime': [0, 0.1]}`` means that starting points for random walks
-            will be sampled uniformly from cells whose pseudotime is in `[0, 0.1]`.
-        stop_ixs
-            Cells which when hit, the random walk is terminated. If `None`, terminate after ``max_iters``.
-            %(rw_ixs)s
-            For example ``{'clusters': ['Alpha', 'Beta']}`` and ``successive_hits = 3`` means that the random walk will
-            stop prematurely after cells in the above specified clusters have been visited successively 3 times in a
-            row.
-        basis
-            Basis in :attr:`anndata.AnnData.obsm` to use as an embedding.
-        cmap
-            Colormap for the random walk lines.
-        linewidth
-            Width of the random walk lines.
-        linealpha
-            Alpha value of the random walk lines.
-        ixs_legend_loc
-            Legend location for the start/top indices.
-        %(parallel)s
-        %(plotting)s
+        x_test
+            Array of shape ``(n_samples,)`` used for confidence interval calculation.
+            If :obj:`None`, use :attr:`x_test`.
         kwargs
-            Keyword arguments for :func:`scvelo.pl.scatter`.
+            Keyword arguments for underlying :attr:`model`'s confidence method
+            or for :meth:`default_confidence_interval`.
 
         Returns
         -------
-        %(just_plots)s
-        For each random walk, the first/last cell is marked by the start/end colors of ``cmap``.
-        """
+        Returns self and updates the following fields:
 
-        def create_ixs(ixs: Indices_t, *, kind: str) -> Optional[np.ndarray]:
-            if ixs is None:
-                return None
-            if isinstance(ixs, dict):
-                # fmt: off
-                if len(ixs) != 1:
-                    raise ValueError(f"Expected to find only 1 cluster key, found `{len(ixs)}`.")
-                key = next(iter(ixs.keys()))
-                if key not in self.adata.obs:
-                    raise KeyError(f"Unable to find data in `adata.obs[{key!r}]`.")
-
-                vals = self.adata.obs[key]
-                if is_categorical_dtype(vals):
-                    ixs = np.where(np.isin(vals, ixs[key]))[0]
-                elif is_numeric_dtype(vals):
-                    if len(ixs[key]) != 2:
-                        raise ValueError(f"Expected range to be of length `2`, found `{len(ixs[key])}`")
-                    minn, maxx = sorted(ixs[key])
-                    ixs = np.where((vals >= minn) & (vals <= maxx))[0]
-                else:
-                    raise TypeError(f"Expected `adata.obs[{key!r}]` to be numeric or categorical, "
-                                    f"found `{infer_dtype(vals)}`.")
-                # fmt: on
-            elif isinstance(ixs, str):
-                ixs = np.where(self.adata.obs_names == ixs)[0]
-            else:
-                ixs = np.where(np.isin(self.adata.obs_names, ixs))[0]
+        - :attr:`conf_int` - %(base_model_conf_int.summary)s
+        """
 
-            if not len(ixs):
-                logg.warning(f"No {kind} indices have been selected, using `None`")
-                return None
+    @d.dedent
+    def default_confidence_interval(
+        self,
+        x_test: Optional[np.ndarray] = None,
+        **kwargs: Any,
+    ) -> np.ndarray:
+        """Calculate the confidence interval, if the underlying :attr:`model` has no method for it.
 
-            return ixs
+        This formula is taken from :cite:`desalvo:70`, eq. 5.
 
-        if self._transition_matrix is None:
-            raise RuntimeError(
-                "Compute transition matrix first as `.compute_transition_matrix()`."
-            )
-        emb = _get_basis(self.adata, basis)
+        Parameters
+        ----------
+        %(base_model_ci.parameters)s
 
-        if isinstance(cmap, str):
-            cmap = plt.get_cmap(cmap)
-        if not isinstance(cmap, LinearSegmentedColormap):
-            if not hasattr(cmap, "colors"):
-                raise AttributeError(
-                    "Unable to create a colormap, `cmap` does not have attribute `colors`."
-                )
-            cmap = LinearSegmentedColormap.from_list(
-                "random_walk", colors=cmap.colors, N=max_iter
-            )
+        Returns
+        -------
+        %(base_model_ci.returns)s
 
-        start_ixs = create_ixs(start_ixs, kind="start")
-        stop_ixs = create_ixs(stop_ixs, kind="stop")
-        rw = RandomWalk(self.transition_matrix, start_ixs=start_ixs, stop_ixs=stop_ixs)
-        sims = rw.simulate_many(
-            n_sims=n_sims,
-            max_iter=max_iter,
-            seed=seed,
-            n_jobs=n_jobs,
-            backend=backend,
-            successive_hits=successive_hits,
-            show_progress_bar=show_progress_bar,
-        )
+        Also updates the following fields:
 
-        fig, ax = plt.subplots(figsize=figsize, dpi=dpi)
-        scv.pl.scatter(self.adata, basis=basis, show=False, ax=ax, **kwargs)
+        - :attr:`x_hat` - %(base_model_x_hat.summary)s
+        - :attr:`y_hat` - %(base_model_y_hat.summary)s
+        """
+        use_ixs = self.w > 0
+        x_hat = self.x[use_ixs]
+        if x_test is None:
+            x_test = self.x_test
 
-        logg.info("Plotting random walks")
-        for sim in sims:
-            x = emb[sim][:, 0]
-            y = emb[sim][:, 1]
-            points = np.array([x, y]).T.reshape(-1, 1, 2)
-            segments = np.concatenate([points[:-1], points[1:]], axis=1)
-            n_seg = len(segments)
-
-            lc = LineCollection(
-                segments,
-                linewidths=linewidth,
-                colors=[cmap(float(i) / n_seg) for i in range(n_seg)],
-                alpha=linealpha,
-                zorder=2,
-            )
-            ax.add_collection(lc)
+        self._y_hat = self.predict(x_hat, key_added="_x_hat", **kwargs)
+        self._y_test = self.predict(x_test, key_added="_x_test", **kwargs)
 
-        for ix in [0, -1]:
-            ixs = [sim[ix] for sim in sims]
-            plot_outline(
-                x=emb[ixs][:, 0],
-                y=emb[ixs][:, 1],
-                outline_color=("black", to_hex(cmap(float(abs(ix))))),
-                kwargs={
-                    "s": kwargs.get("s", default_size(self.adata)) * 1.1,
-                    "alpha": 0.9,
-                },
-                ax=ax,
-                zorder=4,
-            )
+        n = np.sum(use_ixs)
+        sigma_hat = np.sqrt(((self.y_hat - self.y[use_ixs].squeeze()) ** 2).sum() / (n - 2))
+        mean = np.mean(self.x)
 
-        if ixs_legend_loc not in (None, "none"):
-            from cellrank.pl._utils import _position_legend
+        # fmt: off
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", RuntimeWarning)
+            stds = sigma_hat * np.sqrt(1 + 1 / n + ((self.x_test - mean) ** 2) / ((self.x - mean) ** 2).sum())
+        # fmt: on
+        stds = np.squeeze(stds)
 
-            h1 = ax.scatter([], [], color=cmap(0.0), label="start")
-            h2 = ax.scatter([], [], color=cmap(1.0), label="stop")
-            legend = ax.get_legend()
-            if legend is not None:
-                ax.add_artist(legend)
-            _position_legend(ax, legend_loc=ixs_legend_loc, handles=[h1, h2])
+        self._conf_int = np.c_[self._y_test - stds / 2.0, self._y_test + stds / 2.0]
 
-        if save is not None:
-            save_fig(fig, save)
+        return self.conf_int
 
-    @d.get_full_description(base="plot_single_flow")
-    @d.get_sections(base="plot_single_flow", sections=["Parameters", "Returns"])
     @d.dedent
-    def plot_single_flow(
+    def plot(
         self,
-        cluster: str,
-        cluster_key: str,
-        time_key: str,
-        clusters: Optional[Sequence[Any]] = None,
-        time_points: Optional[Sequence[Union[int, float]]] = None,
-        min_flow: float = 0,
-        remove_empty_clusters: bool = True,
-        ascending: Optional[bool] = False,
-        legend_loc: Optional[str] = "upper right out",
-        alpha: Optional[float] = 0.8,
-        xticks_step_size: Optional[int] = 1,
-        figsize: Optional[Tuple[float, float]] = None,
-        dpi: Optional[int] = None,
-        save: Optional[Union[str, Path]] = None,
-        show: bool = True,
-    ) -> Optional[plt.Axes]:
-        """
-        Visualize outgoing flow from a cluster of cells :cite:`mittnenzweig:21`.
+        figsize: Tuple[float, float] = (8, 5),
+        same_plot: bool = False,
+        hide_cells: bool = False,
+        perc: Tuple[float, float] = None,
+        fate_prob_cmap: colors.ListedColormap = cm.viridis,
+        cell_color: Optional[str] = None,
+        lineage_color: str = "black",
+        alpha: float = 0.8,
+        lineage_alpha: float = 0.2,
+        title: Optional[str] = None,
+        size: int = 15,
+        lw: float = 2,
+        cbar: bool = True,
+        margins: float = 0.015,
+        xlabel: str = "pseudotime",
+        ylabel: str = "expression",
+        conf_int: bool = True,
+        lineage_probability: bool = False,
+        lineage_probability_conf_int: Union[bool, float] = False,
+        lineage_probability_color: Optional[str] = None,
+        obs_legend_loc: Optional[str] = "best",
+        dpi: int = None,
+        fig: mpl.figure.Figure = None,
+        ax: mpl.axes.Axes = None,
+        return_fig: bool = False,
+        save: Optional[str] = None,
+        **kwargs: Any,
+    ) -> Optional[mpl.figure.Figure]:
+        """Plot the smoothed gene expression.
 
         Parameters
         ----------
-        cluster
-            Cluster for which to visualize outgoing flow.
-        cluster_key
-            Key in :attr:`anndata.AnnData.obs` where clustering is stored.
-        time_key
-            Key in :attr:`anndata.AnnData.obs` where experimental time is stored.
-        clusters
-            Visualize flow only for these clusters. If `None`, use all clusters.
-        time_points
-            Visualize flow only for these time points. If `None`, use all time points.
-        %(flow.parameters)s
-        %(plotting)s
-        show
-            If `False`, return :class:`matplotlib.pyplot.Axes`.
+        figsize
+            Size of the figure.
+        same_plot
+            Whether to plot all trends in the same plot.
+        hide_cells
+            Whether to hide the cells.
+        perc
+            Percentile by which to clip the fate probabilities.
+        fate_prob_cmap
+            Colormap to use when coloring in the fate probabilities.
+        cell_color
+            Key in :attr:`~anndata.AnnData.obs` or :attr:`~anndata.AnnData.var_names` used for coloring the cells.
+        lineage_color
+            Color for the lineage.
+        alpha
+            Alpha value in :math:`[0, 1]` for the transparency of cells.
+        lineage_alpha
+            Alpha value in :math:`[0, 1]` for the transparency lineage confidence intervals.
+        title
+            Title of the plot.
+        size
+            Size of the points.
+        lw
+            Line width for the smoothed values.
+        cbar
+            Whether to show the colorbar.
+        margins
+            Margins around the plot.
+        xlabel
+            Label on the x-axis.
+        ylabel
+            Label on the y-axis.
+        conf_int
+            Whether to show the confidence interval.
+        lineage_probability
+            Whether to show smoothed lineage probability as a dashed line.
+            Note that this will require 1 additional model fit.
+        lineage_probability_conf_int
+            Whether to compute and show smoothed lineage probability confidence interval.
+        lineage_probability_color
+            Color to use when plotting the smoothed ``lineage_probability``.
+            If :obj:`None`, it's the same as ``lineage_color``. Only used when ``show_lineage_probability = True``.
+        obs_legend_loc
+            Location of the legend when ``cell_color`` corresponds to a categorical variable.
+        dpi
+            Dots per inch.
+        fig
+            Figure to use. If :obj:`None`, create a new one.
+        ax
+            Ax to use. If :obj:`None`, create a new one.
+        return_fig
+            If :obj:`True`, return the figure object.
+        save
+            Filename where to save the plot. If :obj:`None`, just shows the plots.
+        kwargs
+            Keyword arguments for :meth:`~matplotlib.axes.Axes.legend`.
 
         Returns
         -------
-        The axes object, if ``show = False``.
         %(just_plots)s
+        """
+        if self.y_test is None:
+            raise RuntimeError("Run `.predict()` first.")
 
-        Notes
-        -----
-        This function is a Python reimplementation of the following
-        `original R function <https://github.com/tanaylab/embflow/blob/main/scripts/generate_paper_figures/plot_vein.r>`_
-        with some minor stylistic differences.
-        This function will not recreate the results from :cite:`mittnenzweig:21`, because there, the Metacell model
-        :cite:`baran:19` was used to compute the flow, whereas here the transition matrix is used.
-        """  # noqa: E501
-        if self._transition_matrix is None:
-            raise RuntimeError(
-                "Compute transition matrix first as `.compute_transition_matrix()`."
-            )
+        if fig is None or ax is None:
+            fig, ax = plt.subplots(figsize=figsize, constrained_layout=True)
 
-        fp = FlowPlotter(self.adata, self.transition_matrix, cluster_key, time_key)
-        fp = fp.prepare(cluster, clusters, time_points)
+        if dpi is not None:
+            fig.set_dpi(dpi)
 
-        ax = fp.plot(
-            min_flow=min_flow,
-            remove_empty_clusters=remove_empty_clusters,
-            ascending=ascending,
-            alpha=alpha,
-            xticks_step_size=xticks_step_size,
-            legend_loc=legend_loc,
-            figsize=figsize,
-            dpi=dpi,
+        conf_int = conf_int and self.conf_int is not None
+        hide_cells = hide_cells or self.x_all is None or self.w_all is None or self.y_all is None
+
+        lineage_probability_color = lineage_color if lineage_probability_color is None else lineage_probability_color
+
+        scaler = kwargs.pop(
+            "scaler",
+            self._create_scaler(
+                lineage_probability,
+                show_conf_int=conf_int,
+            ),
         )
 
-        if save is not None:
-            save_fig(ax.figure, save)
+        if lineage_probability and ylabel in ("expression", self._gene):
+            ylabel = f"scaled {ylabel}"
 
-        if not show:
-            return ax
+        vmin, vmax = None, None
+        key, color, typp, mapper = self._get_colors(cell_color, same_plot=same_plot)
 
-    def __xor__(self, other: "KernelExpression") -> "KernelExpression":
-        return self.__rxor__(other)
-
-    def __rxor__(self, other: "KernelExpression") -> "KernelExpression":
-        def convert(obj):
-            if _is_adaptive_type(obj):
-                if obj._mat_scaler is None:
-                    raise ValueError(_ERROR_VAR_NOT_FOUND.format(obj))
-                return KernelMul(
-                    [
-                        ConstantMatrix(
-                            obj.adata, 1, obj._mat_scaler, backward=obj.backward
-                        ),
-                        obj,
-                    ]
-                )
-            if _is_adaptive_type(_is_bin_mult(obj, return_constant=False)):
-                e, c = _get_expr_and_constant(obj)
-                if e._mat_scaler is None:
-                    raise ValueError(_ERROR_VAR_NOT_FOUND.format(e))
-                return KernelMul(
-                    [ConstantMatrix(e.adata, c, e._mat_scaler, backward=e.backward), e]
+        if not hide_cells:
+            cbar = cbar and (typp == ColorType.CONT)
+            if typp == ColorType.CONT:
+                vmin, vmax = _minmax(color, perc)
+
+            _ = ax.scatter(
+                self.x_all.squeeze(),
+                scaler(self.y_all.squeeze()),
+                c=color,
+                s=size,
+                cmap=fate_prob_cmap,
+                vmin=vmin,
+                vmax=vmax,
+                alpha=alpha,
+            )
+
+        if title is None:
+            title = f"{self._gene} @ {self._lineage}" if self._lineage is not None else f"{self._gene}"
+
+        ax.plot(self.x_test, scaler(self.y_test), color=lineage_color, lw=lw, label=title)
+
+        if title is not None:
+            ax.set_title(title)
+        if ylabel is not None:
+            ax.set_ylabel(ylabel)
+        if xlabel is not None:
+            ax.set_xlabel(xlabel)
+
+        ax.margins(margins)
+
+        if conf_int:
+            ax.fill_between(
+                self.x_test.squeeze(),
+                scaler(self.conf_int[:, 0]),
+                scaler(self.conf_int[:, 1]),
+                alpha=lineage_alpha,
+                color=lineage_color,
+                linestyle="--",
+            )
+
+        if lineage_probability and not isinstance(self, FittedModel) and not np.allclose(self.w, 1.0):
+            from cellrank.pl._utils import _is_any_gam_mgcv
+
+            model = copy.deepcopy(self)
+            model._y = self._reshape_and_retype(self.w).copy()
+            model = model.fit()
+
+            if not lineage_probability_conf_int:
+                y = model.predict()
+            elif _is_any_gam_mgcv(model):
+                y = model.predict(
+                    level=lineage_probability_conf_int if isinstance(lineage_probability_conf_int, float) else 0.95
                 )
+            else:
+                y = model.predict()
+                model.confidence_interval()
 
-            return obj
-
-        if (
-            not _is_adaptive_type(self)
-            and not isinstance(self, KernelAdaptiveAdd)
-            and not _is_adaptive_type(_is_bin_mult(self, return_constant=False))
-        ):
-            raise TypeError(_ERROR_CONF_ADAPT.format(self.__class__.__name__))
-        if (
-            not _is_adaptive_type(other)
-            and not isinstance(other, KernelAdaptiveAdd)
-            and not _is_adaptive_type(_is_bin_mult(other, return_constant=False))
-        ):
-            raise TypeError(_ERROR_CONF_ADAPT.format(other.__class__.__name__))
-
-        s = convert(self)
-        o = convert(other)
-
-        if isinstance(s, KernelAdaptiveAdd):
-            exprs = list(s) + (list(o) if isinstance(o, KernelAdaptiveAdd) else [o])
-            # (c1 * x + c2 * y + ...) + (c3 * z) => (c1 * x + c2 * y + c3 + ... + * z)
-            if all(_is_bin_mult(k, ConstantMatrix) for k in exprs):
-                return KernelAdaptiveAdd(exprs)
-
-        # same but reverse
-        if isinstance(o, KernelAdaptiveAdd):
-            exprs = (list(s) if isinstance(s, KernelAdaptiveAdd) else [s]) + list(o)
-            if all(_is_bin_mult(k, ConstantMatrix) for k in exprs):
-                return KernelAdaptiveAdd(exprs)
-
-        return KernelAdaptiveAdd([s, o])
-
-    def __add__(self, other: "KernelExpression") -> "KernelExpression":
-        return self.__radd__(other)
-
-    def __radd__(self, other: "KernelExpression") -> "KernelExpression":
-        if not isinstance(other, KernelExpression):
-            raise TypeError(
-                f"Expected type `KernelExpression`, found `{other.__class__.__name__}`."
-            )
-
-        s = self * 1 if isinstance(self, Kernel) else self
-        o = other * 1 if isinstance(other, Kernel) else other
-
-        if isinstance(s, KernelSimpleAdd):
-            exprs = list(s) + [o]
-            # (c1 * x + c2 * y + ...) + (c3 * z) => (c1 * x + c2 * y + c3 + ... + * z)
-            if all(_is_bin_mult(k) for k in exprs):
-                return KernelSimpleAdd(exprs)
-
-        # same but reverse
-        if isinstance(o, KernelSimpleAdd):
-            exprs = [s] + list(o)
-            if all(_is_bin_mult(k) for k in exprs):
-                return KernelSimpleAdd(exprs)
-
-        # (c1 + c2) => c3
-        if isinstance(s, Constant) and isinstance(o, Constant):
-            assert s.backward == o.backward, _ERROR_DIRECTION_MSG
-            return Constant(
-                s.adata, s.transition_matrix + o.transition_matrix, backward=s.backward
-            )
-
-        ss = s * 1 if not isinstance(s, KernelMul) else s
-        oo = o * 1 if not isinstance(o, KernelMul) else o
+                ax.fill_between(
+                    model.x_test.squeeze(),
+                    model.conf_int[:, 0],
+                    model.conf_int[:, 1],
+                    alpha=lineage_alpha,
+                    color=lineage_probability_color,
+                    linestyle="--",
+                )
 
-        return KernelSimpleAdd([ss, oo])
+            handle = ax.plot(
+                model.x_test,
+                y,
+                color=lineage_probability_color,
+                lw=lw,
+                linestyle="--",
+                zorder=-1,
+                label="probability",
+            )
+
+            self._maybe_add_legend(fig, ax, mapper=handle, title=None, **kwargs)
+
+        if cbar and not hide_cells and not same_plot and not np.allclose(self.w_all, 1.0):
+            norm = colors.Normalize(vmin=vmin, vmax=vmax)
+            divider = make_axes_locatable(ax)
+            cax = divider.append_axes("right", size="2%", pad=0.1)
+            _ = mpl.colorbar.ColorbarBase(
+                cax,
+                norm=norm,
+                cmap=fate_prob_cmap,
+                ticks=np.linspace(norm.vmin, norm.vmax, 5),
+            )
+            cax.set_ylabel(key)
+        elif typp == ColorType.CAT:
+            self._maybe_add_legend(fig, ax, mapper, title=key, loc=obs_legend_loc, is_line=False)
 
-    def __rmul__(
-        self, other: Union[int, float, "KernelExpression"]
-    ) -> "KernelExpression":
-        return self.__mul__(other)
+        if save is not None:
+            save_fig(fig, save)
 
-    def __mul__(
-        self, other: Union[float, int, "KernelExpression"]
-    ) -> "KernelExpression":
+        if return_fig:
+            return fig
 
-        if isinstance(other, (int, float)):
-            other = Constant(self.adata, other, backward=self.backward)
+    def _maybe_add_legend(
+        self,
+        fig: mpl.figure.Figure,
+        ax: mpl.axes.Axes,
+        mapper: Union[Sequence[Any], Mapping[str, Any]],
+        title: Optional[str] = None,
+        loc: Optional[str] = "best",
+        is_line: bool = True,
+        **kwargs: Any,
+    ) -> None:
+        from cellrank.pl._utils import _position_legend
 
-        if not isinstance(other, KernelExpression):
-            raise TypeError(
-                f"Expected type `KernelExpression`, found `{other.__class__.__name__}`."
-            )
+        if loc in ("none", None):
+            return
 
-        # (c1 * c2) => c3
-        if isinstance(self, Constant) and isinstance(
-            other, Constant
-        ):  # small optimization
-            assert self.backward == other.backward, _ERROR_DIRECTION_MSG
-            return Constant(
-                self.adata,
-                self.transition_matrix * other.transition_matrix,
-                backward=self.backward,
-            )
+        if isinstance(mapper, dict):
+            handles = [
+                ax.plot([], [], label=name, color=color)[0] if is_line else ax.scatter([], [], label=name, color=color)
+                for name, color in mapper.items()
+            ]
+        else:
+            handles = mapper
 
-        s = (
-            self
-            if isinstance(self, (KernelMul, Constant))
-            else KernelMul([Constant(self.adata, 1, backward=self.backward), self])
-        )
-        o = (
-            other
-            if isinstance(other, (KernelMul, Constant))
-            else KernelMul([Constant(other.adata, 1, backward=other.backward), other])
+        legend = _position_legend(
+            ax,
+            legend_loc=loc,
+            handles=handles,
+            title=title,
+            **kwargs,
         )
+        fig.add_artist(legend)
 
-        cs, co = _is_bin_mult(s), _is_bin_mult(o)
-        if cs and isinstance(o, Constant):
-            cs._transition_matrix *= o.transition_matrix
-            return s
-
-        if co and isinstance(s, Constant):
-            co._transition_matrix *= s.transition_matrix
-            return o
-
-        return KernelMul([s, o])
-
-    def __invert__(self: "KernelExpression") -> "KernelExpression":
-        # mustn't return a copy because transition matrix
-        self._transition_matrix = None
-        self._params = {}
-        self._backward = not self.backward
-
-        return self
-
-    def __copy__(self) -> "KernelExpression":
-        return self.copy()
-
-    def __deepcopy__(self, memodict={}) -> "KernelExpression":  # noqa
-        res = self.copy()
-        if self._parent is None:
-            res.adata = self.adata.copy()
-        memodict[id(self)] = res
-
-        return res
+    def _reshape_and_retype(self, arr: np.ndarray) -> np.ndarray:
+        """Convert 1D or 2D array to 2D array of shape ``(n, 1)`` and set the data type.
 
-
-class UnaryKernelExpression(KernelExpression, ABC):
-    """Base class for unary kernel expressions, such as kernels or constants."""
-
-    def __init__(
-        self,
-        adata,
-        backward: bool = False,
-        op_name: Optional[str] = None,
-        compute_cond_num: bool = False,
-        **kwargs,
-    ):
-        super().__init__(op_name, backward=backward, compute_cond_num=compute_cond_num)
-        assert (
-            op_name is None
-        ), "Unary kernel does not support any kind operation associated with it."
-        self._adata = adata
-        self._n_obs = adata.n_obs
-
-    @property
-    @d.dedent
-    def adata(self) -> AnnData:
-        """
-        Annotated data object.
+        Parameters
+        ----------
+        arr
+            Array to convert.
 
         Returns
         -------
-        %(adata_ret)s
+        Array of shape ``(n, 1)`` with dtype set to :attr:`_dtype`.
         """
-        return self._adata
-
-    @property
-    def shape(self) -> Tuple[int, int]:
-        """`(n_cells, n_cells)`."""
-        return self._n_obs, self._n_obs
-
-    @adata.setter
-    def adata(self, adata: Optional[AnnData]) -> None:
-        if adata is None:
-            self._adata = None
-            return
-        if not isinstance(adata, AnnData):
-            raise TypeError(
-                f"Expected argument of type `anndata.AnnData`, found `{type(adata).__name__!r}`."
-            )
-        shape = (adata.n_obs, adata.n_obs)
-        if self.shape != shape:
-            raise ValueError(
-                f"Expected the new object to have same shape as previous object `{self.shape}`, "
-                f"found `{shape}`."
-            )
-        self._adata = adata
-
-    def __repr__(self):
-        return f"{'~' if self.backward and self._parent is None else ''}<{self.__class__.__name__}>"
-
-    def __str__(self):
-        params_fmt = self._format_params()
-        if params_fmt:
-            return (
-                f"{'~' if self.backward and self._parent is None else ''}"
-                f"<{self.__class__.__name__}[{params_fmt}]>"
-            )
-        return repr(self)
-
+        if arr.ndim not in (1, 2):
+            raise ValueError(f"Expected array to be 1 or 2 dimensional, found `{arr.ndim}` dimension(s).")
+        if arr.ndim == 2 and arr.shape[1] != 1:
+            raise ValueError(f"Expected the 2nd dimension to be 1, found `{arr.shape[1]}.`")
 
-class NaryKernelExpression(KernelExpression, ABC):
-    """Base class for n-ary kernel expressions."""
+        return np.reshape(arr, (-1, 1)).astype(self._dtype)
 
-    def __init__(self, kexprs: List[KernelExpression], op_name: Optional[str] = None):
-        assert len(kexprs), "No kernel expressions specified."
+    def _check(self, attr_name: Optional[str], arr: Optional[np.ndarray], ndim: int = 2) -> Optional[np.ndarray]:
+        """Check if the attribute exists with the correct dimension and optionally set it.
 
-        backward = kexprs[0].backward
-        assert all(k.backward == backward for k in kexprs), _ERROR_DIRECTION_MSG
-
-        # use OR instead of AND
-        super().__init__(
-            op_name,
-            backward=backward,
-            compute_cond_num=any(k._compute_cond_num for k in kexprs),
-        )
-
-        # copies of constants are necessary because of the recalculation
-        self._kexprs = [copy(k) if isinstance(k, Constant) else k for k in kexprs]
-
-        for kexprs in self._kexprs:
-            kexprs._parent = self
-
-    @property
-    def shape(self) -> Tuple[int, int]:
-        """`(n_cells, n_cells)`."""
-        return self.kernels[0].shape
-
-    def _maybe_recalculate_constants(self, type_: Type):
-        if type_ == Constant:
-            accessor = "transition_matrix"
-        elif type_ == ConstantMatrix:
-            accessor = "_value"
-        else:
-            raise RuntimeError(
-                f"Unable to determine accessor for type `{type(type_).__name__}`."
-            )
-
-        constants = [_is_bin_mult(k, type_) for k in self]
-        if all(c is not None for c in constants):
-            assert all(
-                isinstance(getattr(c, accessor), (int, float)) for c in constants
-            )
-            total = sum(getattr(c, accessor) for c in constants) + 0.0
-            for c in constants:
-                c._recalculate(getattr(c, accessor) / total)
-
-            for kexpr in self._kexprs:  # don't normalize  (c * x)
-                kexpr._normalize = False
-
-    def _get_kernels(self) -> Iterable["Kernel"]:
-        for k in self:
-            if isinstance(k, Kernel) and not isinstance(k, (Constant, ConstantMatrix)):
-                yield k
-            elif isinstance(k, NaryKernelExpression):
-                yield from k._get_kernels()
-
-    @property
-    @d.dedent
-    def adata(self) -> AnnData:
-        """
-        Annotated data object.
+        Parameters
+        ----------
+        attr_name
+            Attribute name to check.
+        arr
+            Value to set. If :obj:`None`, just perform the checking.
+        ndim
+            Expected number of dimensions of the ``arr``.
 
         Returns
         -------
-        %(adata_ret)s
+        The attribute under ``attr_name``.
         """
-        # we can do this because Constant requires adata as well
-        return self._kexprs[0].adata
-
-    @adata.setter
-    def adata(self, adata: Optional[AnnData]) -> None:
-        for kexpr in self._kexprs:
-            kexpr.adata = adata
-
-    def __invert__(self) -> "NaryKernelExpression":
-        super().__invert__()
-        self._kexprs = [~kexpr for kexpr in self]
-        return self
+        if attr_name is None:
+            return
+        if arr is None:  # already called prepare
+            if not hasattr(self, attr_name):
+                raise AttributeError(f"No attribute `{attr_name!r}` found.")
+            if not isinstance(getattr(self, attr_name, None), np.ndarray):
+                raise AttributeError(
+                    f"Expected `{attr_name!r}` to be `numpy.ndarray`, "
+                    f"found `{type(getattr(self, attr_name, None)).__name__!r}`."
+                )
+            if getattr(self, attr_name).ndim != ndim:
+                raise ValueError(
+                    f"Expected attribute `{attr_name!r}` to have `{ndim}` dimensions, "
+                    f"found `{getattr(self, attr_name).ndim}` dimensions."
+                )
+            return getattr(self, attr_name)
 
-    def __len__(self) -> int:
-        return len(self._kexprs)
+        setattr(self, attr_name, self._reshape_and_retype(arr))
+        if attr_name.startswith("_"):
+            try:
+                getattr(self, attr_name[1:])
+            except AttributeError:
+                setattr(
+                    self,
+                    attr_name[1:],
+                    property(lambda self: getattr(self, attr_name)),
+                )
+        return getattr(self, attr_name)
 
-    def __getitem__(self, item) -> "KernelExpression":
-        return self._kexprs[item]
+    def _deepcopy_attributes(self, dst: "BaseModel") -> None:
+        # __deepcopy__ will usually call `_shallowcopy_attributes` twice, since it calls `.copy()`,
+        # which should always call it (it copies the lineage and gene names + deepcopies the model)
+
+        self._shallowcopy_attributes(dst)
+        for attr in [
+            "_x_all",
+            "_y_all",
+            "_w_all",
+            "_x",
+            "_y",
+            "_w",
+            "_x_test",
+            "_y_test",
+            "_x_hat",
+            "_y_hat",
+            "_conf_int",
+            "_prepared",
+        ]:
+            setattr(dst, attr, copy.copy(getattr(self, attr)))
+
+    def _shallowcopy_attributes(self, dst: "BaseModel") -> None:
+        for attr in ["_gene", "_lineage", "_use_raw", "_data_key", "_is_bulk"]:
+            setattr(dst, attr, copy.copy(getattr(self, attr)))
+        # user is not exposed to this
+        dst._obs_names = self._obs_names
+        # always deepcopy the model (we're manipulating it in multiple threads/processed)
+        dst._model = copy.deepcopy(self.model)
 
-    def __repr__(self) -> str:
-        return (
-            f"{'~' if self.backward and self._parent is None else ''}("
-            + f" {self._op_name} ".join(repr(kexpr) for kexpr in self._kexprs)
-            + ")"
-        )
+    @abc.abstractmethod
+    @d.dedent
+    def copy(self) -> "BaseModel":
+        """%(copy)s"""  # noqa
 
-    def __str__(self) -> str:
-        return (
-            f"{'~' if self.backward and self._parent is None else ''}("
-            + f" {self._op_name} ".join(str(kexpr) for kexpr in self._kexprs)
-            + ")"
-        )
+    def __copy__(self) -> "BaseModel":
+        return self.copy()
 
+    def __deepcopy__(self, memodict={}) -> "BaseModel":  # noqa
+        # deepcopy expects that `.copy()` makes a really shallow copy (i.e. only references to the arrays)
+        # it should also not copy the `.prepared` attribute, since copying is happening mostly during
+        # parallelization and it serves as 1 extra sanity check (a precaution that's not necessary, per-se, but highly
+        # desirable)
+        res = self.copy()
+        # we don't copy the adata object for 2 reasons:
+        # 1. these objects are meant to be as lightweight as possible
+        # 2. in `.plot`, we deepcopy the model when plotting smoothed probabilities
+        self._deepcopy_attributes(res)
+        memodict[id(self)] = res
 
-@d.dedent
-class Kernel(UnaryKernelExpression, ABC):
-    """
-    A base class from which all kernels are derived.
+        return res
 
-    These kernels read from a given AnnData object, usually the KNN graph and additional variables, to compute a
-    weighted, directed graph. Every kernel object has a direction. The kernels defined in the derived classes are not
-    strictly kernels in the mathematical sense because they often only take one input argument - however, they build
-    on other functions which have computed a similarity based on two input arguments. The role of the kernels defined
-    here is to add directionality to these symmetric similarity relations or to transform them.
+    def __bool__(self):
+        return True
 
-    Parameters
-    ----------
-    %(adata)s
-    %(backward)s
-    %(cond_num)s
-    check_connectivity
-        Check whether the underlying KNN graph is connected.
-    kwargs
-        Keyword arguments which can specify key to be read from :attr:`adata` object.
-    """
+    def __str__(self) -> str:
+        return repr(self)
 
-    def __init__(
-        self,
-        adata: AnnData,
-        backward: bool = False,
-        compute_cond_num: bool = False,
-        check_connectivity: bool = False,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            adata, backward, op_name=None, compute_cond_num=compute_cond_num, **kwargs
+    def __repr__(self) -> str:
+        return "<{}[gene={!r}, lineage={!r}, model={}]>".format(
+            self.__class__.__name__,
+            self._gene,
+            self._lineage,
+            None if self.model is None else _dup_spaces.sub(" ", str(self.model).replace("\n", " ")).strip(),
         )
-        self._read_from_adata(check_connectivity=check_connectivity, **kwargs)
 
-    # TODO: move to a mixin class
-    def _read_from_adata(
+    def _get_colors(
         self,
-        conn_key: Optional[str] = "connectivities",
-        read_conn: bool = True,
-        **kwargs: Any,
-    ) -> None:
+        key: Optional[str],
+        *,
+        same_plot: bool = False,
+    ) -> Tuple[Optional[str], Optional[Union[str, np.ndarray]], ColorType, Optional[Dict[str, Any]],]:
         """
-        Import the base-KNN graph and optionally check for symmetry and connectivity.
+        Get color array.
 
         Parameters
         ----------
-        conn_key
-            Key in :attr:`anndata.AnnData.uns` where connectivities are stored.
-        read_conn
-            Whether to read connectivities or set them to `None`. Useful when not exposing density normalization or
-            when KNN connectivities are not used to compute the transition matrix.
-        kwargs
-            Additional keyword arguments.
+        key
+            Key in :attr:`~anndata.AnnData.obs`, :attr:`~anndata.AnnData.var_names` or
+            :attr:`~anndata.AnnData.raw.var_names`. Search first starts in `.obs`, then `.raw.var_names` and lastly
+            `.layers`, using :meth:`~anndata.AnnData.obs_vector`.
 
         Returns
         -------
-        Nothing, just sets :attr:`_conn`.
-        """
-        if not read_conn:
-            self._conn = None
-            return
+        Triple of the following:
 
-        self._conn = _get_neighs(
-            self.adata, mode="connectivities", key=conn_key
-        ).astype(_dtype)
-
-        check_connectivity = kwargs.pop("check_connectivity", False)
-        if check_connectivity:
-            start = logg.debug("Checking the KNN graph for connectedness")
-            if not _connected(self._conn):
-                logg.warning("KNN graph is not connected", time=start)
-            else:
-                logg.debug("KNN graph is connected", time=start)
+        - name of the colorbar label.
+        - array of values to map.
+        - type of the color.
+        - color mapper for categorical colors.
+        """
+        if colors.is_color_like(key):
+            return None, key, ColorType.STR, None
+
+        if key in self.adata.obs:
+            if is_categorical_dtype(self.adata.obs[key]):
+                add_colors_for_categorical_sample_annotation(
+                    self.adata,
+                    key=key,
+                    force_update_colors=False,
+                    palette=None,
+                )
+                col_dict = collections.defaultdict(
+                    lambda: colors.to_rgb("grey"),
+                    zip(
+                        self.adata.obs[key].cat.categories,
+                        [colors.to_rgb(i) for i in self.adata.uns[f"{key}_colors"]],
+                    ),
+                )
+                return (
+                    key,
+                    np.array([col_dict[v] for v in self.adata.obs[key]]),
+                    ColorType.CAT,
+                    col_dict,
+                )
 
-        start = logg.debug("Checking the KNN graph for symmetry")
-        if not _symmetric(self._conn):
-            logg.warning("KNN graph is not symmetric", time=start)
-        else:
-            logg.debug("KNN graph is symmetric", time=start)
+            if is_numeric_dtype(self.adata.obs[key]):
+                return key, self.adata.obs[key].values, ColorType.CONT, None
 
-    def _density_normalize(
-        self, other: Union[np.ndarray, spmatrix]
-    ) -> Union[np.ndarray, spmatrix]:
-        """
-        Density normalization by the underlying KNN graph.
+            logg.debug(f"Unable to interpret cell color from type `{infer_dtype(self.adata.obs[key])}`")
+            return None, "black", ColorType.STR, None
 
-        Parameters
-        ----------
-        other
-            Matrix to normalize.
-
-        Returns
-        -------
-        :class:`np.ndarray` or :class:`scipy.sparse.spmatrix`
-            Density normalized transition matrix.
+        if self._use_raw and key in self.adata.raw.var_names:
+            return (
+                key,
+                _densify_squeeze(self.adata.raw[:, key], np.float64),
+                ColorType.CONT,
+                None,
+            )
 
-        Raises
-        ------
-        ValueError
-            If KNN connectivities are not set.
-        """
-        if self._conn is None:
-            raise ValueError(
-                "Unable to density normalize the transition matrix "
-                "because KNN connectivities are not set."
+        try:
+            # can in principle return data from `.obs`, in which case it's mostly invalid
+            return (
+                key,
+                self.adata.obs_vector(key, layer=self._data_key),
+                ColorType.CONT,
+                None,
+            )
+        except KeyError:
+            logg.debug(
+                f"Key `{key!r}` not found in `adata.obs` or "
+                f"`adata{'.raw' if self._use_raw else ''}.var_names`. Ignoring`"
             )
 
-        logg.debug("Density-normalizing the transition matrix")
+        if same_plot or np.allclose(self.w_all, 1.0):
+            return None, "black", ColorType.STR, None
 
-        q = np.asarray(self._conn.sum(axis=0))
-        Q = spdiags(1.0 / q, 0, other.shape[0], other.shape[0])
+        return "fate probability", np.squeeze(self.w_all), ColorType.CONT, None
 
-        return Q @ other @ Q
+    def _create_scaler(self, show_lineage_probability: bool, show_conf_int: bool):
+        if not show_lineage_probability:
+            return lambda _: _
 
-    def _get_kernels(self) -> Iterable["Kernel"]:
-        yield self
+        minn, maxx = self._return_min_max(show_conf_int)
+        return lambda x: (x - minn) / (maxx - minn)
 
-    def _compute_transition_matrix(
-        self,
-        matrix: Union[np.ndarray, spmatrix],
-        density_normalize: bool = True,
-        check_irreducibility: bool = False,
-    ):
-        if matrix.shape[0] != matrix.shape[1]:
-            raise ValueError(f"Expected a square matrix, found `{matrix.shape}`.")
-        if matrix.shape[0] != self.adata.n_obs:
-            raise ValueError(
-                f"Expected matrix to be of shape `{(self.adata.n_obs, self.adata.n_obs)}`, "
-                f"found `{matrix.shape}`."
-            )
+    def _return_min_max(self, show_conf_int: bool):
+        if self.y_test is None:
+            raise RuntimeError("Run `.predict()` first.")
 
-        matrix = matrix.astype(_dtype)
-        if issparse(matrix) and not isspmatrix_csr(matrix):
-            matrix = csr_matrix(matrix)
-
-        # density correction based on node degrees in the KNN graph
-        if density_normalize:
-            matrix = self._density_normalize(matrix)
-
-        # check for zero-rows
-        problematic_indices = np.where(np.array(matrix.sum(1)).flatten() == 0)[0]
-        if len(problematic_indices):
-            logg.warning(
-                f"Detected `{len(problematic_indices)}` absorbing states in the transition matrix. "
-                f"This matrix won't be irreducible"
-            )
-            matrix[problematic_indices, problematic_indices] = 1.0
+        vals = [self.y_test]
+        # FittedModel Does not need to have these
+        if self.y_all is not None:
+            vals.append(self.y_all)
+        if show_conf_int and self.conf_int is not None:
+            vals.append(self.conf_int)
 
-        if check_irreducibility:
-            _irreducible(matrix)
+        minn = min(map(np.min, vals))
+        maxx = max(map(np.max, vals))
 
-        # setting this property automatically row-normalizes
-        self.transition_matrix = matrix
-        self._maybe_compute_cond_num()
+        return minn, maxx
 
 
-@d.dedent
-class Constant(Kernel):
-    """
-    Kernel representing a multiplication by a constant number.
+class FailedModel(BaseModel):
+    """Model representing a failure of the original :attr:`model`.
 
     Parameters
     ----------
-    %(adata)s
-    value
-        Constant value by which to multiply. Must be a positive number.
-    %(backward)s
+    model
+        The original model which has failed.
+    exc
+        The exception that caused the :attr:`model` to fail or a :class:`str` containing the message.
+        In the latter case, :meth:`~cellrank.models.FailedModel.reraise` a :class:`RuntimeError` with that message.
+        If :obj:`None`, :class`UnknownModelError` will eventually be raised.
     """
 
-    def __init__(
-        self, adata: AnnData, value: Union[int, float], backward: bool = False
-    ):
-        super().__init__(adata, backward=backward)
-        if not isinstance(value, (int, float)):
-            raise TypeError(
-                f"Value must be a `float` or `int`, found `{type(value).__name__}`."
-            )
-        if value <= 0:
-            raise ValueError(f"Expected the constant to be positive, found `{value}`.")
-        self._recalculate(value)
-
-    def _recalculate(self, value) -> None:
-        self._transition_matrix = value
-        self._params = {"value": value}
-
-    def _read_from_adata(self, **kwargs: Any) -> None:
-        pass
-
-    def compute_transition_matrix(self, *args, **kwargs) -> "Constant":
-        """Return self."""
-        return self
-
-    @d.dedent
-    def copy(self) -> "Constant":
-        """%(copy)s"""  # noqa: D400, D401
-        return Constant(self.adata, self.transition_matrix, self.backward)
-
-    def __invert__(self) -> "Constant":
-        # do not call parent's invert, since it removes the transition matrix
-        self._backward = not self.backward
-        return self
-
-    def __repr__(self) -> str:
-        return repr(round(self.transition_matrix, _n_dec))
+    # in a functional programming language like Haskell essentially BaseModel would be a Maybe monad and this Nothing
+    def __init__(self, model: BaseModel, exc: Optional[Union[BaseException, str]] = None):
+        if not isinstance(model, BaseModel):
+            raise TypeError(f"Expected `model` to be of type `BaseModel`, found `{type(model).__name__!r}`.")
+        if exc is not None:
+            if isinstance(exc, str):
+                exc = RuntimeError(exc)
+            if not isinstance(exc, BaseException):
+                raise TypeError(
+                    f"Expected `exc` to be either a string or a `BaseException`, found `{type(exc).__name__!r}`."
+                )
+        else:
+            exc = UnknownModelError()
 
-    def __str__(self) -> str:
-        return str(round(self.transition_matrix, _n_dec))
+        super().__init__(model.adata, model)
 
+        self._gene = model._gene
+        self._lineage = model._lineage
+        self._prepared = model._prepared
+        self._is_bulk = model._is_bulk
 
-class ConstantMatrix(Kernel):
-    """Kernel representing multiplication by a constant matrix."""
+        self._exc = exc
 
-    def __init__(
+    def prepare(
         self,
-        adata: AnnData,
-        value: Union[int, float],
-        variances: Union[np.ndarray, spmatrix],
-        backward: bool = False,
-    ):
-        super().__init__(adata, backward=backward)
-        conn_shape = self._conn.shape
-        if variances.shape != conn_shape:
-            raise ValueError(
-                f"Expected variances of shape `{conn_shape}`, found `{variances.shape}`."
-            )
-        if not isinstance(value, (int, float)):
-            raise TypeError(
-                f"Value must be on `float` or `int`, found `{type(value).__name__!r}`."
-            )
-        if value <= 0:
-            raise ValueError(f"Expected the constant to be positive, found `{value}`.")
-
-        self._value = value
-        self._mat_scaler = (
-            csr_matrix(variances) if not issparse(variances) else variances
-        )
-        self._recalculate(value)
-
-    @d.dedent
-    def copy(self) -> "ConstantMatrix":
-        """%(copy)s"""  # noqa: D400, D401
-        return ConstantMatrix(
-            self.adata, self._value, copy(self._mat_scaler), self.backward
-        )
-
-    def _recalculate(self, value) -> None:
-        self._value = value
-        self._params = {"value": value}
-        self._transition_matrix = value * self._mat_scaler
-
-    def compute_transition_matrix(self, *args, **kwargs) -> "ConstantMatrix":
-        """Return self."""
+        *_args,
+        **_kwargs,
+    ) -> "FailedModel":
+        """Do nothing and return self."""
         return self
 
-    def __invert__(self) -> "ConstantMatrix":
-        # do not call parent's invert, since it removes the transition matrix
-        self._backward = not self.backward
+    def fit(
+        self,
+        x: Optional[np.ndarray] = None,
+        y: Optional[np.ndarray] = None,
+        w: Optional[np.ndarray] = None,
+        **kwargs: Any,
+    ) -> "FailedModel":
+        """Do nothing and return self."""
         return self
 
-    def __repr__(self) -> str:
-        return repr(round(self._value, _n_dec))
-
-    def __str__(self) -> str:
-        return str(round(self._value, _n_dec))
-
+    def predict(
+        self,
+        x_test: Optional[np.ndarray] = None,
+        key_added: Optional[str] = "_x_test",
+        **kwargs: Any,
+    ) -> np.ndarray:
+        """Do nothing."""
 
-class SimpleNaryExpression(NaryKernelExpression):
-    """Base class for n-ary operations."""
+    def confidence_interval(self, x_test: Optional[np.ndarray] = None, **kwargs) -> np.ndarray:
+        """Do nothing."""
 
-    def __init__(self, kexprs: List[KernelExpression], op_name: str, fn: Callable):
-        super().__init__(kexprs, op_name=op_name)
-        self._fn = fn
-
-    def compute_transition_matrix(self, *args, **kwargs) -> "SimpleNaryExpression":
-        """Compute and combine the transition matrices."""
-        # must be done before, because the underlying expression don't have to be normed
-        if isinstance(self, KernelSimpleAdd):
-            self._maybe_recalculate_constants(Constant)
-        elif isinstance(self, KernelAdaptiveAdd):
-            self._maybe_recalculate_constants(ConstantMatrix)
-
-        for kexpr in self:
-            if kexpr._transition_matrix is None:
-                if isinstance(kexpr, Kernel):
-                    raise RuntimeError(
-                        f"Kernel `{kexpr}` is uninitialized. "
-                        f"Compute its transition matrix first as `.compute_transition_matrix()`."
-                    )
-                kexpr.compute_transition_matrix()
-            elif isinstance(kexpr, Kernel):
-                logg.debug(_LOG_USING_CACHE)
+    def default_confidence_interval(
+        self,
+        x_test: Optional[np.ndarray] = None,
+        **kwargs: Any,
+    ) -> np.ndarray:
+        """Do nothing."""
 
-        self.transition_matrix = csr_matrix(
-            self._fn([kexpr.transition_matrix for kexpr in self])
-        )
+    def reraise(self) -> None:
+        """Raise the original exception with additional model information."""
+        # retain the exception type and also the original exception
+        raise type(self._exc)(f"Fatal model failure `{self}`.") from self._exc
 
-        # only the top level expression and kernels will have condition number computed
-        if self._parent is None:
-            self._maybe_compute_cond_num()
+    def _get_colors(
+        self,
+        key: Optional[str],
+        *,
+        same_plot: bool = False,
+    ) -> Tuple[Optional[str], Optional[Union[str, np.ndarray]], ColorType, Optional[Dict[str, Any]],]:
+        return None, "black", ColorType.STR, None
 
-        return self
+    def _return_min_max(self, show_conf_int: bool):
+        return np.inf, -np.inf
 
     @d.dedent
-    def copy(self) -> "SimpleNaryExpression":
-        """%(copy)s"""  # noqa: D400, D401
-        constructor = type(self)
-        kwargs = {"op_name": self._op_name, "fn": self._fn}
-
-        # preserve the type information so that combination can properly work
-        # we test for this
-        sne = constructor(
-            [copy(k) for k in self], **_filter_kwargs(constructor, **kwargs)
-        )
-
-        # TODO: copying's a bit buggy - the parent stays the same
-        # we could disallow it for inner expressions
-        sne._transition_matrix = copy(self._transition_matrix)
-        sne._condition_number = self._cond_num
-        sne._normalize = self._normalize
-
-        return sne
-
-
-class KernelAdd(SimpleNaryExpression):
-    """Base class that represents the addition of :class:`KernelExpression`."""
-
-    def __init__(self, kexprs: List[KernelExpression], op_name: str):
-        super().__init__(kexprs, op_name=op_name, fn=Reductor(np.add, 0))
-
-
-class KernelSimpleAdd(KernelAdd):
-    """Addition of :class:`KernelExpression`."""
+    def copy(self) -> "FailedModel":
+        """%(copy)s"""  # noqa
+        return FailedModel(self.model.copy(), exc=self._exc)
 
-    def __init__(self, kexprs: List[KernelExpression]):
-        super().__init__(kexprs, op_name="+")
-
-
-class KernelAdaptiveAdd(KernelAdd):
-    """Adaptive addition of :class:`KernelExpression`."""
-
-    def __init__(self, kexprs: List[KernelExpression]):
-        super().__init__(kexprs, op_name="^")
-
-
-class KernelMul(SimpleNaryExpression):
-    """Multiplication of :class:`KernelExpression`."""
+    def __bool__(self):
+        return False
 
-    def __init__(self, kexprs: List[KernelExpression]):
-        super().__init__(kexprs, op_name="*", fn=Reductor(np.multiply, 1))
+    def __str__(self) -> str:
+        return repr(self)
 
+    def __repr__(self) -> str:
+        return f"<{self.__class__.__name__}[origin={repr(self.model).strip('<>')}]>"
 
-class Reductor:
-    """
-    Class that reduces an iterable.
 
-    We don't define a decorator because of pickling.
+@d.dedent
+class FittedModel(BaseModel):
+    """Class representing an already fitted model. Useful when the smoothed gene expression was computed externally.
 
     Parameters
     ----------
-    func
-        Reduction function.
-    initial
-        Initial value for :func:`reduce`.
+    x_test
+        %(base_model_x_test.summary)s
+    y_test
+        %(base_model_y_test.summary)s
+    conf_int
+        %(base_model_conf_int.summary)s
+        If :obj:`None`, always set ``conf_int=False`` in :meth:`~cellrank.models.BaseModel.plot`.
+    x_all
+        %(base_model_x_all.summary)s
+        If :obj:`None`, always sets ``hide_cells=True`` in :meth:`~cellrank.models.BaseModel.plot`.
+    y_all
+        %(base_model_y_all.summary)s
+        If :obj:`None`, always sets `hide_cells=True`` in :meth:`~cellrank.models.BaseModel.plot`.
+    w_all
+        %(base_model_w_all.summary)s
+        If :obj:`None` and :attr:`x_all` and :attr:`y_all` are present, it will be set an array of :math:`1`.
     """
 
-    def __init__(self, func: Callable, initial: Union[int, float]):
-        self._func = func
-        self._initial = initial
-
-    def __call__(self, seq: Iterable):  # noqa
-        return reduce(self._func, seq, self._initial)
+    def __init__(
+        self,
+        x_test: ArrayLike,
+        y_test: ArrayLike,
+        conf_int: Optional[ArrayLike] = None,
+        x_all: Optional[ArrayLike] = None,
+        y_all: Optional[ArrayLike] = None,
+        w_all: Optional[ArrayLike] = None,
+    ):
+        super().__init__(None, None)
 
+        self._x_test = _densify_squeeze(x_test, self._dtype)[:, np.newaxis]
+        self._y_test = _densify_squeeze(y_test, self._dtype)
 
-def _get_expr_and_constant(k: KernelMul) -> Tuple[KernelExpression, Union[int, float]]:
-    """
-    Get the value of a constant in binary multiplication.
+        if self.x_test.ndim != 2 or self.x_test.shape[1] != 1:
+            raise ValueError(f"Expected `x_test` to be of shape `(..., 1)`, found `{self.x_test.shape}`.")
 
-    Parameters
-    ----------
-    k
-        Binary multiplication involving a constant and a kernel.
+        if self.y_test.shape != (self.x_test.shape[0],):
+            raise ValueError(
+                f"Expected `y_test` to be of shape `({self.x_test.shape[0]},)`, " f"found `{self.y_test.shape}`."
+            )
 
-    Returns
-    -------
-    :class:`KernelExpression`, int or float
-        The expression which is being multiplied and the value of the constant.
-    """
+        if conf_int is not None:
+            self._conf_int = _densify_squeeze(conf_int, self._dtype)
+            if self.conf_int.shape != (self.x_test.shape[0], 2):
+                raise ValueError(f"Expected `conf_int` to be of shape `({self.x_test.shape[0]}, 2)`.")
+        else:
+            logg.debug("No `conf_int` have been supplied, will be ignored during plotting")
 
-    if not isinstance(k, KernelMul):
-        raise TypeError(
-            f"Expected expression to be of type `KernelMul`, found `{type(k).__name__}`."
-        )
-    if len(k) != 2:
-        raise ValueError(
-            f"Expected expression to be binary, found `{len(k)}` subexpressions."
-        )
-    e1, e2 = k[0], k[1]
+        if x_all is not None and y_all is not None:
+            self._x_all = _densify_squeeze(x_all, self._dtype)[:, np.newaxis]
+            if self.x_all.ndim != 2 or self.x_all.shape[1] != 1:
+                raise ValueError(f"Expected `x_all` to be of shape `(..., 1)`, found `{self.x_all.shape}`.")
+
+            self._y_all = _densify_squeeze(y_all, self._dtype)[:, np.newaxis]
+            if self.y_all.shape != self.x_all.shape:
+                raise ValueError(
+                    f"Expected `y_all` to be of shape `({self.x_all.shape[0]}, 1)`, found `{self.y_all.shape}`."
+                )
 
-    if isinstance(e1, Constant):
-        return e2, e1.transition_matrix
-    elif isinstance(e2, Constant):
-        return e1, e2.transition_matrix
-    else:
-        raise ValueError(
-            "Expected one of the subexpressions to be `Constant`, found "
-            f"`{type(e1).__name__}` and `{type(e2).__name__}`."
-        )
+            if w_all is not None:
+                self._w_all = _densify_squeeze(w_all, self._dtype)
+                if self.w_all.ndim != 1 or self.w_all.shape[0] != self.x_all.shape[0]:
+                    raise ValueError(
+                        f"Expected `w_all` to be of shape `({self.x_all.shape[0]},)`, " f"found `{self.w_all.shape}`."
+                    )
+            else:
+                logg.debug("Setting `w_all` to an array of `1`")
+                self._w_all = np.ones_like(self.x_all, dtype=np.float64).squeeze(1)
+        else:
+            logg.debug(
+                "None or partially incomplete `x_all` and `y_all` have been supplied, "
+                "will be ignored during plotting"
+            )
 
+        self._prepared = True
 
-def _is_bin_mult(
-    k: KernelExpression,
-    const_type: Union[Type, Tuple[Type]] = Constant,
-    return_constant: bool = True,
-) -> Optional[KernelExpression]:
-    """
-    Check if an expression is a binary multiplication.
+    def _get_colors(
+        self,
+        key: Optional[str],
+        *,
+        same_plot: bool = False,
+    ) -> Tuple[Optional[str], Optional[Union[str, np.ndarray]], ColorType, Optional[Dict[str, Any]],]:
+        # w_all does not need to be defined
+        if same_plot or self.w_all is None or np.allclose(self.w_all, 1.0):
+            return None, "black", ColorType.STR, None
+        return "fate probability", np.squeeze(self.w_all), ColorType.CONT, None
 
-    Parameters
-    ----------
-    k
-        Kernel expression to check.
-    const_type
-        Type of the constant.
-    return_constant
-        Whether to return the constant in the expression or the multiplied expression.
-
-    Returns
-    -------
-    None
-        If the expression is not a binary multiplication.
-    :class:`cellrank.tl.kernels.KernelExpression`
-        Depending on ``return_constant``, it either returns the constant multiplier or the expression being multiplied.
-    """
+    def prepare(self, *_args, **_kwargs) -> "FittedModel":
+        """Do nothing and return self."""
+        return self
 
-    if not isinstance(k, KernelMul):
-        return None
+    def fit(
+        self,
+        x: Optional[np.ndarray] = None,
+        y: Optional[np.ndarray] = None,
+        w: Optional[np.ndarray] = None,
+        **kwargs: Any,
+    ) -> "FittedModel":
+        """Do nothing and return self."""
+        return self
 
-    if len(k) != 2:
-        return None
+    @d.dedent
+    def predict(
+        self,
+        x_test: Optional[np.ndarray] = None,
+        key_added: Optional[str] = "_x_test",
+        **kwargs: Any,
+    ) -> np.ndarray:
+        """%(base_model_y_test.summary)s."""
+        return self._y_test
 
-    lhs, rhs = k[0], k[1]
+    @d.dedent
+    def confidence_interval(self, x_test: Optional[np.ndarray] = None, **kwargs) -> np.ndarray:
+        """%(base_model_conf_int.summary)s Raise a :class:`RuntimeError` if not present."""
+        if self.conf_int is None:
+            raise RuntimeError(
+                "No confidence interval has been supplied. " "Use `conf_int=...` when instantiating this class."
+            )
+        return self.conf_int
 
-    if isinstance(lhs, const_type):
-        return lhs if return_constant else rhs
-    if isinstance(rhs, const_type):
-        return rhs if return_constant else lhs
+    @d.dedent
+    def default_confidence_interval(
+        self,
+        x_test: Optional[np.ndarray] = None,
+        **kwargs: Any,
+    ) -> np.ndarray:
+        """%(base_model_conf_int.summary)s Raise a :class:`RuntimeError` if not present."""
+        return self.confidence_interval()
 
-    return None
+    @d.dedent
+    def copy(self) -> "FittedModel":
+        """%(copy)s"""  # noqa
+        # here we return a deepcopy since it doesn't make sense to make a shallow one
+        return FittedModel.from_model(self)
+
+    @staticmethod
+    def from_model(model: BaseModel) -> "FittedModel":
+        """Create a :class:`~cellrank.models.FittedModel` from a :class:`~cellrank.models.BaseModel`."""
+        if not isinstance(model, BaseModel):
+            raise TypeError(f"Expected `model` to be of type `BaseModel`, found `{type(model).__name__!r}`.")
+
+        fm = FittedModel(
+            model.x_test,
+            model.y_test,
+            conf_int=model.conf_int,
+            x_all=model.x_all,
+            y_all=model.y_all,
+            w_all=model.w_all,
+        )
 
+        fm._gene = model._gene
+        fm._lineage = model._lineage
+        fm._is_bulk = model._is_bulk
+        fm._prepared = True
 
-def _is_adaptive_type(k: KernelExpression) -> bool:
-    return isinstance(k, Kernel) and not isinstance(k, (Constant, ConstantMatrix))
+        return fm
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_connectivity_kernel.py` & `cellrank-2.0.0/src/cellrank/kernels/_connectivity_kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,76 @@
-from copy import copy
-
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank.ul._docs import d
-from cellrank.tl.kernels import Kernel
+from cellrank._utils._docs import d
+from cellrank.kernels._base_kernel import UnidirectionalKernel
+from cellrank.kernels.mixins import ConnectivityMixin
+
+__all__ = ["ConnectivityKernel"]
 
 
 @d.dedent
-class ConnectivityKernel(Kernel):
-    """
-    Kernel which computes transition probabilities based on similarities among cells.
+class ConnectivityKernel(ConnectivityMixin, UnidirectionalKernel):
+    """Kernel which computes transition probabilities based on similarities among cells.
 
     As a measure of similarity, we currently support:
 
-        - transcriptomic similarities, computed using e.g. :func:`scanpy.pp.neighbors`, see :cite:`wolf:18`.
-        - spatial similarities, computed using e.g. :func:`squidpy.gr.spatial_neighbors`, see :cite:`palla:21`.
+    - transcriptomic similarities, computed using, e.g., :func:`~scanpy.pp.neighbors`, see :cite:`wolf:18`.
+    - spatial similarities, computed using, e.g., :func:`~squidpy.gr.spatial_neighbors`, see :cite:`palla:21`.
 
     The resulting transition matrix is symmetric and thus cannot be used to learn about the direction of the biological
     process. To include this direction, consider combining with a velocity-derived transition matrix via
-    :class:`cellrank.tl.kernels.VelocityKernel`.
+    :class:`~cellrank.kernels.VelocityKernel`.
 
     %(density_correction)s
 
     Parameters
     ----------
     %(adata)s
-    %(backward)s
     conn_key
-        Key in :attr:`anndata.AnnData.obsp` to obtain the connectivity matrix describing cell-cell similarity.
-    %(cond_num)s
+        Key in :attr:`~anndata.AnnData.obsp` where connectivity matrix describing cell-cell similarity is stored.
     check_connectivity
-        Check whether the underlying KNN graph is connected.
+        Check whether the underlying kNN graph is connected.
     """
 
     def __init__(
         self,
         adata: AnnData,
-        backward: bool = False,
         conn_key: str = "connectivities",
-        compute_cond_num: bool = False,
         check_connectivity: bool = False,
     ):
         super().__init__(
             adata,
-            backward=backward,
-            compute_cond_num=compute_cond_num,
-            check_connectivity=check_connectivity,
             conn_key=conn_key,
+            check_connectivity=check_connectivity,
         )
-        self._key = conn_key
 
-    def compute_transition_matrix(
-        self, density_normalize: bool = True
-    ) -> "ConnectivityKernel":
-        """
-        Compute transition matrix based on transcriptomic similarity.
+    def compute_transition_matrix(self, density_normalize: bool = True) -> "ConnectivityKernel":
+        """Compute transition matrix based on transcriptomic similarity.
 
-        Uses symmetric, weighted KNN graph to compute symmetric transition matrix. The connectivities are computed
-        using :func:`scanpy.pp.neighbors`. Depending on the parameters used there, they can be UMAP connectivities or
-        gaussian-kernel-based connectivities with adaptive kernel width.
+        Uses symmetric, weighted kNN graph to compute symmetric transition matrix. The connectivities are computed
+        using :func:`~scanpy.pp.neighbors`. Depending on the parameters used there, they can be UMAP connectivities or
+        Gaussian-kernel-based connectivities with adaptive kernel width.
 
         Parameters
         ----------
         density_normalize
-            Whether or not to use the underlying KNN graph for density normalization.
+            Whether to use the underlying kNN graph for density normalization.
 
         Returns
         -------
-        Self and updated :attr:`transition_matrix`.
+        Returns self and updates :attr:`transition_matrix` and :attr:`params`.
         """
-
         # fmt: off
-        start = logg.info(f"Computing transition matrix based on `adata.obsp[{self._key!r}]`")
-
-        if self._reuse_cache({"dnorm": density_normalize, "key": self._key}, time=start):
+        start = logg.info(f"Computing transition matrix based on `adata.obsp[{self._conn_key!r}]`")
+        if self._reuse_cache({"dnorm": density_normalize, "key": self._conn_key}, time=start):
             return self
 
-        self._compute_transition_matrix(matrix=self._conn.copy(), density_normalize=density_normalize)
+        conn = self.connectivities
+        if density_normalize:
+            conn = self._density_normalize(conn)
+
+        self.transition_matrix = conn
         logg.info("    Finish", time=start)
         # fmt: on
 
         return self
-
-    def copy(self) -> "ConnectivityKernel":
-        """Return a copy of self."""
-        ck = ConnectivityKernel(self.adata, backward=self.backward)
-        ck._params = copy(self.params)
-        ck._cond_num = self.condition_number
-        ck._transition_matrix = copy(self._transition_matrix)
-
-        return ck
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_cytotrace_kernel.py` & `cellrank-2.0.0/src/cellrank/kernels/_cytotrace_kernel.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,260 +1,276 @@
-from typing import Any
-from typing_extensions import Literal
+import enum
+from typing import Any, List, Literal, Optional, Tuple
 
-from enum import auto
+import numpy as np
+import pandas as pd
+import scipy.sparse as sp
+import scipy.stats as st
 
 from anndata import AnnData
-from cellrank import logging as logg
-from cellrank._key import Key
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d, inject_docs
-from cellrank.tl._utils import _correlation_test_helper
-from cellrank.tl.kernels._pseudotime_kernel import PseudotimeKernel
 
-import numpy as np
-from scipy.stats import gmean, hmean
-from scipy.sparse import issparse
+from cellrank import logging as logg
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._key import Key
+from cellrank._utils._utils import _correlation_test
+from cellrank.kernels._pseudotime_kernel import PseudotimeKernel
+
+__all__ = ["CytoTRACEKernel"]
 
 
-class CytoTRACEAggregation(ModeEnum):  # noqa: D101
-    MEAN = auto()
-    MEDIAN = auto()
-    GMEAN = auto()
-    HMEAN = auto()
+class CytoTRACEAggregation(ModeEnum):
+    MEAN = enum.auto()
+    MEDIAN = enum.auto()
+    GMEAN = enum.auto()
+    HMEAN = enum.auto()
 
 
 @d.dedent
 class CytoTRACEKernel(PseudotimeKernel):
-    """
-    Kernel which computes directed transition probabilities based on a KNN graph and the CytoTRACE score \
-    :cite:`gulati:20`.
+    """Kernel which computes directed transition probabilities using the CytoTRACE score :cite:`gulati:20`.
 
-    The KNN graph contains information about the (undirected) connectivities among cells, reflecting their similarity.
+    .. seealso::
+        - See :doc:`../../../notebooks/tutorials/kernels/400_cytotrace` on how to
+          compute the :attr:`~cellrank.kernels.CytoTRACEKernel.transition_matrix` based on the CytoTRACE score.
+
+    The k-NN graph contains information about the (undirected) connectivities among cells, reflecting their similarity.
     CytoTRACE can be used to estimate cellular plasticity and in turn, a pseudotemporal ordering of cells from more
-    plastic to less plastic states.
-    This kernel internally uses the :class:`cellrank.tl.kernels.PseudotimeKernel` to direct the KNN graph
-    on the basis of the CytoTRACE-derived pseudotime.
+    plastic to less plastic states. It relies on the assumption that differentiated cells express, on average,
+    fewer genes than naive cells.
+
+    This kernel internally uses the :class:`~cellrank.kernels.PseudotimeKernel` to direct the k-NN graph
+    on the basis of the CytoTRACE pseudotime.
 
     %(density_correction)s
 
     Parameters
     ----------
     %(adata)s
     %(backward)s
-    %(cytotrace.parameters)s
-
-    %(cond_num)s
-    check_connectivity
-        Check whether the underlying KNN graph is connected.
     kwargs
-        Keyword arguments for :class:`cellrank.tl.kernels.PseudotimeKernel`.
+        Keyword arguments for the :class:`~cellrank.kernels.PseudotimeKernel`.
 
-    Example
-    -------
-    Workflow::
+    Examples
+    --------
+    .. code-block::
 
-        # import packages and load data
         import scvelo as scv
         import cellrank as cr
+
         adata = cr.datasets.pancreas()
 
-        # standard pre-processing
         sc.pp.filter_genes(adata, min_cells=10)
         sc.pp.normalize_total(adata)
         sc.pp.log1p(adata)
         sc.pp.highly_variable_genes(adata)
 
-        # CytoTRACE by default uses imputed data - a simple way to compute KNN-imputed data is to use scVelo's moments
-        # function. However, note that this function expects `spliced` counts because it's designed for RNA velocity,
-        # so we're using a simple hack here:
+        # CytoTRACE by default uses imputed data - a simple way to compute
+        # k-NN imputed data is to use scVelo's moments function.
+        # However, note that this function expects `spliced` counts because
+        # it's designed for RNA velocity, so we're using a simple hack here:
         if 'spliced' not in adata.layers or 'unspliced' not in adata.layers:
             adata.layers['spliced'] = adata.X
             adata.layers['unspliced'] = adata.X
-
-        # compute KNN-imputation using scVelo's moments function
         scv.pp.moments(adata)
 
-        # import and initialize the CytoTRACE kernel, compute transition matrix - done!
-        from cellrank.tl.kernels import CytoTRACEKernel
-        ctk = CytoTRACEKernel(adata).compute_transition_matrix()
+        ctk = cr.kernels.CytoTRACEKernel(adata)
+        ckt = ctk.compute_cytotrace().compute_transition_matrix()
     """
 
     def __init__(
         self,
         adata: AnnData,
         backward: bool = False,
-        layer: str = "Ms",
-        aggregation: Literal[
-            "mean", "median", "hmean", "gmean"
-        ] = CytoTRACEAggregation.MEAN,
-        use_raw: bool = False,
-        compute_cond_num: bool = False,
-        check_connectivity: bool = False,
         **kwargs: Any,
     ):
+        _ = kwargs.pop("time_key", None)
         super().__init__(
             adata,
             backward=backward,
             time_key=Key.cytotrace("pseudotime"),
-            compute_cond_num=compute_cond_num,
-            check_connectivity=check_connectivity,
-            layer=layer,
-            aggregation=aggregation,
-            use_raw=use_raw,
             **kwargs,
         )
-        self._time_key = Key.cytotrace("pseudotime")  # quirk or PT kernel
 
     def _read_from_adata(
         self,
         time_key: str,
-        layer: str = "Ms",
-        aggregation: Literal[
-            "mean", "median", "hmean", "gmean"
-        ] = CytoTRACEAggregation.MEAN,
-        use_raw: bool = True,
         **kwargs: Any,
     ) -> None:
-        self.compute_cytotrace(layer=layer, aggregation=aggregation, use_raw=use_raw)
-
-        super()._read_from_adata(time_key=time_key, **kwargs)
+        try:
+            super()._read_from_adata(time_key=time_key, **kwargs)
+        except KeyError as e:
+            self._pseudotime: Optional[np.ndarray] = None
+            if "Unable to find pseudotime" not in str(e):
+                raise
+            super(PseudotimeKernel, self)._read_from_adata(**kwargs)
 
     @d.get_sections(base="cytotrace", sections=["Parameters"])
     @inject_docs(ct=CytoTRACEAggregation)
     def compute_cytotrace(
         self,
-        layer: str = "Ms",
-        aggregation: Literal[
-            "mean", "median", "hmean", "gmean"
-        ] = CytoTRACEAggregation.MEAN,
+        layer: Optional[str] = "Ms",
+        aggregation: Literal["mean", "median", "hmean", "gmean"] = CytoTRACEAggregation.MEAN,
         use_raw: bool = False,
-    ) -> None:
-        """
-        Re-implementation of the CytoTRACE algorithm :cite:`gulati:20` to estimate cellular plasticity.
+        n_genes: int = 200,
+    ) -> "CytoTRACEKernel":
+        """Re-implementation of the CytoTRACE algorithm :cite:`gulati:20` to estimate cellular plasticity.
 
         Computes the number of genes expressed per cell and ranks genes according to their correlation with this
         measure. Next, it selects to top-correlating genes and aggregates their (imputed) expression to obtain
         the CytoTRACE score. A high score stands for high differentiation potential (naive, plastic cells) and
         a low score stands for low differentiation potential (mature, differentiation cells).
 
         Parameters
         ----------
         layer
-            Key in :attr:`anndata.AnnData.layers` or `'X'` for :attr:`anndata.AnnData.X`
+            Key in :attr:`~anndata.AnnData.layers` or ``'X'`` for :attr:`~anndata.AnnData.X`
             from where to get the expression.
         aggregation
             How to aggregate expression of the top-correlating genes. Valid options are:
 
-                - `{ct.MEAN!r}` - arithmetic mean.
-                - `{ct.MEDIAN!r}` - median.
-                - `{ct.HMEAN!r}` - harmonic mean.
-                - `{ct.GMEAN!r}` - geometric mean.
-
+            - ``{ct.MEAN!r}`` - arithmetic mean.
+            - ``{ct.MEDIAN!r}`` - median.
+            - ``{ct.HMEAN!r}`` - harmonic mean.
+            - ``{ct.GMEAN!r}`` - geometric mean.
         use_raw
-            Whether to use the :attr:`anndata.AnnData.raw` to compute the number of genes expressed per cell
+            Whether to use the :attr:`~anndata.AnnData.raw` to compute the number of genes expressed per cell
             (#genes/cell) and the correlation of gene expression across cells with #genes/cell.
+        n_genes
+            Number of top positively correlated genes to compute the CytoTRACE score.
 
         Returns
         -------
-        Nothing, just modifies :attr:`anndata.AnnData.obs` with the following keys:
+        Nothing, just modifies :attr:`~anndata.AnnData.obs` with the following keys:
 
-            - `'ct_score'` - the normalized CytoTRACE score.
-            - `'ct_pseudotime'` - associated pseudotime, essentially `1 - CytoTRACE score`.
-            - `'ct_num_exp_genes'` - the number of genes expressed per cell, basis of the CytoTRACE score.
+        - ``'ct_score'`` - the normalized CytoTRACE score.
+        - ``'ct_pseudotime'`` - associated pseudotime, essentially ``1 - CytoTRACE score``.
+        - ``'ct_num_exp_genes'`` - the number of genes expressed per cell, basis of the CytoTRACE score.
 
-        It also modifies :attr:`anndata.AnnData.var` with the following keys:
+        It also modifies :attr:`~anndata.AnnData.var` with the following keys:
 
-            - `'ct_gene_corr'` - the correlation as specified above.
-            - `'ct_correlates'` - indication of the genes used to compute the CytoTRACE score, i.e. the ones that
-              correlated best with `'num_exp_genes'`.
+        - ``'ct_gene_corr'`` - the correlation as specified above.
+        - ``'ct_correlates'`` - indication of the genes used to compute the CytoTRACE score, i.e. the ones that
+          correlated positively with ``'ct_num_exp_genes'``.
 
         Notes
         -----
         This will not exactly reproduce the results of the original CytoTRACE algorithm :cite:`gulati:20` because we
         allow for any normalization and imputation techniques whereas CytoTRACE has built-in specific methods for that.
         """
-        # check use_raw
+        from cellrank._utils import Lineage
+
         aggregation = CytoTRACEAggregation(aggregation)
+
         if use_raw and self.adata.raw is None:
             logg.warning("`adata.raw` is `None`. Setting `use_raw=False`")
             use_raw = False
-        if use_raw and self.adata.raw.n_vars != self.adata.n_vars:
-            logg.warning(
-                f"`adata.raw` has different number of genes ({self.adata.raw.n_vars}) "
-                f"than `adata` ({self.adata.n_vars}). Setting `use_raw=False`"
-            )
-            use_raw = False
-
-        adata_mraw = self.adata.raw if use_raw else self.adata
-        if layer != "X" and layer not in self.adata.layers:
+        if layer not in (None, "X") and layer not in self.adata.layers:
             raise KeyError(
                 f"Unable to find `{layer!r}` in `adata.layers`. "
                 f"Valid option are: `{sorted({'X'} | set(self.adata.layers.keys()))}`."
             )
 
-        msg = f"Computing CytoTRACE score with `{self.adata.n_vars}` genes"
-        if self.adata.n_vars < 10000:
+        adata_mraw = self.adata.raw if use_raw else self.adata
+        msg = f"Computing CytoTRACE score with `{adata_mraw.n_vars}` genes"
+        if adata_mraw.n_vars < 10000:
             msg += ". Consider using more than `10000` genes"
         start = logg.info(msg)
 
         # compute number of expressed genes per cell
-        logg.debug(
-            f"Computing number of genes expressed per cell with `use_raw={use_raw}`"
-        )
-        num_exp_genes = np.array((adata_mraw.X > 0).sum(axis=1)).reshape(-1)
-        self.adata.obs[Key.cytotrace("num_exp_genes")] = num_exp_genes
+        num_exp_genes = np.asarray((adata_mraw.X > 0).sum(axis=1)).squeeze()
 
-        # fmt: off
-        # compute correlation with all genes
         logg.debug("Correlating all genes with number of genes expressed per cell")
-        gene_corr, _, _, _ = _correlation_test_helper(adata_mraw.X.T, num_exp_genes[:, None])
-
-        # annotate the top 200 genes in terms of correlation
-        logg.debug("Finding the top `200` most correlated genes")
-        self.adata.var[Key.cytotrace("gene_corr")] = gene_corr
-        top_200 = self.adata.var.sort_values(by=Key.cytotrace("gene_corr"), ascending=False).index[:200]
-        self.adata.var[Key.cytotrace("correlates")] = False
-        self.adata.var.loc[top_200, Key.cytotrace("correlates")] = True
+        gene_corr = _correlation_test(
+            adata_mraw.X,
+            Lineage(num_exp_genes[:, None], names=["gene"]),
+            gene_names=adata_mraw.var_names,
+        )["gene_corr"]
 
-        # compute mean/median over top 200 genes, aggregate over genes and shift to [0, 1] range
-        logg.debug(f"Aggregating imputed gene expression using aggregation `{aggregation}` in layer `{layer}`")
-        corr_mask = self.adata.var[Key.cytotrace("correlates")]
-        imputed_exp = self.adata[:, corr_mask].X if layer == "X" else self.adata[:, corr_mask].layers[layer]
-        if issparse(imputed_exp):
-            imputed_exp = imputed_exp.A
-
-        # aggregate across the top 200 genes
-        if aggregation == CytoTRACEAggregation.MEAN:
-            cytotrace_score = np.mean(imputed_exp, axis=1)
-        elif aggregation == CytoTRACEAggregation.MEDIAN:
-            cytotrace_score = np.median(imputed_exp, axis=1)
-        elif aggregation == CytoTRACEAggregation.GMEAN:
-            cytotrace_score = gmean(imputed_exp, axis=1)
-        elif aggregation == CytoTRACEAggregation.HMEAN:
-            cytotrace_score = hmean(imputed_exp, axis=1)
-        else:
-            raise NotImplementedError(f"Aggregation method `{aggregation}` is not yet implemented.")
-        # fmt: on
+        cytotrace_score, pos_top_genes = self._compute_score(
+            gene_corr,
+            layer=layer,
+            aggregation=aggregation,
+            ascending=False,
+            n_genes=n_genes,
+        )
+        cytotrace_score -= cytotrace_score.min()
+        cytotrace_score /= cytotrace_score.max()
 
-        # scale to 0-1 range
-        cytotrace_score -= np.min(cytotrace_score)
-        cytotrace_score /= np.max(cytotrace_score)
         self.adata.obs[Key.cytotrace("score")] = cytotrace_score
-        self.adata.obs[Key.cytotrace("pseudotime")] = 1 - cytotrace_score
-
+        self.adata.obs[Key.cytotrace("pseudotime")] = self._pseudotime = 1 - cytotrace_score
+        self.adata.obs[Key.cytotrace("num_exp_genes")] = num_exp_genes
+        self.adata.var[Key.cytotrace("gene_corr")] = gene_corr
+        self.adata.var[Key.cytotrace("correlates")] = False
+        self.adata.var.loc[pos_top_genes, Key.cytotrace("correlates")] = True
         self.adata.uns[Key.cytotrace("params")] = {
-            "aggregation": aggregation,
+            "aggregation": str(aggregation),
             "layer": layer,
             "use_raw": use_raw,
+            "n_genes": len(pos_top_genes),
         }
 
         logg.info(
             f"Adding `adata.obs[{Key.cytotrace('score')!r}]`\n"
             f"       `adata.obs[{Key.cytotrace('pseudotime')!r}]`\n"
             f"       `adata.obs[{Key.cytotrace('num_exp_genes')!r}]`\n"
             f"       `adata.var[{Key.cytotrace('gene_corr')!r}]`\n"
             f"       `adata.var[{Key.cytotrace('correlates')!r}]`\n"
             f"       `adata.uns[{Key.cytotrace('params')!r}]`\n"
             f"    Finish",
             time=start,
         )
+
+        return self
+
+    def _compute_score(
+        self,
+        gene_corr: pd.Series,
+        *,
+        layer: Optional[str] = None,
+        aggregation: CytoTRACEAggregation.MEAN,
+        ascending: bool = False,
+        n_genes: int = 200,
+    ) -> Tuple[np.ndarray, List[str]]:
+        from sklearn.utils.sparsefuncs import csc_median_axis_0
+
+        # fmt: off
+        modifier = "negatively" if ascending else "positively"
+        if n_genes <= 0:
+            raise ValueError(f"Expected number of {modifier} correlated genes to be positive, found `{n_genes}`.")
+        top_genes = [g for g in gene_corr.sort_values(ascending=ascending).index if g in self.adata.var_names]
+        top_genes = top_genes[:n_genes]
+        invalid_genes = int(gene_corr.loc[top_genes].isnull().sum())
+        # fmt: on
+
+        if invalid_genes:
+            raise ValueError(
+                f"Top `{len(top_genes)}` {modifier} correlated genes contain `{invalid_genes}` NaN values."
+            )
+        if not len(top_genes):
+            raise ValueError("No genes have been selected.")
+
+        if len(top_genes) != n_genes:
+            logg.warning(
+                f"Unable to get requested top {modifier} correlated `{n_genes}`. " f"Using top `{len(top_genes)}` genes"
+            )
+
+        # fmt: off
+        imputed_exp = self.adata[:, top_genes].X if layer == "X" else self.adata[:, top_genes].layers[layer]
+        if sp.issparse(imputed_exp) and aggregation not in (CytoTRACEAggregation.MEAN, CytoTRACEAggregation.MEDIAN):
+            imputed_exp = imputed_exp.A
+
+        if aggregation == CytoTRACEAggregation.MEAN:
+            cytotrace_score = np.asarray(imputed_exp.mean(axis=1)).reshape((-1,))
+        elif aggregation == CytoTRACEAggregation.MEDIAN:
+            if sp.issparse(imputed_exp):
+                cytotrace_score = np.asarray(csc_median_axis_0(imputed_exp.T.tocsc())).reshape((-1,))
+            else:
+                cytotrace_score = np.median(imputed_exp, axis=1)
+        elif aggregation == CytoTRACEAggregation.GMEAN:
+            cytotrace_score = st.gmean(imputed_exp, axis=1)
+        elif aggregation == CytoTRACEAggregation.HMEAN:
+            cytotrace_score = st.hmean(imputed_exp, axis=1)
+        else:
+            raise NotImplementedError(f"Aggregation method `{aggregation}` is not yet implemented.")
+        # fmt: on
+        return cytotrace_score, top_genes
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_pseudotime_kernel.py` & `cellrank-2.0.0/src/cellrank/kernels/_pseudotime_kernel.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,149 +1,150 @@
-from typing import Any, Union, Callable, Optional
-from typing_extensions import Literal
+import enum
+from typing import Any, Callable, Literal, Optional, Union
 
-from copy import copy
-from enum import auto
+import numpy as np
 
 from anndata import AnnData
+
 from cellrank import logging as logg
-from cellrank.tl._enum import _DEFAULT_BACKEND, ModeEnum, Backend_t
-from cellrank.ul._docs import d
-from cellrank.tl._utils import _connected
-from cellrank.tl.kernels import Kernel
-from cellrank.tl.kernels._base_kernel import _dtype
-from cellrank.tl.kernels._pseudotime_schemes import (
-    ThresholdSchemeABC,
+from cellrank._utils._docs import d
+from cellrank._utils._enum import DEFAULT_BACKEND, Backend_t, ModeEnum
+from cellrank._utils._utils import _connected, _irreducible
+from cellrank.kernels._base_kernel import BidirectionalKernel
+from cellrank.kernels.mixins import ConnectivityMixin
+from cellrank.kernels.utils._pseudotime_scheme import (
+    CustomThresholdScheme,
     HardThresholdScheme,
     SoftThresholdScheme,
-    CustomThresholdScheme,
+    ThresholdSchemeABC,
 )
 
-import numpy as np
+__all__ = ["PseudotimeKernel"]
 
 
-class ThresholdScheme(ModeEnum):  # noqa: D101
-    SOFT = auto()
-    HARD = auto()
+class ThresholdScheme(ModeEnum):
+    SOFT = enum.auto()
+    HARD = enum.auto()
 
 
 @d.dedent
-class PseudotimeKernel(Kernel):
-    """
-    Kernel which computes directed transition probabilities based on a KNN graph and pseudotime.
+class PseudotimeKernel(ConnectivityMixin, BidirectionalKernel):
+    """Kernel which computes directed transition probabilities based on a k-NN graph and pseudotime.
+
+    .. seealso::
+        - See :doc:`../../../notebooks/tutorials/kernels/300_pseudotime` on how to
+          compute the :attr:`~cellrank.kernels.PseudotimeKernel.transition_matrix` based on the pseudotime.
 
-    The KNN graph contains information about the (undirected) connectivities among cells, reflecting their similarity.
+    The k-NN graph contains information about the (undirected) connectivities among cells, reflecting their similarity.
     Pseudotime can be used to either remove edges that point against the direction of increasing pseudotime
-    :cite:`setty:19`, or to downweight them :cite:`stassen:21`.
+    :cite:`setty:19` or to down-weight them :cite:`stassen:21`.
 
     Parameters
     ----------
     %(adata)s
     %(backward)s
+        If :obj:`True`, the :attr:`pseudotime` will be set to ``max(pseudotime) - pseudotime``.
     time_key
-        Key in :attr:`adata` ``.obs`` where the pseudotime is stored.
-    %(cond_num)s
+        Key in :attr:`~anndata.AnnData.obs` where the pseudotime is stored.
     kwargs
-        Keyword arguments for :class:`cellrank.tl.kernels.Kernel`.
+        Keyword arguments for the :class:`~cellrank.kernels.ConnectivityKernel`.
     """
 
     def __init__(
         self,
         adata: AnnData,
+        time_key: str,
         backward: bool = False,
-        time_key: str = "dpt_pseudotime",
-        compute_cond_num: bool = False,
-        check_connectivity: bool = False,
         **kwargs: Any,
     ):
         super().__init__(
             adata,
             backward=backward,
             time_key=time_key,
-            compute_cond_num=compute_cond_num,
-            check_connectivity=check_connectivity,
             **kwargs,
         )
-        self._time_key = time_key
 
     def _read_from_adata(self, time_key: str, **kwargs: Any) -> None:
         super()._read_from_adata(**kwargs)
+        # fmt: off
+        self._time_key = time_key
+        if time_key not in self.adata.obs:
+            raise KeyError(f"Unable to find pseudotime in `adata.obs[{time_key!r}]`.")
 
-        if time_key not in self.adata.obs.keys():
-            raise KeyError(f"Could not find time key in `adata.obs[{time_key!r}]`.")
-
-        self._pseudotime = np.array(self.adata.obs[time_key]).astype(_dtype)
-        if self.backward:
-            self._pseudotime = np.max(self.pseudotime) - self.pseudotime
-
+        self._pseudotime = np.array(self.adata.obs[time_key]).astype(np.float64, copy=True)
         if np.any(np.isnan(self._pseudotime)):
             raise ValueError("Encountered NaN values in pseudotime.")
+        # fmt: on
 
     @d.dedent
     def compute_transition_matrix(
         self,
-        threshold_scheme: Union[Literal["soft", "hard"], Callable] = "hard",
+        threshold_scheme: Union[
+            Literal["soft", "hard"],
+            Callable[[float, np.ndarray, np.ndarray], np.ndarray],
+        ] = "hard",
         frac_to_keep: float = 0.3,
         b: float = 10.0,
         nu: float = 0.5,
         check_irreducibility: bool = False,
         n_jobs: Optional[int] = None,
-        backend: Backend_t = _DEFAULT_BACKEND,
+        backend: Backend_t = DEFAULT_BACKEND,
         show_progress_bar: bool = True,
         **kwargs: Any,
     ) -> "PseudotimeKernel":
-        """
-        Compute transition matrix based on KNN graph and pseudotemporal ordering.
+        """Compute transition matrix based on k-NN graph and pseudotemporal ordering.
 
-        Depending on the choice of the `thresholding_scheme`, this is based on ideas by either *Palantir*
+        Depending on the choice of the ``threshold_scheme``, it is based on ideas by either *Palantir*
         :cite:`setty:19` or *VIA* :cite:`stassen:21`.
 
         Parameters
         ----------
         threshold_scheme
             Which method to use when biasing the graph. Valid options are:
 
-                - `'hard'` - based on *Palantir* :cite:`setty:19` which removes some edges that point against
-                  the direction of increasing pseudotime. To avoid disconnecting the graph, it does not
-                  remove all edges that point against the direction of increasing pseudotime, but keeps the ones
-                  that point to cells inside a close radius. This radius is chosen according to the local cell density.
-                - `'soft'` - based on *VIA* :cite:`stassen:21` which downweights edges that points against the direction
-                  of increasing pseudotime. Essentially, the further "behind" a query cell is in pseudotime with respect
-                  to the current reference cell, the more penalized will be its graph-connectivity.
-                - :class:`callable` - any function conforming to the signature of
-                  :func:`cellrank.tl.kernels.ThresholdSchemeABC.__call__`.
+            - ``'hard'`` - based on *Palantir* :cite:`setty:19` which removes some edges that point against
+              the direction of increasing pseudotime. To avoid disconnecting the graph, it does not
+              remove all edges that point against the direction of increasing pseudotime, but keeps the ones
+              that point to cells inside a close radius. This radius is chosen according to the local cell density.
+            - ``'soft'`` - based on *VIA* :cite:`stassen:21` which down-weights edges that points against
+              the direction of increasing pseudotime. Essentially, the further "behind"
+              a query cell is in pseudotime with respect
+              to the current reference cell, the more penalized will be its graph-connectivity.
+            - :class:`callable` - any function conforming to the signature of
+              :func:`cellrank.kernels.utils.ThresholdSchemeABC.__call__`.
         frac_to_keep
-            The `frac_to_keep` * number of the closest neighbors (according to graph connectivities) are kept, no matter
-            whether they lie in the pseudotemporal past or future. This is done to ensure that the graph remains
-            connected. Only used when ``threshold_scheme = 'hard'``. Needs to fall within the interval `[0, 1]`.
+            Fraction of the closest neighbors (according to graph connectivities) are kept, no matter whether they lie
+            in the pseudotemporal past or future. This is done to ensure that the graph remains connected.
+            Only used when ``threshold_scheme = 'hard'``. Must be in :math:`[0, 1]`.
         %(soft_scheme_kernel)s
         check_irreducibility
             Optional check for irreducibility of the final transition matrix.
         %(parallel)s
         kwargs
             Keyword arguments for ``threshold_scheme``.
 
         Returns
         -------
-        Self and updated :attr:`transition_matrix`.
+        Returns self and updates :attr:`transition_matrix` and :attr:`params`.
         """
-        start = logg.info(f"Computing transition matrix based on `{self._time_key}`")
+        if self.pseudotime is None:
+            raise ValueError("Compute pseudotime first.")  # CytoTraceKernel
+
+        start = logg.info("Computing transition matrix based on pseudotime")
         if isinstance(threshold_scheme, str):
             threshold_scheme = ThresholdScheme(threshold_scheme)
             if threshold_scheme == ThresholdScheme.SOFT:
                 scheme = SoftThresholdScheme()
                 kwargs["b"] = b
                 kwargs["nu"] = nu
             elif threshold_scheme == ThresholdScheme.HARD:
                 scheme = HardThresholdScheme()
                 kwargs["frac_to_keep"] = frac_to_keep
             else:
-                raise NotImplementedError(
-                    f"Threshold scheme `{threshold_scheme}` is not yet implemented."
-                )
+                raise NotImplementedError(f"Threshold scheme `{threshold_scheme}` is not yet implemented.")
         elif isinstance(threshold_scheme, ThresholdSchemeABC):
             scheme = threshold_scheme
         elif callable(threshold_scheme):
             scheme = CustomThresholdScheme(threshold_scheme)
         else:
             raise TypeError(
                 f"Expected `threshold_scheme` to be either a `str` or a `callable`, found `{type(threshold_scheme)}`."
@@ -151,49 +152,40 @@
 
         # fmt: off
         if self._reuse_cache({"dnorm": False, "scheme": str(threshold_scheme), **kwargs}, time=start):
             return self
         # fmt: on
 
         biased_conn = scheme.bias_knn(
-            self._conn,
+            self.connectivities,
             self.pseudotime,
             n_jobs=n_jobs,
             backend=backend,
             show_progress_bar=show_progress_bar,
             **kwargs,
         )
 
         # make sure the biased graph is still connected
         if not _connected(biased_conn):
-            logg.warning("Biased KNN graph is disconnected")
+            logg.warning("Biased k-NN graph is disconnected")
+        if check_irreducibility and not _irreducible(biased_conn):
+            logg.warning("Biased k-NN graph is not irreducible")
 
-        self._compute_transition_matrix(
-            matrix=biased_conn,
-            density_normalize=False,
-            check_irreducibility=check_irreducibility,
-        )
+        self.transition_matrix = biased_conn
         logg.info("    Finish", time=start)
 
         return self
 
     @property
-    def pseudotime(self) -> np.array:
+    def pseudotime(self) -> Optional[np.array]:
         """Pseudotemporal ordering of cells."""
+        if self._pseudotime is None:
+            return None
+        if self.backward:
+            return np.max(self._pseudotime) - self._pseudotime
         return self._pseudotime
 
-    def copy(self) -> "PseudotimeKernel":
-        """Return a copy of self."""
-        pk = PseudotimeKernel(
-            self.adata, backward=self.backward, time_key=self._time_key
-        )
-        pk._pseudotime = copy(self.pseudotime)
-        pk._params = copy(self._params)
-        pk._cond_num = self.condition_number
-        pk._transition_matrix = copy(self._transition_matrix)
-
-        return pk
-
     def __invert__(self) -> "PseudotimeKernel":
-        super().__invert__()
-        self._pseudotime = np.max(self.pseudotime) - self.pseudotime
-        return self
+        pk = self._copy_ignore("_transition_matrix")
+        pk._backward = not self.backward
+        pk._params = {}
+        return pk
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_pseudotime_schemes.py` & `cellrank-2.0.0/src/cellrank/kernels/utils/_pseudotime_scheme.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,62 @@
-from typing import Any, Tuple, Callable, Optional
+import abc
+from typing import Any, Callable, Optional, Tuple
 
-from abc import ABC, abstractmethod
+import numpy as np
+import scipy.sparse as sp
 
-from cellrank.ul._docs import d
-from cellrank.ul._parallelize import parallelize
+from cellrank._utils._docs import d
+from cellrank._utils._parallelize import parallelize
 
-import numpy as np
-from scipy.sparse import csr_matrix
+__all__ = ["HardThresholdScheme", "SoftThresholdScheme", "CustomThresholdScheme"]
 
 
-class ThresholdSchemeABC(ABC):
+class ThresholdSchemeABC(abc.ABC):
     """Base class for all connectivity biasing schemes."""
 
     @d.get_summary(base="pt_scheme")
     @d.get_sections(base="pt_scheme", sections=["Parameters", "Returns"])
-    @abstractmethod
+    @abc.abstractmethod
     def __call__(
         self,
         cell_pseudotime: float,
         neigh_pseudotime: np.ndarray,
         neigh_conn: np.ndarray,
         **kwargs: Any,
     ) -> np.ndarray:
-        """
-        Calculate biased connections for a given cell.
+        """Calculate biased connections for a given cell.
 
         Parameters
         ----------
         cell_pseudotime
             Pseudotime of the current cell.
         neigh_pseudotime
-            Array of shape ``(n_neighbors,)`` containing pseudotimes of neighbors.
+            Array of shape ``(n_neighbors,)`` containing pseudotime of neighbors.
         neigh_conn
             Array of shape ``(n_neighbors,)`` containing connectivities of the current cell and its neighbors.
 
         Returns
         -------
         Array of shape ``(n_neighbors,)`` containing the biased connectivities.
         """
 
     def _bias_knn_helper(
         self,
         ixs: np.ndarray,
-        conn: csr_matrix,
+        conn: sp.csr_matrix,
         pseudotime: np.ndarray,
         queue=None,
         **kwargs: Any,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-
-        indices, indptr, data = [], [], []
-
+        i, indices, indptr, data = 0, [], [], []
         for i in ixs:
             row = conn[i]
-            biased_row = self(
-                pseudotime[i], pseudotime[row.indices], row.data, **kwargs
-            )
+            biased_row = self(pseudotime[i], pseudotime[row.indices], row.data, **kwargs)
             if np.shape(biased_row) != row.data.shape:
-                raise ValueError(
-                    f"Expected row of shape `{row.data.shape}`, found `{np.shape(biased_row)}`."
-                )
+                raise ValueError(f"Expected row of shape `{row.data.shape}`, found `{np.shape(biased_row)}`.")
 
             data.extend(biased_row)
             indices.extend(row.indices)
             indptr.append(conn.indptr[i])
 
             if queue is not None:
                 queue.put(1)
@@ -73,23 +67,22 @@
             queue.put(None)
 
         return np.array(data), np.array(indices), np.array(indptr)
 
     @d.dedent
     def bias_knn(
         self,
-        conn: csr_matrix,
+        conn: sp.csr_matrix,
         pseudotime: np.ndarray,
         n_jobs: Optional[int] = None,
         backend: str = "loky",
         show_progress_bar: bool = True,
         **kwargs: Any,
-    ) -> csr_matrix:
-        """
-        Bias cell-cell connectivities of a KNN graph.
+    ) -> sp.csr_matrix:
+        """Bias cell-cell connectivities of a KNN graph.
 
         Parameters
         ----------
         conn
             Sparse matrix of shape ``(n_cells, n_cells)`` containing the nearest neighbor connectivities.
         pseudotime
             Pseudotemporal ordering of cells.
@@ -106,71 +99,64 @@
             unit="cell",
             n_jobs=n_jobs,
             backend=backend,
             show_progress_bar=show_progress_bar,
         )(conn, pseudotime, **kwargs)
         data, indices, indptr = zip(*res)
 
-        conn = csr_matrix(
-            (np.concatenate(data), np.concatenate(indices), np.concatenate(indptr))
-        )
+        conn = sp.csr_matrix((np.concatenate(data), np.concatenate(indices), np.concatenate(indptr)))
         conn.eliminate_zeros()
 
         return conn
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}>"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return repr(self)
 
 
 class HardThresholdScheme(ThresholdSchemeABC):
-    """
-    Thresholding scheme inspired by *Palantir* :cite:`setty:19`.
+    """Thresholding scheme inspired by *Palantir* :cite:`setty:19`.
 
-    Note that this won't exactly reproduce the original *Palantir* results, for three reasons:
+    Note that this won't exactly reproduce the original *Palantir* results:
 
-        - *Palantir* computes the KNN graph in a scaled space of diffusion components.
-        - *Palantir* uses its own pseudotime to bias the KNN graph which is not implemented here.
-        - *Palantir* uses a slightly different mechanism to ensure the graph remains connected when removing edges
-          that point into the "pseudotime past".
+    - *Palantir* computes the kNN graph in a scaled space of diffusion components.
+    - *Palantir* uses its own pseudotime to bias the kNN graph which is not implemented here.
+    - *Palantir* uses a slightly different mechanism to ensure the graph remains connected when removing edges
+      that point into the "pseudotime past".
     """
 
     @d.dedent
     def __call__(
         self,
         cell_pseudotime: float,
         neigh_pseudotime: np.ndarray,
         neigh_conn: np.ndarray,
         frac_to_keep: float = 0.3,
     ) -> np.ndarray:
-        """
-        Convert the undirected graph of cell-cell similarities into a directed one by removing "past" edges.
+        """Convert the undirected graph of cell-cell similarities into a directed one by removing "past" edges.
 
         This uses a pseudotemporal measure to remove graph-edges that point into the pseudotime-past. For each cell,
         it keeps the closest neighbors, even if they are in the pseudotime past, to make sure the graph remains
         connected.
 
         Parameters
         ----------
         %(pt_scheme.parameters)s
         frac_to_keep
-            The `frac_to_keep` * n_neighbors closest neighbors (according to graph connectivities) are kept, no matter
-            whether they lie in the pseudotemporal past or future. `frac_to_keep` needs to fall within the
-            interval `[0, 1]`.
+            The ``frac_to_keep`` * n_neighbors closest neighbors (according to graph connectivities) are kept, no matter
+            whether they lie in the pseudotemporal past or future. Must be in :math:`[0, 1]`.
 
         Returns
         -------
         %(pt_scheme.returns)s
         """
         if not (0 <= frac_to_keep <= 1):
-            raise ValueError(
-                f"Expected `frac_to_keep` to be in `[0, 1]`, found `{frac_to_keep}`."
-            )
+            raise ValueError(f"Expected `frac_to_keep` to be in `[0, 1]`, found `{frac_to_keep}`.")
 
         k_thresh = max(0, min(30, int(np.floor(len(neigh_conn) * frac_to_keep))))
         ixs = np.flip(np.argsort(neigh_conn))
         close_ixs, far_ixs = ixs[:k_thresh], ixs[k_thresh:]
 
         mask_keep = cell_pseudotime <= neigh_pseudotime[far_ixs]
         far_ixs_keep = far_ixs[mask_keep]
@@ -179,16 +165,15 @@
         biased_conn[close_ixs] = neigh_conn[close_ixs]
         biased_conn[far_ixs_keep] = neigh_conn[far_ixs_keep]
 
         return biased_conn
 
 
 class SoftThresholdScheme(ThresholdSchemeABC):
-    """
-    Thresholding scheme inspired by :cite:`stassen:21`.
+    """Thresholding scheme inspired by :cite:`stassen:21`.
 
     The idea is to downweight edges that points against the direction of increasing pseudotime. Essentially, the
     further "behind" a query cell is in pseudotime with respect to the current reference cell, the more penalized will
     be its graph-connectivity.
     """
 
     @d.dedent
@@ -196,16 +181,15 @@
         self,
         cell_pseudotime: float,
         neigh_pseudotime: np.ndarray,
         neigh_conn: np.ndarray,
         b: float = 10.0,
         nu: float = 0.5,
     ) -> np.ndarray:
-        """
-        Bias the connectivities by downweighting ones to past cells.
+        """Bias the connectivities by downweighting ones to past cells.
 
         This function uses `generalized logistic regression
         <https://en.wikipedia.org/wiki/Generalized_logistic_function>`_ to weight the past connectivities.
 
         Parameters
         ----------
         %(pt_scheme.parameters)s
@@ -224,42 +208,38 @@
         dt = cell_pseudotime - neigh_pseudotime[past_ixs]
         weights[past_ixs] = 2.0 / ((1.0 + np.exp(b * dt)) ** (1.0 / nu))
 
         return neigh_conn * weights
 
 
 class CustomThresholdScheme(ThresholdSchemeABC):
-    """
-    Class that wraps a user supplied scheme.
+    """Class that wraps a user supplied scheme.
 
     Parameters
     ----------
     callback
         Function which returns the biased connectivities.
     """
 
     def __init__(
         self,
-        callback: Callable[
-            [float, np.ndarray, np.ndarray, np.ndarray, Any], np.ndarray
-        ],
+        callback: Callable[[float, np.ndarray, np.ndarray, np.ndarray, Any], np.ndarray],
     ):
         super().__init__()
         self._callback = callback
 
     @d.dedent
     def __call__(
         self,
         cell_pseudotime: float,
         neigh_pseudotime: np.ndarray,
         neigh_conn: np.ndarray,
         **kwargs: Any,
     ) -> np.ndarray:
-        """
-        %(pt_scheme.summary)s
+        """%(pt_scheme.summary)s
 
         Parameters
         ----------
         %(pt_scheme.parameters)s
         kwargs
             Additional keyword arguments.
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_tmat_flow.py` & `cellrank-2.0.0/src/cellrank/kernels/utils/_tmat_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,65 +1,64 @@
-from typing import Any, List, Tuple, Union, Mapping, Optional, Sequence
-
-from functools import lru_cache
-from dataclasses import dataclass
-from statsmodels.nonparametric.smoothers_lowess import lowess
-
-from anndata import AnnData
-from cellrank import logging as logg
-from cellrank.ul._docs import d
-from cellrank.tl._utils import _unique_order_preserving
-from cellrank.tl._colors import _create_categorical_colors
-from cellrank.tl.kernels._utils import _ensure_numeric_ordered
+import dataclasses
+from typing import Any, List, Mapping, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from scipy.stats import logistic
-from scipy.sparse import issparse, spmatrix
-from pandas.api.types import infer_dtype
+import scipy.sparse as sp
+import scipy.stats as st
+from pandas.api.types import infer_dtype, is_categorical_dtype
 from scipy.interpolate import interp1d
-from pandas.core.dtypes.common import is_categorical_dtype
+from statsmodels.nonparametric.smoothers_lowess import lowess
 
 import matplotlib.pyplot as plt
-from matplotlib.colors import to_rgb
 from matplotlib.collections import PolyCollection
+from matplotlib.colors import to_rgb
+
+from anndata import AnnData
+
+from cellrank import logging as logg
+from cellrank._utils._colors import _create_categorical_colors
+from cellrank._utils._docs import d
+from cellrank._utils._utils import _unique_order_preserving
+from cellrank.kernels._utils import _ensure_numeric_ordered
+
+__all__ = ["FlowPlotter"]
 
 Numeric_t = Union[float, int]
 
 
-@dataclass(frozen=True)
-class Point:  # noqa: D101
+@dataclasses.dataclass(frozen=True)
+class Point:
     x: float
     xt: float
 
 
 @d.dedent
 class FlowPlotter:
-    """
-    Class that plots outgoing flow for a specific cluster :cite:`mittnenzweig:21`.
+    """Class that plots outgoing flow for a specific cluster :cite:`mittnenzweig:21`.
 
-    It should be able to recreate (to a high degree) figures such as Fig. 4a in the above mentioned paper.
+    It should be able to recreate (to a high degree) figures such as Fig. 4a in the above-mentioned paper.
 
     Parameters
     ----------
     %(adata)s
     tmat
         Matrix of shape ``(adata.n_obs, adata.n_obs)``.
     cluster_key
-        Key in :attr:`adata` ``.obs`` where clustering is stored.
+        Key in :attr:`~anndata.AnnData.obs` where clustering is stored.
     time_key
-        Key in :attr:`adata` ``.obs`` where experimental time is stored.
+        Key in :attr:`~anndata.AnnData.obs` where experimental time is stored.
     """
 
     TIME_KEY = "time"
 
     def __init__(
         self,
         adata: AnnData,
-        tmat: Union[np.ndarray, spmatrix],
+        tmat: Union[np.ndarray, sp.spmatrix],
         cluster_key: str,
         time_key: str,
     ):
         self._adata = adata
         self._tmat = tmat
         self._ckey = cluster_key
         self._tkey = time_key
@@ -81,29 +80,28 @@
 
     def prepare(
         self,
         cluster: str,
         clusters: Optional[Sequence[Any]] = None,
         time_points: Optional[Sequence[Numeric_t]] = None,
     ) -> "FlowPlotter":
-        """
-        Prepare itself for plotting by computing flow and contingency matrix.
+        """Prepare itself for plotting by computing flow and contingency matrix.
 
         Parameters
         ----------
         cluster
             Source cluster for flow calculation.
         clusters
-            Target clusters for flow calculation. If `None`, use all clusters.
+            Target clusters for flow calculation. If :obj:`None`, use all clusters.
         time_points
-            Restrict flow calculation only to these time points. If `None`, use all time points.
+            Restrict flow calculation only to these time points. If :obj:`None`, use all time points.
 
         Returns
         -------
-        Returns self and modifies internal internal attributes.
+        Returns and modifies self.
         """
         if clusters is None:
             self._clusters = self.clusters.cat.categories
         else:
             clusters = _unique_order_preserving([cluster] + list(clusters))
             mask = self.clusters.isin(clusters).values
 
@@ -113,35 +111,29 @@
             self._tmat = self._tmat[mask, :][:, mask]
             self._clusters = [c for c in clusters if c in self.clusters.cat.categories]
 
         if cluster not in self._clusters:
             raise ValueError(f"Invalid source cluster `{cluster!r}`.")
 
         if len(self._clusters) < 2:
-            raise ValueError(
-                f"Expected at least `2` clusters, found `{len(clusters)}`."
-            )
+            raise ValueError(f"Expected at least `2` clusters, found `{len(clusters)}`.")
 
         if time_points is not None:
             time_points = _unique_order_preserving(time_points)
             if len(time_points) < 2:
-                raise ValueError(
-                    f"Expected at least `2` time points, found `{len(time_points)}`."
-                )
+                raise ValueError(f"Expected at least `2` time points, found `{len(time_points)}`.")
 
             mask = self.time.isin(time_points)
 
             self._adata = self._adata[mask]
             if not self._adata.n_obs:
                 raise ValueError("No valid time points have been selected.")
             self._tmat = self._tmat[mask, :][:, mask]
 
-        time_points = list(
-            zip(self.time.cat.categories[:-1], self.time.cat.categories[1:])
-        )
+        time_points = list(zip(self.time.cat.categories[:-1], self.time.cat.categories[1:]))
 
         logg.info(
             f"Computing flow from `{cluster}` into `{len(self._clusters) - 1}` cluster(s) "
             f"in `{len(time_points)}` time points"
         )
         self._cluster = cluster
         self._cmat = self.compute_contingency_matrix()
@@ -150,47 +142,47 @@
         return self
 
     def compute_flow(
         self,
         time_points: Sequence[Tuple[Numeric_t, Numeric_t]],
         cluster: Optional[str] = None,
     ) -> pd.DataFrame:
-        """
-        Compute outgoing flow.
+        """Compute outgoing flow.
 
         Parameters
         ----------
         time_points
             Time point pair for which to calculate the flow.
         cluster
-            Cluster for which to calculate the outgoing flow. If `None`, calculate the flow for all clusters.
+            Cluster for which to calculate the outgoing flow. If :obj:`None`, calculate the flow for all clusters.
 
         Returns
         -------
         Dataframe of shape ``(n_time_points, n_clusters)`` if ``cluster != None`` or
         a dataframe of shape ``(n_time_points * n_clusters, n_clusters)`` otherwise.
-        The dataframe's index is a multi-index and the 1st level corresponds to time, the 2nd level to source clusters.
+        The dataframe's index is a multi-index and the 1st level corresponds to time and
+        the 2nd level to source clusters.
         """
 
         def default_helper(t1: Numeric_t, t2: Numeric_t) -> pd.DataFrame:
             subset, row_cls, col_cls = self._get_time_subset(t1, t2)
 
-            df = pd.DataFrame(subset.A if issparse(subset) else subset)
+            df = pd.DataFrame(subset.A if sp.issparse(subset) else subset)
             df = df.groupby(row_cls).sum().T.groupby(col_cls).sum().T
 
             res = pd.DataFrame(np.zeros((n, n)), index=categories, columns=categories)
             res.loc[df.index, df.columns] = df
             res.fillna(0, inplace=True)
 
             return res
 
         def cluster_helper(t1: Numeric_t, t2: Numeric_t) -> pd.DataFrame:
             subset, row_cls, col_cls = self._get_time_subset(t1, t2, cluster=cluster)
 
-            df = pd.DataFrame(subset.A if issparse(subset) else subset).sum(0)
+            df = pd.DataFrame(subset.A if sp.issparse(subset) else subset).sum(0)
             df = df.groupby(col_cls).sum()
             df = pd.DataFrame([df], index=[cluster], columns=df.index)
 
             res = pd.DataFrame(np.zeros((1, n)), index=[cluster], columns=categories)
             res.loc[df.index, df.columns] = df
             res.fillna(0, inplace=True)
 
@@ -226,41 +218,42 @@
         ascending: Optional[bool] = False,
         alpha: float = 0.8,
         xticks_step_size: Optional[int] = 1,
         legend_loc: Optional[str] = "upper right out",
         figsize: Optional[Tuple[float, float]] = None,
         dpi: Optional[int] = None,
     ) -> plt.Axes:
-        """
-        Plot outgoing flow.
+        """Plot outgoing flow.
 
         Parameters
         ----------
         min_flow
-            Only show flow edges with flow greater than this value. Flow values are always in `[0, 1]`.
+            Only show flow edges with flow greater than this value. Flow values are always in :math:`[0, 1]`.
         remove_empty_clusters
             Whether to remove clusters with no incoming flow edges.
         ascending
             Whether to sort the cluster by ascending or descending incoming flow.
             If `None`, use the order as in defined by ``clusters``.
         alpha
             Alpha value for cell proportions.
         xticks_step_size
-            Show only every n-th ticks on x-axis. If `None`, don't show any ticks.
+            Show only every other *n-th* tick on the x-axis. If :obj:`None`, don't show any ticks.
         legend_loc
-            Position of the legend. If `None`, do not show the legend.
+            Position of the legend. If :obj:`None`, do not show the legend.
+        figsize
+            Size of the figure.
+        dpi
+            Dots per inch.
 
         Returns
         -------
         The axes object.
         """
         if self._flow is None or self._cmat is None:
-            raise RuntimeError(
-                "Compute flow and contingency matrix first as `.prepare()`."
-            )
+            raise RuntimeError("Compute flow and contingency matrix first as `.prepare()`.")
 
         flow, cmat = self._flow, self._cmat
         try:
             if remove_empty_clusters:
                 self._remove_min_clusters(min_flow)
             logg.info(
                 f"Plotting flow from `{self._cluster}` into `{len(self._flow.columns) - 1}` cluster(s) "
@@ -278,15 +271,15 @@
             )
         finally:
             self._flow = flow
             self._cmat = cmat
 
     def _get_time_subset(
         self, t1: Numeric_t, t2: Numeric_t, cluster: Optional[str] = None
-    ) -> Tuple[Union[np.ndarray, spmatrix], pd.Series, pd.Series]:
+    ) -> Tuple[Union[np.ndarray, sp.spmatrix], pd.Series, pd.Series]:
         if cluster is None:
             row_ixs = np.where(self.time == t1)[0]
         else:
             row_ixs = np.where((self.time == t1) & (self.clusters == cluster))[0]
 
         col_ixs = np.where(self.time == t2)[0]
         row_cls = self.clusters.values[row_ixs]
@@ -295,59 +288,43 @@
         return self._tmat[row_ixs, :][:, col_ixs], row_cls, col_cls
 
     def _remove_min_clusters(self, min_flow: float) -> None:
         logg.debug("Removing clusters with no incoming flow edges")
         columns = (self._flow.loc[(slice(None), self._cluster), :] > min_flow).any()
         columns = columns[columns].index
         if not len(columns):
-            raise ValueError(
-                "After removing clusters with no incoming flow edges, none remain."
-            )
+            raise ValueError("After removing clusters with no incoming flow edges, none remain.")
         self._flow = self._flow[columns]
 
     def _rename_times(self) -> Sequence[Numeric_t]:
         # make sure we have enough horizontal space to draw the flow (i.e. time points are at least 1 unit apart)
         old_times = self._cmat.columns
         tmp = np.array(old_times)
         tmp = (tmp - tmp.min()) / (tmp.max() - tmp.min())
         tmp /= np.min(tmp[1:] - tmp[:-1])
         time_mapper = dict(zip(old_times, tmp))
-        self._flow.index = pd.MultiIndex.from_tuples(
-            [(time_mapper[t], c) for t, c in self._flow.index]
-        )
+        self._flow.index = pd.MultiIndex.from_tuples([(time_mapper[t], c) for t, c in self._flow.index])
         self._cmat.columns = tmp
         return old_times
 
-    def _order_clusters(
-        self, cluster: str, ascending: Optional[bool] = False
-    ) -> Tuple[List[Any], List[Any]]:
+    def _order_clusters(self, cluster: str, ascending: Optional[bool] = False) -> Tuple[List[Any], List[Any]]:
         if ascending is not None:
             tmp = [[], []]
-            total_flow = (
-                self._flow.loc[(slice(None), cluster), :]
-                .sum()
-                .sort_values(ascending=ascending)
-            )
+            total_flow = self._flow.loc[(slice(None), cluster), :].sum().sort_values(ascending=ascending)
             for i, c in enumerate(c for c in total_flow.index if c != cluster):
                 tmp[i % 2].append(c)
             return tmp[0][::-1], tmp[1]
 
         clusters = [c for c in self._clusters if c != cluster]
         return clusters[: len(clusters) // 2], clusters[len(clusters) // 2 :]
 
-    def _calculate_y_offsets(
-        self, clusters: Sequence[Any], delta: float = 0.2
-    ) -> Mapping[Any, float]:
+    def _calculate_y_offsets(self, clusters: Sequence[Any], delta: float = 0.2) -> Mapping[Any, float]:
         offset = [0]
         for i in range(1, len(clusters)):
-            offset.append(
-                offset[-1]
-                + delta
-                + np.max(self._cmat.loc[clusters[i]] + self._cmat.loc[clusters[i - 1]])
-            )
+            offset.append(offset[-1] + delta + np.max(self._cmat.loc[clusters[i]] + self._cmat.loc[clusters[i - 1]]))
         return dict(zip(clusters, offset))
 
     def _plot_smoothed_proportion(
         self,
         ax: plt.Axes,
         clusters: Sequence[Any],
         y_offset: Mapping[Any, float],
@@ -456,32 +433,28 @@
         ):
             smooth_cluster = float(smoothed_proportions[self._cluster][r(curr_t)])
             flow = self._flow.loc[curr_t]
             for clust in clusters:
                 fl = flow.loc[self._cluster, clust]
                 if fl > min_flow:
                     fl = np.clip(fl, 0, 0.95)
-                    smooth_cluster_fl = smoothed_proportions[self._cluster][
-                        r(curr_t + fl)
-                    ]
+                    smooth_cluster_fl = smoothed_proportions[self._cluster][r(curr_t + fl)]
 
                     if bottom:
                         self._draw_flow_edge(
                             ax,
                             x1=Point(curr_t, 0),
                             x2=Point(next_t - fl, next_t - fl - 0.05),
                             y1=Point(
                                 cluster_offset - smooth_cluster,
                                 cluster_offset - smooth_cluster_fl,
                             ),
                             y2=Point(
-                                y_offset[clust]
-                                + smoothed_proportions[clust][r(next_t)],
-                                y_offset[clust]
-                                + smoothed_proportions[clust][r(next_t - fl - 0.05)],
+                                y_offset[clust] + smoothed_proportions[clust][r(next_t)],
+                                y_offset[clust] + smoothed_proportions[clust][r(next_t - fl - 0.05)],
                             ),
                             flow=fl,
                             start_color=self.cmap[self._cluster],
                             end_color=self.cmap[clust],
                             alpha=alpha,
                         )
                     else:
@@ -490,18 +463,16 @@
                             x1=Point(curr_t + fl, 0),
                             x2=Point(next_t - 0.05, next_t),
                             y1=Point(
                                 cluster_offset + smooth_cluster_fl,
                                 cluster_offset + smooth_cluster,
                             ),
                             y2=Point(
-                                y_offset[clust]
-                                - smoothed_proportions[clust][r(next_t - fl - 0.05)],
-                                y_offset[clust]
-                                - smoothed_proportions[clust][r(next_t)],
+                                y_offset[clust] - smoothed_proportions[clust][r(next_t - fl - 0.05)],
+                                y_offset[clust] - smoothed_proportions[clust][r(next_t)],
                             ),
                             flow=-fl,
                             start_color=self.cmap[self._cluster],
                             end_color=self.cmap[clust],
                             alpha=alpha,
                         )
 
@@ -512,17 +483,15 @@
 
         clusters_bottom, clusters_top = self._order_clusters(self._cluster, ascending)
         all_clusters = clusters_bottom + [self._cluster] + clusters_top
 
         y_offset = self._calculate_y_offsets(all_clusters)
         cluster_offset = y_offset[self._cluster]
 
-        smoothed_proportions, handles = self._plot_smoothed_proportion(
-            ax, all_clusters, y_offset, alpha=alpha
-        )
+        smoothed_proportions, handles = self._plot_smoothed_proportion(ax, all_clusters, y_offset, alpha=alpha)
 
         for curr_t, next_t in zip(times[:-1], times[1:]):
             draw_edges(curr_t, next_t, clusters_bottom, bottom=True)
             draw_edges(curr_t, next_t, clusters_top, bottom=False)
 
         ax.margins(0.025)
         ax.set_title(self._cluster)
@@ -551,25 +520,22 @@
 
     @property
     def time(self) -> pd.Series:
         """Time points."""
         return self._adata.obs[self._tkey]
 
     @property
-    @lru_cache(1)
     def cmap(self) -> Mapping[str, Any]:
         """Colormap for :attr:`clusters`."""
         return dict(
             zip(
                 self.clusters.cat.categories,
                 self._adata.uns.get(
                     f"{self._ckey}_colors",
                     _create_categorical_colors(len(self.clusters.cat.categories)),
                 ),
             )
         )
 
 
-def _lcdf(
-    x: Union[int, float, np.ndarray], loc: float = 0.5, scale: float = 0.2
-) -> float:
-    return logistic.cdf(x, loc=loc, scale=scale)
+def _lcdf(x: Union[int, float, np.ndarray], loc: float = 0.5, scale: float = 0.2) -> float:
+    return st.logistic.cdf(x, loc=loc, scale=scale)
```

### Comparing `cellrank-1.5.1/cellrank/tl/kernels/_velocity_schemes.py` & `cellrank-2.0.0/src/cellrank/kernels/utils/_similarity.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,104 +1,98 @@
+import abc
+import enum
+import functools
 from typing import Any, Tuple
 
-from abc import ABC, abstractmethod
-from enum import auto
-from functools import partial
-
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d
-from cellrank.ul._utils import valuedispatch
-from cellrank.tl.kernels._utils import norm, np_mean, jit_kwargs
-
+import numba as nb
 import numpy as np
-from numba import njit
+
+from cellrank._utils._docs import d
+from cellrank._utils._enum import ModeEnum
+from cellrank.kernels._utils import jit_kwargs, norm, np_mean
+
+__all__ = ["DotProduct", "Cosine", "Correlation", "SimilarityABC"]
 
 
-class Scheme(ModeEnum):  # noqa: D101
-    DOT_PRODUCT = auto()
-    COSINE = auto()
-    CORRELATION = auto()
+class Similarity(ModeEnum):
+    DOT_PRODUCT = enum.auto()
+    COSINE = enum.auto()
+    CORRELATION = enum.auto()
 
 
 try:
     import jax.numpy as jnp
-    from jax import jit, hessian
+    from jax import hessian, jit
 
     @jit
     def _softmax_jax(x: np.ndarray, softmax_scale) -> np.ndarray:
         numerator = x * softmax_scale
         numerator = jnp.exp(numerator - jnp.max(numerator))
         return numerator / jnp.sum(numerator)
 
     @jit
-    def _softmax_masked_jax(
-        x: np.ndarray, mask: np.ndarray, softmax_scale
-    ) -> np.ndarray:
+    def _softmax_masked_jax(x: np.ndarray, mask: np.ndarray, softmax_scale) -> np.ndarray:
         numerator = x * softmax_scale
         numerator = jnp.exp(numerator - jnp.nanmax(numerator))
         numerator = jnp.where(mask, 0, numerator)  # essential
 
         return numerator / jnp.nansum(numerator)
 
-    @partial(jit, static_argnums=(3, 4))
+    @functools.partial(jit, static_argnums=(3, 4))
     def _predict_transition_probabilities_jax(
         X: np.ndarray,
         W: np.ndarray,
         softmax_scale: float = 1.0,
         center_mean: bool = True,
         scale_by_norm: bool = True,
-    ):
+    ) -> np.ndarray:
         if center_mean:
             # pearson correlation, otherwise cosine
             W -= W.mean(axis=1)[:, None]
             X -= X.mean()
 
         if scale_by_norm:
             denom = jnp.linalg.norm(X) * jnp.linalg.norm(W, axis=1)
             mask = jnp.isclose(denom, 0)
             denom = jnp.where(jnp.isclose(denom, 0), 1, denom)  # essential
             return _softmax_masked_jax(W.dot(X) / denom, mask, softmax_scale)
 
         return _softmax_jax(W.dot(X), softmax_scale)
 
-    _predict_transition_probabilities_jax_H = hessian(
-        _predict_transition_probabilities_jax
-    )
+    _predict_transition_probabilities_jax_H = hessian(_predict_transition_probabilities_jax)
 
     _HAS_JAX = True
 except ImportError:
     _HAS_JAX = False
 
     hessian = jit = lambda _: _
 
     def _predict_transition_probabilities_jax(*_args, **_kwargs):
         raise NotImplementedError("No `jax` installation found.")
 
     _predict_transition_probabilities_jax_H = _predict_transition_probabilities_jax
 
 
-@njit(**jit_kwargs)
+@nb.njit(**jit_kwargs)
 def _softmax(x: np.ndarray, softmax_scale: float) -> Tuple[np.ndarray, np.ndarray]:
     numerator = x * softmax_scale
     numerator = np.exp(numerator - np.max(numerator))
     return numerator / np.sum(numerator), x
 
 
-@njit(**jit_kwargs)
-def _softmax_masked(
-    x: np.ndarray, mask: np.ndarray, softmax_scale: float
-) -> Tuple[np.ndarray, np.ndarray]:
+@nb.njit(**jit_kwargs)
+def _softmax_masked(x: np.ndarray, mask: np.ndarray, softmax_scale: float) -> Tuple[np.ndarray, np.ndarray]:
     numerator = x * softmax_scale
     numerator = np.exp(numerator - np.nanmax(numerator))
     numerator = np.where(mask, 0, numerator)  # essential
 
     return numerator / np.nansum(numerator), x
 
 
-@njit(parallel=False, **jit_kwargs)
+@nb.njit(parallel=False, **jit_kwargs)
 def _predict_transition_probabilities_numpy(
     X: np.ndarray,
     W: np.ndarray,
     softmax_scale: float = 1.0,
     center_mean: bool = True,
     scale_by_norm: bool = True,
 ) -> Tuple[np.ndarray, np.ndarray]:
@@ -131,28 +125,23 @@
         denom[mask] = 1
         return _softmax_masked(
             np.array([np.dot(X[i], W[i]) for i in range(X.shape[0])]) / denom,
             mask,
             softmax_scale,
         )
 
-    return _softmax(
-        np.array([np.dot(X[i], W[i]) for i in range(X.shape[0])]), softmax_scale
-    )
+    return _softmax(np.array([np.dot(X[i], W[i]) for i in range(X.shape[0])]), softmax_scale)
 
 
-class Hessian(ABC):  # noqa: D101
+class Hessian(abc.ABC):
     @d.get_full_description(base="hessian")
     @d.get_sections(base="hessian", sections=["Parameters", "Returns"])
-    @abstractmethod
-    def hessian(
-        self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0
-    ) -> np.ndarray:
-        """
-        Compute the Hessian.
+    @abc.abstractmethod
+    def hessian(self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0) -> np.ndarray:
+        """Compute the Hessian.
 
         Parameters
         ----------
         v
             Array of shape ``(n_genes,)`` containing the velocity vector.
         D
             Array of shape ``(n_neighbors, n_genes)`` corresponding to the transcriptomic displacement of the current
@@ -165,170 +154,146 @@
         The full Hessian of shape ``(n_neighbors, n_genes, n_genes)`` or only its diagonal of shape
         ``(n_neighbors, n_genes)``.
 
         Developer notes
         ---------------
         This class should be used in conjunction with any class that implements the ``__call__`` method and should
         compute the Hessian of such function. This it does not need to handle the case of a backward process,
-        i.e. when the velocity vector `v` is of shape ``(n_genes, n_neighbors)``.
+        i.e., when the velocity vector :math:`v` is of shape ``(n_genes, n_neighbors)``.
 
-        If using :mod:`jax` to compute the Hessian, please specify a class attribute ``__use_jax__ = True``.
+        If using :mod:`jax` to compute the Hessian, please specify the class attribute ``__use_jax__ = True``.
         """
 
 
-class SimilaritySchemeABC(ABC):
+class SimilarityABC(abc.ABC):
     """Base class for all similarity schemes."""
 
     @d.get_full_description(base="sim_scheme")
     @d.get_sections(base="sim_scheme", sections=["Parameters", "Returns"])
-    @abstractmethod
-    def __call__(
-        self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        Compute transition probability of a cell to its nearest neighbors using RNA velocity.
+    @abc.abstractmethod
+    def __call__(self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0) -> Tuple[np.ndarray, np.ndarray]:
+        """Compute transition probability of a cell to its nearest neighbors using RNA velocity.
 
         Parameters
         ----------
         v
             Array of shape ``(n_genes,)`` or ``(n_neighbors, n_genes)`` containing the velocity vector(s).
             The second case is used for the backward process.
         D
             Array of shape ``(n_neighbors, n_genes)`` corresponding to the transcriptomic displacement of the current
             cell with respect to ist nearest neighbors.
         softmax_scale
             Scaling factor for the softmax function.
 
         Returns
         -------
-        The probability and logits arrays of shape ``(n_neighbors,)``.
+        The probability and unscaled logits arrays of shape ``(n_neighbors,)``.
         """
 
+    @staticmethod
+    def create(scheme: Similarity) -> "SimilarityABC":
+        if scheme == Similarity.CORRELATION:
+            return Correlation()
+        if scheme == Similarity.COSINE:
+            return Cosine()
+        if scheme == Similarity.DOT_PRODUCT:
+            return DotProduct()
+        raise NotImplementedError(scheme)
+
     def __repr__(self):
         return f"<{self.__class__.__name__}>"
 
     def __str__(self):
         return repr(self)
 
 
-class SimilaritySchemeHessian(SimilaritySchemeABC, Hessian):
-    """
-    Base class for all similarity schemes as defined in :cite:`li:20`.
+class SimilarityHessian(SimilarityABC, Hessian):
+    """Base class for all similarity schemes as defined in :cite:`li:20`.
 
     Parameters
     ----------
     center_mean
-        Whether to center the velocity vector(s) and the transcriptomic displacement matrix.
+        Whether to center the velocity vectors and the transcriptomic displacement matrix.
     scale_by_norm
-        Whether to scale the velocity vector(s) and the transcriptomic displacement matrix by their norms.
+        Whether to scale the velocity vectors) and the transcriptomic displacement matrix by their norms.
     """
 
     __use_jax__: bool = True
 
     def __init__(self, center_mean: bool, scale_by_norm: bool):
         self._center_mean = center_mean
         self._scale_by_norm = scale_by_norm
 
     @d.dedent
-    def __call__(
-        self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        %(sim_scheme.full_desc)s
+    def __call__(self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0) -> Tuple[np.ndarray, np.ndarray]:
+        """%(sim_scheme.full_desc)s
 
         Parameters
         ----------
         %(sim_scheme.parameters)s
 
         Returns
         -------
         %(sim_scheme.returns)s
         """  # noqa: D400
-        return _predict_transition_probabilities_numpy(
-            v, D, softmax_scale, self._center_mean, self._scale_by_norm
-        )
+        return _predict_transition_probabilities_numpy(v, D, softmax_scale, self._center_mean, self._scale_by_norm)
 
     @d.dedent
-    def hessian(
-        self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0
-    ) -> np.ndarray:
-        """
-        %(hessian.full_desc)s
+    def hessian(self, v: np.ndarray, D: np.ndarray, softmax_scale: float = 1.0) -> np.ndarray:
+        """%(hessian.full_desc)s
 
         Parameters
         ----------
         %(hessian.parameters)s
 
         Returns
         -------
         %(hessian.returns)s
         """  # noqa: D400
-        return _predict_transition_probabilities_jax_H(
-            v, D, softmax_scale, self._center_mean, self._scale_by_norm
-        )
+        return _predict_transition_probabilities_jax_H(v, D, softmax_scale, self._center_mean, self._scale_by_norm)
 
     def __getattribute__(self, name: str) -> Any:
         if name == "hessian" and self.__use_jax__ and not _HAS_JAX:
             raise NotImplementedError("No `jax` installation found.")
         return super().__getattribute__(name)
 
 
-class DotProductScheme(SimilaritySchemeHessian):
-    r"""
-    Dot product scheme as defined in eq. (4.9) :cite:`li:20`.
+class DotProduct(SimilarityHessian):
+    r"""Dot product scheme as defined in eq. (4.9) :cite:`li:20`.
 
-        :math:`v(s_i, s_j) = g(\delta_{i, j}^T v_i)`
+    .. math::
+        v(s_i, s_j) := g(\delta_{i, j}^T v_i)
 
     where :math:`v_i` is the velocity vector of cell :math:`i`, :math:`\delta_{i, j}` corresponds to the transcriptional
     displacement between cells :math:`i` and :math:`j` and :math:`g` is a softmax function with some scaling parameter.
     """
 
     def __init__(self):
         super().__init__(center_mean=False, scale_by_norm=False)
 
 
-class CosineScheme(SimilaritySchemeHessian):
-    r"""
-    Cosine similarity scheme as defined in eq. (4.7) :cite:`li:20`.
+class Cosine(SimilarityHessian):
+    r"""Cosine similarity scheme as defined in eq. (4.7) :cite:`li:20`.
 
-        :math:`v(s_i, s_j) = g(cos(\delta_{i, j}, v_i))`
+    .. math::
+        v(s_i, s_j) := g(cos(\delta_{i, j}, v_i))
 
     where :math:`v_i` is the velocity vector of cell :math:`i`, :math:`\delta_{i, j}` corresponds to the transcriptional
     displacement between cells :math:`i` and :math:`j` and :math:`g` is a softmax function with some scaling parameter.
     """
 
     def __init__(self):
         super().__init__(center_mean=False, scale_by_norm=True)
 
 
-class CorrelationScheme(SimilaritySchemeHessian):
-    r"""
-    Pearson correlation scheme as defined in eq. (4.8) :cite:`li:20`.
+class Correlation(SimilarityHessian):
+    r"""Pearson correlation scheme as defined in eq. (4.8) :cite:`li:20`.
 
-        :math:`v(s_i, s_j) = g(corr(\delta_{i, j}, v_i))`
+    .. math::
+        v(s_i, s_j) := g(corr(\delta_{i, j}, v_i))
 
     where :math:`v_i` is the velocity vector of cell :math:`i`, :math:`\delta_{i, j}` corresponds to the transcriptional
     displacement between cells :math:`i` and :math:`j` and :math:`g` is a softmax function with some scaling parameter.
     """
 
     def __init__(self):
         super().__init__(center_mean=True, scale_by_norm=True)
-
-
-@valuedispatch
-def _get_scheme(scheme: Scheme, *_args, **_kwargs) -> SimilaritySchemeABC:
-    raise NotImplementedError(scheme)
-
-
-@_get_scheme.register(Scheme.DOT_PRODUCT)
-def _():
-    return DotProductScheme()
-
-
-@_get_scheme.register(Scheme.COSINE)
-def _():
-    return CosineScheme()
-
-
-@_get_scheme.register(Scheme.CORRELATION)
-def _():
-    return CorrelationScheme()
```

### Comparing `cellrank-1.5.1/cellrank/ul/_docs.py` & `cellrank-2.0.0/src/cellrank/_utils/_docs.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,183 +1,204 @@
+import textwrap
 from typing import Any
 
 from docrep import DocstringProcessor
-from textwrap import dedent
+
+__all__ = ["d", "inject_docs"]
 
 _adata = """\
-adata : :class:`anndata.AnnData`
+adata
     Annotated data object."""
 _adata_ret = """\
 :class:`anndata.AnnData`
     Annotated data object."""
 _plotting = """\
 figsize
     Size of the figure.
 dpi
     Dots per inch.
 save
     Filename where to save the plot."""
 _n_jobs = """\
 n_jobs
-    Number of parallel jobs. If `-1`, use all available cores. If `None` or `1`, the execution is sequential."""
+    Number of parallel jobs. If -1, use all available cores. If :obj:`None` or 1, the execution is sequential."""
 _parallel = f"""\
 show_progress_bar
     Whether to show a progress bar. Disabling it may slightly improve performance.
 {_n_jobs}
 backend
-    Which backend to use for parallelization. See :class:`joblib.Parallel` for valid options."""
+    Which backend to use for parallelization. See :class:`~joblib.Parallel` for valid options."""
 _model = """\
 model
-    Model based on :class:`cellrank.ul.models.BaseModel` to fit.
-
+    Model based on :class:`~cellrank.models.BaseModel` to fit.
     If a :class:`dict`, gene and lineage specific models can be specified. Use ``'*'`` to indicate
     all genes or lineages, for example ``{'gene_1': {'*': ...}, 'gene_2': {'lineage_1': ..., '*': ...}}``."""
 _just_plots = """\
 Nothing, just plots the figure. Optionally saves it based on ``save``."""
 _plots_or_returns_models = """\
-None
-    If ``return_models = False``, just plots the figure and optionally saves it based on ``save``.
-Dict[str, Dict[str, :class:`cellrank.ul.models.BaseModel`]]
-    Otherwise returns the fitted models as ``{'gene_1': {'lineage_1': <model_11>, ...}, ...}``.
-    Models which have failed will be instances of :class:`cellrank.ul.models.FailedModel`."""
+If ``return_models = False``, just plots the figure and optionally saves it based on ``save``.
+Otherwise returns the fitted models as ``{'gene_1': {'lineage_1': <model_11>, ...}, ...}``.
+Models which have failed will be instances of :class:`cellrank.models.FailedModel`."""
 _backward = """\
 backward
     Direction of the process."""
 _eigen = """\
 which
     How to sort the eigenvalues. Valid option are:
 
-        - `'LR'` - the largest real part.
-        - `'LM'` - the largest magnitude.
+    - ``'LR'`` - the largest real part.
+    - ``'LM'`` - the largest magnitude.
 alpha
     Used to compute the *eigengap*. ``alpha`` is the weight given to the deviation of an eigenvalue from one."""
 _n_cells = """\
 n_cells
     Number of most likely cells from each macrostate to select."""
 _fit = """\
 n_lineages
-    Number of lineages. If `None`, it will be determined automatically.
+    Number of lineages. If :obj:`None`, it will be determined automatically.
 cluster_key
     Match computed states against pre-computed clusters to annotate the states.
-    For this, provide a key from :attr:`adata` ``.obs`` where cluster labels have been computed.
+    For this, provide a key from :attr:`anndata.AnnData.obs` where cluster labels have been computed.
 keys
-    Determines which %(initial_or_terminal)s states to use by passing their names.
-    Further, %(initial_or_terminal)s states can be combined. If e.g. the %(terminal)s states are
-    ['Neuronal_1', 'Neuronal_1', 'Astrocytes', 'OPC'], then passing ``keys=['Neuronal_1, Neuronal_2', 'OPC']``
-    means that the two neuronal %(terminal)s states are treated as one and the 'Astrocyte' state is excluded."""
+    Determines which states to use by passing their names. Furthermore, these states can be combined, e.g.,
+    if the states are ``['Neuronal_1', 'Neuronal_1', 'OPC']``, then passing
+    ``keys = ['Neuronal_1, Neuronal_2', 'OPC']`` means that the two neuronal states are treated as one."""
 _density_correction = (
     "Optionally, we apply a density correction as described in :cite:`coifman:05`, "
     "where we use the implementation of :cite:`haghverdi:16`."
 )
 _time_range = """\
 time_range
     Specify start and end times:
 
-        - If a :class:`tuple`, it specifies the minimum and maximum pseudotime. Both values can be `None`,
-          in which case the minimum is the earliest pseudotime and the maximum is automatically determined.
-        - If a :class:`float`, it specifies the maximum pseudotime."""
+    - :class:`tuple` - it specifies the minimum and maximum pseudotime. Both values can be :obj:`None`,
+      in which case the minimum is the earliest pseudotime and the maximum is automatically determined.
+    - :class:`float` - it specifies the maximum pseudotime."""
 
 _velocity_mode = """\
 mode
     How to compute transition probabilities. Valid options are:
 
-        - `{m.DETERMINISTIC!r}` - deterministic computation that doesn't propagate uncertainty.
-        - `{m.MONTE_CARLO!r}` - Monte Carlo average of randomly sampled velocity vectors.
-        - `{m.STOCHASTIC!r}` - second order approximation, only available when :mod:`jax` is installed.
-        - `{m.SAMPLING!r}` - sample 1 transition matrix from the velocity distribution."""
+    - ``{m.DETERMINISTIC!r}`` - deterministic computation that doesn't propagate uncertainty.
+    - ``{m.MONTE_CARLO!r}`` - Monte Carlo average of randomly sampled velocity vectors.
+    - ``{m.STOCHASTIC!r}`` - second order approximation, only available when :mod:`jax` is installed."""
 _velocity_backward_mode = """\
 backward_mode
-    Only matters if initialized as :attr:`backward` ``= True``.  Valid options are:
+    Only matters if initialized as :attr:`backward = True <backward>`. Valid options are:
 
-        - `{b.TRANSPOSE!r}` - compute transitions from neighboring cells :math:`j` to cell :math:`i`.
-        - `{b.NEGATE!r}` - negate the velocity vector."""
-_velocity_backward_mode_high_lvl = """\
-backward_mode
-    How to compute the backward transitions. Valid options are:
-
-        - `{b.TRANSPOSE!r}` - compute transitions from neighboring cells :math:`j` to cell :math:`i`.
-        - `{b.NEGATE!r}` - negate the velocity vector."""
+    - ``{b.TRANSPOSE!r}`` - compute transitions from neighboring cells :math:`j` to cell :math:`i`.
+    - ``{b.NEGATE!r}`` - negate the velocity vector."""
 _copy = """Return a copy of self."""
 _initial = "initial"
 _terminal = "terminal"
 _model_callback = """\
 callback
-    Function which takes a :class:`cellrank.ul.models.BaseModel` and some keyword arguments
-    for :meth:`cellrank.ul.models.BaseModel.prepare` and returns the prepared model.
-    Can be specified in gene- and lineage-specific manner, similarly to :attr:`model`."""
+    Function which takes a :class:`~cellrank.models.BaseModel` and some keyword arguments
+    for :meth:`~cellrank.models.BaseModel.prepare` and returns the prepared model.
+    Can be specified in gene- and lineage-specific manner, similarly to the :attr:`model`."""
 _genes = """\
 genes
-    Genes in :attr:`anndata.AnnData.var_names` or in :attr:`anndata.AnnData.raw.var_names`, if ``use_raw = True``."""
+    Genes in :attr:`~anndata.AnnData.var_names`."""
 _softmax_scale = """\
 softmax_scale
-    Scaling parameter for the softmax. If `None`, it will be estimated using ``1 / median(correlations)``.
+    Scaling parameter for the softmax. If :obj:`None`, it will be estimated using ``1 / median(correlations)``.
     The idea behind this is to scale the softmax to counter everything tending to orthogonality in high dimensions."""
 _time_mode = """\
 mode
     Valid options are:
 
-        - `'embedding'` - plot the embedding while coloring in continuous or categorical observations.
-        - `'time'` - plot the pseudotime on x-axis and the probabilities/memberships on y-axis."""
+    - ``'embedding'`` - plot the embedding while coloring in continuous or categorical observations.
+    - ``'time'`` - plot the pseudotime on x-axis and the probabilities/memberships on y-axis."""
 _write_to_adata = """\
 Updates the :attr:`adata` with the following fields:
 
-        - ``.obsp['{{key}}']`` - the transition matrix.
-        - ``.uns['{{key}}_params']`` - parameters used for calculation."""
+- :attr:`obsp['{{key}}'] <anndata.AnnData.obsp>` - the transition matrix.
+- :attr:`uns['{{key}}_params'] <anndata.AnnData.uns>` - parameters used for the calculation."""
 _en_cutoff_p_thresh = """\
 en_cutoff
     If ``cluster_key`` is given, this parameter determines when an approximate recurrent class will
     be labeled as *'Unknown'*, based on the entropy of the distribution of cells over transcriptomic clusters.
 p_thresh
     If cell cycle scores were provided, a *Wilcoxon rank-sum test* is conducted to identify cell-cycle states.
     If the test returns a positive statistic and a p-value smaller than ``p_thresh``, a warning will be issued."""
 _return_models = """\
 return_models
-    If `True`, return the fitted models for each gene in ``genes`` and lineage in ``lineages``."""
+    If :obj:`True`, return the fitted models for each gene in ``genes`` and lineage in ``lineages``."""
 _basis = """\
 basis
-    Basis to use when ``mode = 'embedding'``. If `None`, use `'umap'`."""
+    Basis to use when ``mode = 'embedding'``. If :obj:`None`, use ``'umap'``."""
 _velocity_scheme = """\
-scheme
-    Similarity scheme between cells as described in :cite:`li:20`. Can be one of the following:
+similarity
+    Similarity measure between cells as described in :cite:`li:20`. Valid options are:
 
-        - `{s.DOT_PRODUCT!r}` - :class:`cellrank.tl.kernels.DotProductScheme`.
-        - `{s.COSINE!r}` - :class:`cellrank.tl.kernels.CosineScheme`.
-        - `{s.CORRELATION!r}` - :class:`cellrank.tl.kernels.CorrelationScheme`.
+    - ``{s.CORRELATION!r}`` - :class:`~cellrank.kernels.utils.Correlation`.
+    - ``{s.COSINE!r}`` - :class:`~cellrank.kernels.utils.Cosine`.
+    - ``{s.DOT_PRODUCT!r}`` - :class:`~cellrank.kernels.utils.DotProduct`.
 
     Alternatively, any function can be passed as long as it follows the signature of
-    :meth:`cellrank.tl.kernels.SimilaritySchemeABC.__call__`."""
+    :meth:`cellrank.kernels.utils.SimilarityABC.__call__`."""
 _cond_num = """\
 compute_cond_num
     Whether to compute condition number of the transition matrix. Note that this might be costly,
     since it does not use sparse implementation."""
 _soft_scheme_fmt = """\
 b
     The growth rate of generalized logistic function.{}
 nu
     Affects near which asymptote maximum growth occurs.{}"""
 _rw_ixs = """\
 Can be specified as:
 
-        - :class:`dict` - dictionary with 1 key in :attr:`anndata.AnnData.obs` with values corresponding
-          to either 1 or more clusters (if the column is categorical) or a :class:`tuple` specifying
-          `[min, max]` interval from which to select the indices.
-        - :class:`typing.Sequence` - sequence of cell ids in :attr:`anndata.AnnData.obs_names`.
+    - :class:`dict` - dictionary with 1 key in :attr:`~anndata.AnnData.obs` with values corresponding
+      to either 1 or more clusters (if the column is categorical) or a :class:`tuple` specifying
+      :math:`[min, max]` interval from which to select the indices.
+    - :class:`~typing.Sequence` - sequence of cell ids in :attr:`~anndata.AnnData.obs_names`.
 """
 _gene_symbols = """\
 gene_symbols
-    Key in :attr:`anndata.AnnData.var` to use instead of :attr:`anndata.AnnData.var_names`."""
+    Key in :attr:`~anndata.AnnData.var` to use instead of :attr:`~anndata.AnnData.var_names`."""
+_absorption_utils = """\
+solver
+    Solver to use for the linear problem. Options are ``'direct'``, ``'gmres'``, ``'lgmres'``, ``'bicgstab'`` or
+    ``'gcrotmk'`` when ``use_petsc = False``.
+
+    Information on the :mod:`scipy` iterative solvers can be found in :mod:`scipy.sparse.linalg` or for
+    the ``petsc`` solvers `here <https://petsc.org/release/overview/linear_solve_table/>`__.
+use_petsc
+    Whether to use solvers from :mod:`petsc4py` or :mod:`scipy`. Recommended for large problems.
+    If no installation is found, defaults to :func:`~scipy.sparse.linalg.gmres`.
+n_jobs
+    Number of parallel jobs to use when using an iterative solver.
+backend
+    Which backend to use for multiprocessing. See :class:`~joblib.Parallel` for valid options.
+show_progress_bar
+    Whether to show progress bar. Only used when ``solver != 'direct'``.
+tol
+    Convergence tolerance for the iterative solver. The default is fine for most cases, only consider
+    decreasing this for severely ill-conditioned matrices.
+preconditioner
+    Preconditioner to use, only available when ``use_petsc = True``. For valid options, see
+    `here <https://petsc.org/release/docs/manual/ksp/?highlight=pctype#preconditioners>`__.
+    We recommend the ``'ilu'`` preconditioner for badly conditioned problems."""
+which = """\
+which
+    Whether to compute initial or terminal states."""
+allow_overlap = """\
+allow_overlap
+    Whether to allow overlapping names between initial and terminal states.
+"""
 
 
-def inject_docs(**kwargs: Any):  # noqa
+def inject_docs(**kwargs: Any):
     def decorator(obj):
-        obj.__doc__ = dedent(obj.__doc__).format(**kwargs)
+        obj.__doc__ = textwrap.dedent(obj.__doc__).format(**kwargs)
         return obj
 
     def decorator2(obj):
-        obj.__doc__ = dedent(kwargs["__doc__"])
+        obj.__doc__ = textwrap.dedent(kwargs["__doc__"])
         return obj
 
     if isinstance(kwargs.get("__doc__", None), str) and len(kwargs) == 1:
         return decorator2
 
     return decorator
 
@@ -198,26 +219,26 @@
     n_cells=_n_cells,
     fit=_fit,
     copy=_copy,
     density_correction=_density_correction,
     time_range=_time_range,
     velocity_mode=_velocity_mode,
     velocity_backward_mode=_velocity_backward_mode,
-    velocity_backward_mode_high_lvl=_velocity_backward_mode_high_lvl,
     model_callback=_model_callback,
     genes=_genes,
     softmax_scale=_softmax_scale,
     time_mode=_time_mode,
     write_to_adata=_write_to_adata,
     en_cutoff_p_thresh=_en_cutoff_p_thresh,
     return_models=_return_models,
     plots_or_returns_models=_plots_or_returns_models,
     basis=_basis,
     velocity_scheme=_velocity_scheme,
     cond_num=_cond_num,
     soft_scheme=_soft_scheme_fmt.format("", "", ""),
-    soft_scheme_kernel=_soft_scheme_fmt.format(
-        *([" Only used when ``threshold_scheme = 'soft'``."] * 3)
-    ),
+    soft_scheme_kernel=_soft_scheme_fmt.format(*([" Only used when ``threshold_scheme = 'soft'``."] * 3)),
     rw_ixs=_rw_ixs,
     gene_symbols=_gene_symbols,
+    absorption_utils=_absorption_utils,
+    which=which,
+    allow_overlap=allow_overlap,
 )
```

### Comparing `cellrank-1.5.1/cellrank/ul/_parallelize.py` & `cellrank-2.0.0/src/cellrank/_utils/_parallelize.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,39 @@
-"""Module used to parallelize model fitting."""
-
-from typing import Any, Union, Callable, Optional, Sequence
+import multiprocessing
+import threading
+from typing import Any, Callable, Optional, Sequence, Union
 
 import joblib as jl
-from threading import Thread
-from multiprocessing import Manager
-
-from cellrank.ul._utils import _get_n_cores
 
 import numpy as np
-from scipy.sparse import issparse, spmatrix
+import scipy.sparse as sp
+
+__all__ = ["parallelize", "_get_n_cores"]
 
 
 def parallelize(
     callback: Callable[[Any], Any],
-    collection: Union[spmatrix, Sequence[Any]],
+    collection: Union[sp.spmatrix, Sequence[Any]],
     n_jobs: Optional[int] = None,
     n_split: Optional[int] = None,
     unit: str = "",
     as_array: bool = True,
     use_ixs: bool = False,
     backend: str = "loky",
     extractor: Optional[Callable[[Any], Any]] = None,
     show_progress_bar: bool = True,
 ) -> Any:
-    """
-    Parallelize function call over a collection of elements.
+    """Parallelize function call over a collection of elements.
 
     Parameters
     ----------
     callback
         Function to parallelize.
     collection
-        Sequence of items which to chunkify or an already .
+        Sequence of items which to chunkify or an already chunked array.
     n_jobs
         Number of parallel jobs.
     n_split
         Split ``collection`` into ``n_split`` chunks. If `None`, split into ``n_jobs`` chunks.
     unit
         Unit of the progress bar.
     as_array
@@ -50,18 +47,16 @@
     show_progress_bar
         Whether to show a progress bar.
 
     Returns
     -------
     The result depending on ``callable``, ``extractor`` and ``as_array``.
     """
-
     if show_progress_bar:
         try:
-            import ipywidgets
             from tqdm.auto import tqdm
         except ImportError:
             try:
                 from tqdm.std import tqdm
             except ImportError:
                 tqdm = None
     else:
@@ -70,17 +65,15 @@
     def update(pbar, queue, n_total):
         n_finished = 0
         while n_finished < n_total:
             try:
                 res = queue.get()
             except EOFError as e:
                 if not n_finished != n_total:
-                    raise RuntimeError(
-                        f"Finished only `{n_finished}` out of `{n_total}` tasks.`"
-                    ) from e
+                    raise RuntimeError(f"Finished only `{n_finished}` out of `{n_total}` tasks.`") from e
                 break
             assert res in (None, (1, None), 1)  # (None, 1) means only 1 job
             if res == (1, None):
                 n_finished += 1
                 if pbar is not None:
                     pbar.update()
             elif res is None:
@@ -89,21 +82,17 @@
                 pbar.update()
 
         if pbar is not None:
             pbar.close()
 
     def wrapper(*args, **kwargs):
         if pass_queue and show_progress_bar:
-            pbar = (
-                None
-                if tqdm is None
-                else tqdm(total=col_len, unit=unit, mininterval=0.125)
-            )
-            queue = Manager().Queue()
-            thread = Thread(target=update, args=(pbar, queue, len(collections)))
+            pbar = None if tqdm is None else tqdm(total=col_len, unit=unit, mininterval=0.125)
+            queue = multiprocessing.Manager().Queue()
+            thread = threading.Thread(target=update, args=(pbar, queue, len(collections)))
             thread.start()
         else:
             pbar, queue, thread = None, None, None
 
         res = jl.Parallel(n_jobs=n_jobs, backend=backend)(
             jl.delayed(callback)(
                 *((i, cs) if use_ixs else (cs,)),
@@ -116,35 +105,55 @@
 
         res = np.array(res) if as_array else res
         if thread is not None:
             thread.join()
 
         return res if extractor is None else extractor(res)
 
-    col_len = collection.shape[0] if issparse(collection) else len(collection)
+    col_len = collection.shape[0] if sp.issparse(collection) else len(collection)
     n_jobs = _get_n_cores(n_jobs, col_len)
     if n_split is None:
         n_split = n_jobs
 
-    if issparse(collection):
+    if sp.issparse(collection):
         n_split = max(1, min(n_split, collection.shape[0]))
         if n_split == collection.shape[0]:
             collections = [collection[[ix], :] for ix in range(collection.shape[0])]
         else:
             step = collection.shape[0] // n_split
-            ixs = [
-                np.arange(i * step, min((i + 1) * step, collection.shape[0]))
-                for i in range(n_split)
-            ]
-            ixs[-1] = np.append(
-                ixs[-1], np.arange(ixs[-1][-1] + 1, collection.shape[0])
-            )
+            ixs = [np.arange(i * step, min((i + 1) * step, collection.shape[0])) for i in range(n_split)]
+            ixs[-1] = np.append(ixs[-1], np.arange(ixs[-1][-1] + 1, collection.shape[0]))
 
             collections = [collection[ix, :] for ix in filter(len, ixs)]
     else:
         collections = list(filter(len, np.array_split(collection, n_split)))
 
     n_split = len(collections)
     n_jobs = min(n_jobs, n_split)
     pass_queue = not hasattr(callback, "py_func")  # we'd be inside a numba function
 
     return wrapper
+
+
+def _get_n_cores(n_cores: Optional[int], n_jobs: Optional[int]) -> int:
+    """Make number of cores a positive integer.
+
+    Parameters
+    ----------
+    n_cores
+        Number of cores to use.
+    n_jobs.
+        Number of jobs. This is just used to determine if the collection is a singleton.
+        If `1`, always returns `1`.
+
+    Returns
+    -------
+    Positive integer corresponding to how many cores to use.
+    """
+    if n_cores == 0:
+        raise ValueError("Number of cores cannot be `0`.")
+    if n_jobs == 1 or n_cores is None:
+        return 1
+    if n_cores < 0:
+        return multiprocessing.cpu_count() + 1 + n_cores
+
+    return n_cores
```

### Comparing `cellrank-1.5.1/cellrank/ul/models/_gamr_model.py` & `cellrank-2.0.0/src/cellrank/models/_gamr_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,138 +1,128 @@
-"""Module containing all models interfacing R's mgcv package."""
-from typing import Any, Tuple, Union, Optional
-from typing_extensions import Literal
-
-from copy import copy, deepcopy
-from enum import auto
-
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d, inject_docs
-from cellrank.ul.models import BaseModel
-from cellrank.ul.models._utils import _OFFSET_KEY, _get_offset, _get_knotlocs
-from cellrank.ul.models._base_model import AnnData, FailedModel
+import copy
+import enum
+from typing import Any, Literal, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
-from scipy.stats import norm
+import scipy.stats as st
 
+from anndata import AnnData
+
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import ModeEnum
+from cellrank.models import BaseModel, FailedModel
+from cellrank.models._utils import _OFFSET_KEY, _get_knotlocs, _get_offset
+
+__all__ = ["GAMR"]
+
+# cache so we don't have to re-load
 _r_lib = None
 _r_lib_name = None
 
 
-class KnotLocs(ModeEnum):  # noqa: D101
-    AUTO = auto()
-    DENSITY = auto()
+class KnotLocs(ModeEnum):
+    AUTO = enum.auto()
+    DENSITY = enum.auto()
 
 
 @inject_docs(key=_OFFSET_KEY, kloc=KnotLocs)
 @d.dedent
 class GAMR(BaseModel):
-    """
-    Wrapper around R's `mgcv <https://cran.r-project.org/web/packages/mgcv/>`__ package for fitting
-    Generalized Additive Models (GAMs).
+    """Wrapper around R's `mgcv <https://cran.r-project.org/web/packages/mgcv/>`__ package for fitting GAMs.
 
     Parameters
     ----------
     %(adata)s
     n_knots
         Number of knots.
     distribution
-        Distribution family in `rpy2.robjects.r`, such as `'gaussian'` or `'nb'` for negative binomial.
-        If `'nb'`, raw count data in :attr:`adata` ``.raw`` is always used.
+        Distribution family in `rpy2.robjects.r`, such as ``'gaussian'`` or ``'nb'`` for negative binomial.
+        If ``'nb'``, raw count data in :attr:`~anndata.AnnData.raw` is always used.
     basis
         Basis for the smoothing term.
         See `here <https://www.rdocumentation.org/packages/mgcv/versions/1.8-33/topics/s>`__ for valid options.
     knotlocs
         Position of the knots. Can be one of the following:
 
-            - `{kloc.AUTO!r}` - let `mgcv` handle the knot positions.
-            - `{kloc.DENSITY!r}` - position the knots based on the density of the pseudotime.
+        - ``{kloc.AUTO!r}`` - let `mgcv` handle the knot positions.
+        - ``{kloc.DENSITY!r}`` - position the knots based on the density of the pseudotime.
     offset
         Offset term for the GAM. Only available when ``distribution='nb'``. If `'default'`, it is calculated
-        according to :cite:`robinson:10`. The values are saved in :attr:`adata` ``.obs[{key!r}]``.
-        If `None`, no offset is used.
+        according to :cite:`robinson:10`. The values are saved in :attr:`adata.obs['{key}'] <anndata.AnnData.obs>`.
+        If :obj:`None`, no offset is used.
     smoothing_penalty
         Penalty for the smoothing term. The larger the value, the smoother the fitted curve.
     kwargs
-        Keyword arguments for ``gam.control``.
-        See `here <https://www.rdocumentation.org/packages/mgcv/versions/1.8-33/topics/gam.control>`__ for reference.
-    """  # noqa
+        Keyword arguments for `gam control
+        <https://www.rdocumentation.org/packages/mgcv/versions/1.8-33/topics/gam.control>`__.
+    """
 
     def __init__(
         self,
         adata: AnnData,
         n_knots: int = 5,
         distribution: str = "gaussian",
         basis: str = "cr",
         knotlocs: Literal["auto", "density"] = KnotLocs.AUTO,
         offset: Optional[Union[np.ndarray, Literal["default"]]] = "default",
         smoothing_penalty: float = 1.0,
-        **kwargs,
+        **kwargs: Any,
     ):
         if n_knots <= 0:
             raise ValueError(f"Expected `n_splines` to be positive, found `{n_knots}`.")
         if smoothing_penalty < 0:
-            raise ValueError(
-                f"Expected `smoothing_penalty` to be non-negative, found `{smoothing_penalty}`."
-            )
+            raise ValueError(f"Expected `smoothing_penalty` to be non-negative, found `{smoothing_penalty}`.")
 
         super().__init__(adata, model=None)
         self._n_knots = n_knots
         self._family = distribution
 
-        self._formula = (
-            f"y ~ s(x, bs={basis!r}, k={self._n_knots}, sp={smoothing_penalty})"
-        )
+        self._formula = f"y ~ s(x, bs={basis!r}, k={self._n_knots}, sp={smoothing_penalty})"
         self._design_mat = None
         self._offset = None
         self._knotslocs = KnotLocs(knotlocs)
 
-        self._control_kwargs = copy(kwargs)
+        self._control_kwargs = copy.copy(kwargs)
 
         self._lib = None
         self._lib_name = None
 
         # it's a bit costly to import, copying just passes the reference
         if kwargs.pop("perform_import_check", True):
             self._lib, self._lib_name = _maybe_import_r_lib("mgcv")
 
         if distribution == "nb" and offset is not None:
             if not isinstance(offset, (np.ndarray, str)):
                 raise TypeError(
-                    f"Expected `offset` to be either `'default'` or `numpy.ndarray`,"
-                    f"got `{type(offset).__name__}`."
+                    f"Expected `offset` to be either `'default'` or `numpy.ndarray`," f"got `{type(offset).__name__}`."
                 )
 
             if isinstance(offset, str):
                 if offset != "default":
-                    raise ValueError(
-                        "Only value `'default'` is allowed when `offset` is a string."
-                    )
+                    raise ValueError("Only value `'default'` is allowed when `offset` is a string.")
                 offset = _get_offset(adata, use_raw=True, recompute=False)
 
             offset = np.asarray(offset, dtype=self._dtype)
 
             if offset.shape != (adata.n_obs,):
-                raise ValueError(
-                    f"Expected offset to be of shape `{(adata.n_obs,)}`, found `{offset.shape}`."
-                )
+                raise ValueError(f"Expected offset to be of shape `{(adata.n_obs,)}`, found `{offset.shape}`.")
             adata.obs[_OFFSET_KEY] = offset
 
             self._formula += " + offset(offset)"
             self._offset = offset
 
     @d.dedent
     def prepare(
         self,
-        *args,
-        **kwargs,
+        *args: Any,
+        **kwargs: Any,
     ) -> "GAMR":
-        """
-        %(base_model_prepare.full_desc)s
+        """%(base_model_prepare.full_desc)s
+
         This also removes the zero and negative weights and prepares the design matrix.
 
         Parameters
         ----------
         %(base_model_prepare.parameters)s
 
         Returns
@@ -164,67 +154,64 @@
 
     @d.dedent
     def fit(
         self,
         x: Optional[np.ndarray] = None,
         y: Optional[np.ndarray] = None,
         w: Optional[np.ndarray] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> "GAMR":
-        """
-        %(base_model_fit.full_desc)s
+        """%(base_model_fit.full_desc)s
 
         Parameters
         ----------
         %(base_model_fit.parameters)s
 
         Returns
         -------
-        Fits the model and returns self. Updates the following fields by filtering out `0` weights :attr:`w`:
+        Fits the model and returns self. Updates the following fields by filtering out :math:`0` weights :attr:`w`:
 
-            - :attr:`x` - %(base_model_x.summary)s
-            - :attr:`y` - %(base_model_y.summary)s
-            - :attr:`w` - %(base_model_w.summary)s
+        - :attr:`x` - %(base_model_x.summary)s
+        - :attr:`y` - %(base_model_y.summary)s
+        - :attr:`w` - %(base_model_w.summary)s
         """  # noqa
 
-        from rpy2.robjects import Formula, r, pandas2ri
+        import rpy2.robjects as ro
+        from rpy2.robjects import pandas2ri
+        from rpy2.robjects.conversion import localconverter
 
         super().fit(x, y, w, **kwargs)
 
-        pandas2ri.activate()
-
-        family = getattr(r, self._family)
+        # order seems to matter, pandas2ri + default_converter results in:
+        # Conversion 'py2rpy' not defined for objects of type '<class 'rpy2.rlike.container.OrdDict'>'
+        with localconverter(pandas2ri.converter + ro.default_converter):
+            family = getattr(ro.r, self._family)
+            kwargs = {}
+            if self._knotslocs != KnotLocs.AUTO:
+                kwargs["knots"] = pd.DataFrame(
+                    _get_knotlocs(
+                        self.x,
+                        self._n_knots,
+                        uniform=False,
+                    ),
+                    columns=["x"],
+                )
 
-        kwargs = {}
-        if self._knotslocs != KnotLocs.AUTO:
-            kwargs["knots"] = pd.DataFrame(
-                _get_knotlocs(
-                    self.x,
-                    self._n_knots,
-                    uniform=False,
-                ),
-                columns=["x"],
+            self._model = self._lib.gam(
+                ro.Formula(self._formula),
+                data=self._design_mat,
+                family=family,
+                weights=pd.Series(self.w),
+                control=self._lib.gam_control(**self._control_kwargs),
+                **kwargs,
             )
 
-        self._model = self._lib.gam(
-            Formula(self._formula),
-            data=self._design_mat,
-            family=family,
-            weights=pd.Series(self.w),
-            control=self._lib.gam_control(**self._control_kwargs),
-            **kwargs,
-        )
-
-        pandas2ri.deactivate()
-
         return self
 
-    def _get_x_test(
-        self, x_test: Optional[np.ndarray] = None, key_added: str = "_x_test"
-    ) -> pd.DataFrame:
+    def _get_x_test(self, x_test: Optional[np.ndarray] = None, key_added: str = "_x_test") -> pd.DataFrame:
         newdata = pd.DataFrame(self._check(key_added, x_test), columns=["x"])
 
         if "offset" in self._design_mat:
             newdata["offset"] = np.mean(self._design_mat["offset"])
 
         return newdata
 
@@ -232,77 +219,68 @@
     def predict(
         self,
         x_test: Optional[np.ndarray] = None,
         key_added: str = "_x_test",
         level: Optional[float] = None,
         **kwargs,
     ) -> np.ndarray:
-        """
-        %(base_model_predict.full_desc)s
+        """%(base_model_predict.full_desc)s
+
         This method can also compute the confidence interval.
 
         Parameters
         ----------
         %(base_model_predict.parameters)s
         level
-            Confidence level for confidence interval calculation. If `None`, don't compute the confidence interval.
-            Must be in the interval `[0, 1]`.
+            Confidence level for confidence interval calculation.
+            If :obj:`None`, don't compute the confidence interval. Must be in :math:`[0, 1]`.
 
         Returns
         -------
         %(base_model_predict.returns)s
         """  # noqa
-
-        from rpy2 import robjects
+        import rpy2.robjects as ro
         from rpy2.robjects import pandas2ri
+        from rpy2.robjects.conversion import localconverter
 
         if self.model is None:
-            raise RuntimeError(
-                "Trying to call an uninitialized model. To initialize it, run `.fit()` first."
-            )
+            raise RuntimeError("Trying to call an uninitialized model. To initialize it, run `.fit()` first.")
         if self._lib is None:
-            raise RuntimeError(
-                f"Unable to run prediction, R package `{self._lib_name!r}` is not imported."
-            )
+            raise RuntimeError(f"Unable to run prediction, R package `{self._lib_name!r}` is not imported.")
 
         if level is not None and not (0 <= level <= 1):
-            raise ValueError(
-                f"Expected the confidence level to be in interval `[0, 1]`, found `{level}`."
-            )
+            raise ValueError(f"Expected the confidence level to be in interval `[0, 1]`, found `{level}`.")
 
         newdata = self._get_x_test(x_test)
 
-        pandas2ri.activate()
-        res = robjects.r.predict(
-            self.model,
-            newdata=pandas2ri.py2rpy(newdata),
-            type="response",
-            se=level is not None,
-        )
-        pandas2ri.deactivate()
+        with localconverter(pandas2ri.converter + ro.default_converter):
+            res = ro.r.predict(
+                self.model,
+                newdata=ro.pandas2ri.py2rpy(newdata),
+                type="response",
+                se=level is not None,
+            )
 
         if level is None:
             self._y_test = np.array(res).squeeze().astype(self._dtype)
         else:
             self._y_test = np.array(res.rx2("fit")).squeeze().astype(self._dtype)
             se = np.array(res.rx2("se.fit")).squeeze().astype(self._dtype)
 
-            level = norm.ppf(level + (1 - level) / 2)
+            level = st.norm.ppf(level + (1 - level) / 2)
             self._conf_int = np.c_[self.y_test - level * se, self.y_test + level * se]
 
         return self.y_test
 
     @d.dedent
-    def confidence_interval(
-        self, x_test: Optional[np.ndarray] = None, level: float = 0.95, **kwargs
-    ) -> np.ndarray:
-        """
-        %(base_model_ci.summary)s
-        Internally, this method calls :meth:`cellrank.ul.models.GAMR.predict` to extract
-        the confidence interval, if needed.
+    def confidence_interval(self, x_test: Optional[np.ndarray] = None, level: float = 0.95, **kwargs) -> np.ndarray:
+        """%(base_model_ci.summary)s
+
+        Internally, this method calls :meth:`~cellrank.models.GAMR.predict` to extract the confidence interval,
+        if needed.
 
         Parameters
         ----------
         %(base_model_ci.parameters)s
         level
             Confidence level.
 
@@ -320,31 +298,29 @@
         if x_test is not None or level != 0.95 or self._conf_int is None:
             _ = self.predict(x_test=x_test, level=level)
 
         return self._conf_int
 
     def _deepcopy_attributes(self, dst: "GAMR") -> None:
         super()._deepcopy_attributes(dst)
-        dst._offset = deepcopy(self._offset)
-        dst._design_mat = deepcopy(self._design_mat)
+        dst._offset = copy.deepcopy(self._offset)
+        dst._design_mat = copy.deepcopy(self._design_mat)
 
     @d.dedent
     def copy(self) -> "GAMR":
         """%(copy)s"""  # noqa
         res = GAMR(
             self.adata,
             self._n_knots,
             distribution=self._family,
             offset=self._offset,
             knotlocs=self._knotslocs,
             perform_import_check=False,
         )
-        self._shallowcopy_attributes(
-            res
-        )  # does not copy `prepared`, since we're not copying the arrays
+        self._shallowcopy_attributes(res)  # does not copy `prepared`, since we're not copying the arrays
 
         res._formula = self._formula  # we don't save the basis inside
         res._design_mat = self._design_mat
         res._offset = self._offset
 
         res._lib = self._lib  # just passing the reference
         res._lib_name = self._lib_name
@@ -357,39 +333,34 @@
         return {k: v for k, v in self.__dict__.items() if k != "_lib"}
 
     def __setstate__(self, state: dict):
         self.__dict__ = state
         self._lib, self._lib_name = _maybe_import_r_lib(self._lib_name, raise_exc=True)
 
 
-def _maybe_import_r_lib(
-    name: str, raise_exc: bool = False
-) -> Tuple[Optional[Any], Optional[str]]:
+def _maybe_import_r_lib(name: str, raise_exc: bool = False) -> Tuple[Optional[Any], Optional[str]]:
     global _r_lib, _r_lib_name
 
     if name == _r_lib_name and _r_lib is not None:
         return _r_lib, _r_lib_name
 
     try:
         from logging import ERROR
+
+        from rpy2.rinterface_lib.callbacks import logger
         from rpy2.robjects import r
         from rpy2.robjects.packages import PackageNotInstalledError, importr
-        from rpy2.rinterface_lib.callbacks import logger
 
         logger.setLevel(ERROR)
         r["options"](warn=-1)
 
     except ImportError as e:
-        raise ImportError(
-            "Unable to import `rpy2`, install it first as `pip install rpy2` version `>=3.3.0`."
-        ) from e
+        raise ImportError("Unable to import `rpy2`, install it first as `pip install rpy2` version `>=3.3.0`.") from e
 
     try:
         _r_lib = importr(name)
         _r_lib_name = name
         return _r_lib, _r_lib_name
     except PackageNotInstalledError as e:
         if not raise_exc:
             return None, None
-        raise RuntimeError(
-            f"Install R library `{name!r}` first as `install.packages({name!r}).`"
-        ) from e
+        raise RuntimeError(f"Install R library `{name!r}` first as `install.packages({name!r}).`") from e
```

### Comparing `cellrank-1.5.1/cellrank/ul/models/_pygam_model.py` & `cellrank-2.0.0/src/cellrank/models/_pygam_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,110 +1,109 @@
-from typing import Any, Union, Mapping, Optional
-from typing_extensions import Literal
+import collections
+import copy
+import enum
+import types
+import warnings
+from typing import Any, Literal, Mapping, Optional, Union
 
-from copy import copy as _copy
-from copy import deepcopy
-from enum import auto
-from types import MappingProxyType
-from collections import defaultdict
-
-from cellrank import logging as logg
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d
-from cellrank.ul.models import BaseModel
-from cellrank.tl.kernels._utils import _filter_kwargs
-from cellrank.ul.models._base_model import AnnData
-
-import numpy as np
 from pygam import GAM as pGAM
 from pygam import (
+    ExpectileGAM,
     GammaGAM,
-    LinearGAM,
-    PoissonGAM,
     InvGaussGAM,
+    LinearGAM,
     LogisticGAM,
-    ExpectileGAM,
+    PoissonGAM,
     s,
 )
 
+import numpy as np
+
+from anndata import AnnData
+
+from cellrank import logging as logg
+from cellrank._utils._docs import d
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._utils import _filter_kwargs
+from cellrank.models import BaseModel
+
+__all__ = ["GAM"]
+
 
-class GamLinkFunction(ModeEnum):  # noqa: D101
-    IDENTITY = auto()
-    LOGIT = auto()
-    INVERSE = auto()
-    LOG = auto()
+class GamLinkFunction(ModeEnum):
+    IDENTITY = enum.auto()
+    LOGIT = enum.auto()
+    INVERSE = enum.auto()
+    LOG = enum.auto()
     INV_SQUARED = "inverse-squared"
 
 
-class GamDistribution(ModeEnum):  # noqa: D101
-    NORMAL = auto()
-    BINOMIAL = auto()
-    POISSON = auto()
-    GAMMA = auto()
-    GAUSSIAN = auto()
-    INV_GAUSS = auto()
+class GamDistribution(ModeEnum):
+    NORMAL = enum.auto()
+    BINOMIAL = enum.auto()
+    POISSON = enum.auto()
+    GAMMA = enum.auto()
+    GAUSSIAN = enum.auto()
+    INV_GAUSS = enum.auto()
 
 
-_gams = defaultdict(
+_gams = collections.defaultdict(
     lambda: pGAM,
     {
         (GamDistribution.NORMAL, GamLinkFunction.IDENTITY): LinearGAM,
         (GamDistribution.BINOMIAL, GamLinkFunction.LOGIT): LogisticGAM,
         (GamDistribution.POISSON, GamLinkFunction.LOG): PoissonGAM,
         (GamDistribution.GAMMA, GamLinkFunction.LOG): GammaGAM,
         (GamDistribution.INV_GAUSS, GamLinkFunction.LOG): InvGaussGAM,
     },
 )
 
 
 @d.dedent
 class GAM(BaseModel):
-    """
-    Fit Generalized Additive Models (GAMs) using :mod:`pygam`.
+    """Fit Generalized Additive Models (GAMs) using :mod:`pygam`.
 
     Parameters
     ----------
     %(adata)s
     n_knots
         Number of knots.
     spline_order
-        Order of the splines, i.e. `3` for cubic splines.
+        Order of the splines, e.g., :math:`3` for cubic splines.
     distribution
         Name of the distribution. Available distributions can be found
         `here <https://pygam.readthedocs.io/en/latest/notebooks/tour_of_pygam.html#Distribution:>`__.
     link
         Name of the link function. Available link functions can be found
         `here <https://pygam.readthedocs.io/en/latest/notebooks/tour_of_pygam.html#Link-function:>`__.
     max_iter
         Maximum number of iterations for optimization.
     expectile
-        Expectile for :class:`pygam.pygam.ExpectileGAM`. This forces the distribution to be `'normal'`
-        and link function to `'identity'`. Must be in interval `(0, 1)`.
+        Expectile for :class:`~pygam.pygam.ExpectileGAM`. This forces the distribution to be ``'normal'``
+        and link function to ``'identity'``. Must be in :math:`(0, 1)`.
     grid
         Whether to perform a grid search. Keys correspond to a parameter names and values to range to be searched.
-        If `'default'`, use the default grid. If `None`, don't perform a grid search.
+        If ``'default'``, use the default grid. If :obj:`None`, don't perform a grid search.
     spline_kwargs
-        Keyword arguments for :class:`pygam.s`.
+        Keyword arguments for :func:`~pygam.terms.s`.
     kwargs
-        Keyword arguments for :class:`pygam.pygam.GAM`.
+        Keyword arguments for the :class:`~pygam.pygam.GAM`.
     """
 
     def __init__(
         self,
         adata: AnnData,
         n_knots: Optional[int] = 6,
         spline_order: int = 3,
-        distribution: Literal[
-            "normal", "binomial", "poisson", "gamma", "gaussian", "inv_gauss"
-        ] = "gamma",
+        distribution: Literal["normal", "binomial", "poisson", "gamma", "gaussian", "inv_gauss"] = "gamma",
         link: Literal["identity", "logit", "inverse", "log", "inverse-squared"] = "log",
         max_iter: int = 2000,
         expectile: Optional[float] = None,
         grid: Optional[Union[str, Mapping[str, Any]]] = None,
-        spline_kwargs: Mapping[str, Any] = MappingProxyType({}),
+        spline_kwargs: Mapping[str, Any] = types.MappingProxyType({}),
         **kwargs: Any,
     ):
         term = s(
             0,
             spline_order=spline_order,
             n_splines=n_knots,
             penalties=["derivative", "l2"],
@@ -113,34 +112,29 @@
         link = GamLinkFunction(link)
         distribution = GamDistribution(distribution)
         if distribution == GamDistribution.GAUSSIAN:
             distribution = GamDistribution.NORMAL
 
         if expectile is not None:
             if not (0 < expectile < 1):
-                raise ValueError(
-                    f"Expected `expectile` to be in `(0, 1)`, found `{expectile}`."
-                )
+                raise ValueError(f"Expected `expectile` to be in `(0, 1)`, found `{expectile}`.")
             if distribution != "normal" or link != "identity":
                 logg.warning(
                     f"Expectile GAM works only with `normal` distribution and `identity` link function,"
                     f"found `{distribution!r}` distribution and {link!r} link functions."
                 )
-            model = ExpectileGAM(
-                term, expectile=expectile, max_iter=max_iter, verbose=False, **kwargs
-            )
+            model = ExpectileGAM(term, expectile=expectile, max_iter=max_iter, verbose=False, **kwargs)
         else:
             # doing it like this ensure that user can specify scale
             gam = _gams[distribution, link]
 
             filtered_kwargs = _filter_kwargs(gam.__init__, **kwargs)
             if len(kwargs) != len(filtered_kwargs):
                 raise TypeError(
-                    f"Invalid arguments `{list(set(kwargs) - set(filtered_kwargs))}` "
-                    f"for `{type(gam).__name__!r}`."
+                    f"Invalid arguments `{list(set(kwargs) - set(filtered_kwargs))}` " f"for `{type(gam).__name__!r}`."
                 )
 
             filtered_kwargs["link"] = link
             filtered_kwargs["distribution"] = distribution
 
             model = gam(
                 term,
@@ -149,125 +143,130 @@
                 **_filter_kwargs(gam.__init__, **filtered_kwargs),
             )
         super().__init__(adata, model=model)
 
         if grid is None:
             self._grid = None
         elif isinstance(grid, dict):
-            self._grid = _copy(grid)
+            self._grid = copy.copy(grid)
         elif isinstance(grid, str):
             self._grid = object() if grid == "default" else None
         else:
-            raise TypeError(
-                f"Expected `grid` to be `dict`, `str` or `None`, found `{type(grid).__name__!r}`."
-            )
+            raise TypeError(f"Expected `grid` to be `dict`, `str` or `None`, found `{type(grid).__name__!r}`.")
 
     @d.dedent
     def fit(
         self,
         x: Optional[np.ndarray] = None,
         y: Optional[np.ndarray] = None,
         w: Optional[np.ndarray] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> "GAM":
-        """
-        %(base_model_fit.full_desc)s
+        """%(base_model_fit.full_desc)s
 
         Parameters
         ----------
         %(base_model_fit.parameters)s
 
         Returns
         -------
         Fits the model and returns self.
         """  # noqa
 
         super().fit(x, y, w, **kwargs)
 
-        if self._grid is not None:
-            # use default search
-            grid = {} if not isinstance(self._grid, dict) else self._grid
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                category=DeprecationWarning,
+                message=".* is a deprecated alias for the builtin",
+            )
+            if self._grid is not None:
+                # use default search
+                grid = {} if not isinstance(self._grid, dict) else self._grid
+                try:
+                    self.model.gridsearch(
+                        self.x,
+                        self.y,
+                        weights=self.w,
+                        keep_best=True,
+                        progress=False,
+                        **grid,
+                        **kwargs,
+                    )
+                    return self
+                except Exception as e:  # noqa: BLE001
+                    # workaround for: https://github.com/dswah/pyGAM/issues/273
+                    self.model.fit(self.x, self.y, weights=self.w, **kwargs)
+                    logg.error(f"Grid search failed, reason: `{e}`. Fitting with default values")
+
             try:
-                self.model.gridsearch(
-                    self.x,
-                    self.y,
-                    weights=self.w,
-                    keep_best=True,
-                    progress=False,
-                    **grid,
-                    **kwargs,
-                )
-                return self
-            except Exception as e:  # noqa: B902
-                # workaround for: https://github.com/dswah/pyGAM/issues/273
                 self.model.fit(self.x, self.y, weights=self.w, **kwargs)
-                logg.error(
-                    f"Grid search failed, reason: `{e}`. Fitting with default values"
-                )
-
-        try:
-            self.model.fit(self.x, self.y, weights=self.w, **kwargs)
-            return self
-        except Exception as e:  # noqa: B902
-            raise RuntimeError(
-                f"Unable to fit `{type(self).__name__}` for gene "
-                f"`{self._gene!r}` in lineage `{self._lineage!r}`. Reason: `{e}`"
-            ) from e
+                return self
+            except Exception as e:  # noqa: BLE001
+                raise RuntimeError(
+                    f"Unable to fit `{type(self).__name__}` for gene "
+                    f"`{self._gene!r}` in lineage `{self._lineage!r}`. Reason: `{e}`"
+                ) from e
 
     @d.dedent
     def predict(
         self,
         x_test: Optional[np.ndarray] = None,
         key_added: Optional[str] = "_x_test",
-        **kwargs,
+        **kwargs: Any,
     ) -> np.ndarray:
-        """
-        %(base_model_predict.full_desc)s
+        """%(base_model_predict.full_desc)s
 
         Parameters
         ----------
         %(base_model_predict.parameters)s
 
         Returns
         -------
         %(base_model_predict.returns)s
         """  # noqa
 
         x_test = self._check(key_added, x_test)
 
-        self._y_test = self.model.predict(x_test, **kwargs)
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                category=DeprecationWarning,
+                message=".* is a deprecated alias for the builtin",
+            )
+            self._y_test = self.model.predict(x_test, **kwargs)
         self._y_test = np.squeeze(self._y_test).astype(self._dtype)
 
         return self.y_test
 
     @d.dedent
-    def confidence_interval(
-        self, x_test: Optional[np.ndarray] = None, **kwargs
-    ) -> np.ndarray:
-        """
-        %(base_model_ci.summary)s
+    def confidence_interval(self, x_test: Optional[np.ndarray] = None, **kwargs: Any) -> np.ndarray:
+        """%(base_model_ci.summary)s
 
         Parameters
         ----------
         %(base_model_ci.parameters)s
 
         Returns
         -------
         %(base_model_ci.returns)s
         """  # noqa
 
         x_test = self._check("_x_test", x_test)
-        self._conf_int = self.model.confidence_intervals(x_test, **kwargs).astype(
-            self._dtype
-        )
+        with warnings.catch_warnings():
+            warnings.filterwarnings(
+                "ignore",
+                category=DeprecationWarning,
+                message=".* is a deprecated alias for the builtin",
+            )
+            self._conf_int = self.model.confidence_intervals(x_test, **kwargs).astype(self._dtype)
 
         return self.conf_int
 
     @d.dedent
     def copy(self) -> "BaseModel":
         """%(copy)s"""  # noqa
         res = GAM(self.adata)
         self._shallowcopy_attributes(res)
-
-        res._grid = deepcopy(self._grid)
-
+        res._grid = copy.deepcopy(self._grid)
         return res
```

### Comparing `cellrank-1.5.1/cellrank/ul/models/_sklearn_model.py` & `cellrank-2.0.0/src/cellrank/models/_sklearn_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-"""Module containing model which wraps around :mod:`sklearn` estimators."""
-from typing import Iterable, Optional
-
+import inspect
 import warnings
-from inspect import signature
-
-from cellrank.ul._docs import d
-from cellrank.ul.models import BaseModel
-from cellrank.ul.models._base_model import AnnData
+from typing import Any, Iterable, Optional
 
 import numpy as np
 from sklearn.base import BaseEstimator
 from sklearn.utils import check_X_y
 
+from anndata import AnnData
+
+from cellrank._utils._docs import d
+from cellrank.models import BaseModel
+
+__all__ = ["SKLearnModel"]
+
 
 @d.dedent
 class SKLearnModel(BaseModel):
-    """
-    Wrapper around :class:`sklearn.base.BaseEstimator`.
+    """Wrapper around :class:`~sklearn.base.BaseEstimator`.
 
     Parameters
     ----------
     %(adata)s
     model
-        Instance of the underlying :mod:`sklearn` estimator, such as :class:`sklearn.svm.SVR`.
+        Instance of the underlying :mod:`sklearn` estimator, such as :class:`~sklearn.svm.SVR`.
     weight_name
-        Name of the weight argument for :attr:`model` ``.fit``. If `None`, to determine it automatically.
-        If and empty string, no weights will be used.
+        Name of the weight argument when fitting the model. If :obj:`None`, to determine it automatically.
+        If an empty :class:`str`, no weights will be used.
     ignore_raise
-        Do not raise an exception if weight argument is not found in the fitting function of :attr:`model`.
-        This is useful in case when weight is passed in ``**kwargs`` and cannot be determined from signature.
+        Do not raise an exception if weight argument is not found when fitting the :attr:`model`.
+        This is useful in case when the weight argument is passed in the ``**kwargs`` and
+        cannot be determined from signature.
     """
 
     _fit_names = ("fit", "__init__")
     _predict_names = ("predict", "__call__")
     _weight_names = ("w", "weights", "sample_weight", "sample_weights")
     _conf_int_names = ("conf_int", "confidence_intervals")
 
@@ -40,40 +41,33 @@
         self,
         adata: AnnData,
         model: BaseEstimator,
         weight_name: Optional[str] = None,
         ignore_raise: bool = False,
     ):
         if not isinstance(model, BaseEstimator):
-            raise TypeError(
-                f"Expected model to be of type `BaseEstimator`, found `{type(model).__name__!r}`."
-            )
+            raise TypeError(f"Expected model to be of type `BaseEstimator`, found `{type(model).__name__!r}`.")
 
         super().__init__(adata, model)
 
         fit_name = self._find_func(self._fit_names)
         predict_name = self._find_func(self._predict_names)
         ci_name = self._find_func(self._conf_int_names, use_default=True, default=None)
 
-        self._weight_name = (
-            self._find_arg_name(fit_name, self._weight_names)
-            if weight_name is None
-            else weight_name
-        )
+        self._weight_name = self._find_arg_name(fit_name, self._weight_names) if weight_name is None else weight_name
 
         if self._weight_name is None:
             raise RuntimeError(
                 f"Unable to determine weights for function `{fit_name!r}`, searched `{self._weight_names}`. "
                 f"Consider specifying it manually as `weight_name=...`."
             )
-        elif (
+        if (
             not ignore_raise
             and self._weight_name != ""
-            and self._weight_name
-            not in signature(getattr(self.model, fit_name)).parameters
+            and self._weight_name not in inspect.signature(getattr(self.model, fit_name)).parameters
         ):
             raise ValueError(
                 f"Unable to detect `{weight_name!r}` in the signature of `{fit_name!r}`."
                 f"If it's in `kwargs`, set `ignore_raise=True.`"
             )
 
         self._fit_fn = getattr(self.model, fit_name)
@@ -82,28 +76,26 @@
 
     @d.dedent
     def fit(
         self,
         x: Optional[np.ndarray] = None,
         y: Optional[np.ndarray] = None,
         w: Optional[np.ndarray] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> "SKLearnModel":
-        """
-        %(base_model_fit.full_desc)s
+        """%(base_model_fit.full_desc)s
 
         Parameters
         ----------
         %(base_model_fit.parameters)s
 
         Returns
         -------
         Fits the model and returns self.
         """  # noqa: D400
-
         super().fit(x, y, w, **kwargs)
 
         if self._weight_name not in (None, ""):
             kwargs[self._weight_name] = self._w
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", UserWarning)
@@ -115,128 +107,110 @@
                 estimator=self.model,
             )
         self._model = self._fit_fn(x, y, **kwargs)
 
         return self
 
     @d.dedent
-    def predict(
-        self, x_test: Optional[np.ndarray] = None, key_added: str = "_x_test", **kwargs
-    ) -> np.ndarray:
-        """
-        %(base_model_predict.full_desc)s
+    def predict(self, x_test: Optional[np.ndarray] = None, key_added: str = "_x_test", **kwargs) -> np.ndarray:
+        """%(base_model_predict.full_desc)s
 
         Parameters
         ----------
         %(base_model_predict.parameters)s
 
         Returns
         -------
         %(base_model_predict.returns)s
-        """  # noqa
-
+        """  # noqa: D400
         x_test = self._check(key_added, x_test)
 
         self._y_test = self._pred_fn(x_test, **kwargs)
         self._y_test = np.squeeze(self._y_test).astype(self._dtype)
 
         return self.y_test
 
     @d.dedent
-    def confidence_interval(
-        self, x_test: Optional[np.ndarray] = None, **kwargs
-    ) -> np.ndarray:
-        """
-        %(base_model_ci.full_desc)s
+    def confidence_interval(self, x_test: Optional[np.ndarray] = None, **kwargs: Any) -> np.ndarray:
+        """%(base_model_ci.full_desc)s
 
         Parameters
         ----------
         %(base_model_ci.parameters)s
 
         Returns
         -------
         %(base_model_ci.returns)s
-        """  # noqa
-
+        """  # noqa: D400
         if self._ci_fn is None:
             return self.default_confidence_interval(x_test=x_test, **kwargs)
 
         x_test = self._check("_x_test", x_test)
         self._conf_int = self._ci_fn(x_test, **kwargs)
 
         return self.conf_int
 
     def _find_func(
         self,
         func_names: Iterable[str],
         use_default: bool = False,
         default: Optional[str] = None,
     ) -> Optional[str]:
-        """
-        Find a function in :attr:`model` from given names.
+        """Find a function in :attr:`model` from given names.
 
-        If `None` is found, use ``default`` or raise a :class:`RuntimeError`.
+        If :obj:`None` is found, use the ``default`` or raise a :class:`RuntimeError`.
 
         Parameters
         ----------
         func_names
             Function names to search. The first one found is returned.
         use_default
-            Whether to return the ``default`` if it is `None` or raise :class:`RuntimeError`.
+            Whether to return the ``default`` if it is :obj:`None` or raise :class:`RuntimeError`.
         default
-            The default function name to use if `None` was found.
+            The default function name to use if :obj:`None` was found.
 
         Returns
         -------
         Name of the function or the default name.
         """
-
         for name in func_names:
             if hasattr(self.model, name) and callable(getattr(self.model, name)):
                 return name
         if use_default:
             return default
-        raise RuntimeError(
-            f"Unable to find function and no default specified, searched for `{list(func_names)}`."
-        )
+        raise RuntimeError(f"Unable to find function and no default specified, searched for `{list(func_names)}`.")
 
-    def _find_arg_name(
-        self, func_name: Optional[str], param_names: Iterable[str]
-    ) -> Optional[str]:
-        """
-        Find an argument in :attr:`model`'s ``func_name``.
+    def _find_arg_name(self, func_name: Optional[str], param_names: Iterable[str]) -> Optional[str]:
+        """Find an argument in :attr:`model`'s ``func_name``.
 
         Parameters
         ----------
         func_name
             Function name of :attr:`model`.
         param_names
             Parameter names to search. The first one found is returned.
 
         Returns
         -------
-        The parameter name or `None`, if `None` was found or ``func_name`` was `None`.
+        The parameter name or :obj:`None`, if :obj:`None` was found or ``func_name`` was :obj:`None`.
         """
-
         if func_name is None:
             return None
 
-        for param in signature(getattr(self.model, func_name)).parameters:
+        for param in inspect.signature(getattr(self.model, func_name)).parameters:
             if param in param_names:
                 return param
 
         return None
 
     @property
     def model(self) -> BaseEstimator:
-        """The underlying :class:`sklearn.base.BaseEstimator`."""  # noqa
+        """The underlying :class:`~sklearn.base.BaseEstimator`."""
         return self._model
 
     @d.dedent
     def copy(self) -> "SKLearnModel":
         """%(copy)s"""  # noqa
-        res = SKLearnModel(
-            self.adata, self._model, weight_name=self._weight_name, ignore_raise=True
-        )
+        res = SKLearnModel(self.adata, self._model, weight_name=self._weight_name, ignore_raise=True)
         self._shallowcopy_attributes(res)  # this deepcopies the underlying model
 
         return res
```

### Comparing `cellrank-1.5.1/cellrank/ul/models/_utils.py` & `cellrank-2.0.0/src/cellrank/models/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from typing import Union, Optional, Sequence
+import enum
+from typing import Any, Optional, Sequence, Union
 
-from enum import auto
+import numba as nb
+import numpy as np
+import scipy.sparse as sp
+from numba import prange
+from sklearn.utils.sparsefuncs import csc_median_axis_0
 
-import cellrank.logging as logg
 from anndata import AnnData
-from cellrank.tl._enum import ModeEnum
-from cellrank.ul._docs import d, inject_docs
-from cellrank.ul._utils import valuedispatch
-from cellrank.ul._parallelize import parallelize
 
-import numpy as np
-from numba import njit, prange
-from scipy.sparse import issparse, spmatrix
-from sklearn.utils.sparsefuncs import csc_median_axis_0
+import cellrank.logging as logg
+from cellrank._utils._docs import d, inject_docs
+from cellrank._utils._enum import ModeEnum
+from cellrank._utils._parallelize import parallelize
+from cellrank._utils._utils import valuedispatch
+
+__all__ = ["_get_offset"]
 
 _OFFSET_KEY = "cellrank_offset"
 
 
 class NormMode(ModeEnum):  # noqa: D101
-    TMM = auto()
-    RLE = auto()
-    UPPER_QUANT = auto()
-    NONE = auto()
+    TMM = enum.auto()
+    RLE = enum.auto()
+    UPPER_QUANT = enum.auto()
+    NONE = enum.auto()
 
 
 @d.dedent
-def _extract_data(
-    data: AnnData, layer: Optional[str] = None, use_raw: bool = True
-) -> Union[np.ndarray, spmatrix]:
-    """
-    Extract expression data from an object.
+def _extract_data(data: AnnData, layer: Optional[str] = None, use_raw: bool = True) -> Union[np.ndarray, sp.spmatrix]:
+    """Extract expression data from an object.
 
     Parameters
     ----------
     data
         Annotated data object or an array.
     layer
-        Key in :attr:`anndata.AnnData.layers` accessed when ``use_raw = False``.
-        Only used when ``data`` is :class:`anndata.AnnData`.
+        Key in :attr:`~anndata.AnnData.layers` accessed when ``use_raw = False``.
+        Only used when ``data`` is :class:`~anndata.AnnData`.
     use_raw
-        Whether to access ``adata.raw``. Only used when ``data`` is :class:`anndata.AnnData`.
+        Whether to access :attr:`anndata.AnnData.raw`. Only used when ``data`` is :class:`~anndata.AnnData`.
 
     Returns
     -------
     The extracted expression data.
     """
     if isinstance(data, AnnData):
         if use_raw:
             if not hasattr(data, "raw"):
                 raise AttributeError("No `.raw` attribute found.")
-            elif data.raw is None:
+            if data.raw is None:
                 raise ValueError("Attribute `.raw` is None.")
             x = data.raw.X
         elif layer is not None:
             if layer not in data.layers:
                 raise KeyError(
                     f"Layer `{layer!s}` not found in `adata.layers`. "
                     f"Valid options are: `{list(data.layers.keys())}`."
                 )
             x = data.layers[layer]
         else:
             x = data.X
-    elif not isinstance(data, (np.ndarray, spmatrix)):
+    elif not isinstance(data, (np.ndarray, sp.spmatrix)):
         raise TypeError(
             f"Expected parameter `data` to be either `anndata.AnnData`, `numpy.ndarray` "
             f"or `scipy.sparse.spmatrix`, found `{type(data).__name__!r}`."
         )
     else:
         x = data
 
     return x
 
 
-@njit(fastmath=True, cache=True)
+@nb.njit(fastmath=True, cache=True)
 def _rankdata(a: np.ndarray, method: str = "average") -> np.ndarray:
     assert method in (
         "average",
         "min",
         "max",
         "dense",
         "ordinal",
@@ -111,90 +111,86 @@
 
     # average method
     return 0.5 * (count[dense] + count[dense - 1] + 1.0)
 
 
 @inject_docs(m=NormMode)
 def _calculate_norm_factors(
-    data: Union[AnnData, np.ndarray, spmatrix],
+    data: Union[AnnData, np.ndarray, sp.spmatrix],
     method: str = NormMode.TMM,
     layer: Optional[str] = None,
     use_raw: bool = True,
     library_size: Optional[np.ndarray] = None,
     ref_ix: Optional[int] = None,
     logratio_trim: float = 0.3,
     sum_trim: float = 0.05,
     weight: bool = True,
     a_cutoff: float = -1e10,
     perc: float = 0.75,
 ) -> np.ndarray:
-    """
-    Calculate normalization factors according to \
-    `edgeR <https://www.rdocumentation.org/packages/edgeR/versions/3.14.0/topics/calcNormFactors>`__.
+    """Calculate normalization factors.
+
+    This uses the `edgeR <https://www.rdocumentation.org/packages/edgeR/versions/3.14.0/topics/calcNormFactors>`_
+    implementation.
 
     Parameters
     ----------
     data
-        Data of shape `(n_cells, n_genes)` containing e.g. the counts.
+        Data of shape ``(n_cells, n_genes)`` containing, e.g., the counts.
     method
         Which method to use. Valid options are:
 
-            - `{m.TMM!r}` - weighted trimmed mean of M-values from :cite:`robinson:10`.
-            - `{m.RLE!r}` - relative log expression from [Anders10]_.
-            - `{m.UPPER_QUANT!r}` - upper-quartile normalization method from [Bullard10]_.
-            - `{m.NONE!r}` - all the factors are set to 1.
+        - ``{m.TMM!r}`` - weighted trimmed mean of M-values from :cite:`robinson:10`.
+        - ``{m.RLE!r}`` - relative log expression from [Anders10]_.
+        - ``{m.UPPER_QUANT!r}`` - upper-quartile normalization method from [Bullard10]_.
+        - ``{m.NONE!r}`` - all the factors are set to :math:`1`.
     layer
         Layer in :attr:`anndata.AnnData.layers` or `None` for :attr:`anndata.AnnData.X`.
         Only used when ``use_raw = False``.
     use_raw
-        Whether to access :attr:`anndata.AnnData.raw` or not.
+        Whether to access :attr:`~anndata.AnnData.raw` or not.
     library_size
-        Library size. If `None`, it will be set as the sum of values for each cell.
+        Library size. If :obj:`None`, it will be set as the sum of values for each cell.
     ref_ix
-        Index of a reference cell. If `None`, it will be determined automatically.
+        Index of a reference cell. If :obj:`None`, it will be determined automatically.
     logratio_trim
-        Amount of trim to use on log-ratios ('M' values) when ``method={m.TMM!r}``.
+        Amount of trim to use on log-ratios ('M' values) when ``method = {m.TMM!r}``.
     sum_trim
         Amount of trim to use on the combined absolute levels ('A' values) when ``method = {m.TMM!r}``.
     weight
         Whether to compute asymptotic binomial precision weights when ``method = {m.TMM!r}``.
     a_cutoff
         Cutoff on 'A' values to use before trimming when ``method = {m.TMM!r}``.
     perc
         Percentile of the counts that is aligned when ``method = {m.UPPER_QUANT!r}``.
 
     Returns
     -------
-    Array of shape `(data.shape[0],)` containing the factors.
+    Array of shape ``(data.shape[0],)`` containing the factors.
 
     References
     ----------
     .. [Anders10] Anders, S. *et al.* (2010),
         *Differential expression analysis for sequence count data*,
         `Genome Biology <https://doi.org/10.1186/gb-2010-11-10-r106>`__.
     .. [Bullard10] Bullard, J. H. *et al.* (2010),
         *Evaluation of statistical methods for normalization and differential expression in mRNA-Seq experiments*,
         `BMC Bioinformatics <https://doi.org/10.1186/1471-2105-11-94>`__.
     """
-
     method = NormMode(method)
 
     if not (0 <= perc <= 1):
-        raise ValueError(
-            f"Expected the percentile to be within interval `[0, 1]`, found `{perc}`."
-        )
+        raise ValueError(f"Expected the percentile to be within interval `[0, 1]`, found `{perc}`.")
 
     x = _extract_data(data, layer, use_raw)
 
     if library_size is None:
         library_size = np.array(x.sum(1)).squeeze()
     elif library_size.shape != (x.shape[0],):
-        raise ValueError(
-            f"Expected `library_size` to be of shape `({x.shape[0]},)`, found `{library_size.shape}`."
-        )
+        raise ValueError(f"Expected `library_size` to be of shape `({x.shape[0]},)`, found `{library_size.shape}`.")
 
     f = _dispatch_computation(
         method,
         x=x,
         library_size=library_size,
         ref_ix=ref_ix,
         logratio_trim=logratio_trim,
@@ -210,25 +206,25 @@
 @valuedispatch
 def _dispatch_computation(mode, *_args, **_kwargs):
     raise NotImplementedError(mode)
 
 
 @_dispatch_computation.register(NormMode.TMM)
 def _(
-    x: Union[np.ndarray, spmatrix],
+    x: Union[np.ndarray, sp.spmatrix],
     library_size: np.ndarray,
     ref_ix: Optional[int] = None,
     **kwargs,
 ) -> np.ndarray:
     if ref_ix is None:
         f75 = _calc_factor_quant(x, library_size=library_size, p=0.75)
         ref_ix = np.argmin(np.abs(f75 - np.mean(f75)))
 
     ref = x[ref_ix]
-    if issparse(ref):
+    if sp.issparse(ref):
         ref = ref.A.squeeze(0)  # (genes,)
 
     return parallelize(
         _calc_factor_weighted,
         collection=np.arange(x.shape[0]),
         show_progress_bar=False,
         as_array=False,
@@ -241,30 +237,28 @@
         ref=ref,
         ref_lib_size=library_size[ref_ix],
         **kwargs,
     )
 
 
 @_dispatch_computation.register(NormMode.UPPER_QUANT)
-def _calc_factor_quant(
-    x: Union[np.ndarray, spmatrix], library_size: np.ndarray, p: float, **_
-) -> np.ndarray:
+def _calc_factor_quant(x: Union[np.ndarray, sp.spmatrix], library_size: np.ndarray, p: float, **_) -> np.ndarray:
     # unused, because we fix the reference cell to 0
 
     library_size = np.array(library_size).reshape((-1, 1))
-    if not issparse(x):
+    if not sp.issparse(x):
         # this is same as below, which is R's default
         # return mquantiles(x / library_size, prob=q, alphap=1, betap=1, axis=1).data.squeeze()
         return np.quantile(x / library_size, p, axis=1)
 
     y = x.multiply(1.0 / library_size).tocsr()
     return _calc_factor_quant_sparse_helper(y.data, y.indptr, p=p, n_cols=y.shape[1])
 
 
-@njit(parallel=True, fastmath=True, cache=True)
+@nb.njit(parallel=True, fastmath=True, cache=True)
 def _calc_factor_quant_sparse_helper(
     data: np.ndarray,
     indptr: np.ndarray,
     p: float,
     n_cols: int,
 ) -> np.ndarray:
     n = len(indptr) - 1
@@ -277,64 +271,62 @@
         tmp[: len(d)] = d
         out[ix] = np.quantile(tmp, p)
 
     return out
 
 
 @_dispatch_computation.register(NormMode.RLE)
-def _(x: Union[np.ndarray, spmatrix], **_) -> np.ndarray:
+def _(x: Union[np.ndarray, sp.spmatrix], **_) -> np.ndarray:
     # unused
 
     # log 0 -> inf -> masked out anyway, so we select only genes in every cell
     # this is the exact replica an in edgeR
     mask = np.array((x > 0).sum(0)).squeeze() == x.shape[0]
     tmp = x[:, mask]
-    if issparse(tmp):
+    if sp.issparse(tmp):
         tmp = tmp.A
 
     gm = np.array(np.exp(np.mean(np.log(tmp), axis=0))).squeeze()
     gm_mask = (gm > 0) & np.isfinite(gm)
 
-    if not issparse(x):
+    if not sp.issparse(x):
         return np.median(x[:, mask][:, gm_mask] / gm[gm_mask], axis=1)
 
-    return csc_median_axis_0(
-        x.tocsr()[:, mask][:, gm_mask].multiply(1.0 / gm[gm_mask]).tocsr().T
-    )
+    return csc_median_axis_0(x.tocsr()[:, mask][:, gm_mask].multiply(1.0 / gm[gm_mask]).tocsr().T)
 
 
 @_dispatch_computation.register(NormMode.NONE)
-def _(x: Union[np.ndarray, spmatrix], **_) -> np.ndarray:
+def _(x: Union[np.ndarray, sp.spmatrix], **_) -> np.ndarray:
     # unused
     return np.ones((x.shape[0],), dtype=x.dtype)
 
 
 def _calc_factor_weighted(
     ixs: np.ndarray,
-    obs_: Union[np.ndarray, spmatrix],
+    obs_: Union[np.ndarray, sp.spmatrix],
     obs_lib_size_: np.ndarray,
     ref: np.ndarray,
     ref_lib_size: float,
     logratio_trim: float = 0.3,
     sum_trim: float = 0.05,
     weight: bool = True,
     a_cutoff: float = -1e10,
     queue=None,
-    **_,
+    **_: Any,
 ) -> np.ndarray:
     with np.errstate(divide="ignore", invalid="ignore"):
         log_ref = np.log2(ref / ref_lib_size)
     res = np.empty(shape=(len(ixs),))
 
     for i, ix in enumerate(ixs):
         if queue is not None:
             queue.put(1)
 
         obs = obs_[ix]
-        if issparse(obs):
+        if sp.issparse(obs):
             obs = obs.A.squeeze(0)  # (genes,)
         obs_lib_size = obs_lib_size_[ix]
 
         res[i] = _calc_factor_weighted_helper(
             obs=obs,
             obs_lib_size=obs_lib_size,
             ref=ref,
@@ -348,15 +340,15 @@
 
     if queue is not None:
         queue.put(None)
 
     return res
 
 
-@njit(fastmath=True, cache=True)
+@nb.njit(fastmath=True, cache=True)
 def _calc_factor_weighted_helper(
     obs: np.ndarray,
     obs_lib_size: float,
     ref: np.ndarray,
     ref_lib_size: float,
     log_ref: np.ndarray,
     a_cutoff: float,
@@ -365,17 +357,15 @@
     weight: bool,
 ) -> float:
     o_scaled = obs / obs_lib_size
     log_obs = np.log2(o_scaled)
 
     log_r = log_obs - log_ref
     abs_e = (log_obs + log_ref) / 2.0
-    v = ((obs_lib_size - obs) / obs_lib_size / obs) + (
-        ref_lib_size - ref
-    ) / ref_lib_size / ref
+    v = ((obs_lib_size - obs) / obs_lib_size / obs) + (ref_lib_size - ref) / ref_lib_size / ref
 
     mask = np.isfinite(log_r) & np.isfinite(abs_e) & (abs_e > a_cutoff)
 
     log_r = log_r[mask]
     abs_e = abs_e[mask]
     v = v[mask]
 
@@ -386,54 +376,43 @@
     lol = np.floor(n * logratio_trim) + 1.0
     hil = n + 1 - lol
 
     los = np.floor(n * sum_trim) + 1.0
     his = n + 1 - los
 
     rank_log_r, rank_abs_e = _rankdata(log_r), _rankdata(abs_e)
-    mask = (
-        (rank_log_r >= lol)
-        & (rank_log_r <= hil)
-        & (rank_abs_e >= los)
-        & (rank_abs_e <= his)
-    )
+    mask = (rank_log_r >= lol) & (rank_log_r <= hil) & (rank_abs_e >= los) & (rank_abs_e <= his)
 
-    f = (
-        (np.nansum(log_r[mask] / v[mask]) / np.nansum(1.0 / v[mask]))
-        if weight
-        else np.nanmean(log_r[mask])
-    )
+    f = (np.nansum(log_r[mask] / v[mask]) / np.nansum(1.0 / v[mask])) if weight else np.nanmean(log_r[mask])
 
     return 2 ** f if np.isfinite(f) else 1.0
 
 
 def _get_knotlocs(
     pseudotime: Union[np.ndarray, Sequence],
     n_knots: int,
     uniform: bool = False,
 ) -> np.ndarray:
-    """
-    Find knot locations.
+    """Find knot locations.
 
     The first and last knots are always placed at the beginning and the of the ``pseudotime``.
 
     Parameters
     ----------
     pseudotime
         Pseudotemporal ordering of cells.
     n_knots
         Number of knots.
     uniform
         Whether to place the knots uniformly across the ``pseudotime`` or place them based on ``pseudotime``'s density.
 
     Returns
     -------
-    Array of shape `(n_knots,)` containing the locations of knots along the pseudotime.
+    Array of shape ``(n_knots,)`` containing the locations of knots along the pseudotime.
     """
-
     if n_knots <= 0:
         raise ValueError(f"Expected number of knots to be positive, found `{n_knots}`.")
 
     if np.any(~np.isfinite(pseudotime)):
         raise ValueError("Not all pseudotime values are finite.")
 
     pseudotime = np.asarray(pseudotime)
@@ -441,106 +420,94 @@
     unique = np.unique(pseudotime)
     if len(unique) in (0, 1):
         raise ValueError(f"All pseudotime values are the same: `{unique}`.")
 
     if pseudotime.ndim == 2 and pseudotime.shape[1] == 1:
         pseudotime = pseudotime.squeeze(1)
     if pseudotime.ndim != 1:
-        raise ValueError(
-            f"Expected `pseudotime` to have `1` dimension, found `{pseudotime.ndim}`."
-        )
+        raise ValueError(f"Expected `pseudotime` to have `1` dimension, found `{pseudotime.ndim}`.")
 
     if uniform:
         # replicate the result from not uniform
         return (
             np.linspace(np.min(pseudotime), np.max(pseudotime), n_knots, endpoint=True)
             if n_knots > 1
             else np.array([np.max(pseudotime)])
         )
 
-    x = np.quantile(
-        pseudotime, q=np.arange(n_knots, dtype=np.float64) / max(n_knots - 1, 1)
-    )
+    x = np.quantile(pseudotime, q=np.arange(n_knots, dtype=np.float64) / max(n_knots - 1, 1))
     x[0] = np.min(pseudotime)
     x[-1] = np.max(pseudotime)
 
     u, ix, c = np.unique(x, return_index=True, return_counts=True)
 
     if len(u) != len(x):
         knotlocs = []
         for start, end, size in zip(x[ix], x[ix[1:]], c):
             knotlocs.extend(np.linspace(start, end, size, endpoint=False))
-        knotlocs.extend(
-            np.linspace(knotlocs[-1], x[ix[-1]], c[-1] + 1, endpoint=True)[1:]
-        )
+        knotlocs.extend(np.linspace(knotlocs[-1], x[ix[-1]], c[-1] + 1, endpoint=True)[1:])
         knotlocs = np.array(knotlocs)
     else:
         knotlocs = x
 
     logg.debug(f"Setting knot locations to `{list(knotlocs)}`")
 
     return knotlocs
 
 
 @inject_docs(key=_OFFSET_KEY)
 @d.dedent
 def _get_offset(
-    adata: Union[AnnData, np.ndarray, spmatrix],
+    adata: Union[AnnData, np.ndarray, sp.spmatrix],
     layer: Optional[str] = None,
     use_raw: bool = True,
     ref_ix: Optional[int] = None,
     recompute: bool = False,
     **kwargs,
 ) -> np.ndarray:
-    """
-    Return an offset for GAM.
+    """Return an offset for GAM.
 
     Parameters
     ----------
     %(adata)s
     layer
-        Layer in ``adata.layers`` or `None` for ``adata.X``. Only used when ``use_raw=False``.
+        Layer in :attr:`~anndata.AnnData.layers`` or :obj:`None` for :attr:`~anndata.AnnData.X`.
+        Only used when ``use_raw=False``.
     use_raw
-        Whether to access ``adata.raw``.
+        Whether to access :attr:`~anndata.AnnData.raw`.
     ref_ix
-        Index of a reference cell. If `None`, it will be determined automatically.
+        Index of a reference cell. If :obj:`None`, it will be determined automatically.
     recompute
-        Whether to recompute the offset if already found in ``adata.obs[{key!r}]``.
+        Whether to recompute the offset if already found in :attr:`adata.obs['{key}'] <anndata.AnnData.obs>`.
     kwargs
-        Keyword arguments for :func:`cellrank.ul.models._utils._calc_norm_factors`.
+        Keyword arguments for :func:`_utils._calc_norm_factors`.
 
     Returns
     -------
-    Array of shape `(adata.n_obs,)` containing the offset.
+    Array of shape ``(adata.n_obs,)`` containing the offset.
     """
     with np.errstate(divide="ignore", invalid="ignore"):
         if not recompute and isinstance(adata, AnnData) and _OFFSET_KEY in adata.obs:
             logg.debug(f"Fetching offset from `adata.obs[{_OFFSET_KEY!r}]`")
             return adata.obs[_OFFSET_KEY].values.copy()
 
         logg.debug(f"Calculating offset for `{adata.shape[0]}` cells")
 
         data = _extract_data(adata, layer=layer, use_raw=use_raw)
         try:
-            nf = _calculate_norm_factors(
-                adata, layer=layer, use_raw=use_raw, ref_ix=ref_ix, **kwargs
-            )
-        except Exception as e:  # noqa: B902
-            logg.debug(
-                f"Unable to calculate the normalization factors, setting them to `1`. Reason: `{e}`"
-            )
+            nf = _calculate_norm_factors(adata, layer=layer, use_raw=use_raw, ref_ix=ref_ix, **kwargs)
+        except Exception as e:  # noqa: BLE001
+            logg.debug(f"Unable to calculate the normalization factors, setting them to `1`. Reason: `{e}`")
             nf = np.ones(len(adata), dtype=np.float64)
 
         offset = np.log(nf * np.array(data.sum(1)).squeeze())
         offset[offset == 0] = 1.0
 
         mask = ~np.isfinite(offset) | np.isnan(offset)
         if np.any(mask):
-            logg.warning(
-                f"`{np.sum(mask)}` elements are not finite. Setting them to `1`"
-            )
+            logg.warning(f"`{np.sum(mask)}` elements are not finite. Setting them to `1`")
             offset[mask] = 1.0
 
         if isinstance(adata, AnnData):
             adata.obs[_OFFSET_KEY] = offset
 
         return offset
```

### Comparing `cellrank-1.5.1/cellrank.egg-info/requires.txt` & `cellrank-2.0.0/src/cellrank.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,42 @@
+anndata>=0.8
 docrep>=0.3.0
 joblib>=0.13.1
-matplotlib>=3.3.0
+matplotlib<3.7.2,>=3.5.0
 networkx>=2.2
-numba>=0.51.0
+numba!=0.57.0,>=0.51.0
 numpy>=1.17.0
-pandas>=1.2.0
+pandas>=1.5.0
 pygam>=0.8.0
-pygpcca>=1.0.3
+pygpcca>=1.0.4
 scanpy>=1.7.2
 scikit-learn>=0.24.0
 scipy>=1.2.0
-scvelo>=0.2.4
+scvelo>=0.2.5
 seaborn>=0.10.0
-setuptools>=41.0.1
-typing_extensions
 wrapt>=1.12.1
 
 [dev]
-pre-commit>=2.9.3
-tox>=3.23.0
-towncrier>=21.3.0
+pre-commit>=3.0.0
+tox>=4
 
 [docs]
-bezier
-ipython
-ipywidgets
-leidenalg
-memory_profiler>=0.58.0
-nbsphinx<0.8.7,>=0.8
-pypandoc
-python-igraph
-sphinx>=4
-sphinx-autodoc-annotation
+sphinx>=5.1.1
+furo>=2022.09.29
+myst-nb>=0.17.1
+sphinx-tippy>=0.4.1
 sphinx-autodoc-typehints>=1.10.3
-sphinx-gallery
-sphinx_copybutton
-sphinx_rtd_theme
+sphinx_copybutton>=0.5.0
+sphinx_design>=0.3.0
 sphinxcontrib-bibtex>=2.3.0
-
-[external]
-statot>=0.0.14
-POT
-
-[krylov]
-pygpcca[slepc]
+sphinxcontrib-spelling>=7.6.2
 
 [test]
-pytest>=6.1.1
-pytest-mock>=3.5.1
-pytest-xdist>=2.1.0
-pytest-cov
-Pillow
-filelock
-python-igraph
+pytest>=7
+pytest-xdist>=3
+pytest-mock>=3.5.0
+pytest-cov>=4
+coverage[toml]>=7
+igraph
 leidenalg
-bezier
+Pillow
 jax
-jaxlib
```

