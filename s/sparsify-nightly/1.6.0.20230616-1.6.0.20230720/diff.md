# Comparing `tmp/sparsify-nightly-1.6.0.20230616.tar.gz` & `tmp/sparsify-nightly-1.6.0.20230720.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sparsify-nightly-1.6.0.20230616.tar", last modified: Fri Jun 16 05:36:00 2023, max compression
+gzip compressed data, was "dist/sparsify-nightly-1.6.0.20230720.tar", last modified: Thu Jul 20 19:17:22 2023, max compression
```

## Comparing `sparsify-nightly-1.6.0.20230616.tar` & `sparsify-nightly-1.6.0.20230720.tar`

### file list

```diff
@@ -1,122 +1,80 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/NOTICE
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3748 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13378 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/projects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1034 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8185 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/jobs.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      633 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1542 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/tensorflow__integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/pytorch__integration.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/pytorch__training.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3042 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    28990 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/projects_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    37555 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/projects_profiles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25153 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/projects_data.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    31922 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/projects_optimizations_pruning.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2658 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/projects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      887 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1775 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/projects_benchmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2354 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/projects_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    30313 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/projects_optimizations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    78858 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/projects_optimizations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18291 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/projects_benchmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2482 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/model_repo.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2663 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/ui.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1318 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2958 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      844 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15464 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/projects_benchmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8351 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/projects_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11049 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/manager.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    25623 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/projects_profiles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12375 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/workers/projects_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/version.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  7042398 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/2.0f4fe034.chunk.js.map
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8276 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/runtime-main.c0a252e2.js.map
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  2123616 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/2.0f4fe034.chunk.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3068 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/2.0f4fe034.chunk.js.LICENSE.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   310741 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/main.a1ae51dc.chunk.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1557 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/runtime-main.c0a252e2.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)  1097786 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/js/main.a1ae51dc.chunk.js.map
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2748 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/project.dd29f0f6.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2084 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/icon.aba82cce.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3579 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/analyze.7c3e0835.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4070 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/icon.819c3ff5.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4009 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/profile.f82adafa.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2440 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/icon.b1f0d69f.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2239 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/icon.2c79b78b.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3804 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/optimize.58851c1b.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1628 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/icon.f1cd4814.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2084 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/model.aba82cce.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4269 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/integrate.152d2596.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      865 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/logo.fe6fc378.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3652 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/static/media/icon.c1c9830b.svg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/robots.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1956 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/precache-manifest.0cd8aa23c0d275b3eeb0d68b8ca88a91.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15406 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/favicon.ico
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12931 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/android-chrome-192x192.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1068 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/favicon-32x32.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/favicon-16x16.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    55271 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/android-chrome-512x512.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11724 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/assets/favicon/apple-touch-icon.png
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2312 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/index.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      567 2023-06-16 05:33:46.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/manifest.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1181 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/service-worker.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/.gitkeep
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1836 2023-06-16 05:35:59.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/ui/asset-manifest.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5018 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/app.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/utils/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/utils/system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/utils/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2456 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/log.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4009 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/base.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3861 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/projects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      946 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2290 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/jobs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1872 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/projects_benchmark.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3239 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/projects_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2857 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/projects_profiles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3106 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/projects_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1933 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/models/projects_optimizations.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3021 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/system.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4484 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/projects.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      989 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3476 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/jobs.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1121 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/errors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4595 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/projects_model.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3476 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/helpers.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9041 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/projects_profiles.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3302 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/projects_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17122 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/projects_optimizations.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5237 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/projects_benchmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4878 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/model_repo.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       48 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18721 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      444 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4119 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/src/sparsify_nightly.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       53 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15239 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4344 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/setup.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18721 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-06-16 05:30:04.000000 sparsify-nightly-1.6.0.20230616/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-06-16 05:36:00.000000 sparsify-nightly-1.6.0.20230616/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1243 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/NOTICE
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/create/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4248 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/create/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      728 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/create/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1817 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/create/schemas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5235 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/login.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/cli/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/cli/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/cli/opts.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5045 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/cli/run.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/version.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      825 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      760 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3325 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/nm_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2161 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/hardware_analyzer.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9333 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6855 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/error_handler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/scripts/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2385 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/scripts/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      617 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/scripts/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/transformers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/transformers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    26268 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/transformers/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13031 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/transformers/runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3701 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/deployment_instructions.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      695 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3356 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18157 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/yolov5/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6896 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/yolov5/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8349 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/yolov5/runner.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      656 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/image_classification/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      676 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/image_classification/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6146 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/image_classification/args.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8345 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/image_classification/runner.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      873 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/main.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      735 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1055 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/pathway_checks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5941 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/ort_health.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/gpu_device.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4247 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/system.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      748 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3681 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/task_name.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      877 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/nm_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4393 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/helpers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5067 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/constants.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      758 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/utils/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/one_shot/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3353 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/one_shot/api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      745 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/one_shot/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3758 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/schemas/tuning_hyperparameters.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11587 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/schemas/auto_api.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      715 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/src/sparsify/schemas/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      159 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      316 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2167 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/src/sparsify_nightly.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      112 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    23875 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4453 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    29051 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       56 2023-07-20 19:15:01.000000 sparsify-nightly-1.6.0.20230720/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      625 2023-07-20 19:17:22.000000 sparsify-nightly-1.6.0.20230720/setup.cfg
```

### Comparing `sparsify-nightly-1.6.0.20230616/NOTICE` & `sparsify-nightly-1.6.0.20230720/NOTICE`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/__init__.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/cli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# flake8: noqa
-
 # Copyright (c) 2021 - present / Neuralmagic, Inc. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/code_samples/pytorch__integration.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/utils/nm_api.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,23 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-# flake8: noqa
+import os
 
-import math
 
-from sparseml.pytorch.optim import ScheduledModifierManager, ScheduledOptimizer
-from sparseml.pytorch.utils import PythonLogger, TensorBoardLogger
+__all__ = ["get_base_url"]
+_DEFAULT_BASE_URL = "https://api.neuralmagic.com"
 
 
-manager = ScheduledModifierManager.from_yaml("/PATH/TO/config.yaml")
-optimizer = ScheduledOptimizer(
-    optimizer,
-    MODEL,
-    manager,
-    steps_per_epoch=math.ceil(len(TRAIN_DATASET) / TRAIN_BATCH_SIZE),
-    loggers=[TensorBoardLogger(), PythonLogger()],
-)
+def get_base_url() -> str:
+    """
+    :return The base url for sparsify backend server
+    """
+    return os.getenv("SPARSIFY_BACKEND_URL", default=_DEFAULT_BASE_URL)
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/__init__.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/schemas/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,18 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Utility functions and classes for flask blueprints
-"""
-
 # flake8: noqa
-from .helpers import *
-from .projects import *
-from .projects_benchmark import *
-from .projects_data import *
-from .projects_optimizations import *
-from .projects_optimizations_pruning import *
+# isort: skip_file
+
+from .tuning_hyperparameters import *
+from .auto_api import *
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/blueprints/utils/helpers.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/create/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,27 +9,13 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Helper functions and classes for flask blueprints
+Interface and utilities for sparsify.create
 """
 
-
-__all__ = [
-    "API_ROOT_PATH",
-    "HTTPNotFoundError",
-]
-
-
-API_ROOT_PATH = "/api"
-
-
-class HTTPNotFoundError(Exception):
-    """
-    Expected error raised when a 404 should be encountered by the user
-    """
-
-    def __init__(self, *args: object) -> None:
-        super().__init__(*args)
+# flake8: noqa
+from .api import *
+from .schemas import *
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/workers/__init__.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/auto/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Code for running background jobs
-"""
-
 # flake8: noqa
-from .base import *
-from .manager import *
-from .projects_benchmark import *
-from .projects_data import *
-from .projects_model import *
-from .projects_profiles import *
+# isort: skip_file
+
+from .helpers import *
+from .error_handler import *
+from .hardware_analyzer import *
+from .nm_api import *
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/version.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/version.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/utils/system.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/utils/system.py`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/utils/__init__.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/auto/tasks/object_detection/yolov5/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,13 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Utility functions for sparsify
-"""
-
 # flake8: noqa
-from .system import *
+
+from .args import *
+from .runner import *
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/__init__.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/utils/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,23 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""
-Schemas for working with the sparsify server
-"""
-
 # flake8: noqa
-from .errors import *
+# isort: skip_file
+
+from .task_name import *
+from .constants import *
+from .nm_api import *
 from .helpers import *
-from .jobs import *
-from .model_repo import *
-from .projects import *
-from .projects_benchmarks import *
-from .projects_data import *
-from .projects_model import *
-from .projects_optimizations import *
-from .projects_profiles import *
-from .system import *
```

### Comparing `sparsify-nightly-1.6.0.20230616/src/sparsify/schemas/errors.py` & `sparsify-nightly-1.6.0.20230720/src/sparsify/check_environment/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,27 +7,20 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from sparsify.check_environment import check_for_gpu, check_ort_health
 
-"""
-Schemas for anything related to errors occurring in the flask app
-"""
 
-from marshmallow import Schema, fields
-
-
-__all__ = ["ErrorSchema"]
-
-
-class ErrorSchema(Schema):
+def main():
     """
-    Error schema to return in the event of an error encountered while running the app
+    Check the environment for compatibility with the sparsifyml package
     """
+    check_for_gpu()
+    check_ort_health()
+
 
-    success = fields.Bool(default=False, missing=False, required=False)
-    error_code = fields.Int(default=-1, missing=-1, required=False)
-    error_type = fields.Str(required=True)
-    error_message = fields.Str(required=True)
+if __name__ == "__main__":
+    main()
```

### Comparing `sparsify-nightly-1.6.0.20230616/LICENSE` & `sparsify-nightly-1.6.0.20230720/LICENSE`

 * *Files identical despite different names*

### Comparing `sparsify-nightly-1.6.0.20230616/setup.py` & `sparsify-nightly-1.6.0.20230720/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
-from sys import platform
 from typing import Dict, List, Tuple
 
 from setuptools import find_packages, setup
 
 
 # default variables to be overwritten by the version.py file
 is_release = None
@@ -29,49 +28,38 @@
 print(f"loaded version {version} from src/sparsify/version.py")
 version_nm_deps = f"{version_major_minor}.0"
 
 _PACKAGE_NAME = "sparsify" if is_release else "sparsify-nightly"
 
 
 _deps = [
-    "apispec>=3.0.0",
-    "flasgger>=0.9.0",
-    "Flask>=1.0.0",
-    "Flask-Cors>=3.0.0",
-    "marshmallow>=3.0.0",
-    "peewee>=3.0.0",
+    "pydantic>=1.8.2,<2.0.0",
+    "pyyaml>=5.0.0",
+    "click~=8.0.0",
+    "tensorboard>=2.0.0",
+    "setuptools>=56.0.0",
+    "optuna>=3.0.2",
+    "onnxruntime-gpu",
 ]
-
 _nm_deps = [
     f"{'sparsezoo' if is_release else 'sparsezoo-nightly'}~={version_nm_deps}",
-    f"{'sparseml' if is_release else 'sparseml-nightly'}~={version_nm_deps}",
+    f"{'sparseml' if is_release else 'sparseml-nightly'}[torchvision,transformers,yolov5]~={version_nm_deps}",  # noqa E501
+    f"{'deepsparse' if is_release else 'deepsparse-nightly'}~={version_nm_deps}",
 ]
 
 
 _dev_deps = [
-    "beautifulsoup4==4.9.3",
     "black>=20.8b1",
     "flake8>=3.8.3",
     "isort>=5.7.0",
-    "m2r2~=0.2.7",
-    "mistune==0.8.4",
-    "myst-parser~=0.14.0",
-    "rinohtype>=0.4.2",
-    "sphinx>=3.4.0",
-    "sphinx-copybutton>=0.3.0",
-    "sphinx-markdown-tables>=0.0.15",
-    "sphinx-multiversion==0.2.4",
-    "sphinx-rtd-theme",
     "pytest>=6.0.0",
     "wheel>=0.36.2",
+    "fastai>=2.7.7",
 ]
 
-if platform == "linux" or platform == "linux2":
-    _deps.extend(["pysqlite3-binary>=0.4.0"])
-
 
 def _setup_packages() -> List:
     return find_packages(
         "src", include=["sparsify", "sparsify.*"], exclude=["*.__pycache__.*"]
     )
 
 
@@ -84,15 +72,21 @@
 
 
 def _setup_extras() -> Dict:
     return {"dev": _dev_deps}
 
 
 def _setup_entry_points() -> Dict:
-    return {"console_scripts": ["sparsify=sparsify.app:main"]}
+    return {
+        "console_scripts": [
+            "sparsify.run=sparsify.cli.run:main",
+            "sparsify.login=sparsify.login:main",
+            "sparsify.check_environment=sparsify.check_environment.main:main",
+        ]
+    }
 
 
 def _setup_long_description() -> Tuple[str, str]:
     return open("README.md", "r", encoding="utf-8").read(), "text/markdown"
 
 
 setup(
@@ -121,14 +115,17 @@
     extras_require=_setup_extras(),
     entry_points=_setup_entry_points(),
     python_requires=">=3.7.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: POSIX :: Linux",
         "Topic :: Scientific/Engineering",
```

### Comparing `sparsify-nightly-1.6.0.20230616/setup.cfg` & `sparsify-nightly-1.6.0.20230720/setup.cfg`

 * *Files identical despite different names*

