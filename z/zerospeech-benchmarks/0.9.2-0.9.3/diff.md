# Comparing `tmp/zerospeech-benchmarks-0.9.2.tar.gz` & `tmp/zerospeech-benchmarks-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zerospeech-benchmarks-0.9.2.tar", last modified: Wed Jul 12 14:54:32 2023, max compression
+gzip compressed data, was "zerospeech-benchmarks-0.9.3.tar", last modified: Thu Jul 20 13:07:34 2023, max compression
```

## Comparing `zerospeech-benchmarks-0.9.2.tar` & `zerospeech-benchmarks-0.9.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.958901 zerospeech-benchmarks-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/.github/workflows/build-conda-recipe.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/.github/workflows/pipy-pyblish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    47928 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/conda-recipe/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/abx17.md
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/abxLS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/prosAudit.md
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/sLM21.md
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/docs/tde17.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abx17.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abxLS.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/prosAudit.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/sLM21.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/benchmark_examples/tde17.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/examples/zr_testing.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.966901 zerospeech-benchmarks-0.9.2/imgs/
--rw-r--r--   0 runner    (1001) docker     (123)    72584 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/imgs/checkpoints.png
--rw-r--r--   0 runner    (1001) docker     (123)    58400 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/imgs/datasets.png
--rw-r--r--   0 runner    (1001) docker     (123)    77287 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/imgs/samples.png
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.970901 zerospeech-benchmarks-0.9.2/zerospeech/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.970901 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abx17.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abxLS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/prosAudit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/sLM21.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/tde17.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.974902 zerospeech-benchmarks-0.9.2/zerospeech/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/cli_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/cmd/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.974902 zerospeech-benchmarks-0.9.2/zerospeech/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2015.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2017.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2019.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2021.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.974902 zerospeech-benchmarks-0.9.2/zerospeech/generics/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/checkpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/data_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/named_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/generics/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/httpw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.978901 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/abxLS.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.978901 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/abxLS.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/sLM21.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/tde17.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/prosaudit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/sLM21.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/tde17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/vocolab_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/networkio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/out.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/startup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.978901 zerospeech-benchmarks-0.9.2/zerospeech/submissions/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/meta_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/score_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/abx17.py
--rw-r--r--   0 runner    (1001) docker     (123)    12721 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/abxLS.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/prosAudit.py
--rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/sLM21.py
--rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/submissions/tde17.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.982902 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/lexical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/prosody.py
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/semantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/syntactic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/tasks/tde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/zerospeech/upload/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/file_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/submission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/upload/user_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/zerospeech/validators/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/validators/base_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-12 14:54:13.000000 zerospeech-benchmarks-0.9.2/zerospeech/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:54:32.986902 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47928 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-12 14:54:32.000000 zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.874681 zerospeech-benchmarks-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.874681 zerospeech-benchmarks-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/.github/workflows/build-conda-recipe.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/.github/workflows/pipy-pyblish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    47931 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.874681 zerospeech-benchmarks-0.9.3/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/conda-recipe/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.878681 zerospeech-benchmarks-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/docs/abx17.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/docs/abxLS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/docs/prosAudit.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/docs/sLM21.md
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/docs/tde17.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.878681 zerospeech-benchmarks-0.9.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.878681 zerospeech-benchmarks-0.9.3/examples/benchmark_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/examples/benchmark_examples/abx17.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/examples/benchmark_examples/abxLS.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/examples/benchmark_examples/prosAudit.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/examples/benchmark_examples/sLM21.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/examples/benchmark_examples/tde17.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16185 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/examples/zr_testing.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.878681 zerospeech-benchmarks-0.9.3/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    72584 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/imgs/checkpoints.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58400 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/imgs/datasets.png
+-rw-r--r--   0 runner    (1001) docker     (123)    77287 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/imgs/samples.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.878681 zerospeech-benchmarks-0.9.3/zerospeech/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.878681 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/abx17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/abxLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/prosAudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/tde17.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.882681 zerospeech-benchmarks-0.9.3/zerospeech/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/cli_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/cmd/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.882681 zerospeech-benchmarks-0.9.3/zerospeech/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/datasets/_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2015.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2019.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2021.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.882681 zerospeech-benchmarks-0.9.3/zerospeech/generics/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/generics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/generics/checkpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/generics/data_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/generics/named_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/generics/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/generics/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/httpw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.882681 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/abxLS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.882681 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/abxLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/tde17.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/prosaudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/tde17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/vocolab_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/networkio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/startup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.882681 zerospeech-benchmarks-0.9.3/zerospeech/submissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/meta_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/score_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7682 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/abx17.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/abxLS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/prosAudit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26111 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/sLM21.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/submissions/tde17.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abx17/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abx17/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abx17/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abx17/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abxLS_phoneme/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abxLS_phoneme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abxLS_phoneme/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abxLS_phoneme/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/lexical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/prosody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/semantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/syntactic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/tasks/tde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/upload/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/upload/file_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15563 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/upload/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/upload/user_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/validators/base_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-20 13:07:16.000000 zerospeech-benchmarks-0.9.3/zerospeech/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:07:34.886681 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47931 2023-07-20 13:07:34.000000 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-07-20 13:07:34.000000 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:07:34.000000 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-20 13:07:34.000000 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-20 13:07:34.000000 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 13:07:34.000000 zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/top_level.txt
```

### Comparing `zerospeech-benchmarks-0.9.2/.github/workflows/build-conda-recipe.yaml` & `zerospeech-benchmarks-0.9.3/.github/workflows/build-conda-recipe.yaml`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/.github/workflows/pipy-pyblish.yaml` & `zerospeech-benchmarks-0.9.3/.github/workflows/pipy-pyblish.yaml`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/LICENSE.txt` & `zerospeech-benchmarks-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/PKG-INFO` & `zerospeech-benchmarks-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerospeech-benchmarks
-Version: 0.9.2
+Version: 0.9.3
 Summary: Toolset for usage of the Zero Resource Challenge Benchmarks.
 Author-email: Nicolas Hamilakis <nicolas.hamilakis@ens.psl.eu>, CoML Team <dev@zerospeech.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,16 +690,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: vocolab
 Provides-Extra: tts019
-Provides-Extra: abx
-Provides-Extra: abx2
+Provides-Extra: abx17
+Provides-Extra: abxLS
 Provides-Extra: tde
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Zero Resource Challenge Benchmark Toolkit  ![BETA](https://img.shields.io/badge/-BETA-blue)
```

### Comparing `zerospeech-benchmarks-0.9.2/README.md` & `zerospeech-benchmarks-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/TODO.md` & `zerospeech-benchmarks-0.9.3/TODO.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/conda-recipe/meta.yaml` & `zerospeech-benchmarks-0.9.3/conda-recipe/meta.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 package:
   name: {{ name|lower }}
   version: {{ version }}
 
 source:
   url: https://pypi.io/packages/source/{{ name[0] }}/{{ name }}/zerospeech-benchmarks-{{ version }}.tar.gz
-  sha256: 59668c988d80386fa94940dbac3afd4a5ea408f8c0472747abbdd332b86e4d52
+  sha256: 7407fffdb4f8ec296f45892d077d3d9c07c1798f1f6f9db4c1e72ee95035a2a0
 
 build:
   entry_points:
     - zrc = zerospeech.startup:main
   noarch: python
   script: {{ PYTHON }} -m pip install . -vv
   number: 0
```

### Comparing `zerospeech-benchmarks-0.9.2/docs/abxLS.md` & `zerospeech-benchmarks-0.9.3/docs/abxLS.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/docs/prosAudit.md` & `zerospeech-benchmarks-0.9.3/docs/prosAudit.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/docs/sLM21.md` & `zerospeech-benchmarks-0.9.3/docs/sLM21.md`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abx17.ipynb` & `zerospeech-benchmarks-0.9.3/examples/benchmark_examples/abx17.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/abxLS.ipynb` & `zerospeech-benchmarks-0.9.3/examples/benchmark_examples/abxLS.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/prosAudit.ipynb` & `zerospeech-benchmarks-0.9.3/examples/benchmark_examples/prosAudit.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/sLM21.ipynb` & `zerospeech-benchmarks-0.9.3/examples/benchmark_examples/sLM21.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/examples/benchmark_examples/tde17.ipynb` & `zerospeech-benchmarks-0.9.3/examples/benchmark_examples/tde17.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/examples/zr_testing.ipynb` & `zerospeech-benchmarks-0.9.3/examples/zr_testing.ipynb`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/imgs/checkpoints.png` & `zerospeech-benchmarks-0.9.3/imgs/checkpoints.png`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/imgs/datasets.png` & `zerospeech-benchmarks-0.9.3/imgs/datasets.png`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/imgs/samples.png` & `zerospeech-benchmarks-0.9.3/imgs/samples.png`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/pyproject.toml` & `zerospeech-benchmarks-0.9.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -47,32 +47,35 @@
 ]
 
 tts019 = [
     # todo migrate towards pypi url once module is public
     "tts019-evaluator @ https://github.com/zerospeech/tts019-evaluator/archive/master.zip"
 ]
 
-abx = [
-    "zerospeech-libriabx>=1.0.5"
+abx17 = [
+    "zerospeech-libriabx>=1.0.5",
+    "virtual-dataset"
 ]
-abx2 = [
+abxLS = [
+    # ABX2 used for ABXLS
     "zerospeech-libriabx2>=0.9.7",
     "virtual-dataset"
 ]
 tde = [
     "zerospeech-tde>=2.0.3"
 ]
 
 all = [
     # TDE
     "zerospeech-tde>=2.0.3",
-    # ABX2
+    # ABX2 used for ABXLS
     "zerospeech-libriabx2>=0.9.8",
     "virtual-dataset",
-    #
+    # ABXLS Legacy (used for abx17)
+    "zerospeech-libriabx>=1.0.5"
 ]
 
 dev = [
     "ipython",
     "jupyter",
     "pytest",
     "twine",
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/_model.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/_model.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abx17.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/abx17.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from pydantic import Field
 
 from zerospeech.datasets import ZRC2017Dataset
 from zerospeech.generics import FileListItem, FileItem
 from zerospeech.submissions import Submission
 from zerospeech.submissions.abx17 import ABX17Submission
-from zerospeech.tasks.abx.abx_librispeech import SimpleABXTask
+from zerospeech.tasks.abx.abx17 import SimpleABXTask
 from ._model import Benchmark
 
 return_type = List[Tuple[str, FileListItem, FileItem]]
 
 
 class ABX17Task(SimpleABXTask):
     """ ABX task for abx-17 """
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/abxLS.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/abxLS.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from zerospeech.datasets import AbxLSDataset
 from zerospeech.generics import (
     FileItem, FileListItem
 )
 from zerospeech.submissions.abxLS import AbxLSSubmission
 from zerospeech.submissions import Submission
-from zerospeech.tasks.abx.abx_phoneme import SimpleABXPhonemeTask, ContextMode
+from zerospeech.tasks.abx.abxLS_phoneme import SimpleABXPhonemeTask, ContextMode
 from ._model import Benchmark
 
 return_type = Tuple[str, FileItem, FileListItem, ContextMode]
 
 
 class AbxLSTask(SimpleABXPhonemeTask):
     """ ABX task for abx-LS-Rob """
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/misc.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/misc.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/prosAudit.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/prosAudit.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/sLM21.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/sLM21.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/benchmarks/tde17.py` & `zerospeech-benchmarks-0.9.3/zerospeech/benchmarks/tde17.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/cmd/benchmarks.py` & `zerospeech-benchmarks-0.9.3/zerospeech/cmd/benchmarks.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/cmd/cli_lib.py` & `zerospeech-benchmarks-0.9.3/zerospeech/cmd/cli_lib.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/cmd/generic.py` & `zerospeech-benchmarks-0.9.3/zerospeech/cmd/generic.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/cmd/submission.py` & `zerospeech-benchmarks-0.9.3/zerospeech/cmd/submission.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/cmd/submit.py` & `zerospeech-benchmarks-0.9.3/zerospeech/cmd/submit.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/cmd/user.py` & `zerospeech-benchmarks-0.9.3/zerospeech/cmd/user.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/data_loaders.py` & `zerospeech-benchmarks-0.9.3/zerospeech/data_loaders.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2015.py` & `zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2015.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2017.py` & `zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2017.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2019.py` & `zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2019.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/datasets/zrc_2021.py` & `zerospeech-benchmarks-0.9.3/zerospeech/datasets/zrc_2021.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/generics/checkpoints.py` & `zerospeech-benchmarks-0.9.3/zerospeech/generics/checkpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import ClassVar, Type
 
-from ..misc import download_extract_zip
-from ..out import console
+from zerospeech.misc import download_extract_archive
+from zerospeech.out import console
+from zerospeech.settings import get_settings
 from .repository import DownloadableItem, RepoItemDir, RepositoryItemType
-from ..settings import get_settings
 
 st = get_settings()
 
 
 class CheckPointItem(DownloadableItem):
     key_name: ClassVar[RepositoryItemType] = "checkpoints"
 
     def pull(self, *, verify: bool = True, quiet: bool = False, show_progress: bool = False):
         md5_hash = ""
         if verify:
             md5_hash = self.origin.md5sum
 
         # download & extract archive
-        download_extract_zip(self.origin.zip_url, self.location, int(self.origin.total_size),
-                             filename=self.name, md5sum_hash=md5_hash, quiet=quiet, show_progress=show_progress)
+        download_extract_archive(self.origin.zip_url, self.location, int(self.origin.total_size),
+                                 filename=self.name, md5sum_hash=md5_hash, quiet=quiet, show_progress=show_progress)
         if not quiet:
             console.print(f"[green]Checkpoint set {self.name} installed successfully !!")
 
 
 class CheckpointDir(RepoItemDir):
     """ Checkpoint Directory Management """
     item_type: ClassVar[Type[DownloadableItem]] = CheckPointItem
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/generics/data_items.py` & `zerospeech-benchmarks-0.9.3/zerospeech/generics/data_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     flac = "flac"
     item = "item"  # abx task file
     tsv = "tsv"
     json = "json"
     yaml = "yaml"
     phn = "phn"  # phone alignment file
     wrd = "wrd"  # words alignment file
-    vad = "vad.csv" # vad segmentation file in csv format
+    vad = "vad.csv"  # vad segmentation file in csv format
 
     @property
     def ext(self) -> str:
         return f".{self.value}"
 
     @classmethod
     def dataframe_types(cls):
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/generics/named_storage.py` & `zerospeech-benchmarks-0.9.3/zerospeech/generics/named_storage.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/generics/repository.py` & `zerospeech-benchmarks-0.9.3/zerospeech/generics/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         current_type = values.get('type', 'internal')
         values['type'] = current_type
         assert current_type in valid_types, f'Type should be one of the following {valid_types}'
 
         if current_type == 'internal':
             assert values.get('zip_url') is not None \
                    or values.get('zip_parts') is not None, \
-                   "Internal Items must have either a zip_url or a zip_parts value."
+                "Internal Items must have either a zip_url or a zip_parts value."
         elif values.get('type') == 'external':
             assert values.get('install_config') is not None, "External items must have an install_config field"
         return values
 
 
 class RepositoryIndex(BaseModel):
     """ Item Indexing all datasets available online various repositories."""
@@ -142,16 +142,16 @@
         pass
 
 
 class ImportableItem(OriginItem, abc.ABC):
     """Abstract class to define item that can be imported from a local resource """
 
     @abc.abstractmethod
-    def import_(self, location: Path, *, verify: bool = True, quiet: bool = False, show_progress: bool = False):
-        """Import items from source material located locally """
+    def import_zip(self, *, archive: Path):
+        """ Import dataset from an archive """
         pass
 
 
 class RepoItemDir(BaseModel, abc.ABC):
     """ Abstract class defining a directory manager for repository items of a specific type """
     root_dir: DirectoryPath
     item_type: ClassVar[Union[Type[DownloadableItem], Type[ImportableItem]]]
@@ -168,25 +168,33 @@
 
     @property
     def available_items(self) -> List[str]:
         index = RepositoryIndex.load()
         item_list: List[RepositoryItem] = getattr(index, self.item_type.key_name, [])
         return [d.name for d in item_list]
 
-    def find_in_repository(self, name: str) -> Optional[RepositoryItem]:
+    def find_by_hash(self, hash_code: str) -> Optional[RepositoryItem]:
+        index = RepositoryIndex.load()
+        item_list: List[RepositoryItem] = getattr(index, self.item_type.key_name, [])
+        for d in item_list:
+            if d.md5sum == hash_code:
+                return d
+        return None
+
+    def find_by_name(self, name: str) -> Optional[RepositoryItem]:
         """Find all relevant items with the same type in repository """
         index = RepositoryIndex.load()
         item_list: List[RepositoryItem] = getattr(index, self.item_type.key_name, [])
         for d in item_list:
             if d.name == name:
                 return d
         return None
 
     def get(self, name, cls: Union[Type[DownloadableItem], Type[ImportableItem]] = None):
         loc = self.root_dir / name
-        repo = self.find_in_repository(name)
+        repo = self.find_by_name(name)
         if repo is None:
             return None
 
         if cls is None:
             return self.item_type(location=loc, origin=repo)
         return cls(location=loc, origin=repo)
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/generics/samples.py` & `zerospeech-benchmarks-0.9.3/zerospeech/generics/samples.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import ClassVar, Type
 
+from zerospeech.misc import download_extract_archive
+from zerospeech.out import console
+from zerospeech.settings import get_settings
 from .repository import DownloadableItem, RepositoryItemType, RepoItemDir
-from ..misc import download_extract_zip
-from ..out import console
-from ..settings import get_settings
 
 st = get_settings()
 
 
 class SampleItem(DownloadableItem):
     key_name: ClassVar[RepositoryItemType] = "samples"
 
     def pull(self, *, verify: bool = True, quiet: bool = False, show_progress: bool = False):
         md5_hash = ""
         if verify:
             md5_hash = self.origin.md5sum
 
         # download & extract archive
-        download_extract_zip(self.origin.zip_url, self.location, int(self.origin.total_size),
-                             filename=self.name, md5sum_hash=md5_hash, quiet=quiet, show_progress=show_progress)
+        download_extract_archive(self.origin.zip_url, self.location, int(self.origin.total_size),
+                                 filename=self.name, md5sum_hash=md5_hash, quiet=quiet, show_progress=show_progress)
         if not quiet:
             console.print(f"[green]Sample {self.name} installed successfully !!")
 
 
 class SamplesDir(RepoItemDir):
     """ Samples Directory Management """
     item_type: ClassVar[Type[DownloadableItem]] = SampleItem
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/httpw.py` & `zerospeech-benchmarks-0.9.3/zerospeech/httpw.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/_models.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/_models.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/abxLS.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/abxLS.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/abxLS.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/abxLS.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/sLM21.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/sLM21.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/exporters/tde17.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/exporters/tde17.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/prosaudit.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/prosaudit.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/sLM21.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/sLM21.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/utils.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/utils.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/leaderboards/vocolab_ext.py` & `zerospeech-benchmarks-0.9.3/zerospeech/leaderboards/vocolab_ext.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/misc.py` & `zerospeech-benchmarks-0.9.3/zerospeech/misc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import _thread as thread
 import contextlib
 import io
 import json
+import re
 import sys
-import sys
+import tarfile
 import threading
-import _thread as thread
-from time import sleep
+import urllib.parse
 from pathlib import Path
 from typing import Dict, List, Union, Optional, Protocol
 from zipfile import ZipFile
 
 import requests
 from Crypto.Hash import MD5  # noqa: the package name is not the same
 # from datasize import DataSize todo: find out why this was deleted ? maybe on unpushed thing on laptop?
@@ -110,46 +111,14 @@
         return self.__root__.human_readable(decimal=True)
 
     @property
     def as_bytes(self):
         return self.__root__
 
 
-# todo: see if i can remove this from the codebase ?
-# todo can we remove humanize from requirements ? or is it still used ?
-# class SizeUnit(enum.Enum):
-#     BYTES = 1
-#     KB = 2
-#     MB = 3
-#     GB = 4
-#
-#     @staticmethod
-#     def get_unit(text):
-#         """ Check contents of text to find units of measurement"""
-#
-#         if any(x in text for x in ("KB", "Ko", "K")):
-#             return SizeUnit.KB
-#         elif any(x in text for x in ("MB", "Mo", "M")):
-#             return SizeUnit.MB
-#         elif any(x in text for x in ("GB", "Go", "G")):
-#             return SizeUnit.GB
-#         else:
-#             return SizeUnit.BYTES
-#
-#     @staticmethod
-#     def convert_to_bytes(size_with_unit: str) -> float:
-#         # todo: replace this ??
-#         #: DataSize(size_with_unit.replace(' ', ''))
-#         return float("123.532")
-#
-#     @staticmethod
-#     def fmt(num: Union[int, float]) -> str:
-#         return humanize.naturalsize(num).replace(' ', '')
-
-
 def load_obj(location: Path) -> Union[Dict, List]:
     """ Loads an object from standard formats (.json, yaml, ...) to a standard structure (Dict, List)"""
     with location.open() as fp, location.open('rb') as bfp:
         if location.suffix == '.json':
             return json.load(fp)
         elif yaml and location.suffix in ('.yaml', '.yml'):
             return yaml.load(fp, Loader=yaml.FullLoader)
@@ -180,28 +149,55 @@
     # create folder if it does not exist
     output.mkdir(exist_ok=True, parents=True)
     # open & extract
     with ZipFile(archive, 'r') as zipObj:
         zipObj.extractall(output)
 
 
+def untar(archive: Path, output: Path):
+    """ Extract a tar archive (supports gzipped format) into the output directory"""
+    # create folder if it does not exist
+    output.mkdir(exist_ok=True, parents=True)
+    # Open & extract
+    with tarfile.open(archive, 'r') as tar:
+        tar.extractall(path=output)
+
+
+def extract(archive: Path, output: Path):
+    """ Extract an archive into the output directory """
+    if archive.suffix in ('.zip',):
+        unzip(archive, output)
+    elif archive.suffix in ('.tar', '.gz', '.tgz', '.bz2', '.tbz2', '.xz', '.txz'):
+        untar(archive, output)
+    else:
+        raise ValueError(f'{archive.suffix}: Unsupported archive format')
+
+
 def zip_folder(archive_file: Path, location: Path):
     """ Create a zip archive from a folder """
     with ZipFile(archive_file, 'w') as zip_obj:
         for file in filter(lambda x: x.is_file(), location.rglob("*")):
             zip_obj.write(file, str(file.relative_to(location)))
 
 
-def download_extract_zip(
-        zip_url: str, target_location: Path, size_in_bytes: int, *, filename: str = "",
+def get_request_filename(response: requests.Response) -> str:
+    """ Get filename from response """
+    if "Content-Disposition" in response.headers.keys():
+        return re.findall("filename=(.+)", response.headers["Content-Disposition"])[0]
+    else:
+        return Path(urllib.parse.unquote(response.url)).name
+
+
+def download_extract_archive(
+        archive_url: str, target_location: Path, size_in_bytes: int, *, filename: str = "",
         md5sum_hash: str = "", quiet: bool = False, show_progress: bool = True,
 ):
     tmp_dir = st.mkdtemp()
-    response = requests.get(zip_url, stream=True)
-    tmp_filename = tmp_dir / "download.zip"
+    response = requests.get(archive_url, stream=True)
+    tmp_filename = tmp_dir / get_request_filename(response)
 
     if quiet:
         _console = void_console
         show_progress = False
     else:
         _console = console
 
@@ -223,16 +219,16 @@
 
         if h == md5sum_hash:
             _console.print("[green]MD5 sum verified!")
         else:
             _console.print("[green]MD5sum Failed, Check with repository administrator.\nExiting...")
             sys.exit(1)
 
-    with _console.status("[red]Unzipping archive..."):
-        unzip(tmp_filename, target_location)
+    with _console.status("[red]Extracting archive..."):
+        extract(tmp_filename, target_location)
 
 
 def symlink_dir_contents(source: Path, dest: Path):
     """ create symlinks of all content in a directory into another """
     dest.mkdir(exist_ok=True, parents=True)
     for item in source.iterdir():
         (dest / item.name).symlink_to(item, target_is_directory=item.is_dir())
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/networkio.py` & `zerospeech-benchmarks-0.9.3/zerospeech/networkio.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         _ = repository.RepositoryIndex(**data)
     except ValidationError:
         error_console.log(f"The given repository @ {st.repository_index} is not valid")
         error_console.log("Please contact the administrator to resolve this issue...")
         sys.exit(1)
 
     with st.repository_index.open('w') as fp:
-        json.dump(data, fp)
+        json.dump(data, fp, indent=4)
     console.log("RepositoryIndex has been updated successfully !!")
 
 
 def check_update_repo_index() -> bool:
     """ Checks if local repo is out of date """
     # no need to check for updates more than once a week
     if st.repository_index.is_file():
@@ -52,10 +52,10 @@
         return False
 
     try:
         with st.repository_index.open() as fp:
             last_update_local = datetime.fromisoformat(json.load(fp).get('last_modified'))
     except ValueError:
         warnings.warn("Local index missing or corrupted !!!")
-        return False
+        return True
 
     return last_update_online > last_update_local
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/out.py` & `zerospeech-benchmarks-0.9.3/zerospeech/out.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/settings.py` & `zerospeech-benchmarks-0.9.3/zerospeech/settings.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/startup.py` & `zerospeech-benchmarks-0.9.3/zerospeech/startup.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/meta_file.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/meta_file.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/score_dir.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/score_dir.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/submission.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/submission.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/_model/validation_context.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/_model/validation_context.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/abx17.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/abx17.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 from typing import Tuple
 
 from zerospeech.misc import load_obj
 from zerospeech.generics import (
     FileTypes, FileListItem, Namespace, Item
 )
-from zerospeech.tasks.abx.abx_librispeech import ABXParameters
+from zerospeech.tasks.abx.abx17 import ABXParameters
 from ._model import MetaFile, Submission
 
 
 class ABX17Submission(Submission):
     """ Submission for ABX-17 """
     sets: Tuple = ('1s', '10s', '120s')
     tasks: Tuple = ('english', 'french', 'mandarin', 'german', 'wolof')
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/abxLS.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/abxLS.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 )
 from zerospeech.leaderboards import EntryDetails, LeaderboardBenchmarkName, LeaderboardEntry
 from zerospeech.leaderboards.abxLS import (
     ABXLSEntry, ABXLSScoreSubType
 )
 from zerospeech.misc import load_obj
 from zerospeech.settings import get_settings
-from zerospeech.tasks.abx import abx_phoneme
+from zerospeech.tasks.abx import abxLS_phoneme
 from ._model import ScoreDir, MetaFile, SubmissionValidation, validation_fn, add_item, Submission
 
 st = get_settings()
 
 
 class AbxLSSubmissionValidator(SubmissionValidation):
     """ File Validation for an ABXLS submission """
@@ -151,15 +151,15 @@
         )
         # add item tag
         add_item('test_other', results)
         return results
 
 
 class ABXLSScoreDir(ScoreDir):
-    params: Optional[abx_phoneme.ABX2Parameters] = abx_phoneme.ABX2Parameters()
+    params: Optional[abxLS_phoneme.ABX2Parameters] = abxLS_phoneme.ABX2Parameters()
 
     @property
     def scores_phonetic(self):
         csv_file = (self.location / self.params.result_filename).with_suffix('.csv')
         return load_dataframe(csv_file)
 
     def get_details(self) -> EntryDetails:
@@ -258,15 +258,15 @@
             sets=sets,
             tasks=tasks,
             location=path
         )
 
         # if params not set export defaults
         if not submission.params_file.is_file():
-            abx_phoneme.ABX2Parameters().export(submission.params_file)
+            abxLS_phoneme.ABX2Parameters().export(submission.params_file)
 
         # Load items
         file_ext = submission.params.score_file_type.replace('.', '')
         file_ext = FileTypes(file_ext)
         items = dict()
         if 'clean' in tasks:
             if 'dev' in sets:
@@ -287,19 +287,19 @@
                 items['test_other'] = FileListItem.from_dir(
                     path / 'test-other', f_type=file_ext
                 )
 
         submission.items = Namespace[Item](store=items)
         return submission
 
-    def load_parameters(self) -> abx_phoneme.ABX2Parameters:
+    def load_parameters(self) -> abxLS_phoneme.ABX2Parameters:
         if self.params_file.is_file():
             obj = load_obj(self.params_file)
-            return abx_phoneme.ABX2Parameters.parse_obj(obj)
-        return abx_phoneme.ABX2Parameters()
+            return abxLS_phoneme.ABX2Parameters.parse_obj(obj)
+        return abxLS_phoneme.ABX2Parameters()
 
     def __validate_submission__(self):
         """ Run validation on the submission data """
         self.validation_output = AbxLSSubmissionValidator().validate(self)
 
     @classmethod
     def init_dir(cls, location: Path):
@@ -309,15 +309,15 @@
         (location / 'dev-clean').mkdir(exist_ok=True, parents=True)
         (location / 'dev-other').mkdir(exist_ok=True, parents=True)
         (location / 'test-clean').mkdir(exist_ok=True, parents=True)
         (location / 'test-other').mkdir(exist_ok=True, parents=True)
         # scores dir
         (location / 'scores').mkdir(exist_ok=True, parents=True)
         # create parameters file
-        abx_phoneme.ABX2Parameters().export(location / abx_phoneme.ABX2Parameters.file_stem)
+        abxLS_phoneme.ABX2Parameters().export(location / abxLS_phoneme.ABX2Parameters.file_stem)
         # create meta-template
         template = MetaFile.to_template(benchmark_name="abxLS")
         template.to_yaml(
             file=location / MetaFile.file_stem,
             excluded={
                 "file_stem": True,
                 "model_info": {"model_id"},
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/prosAudit.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/prosAudit.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/sLM21.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/sLM21.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/submissions/tde17.py` & `zerospeech-benchmarks-0.9.3/zerospeech/submissions/tde17.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/_model.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/_model.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/params.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abx17/params.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,17 +37,17 @@
     # Path to a CPC checkpoint
     path_checkpoint: Optional[str] = None
     # size of a single feature
     feature_size: Optional[float] = float(0.1)
     # Use the GPU to compute distances
     cuda: bool = True
     # Choose the mode of the ABX score to compute
-    mode: ABXMode = 'all'
+    mode: ABXMode = ABXMode.all
     # Choose the kind of distance to use to compute
-    distance_mode: ABXDistanceMode = 'cosine'
+    distance_mode: ABXDistanceMode = ABXDistanceMode.cosine
     # Max size of a group while computing the ABX score
     max_size_group: int = 10
     # When computing the ABX across score, maximum
     # number of speaker X to sample per couple A,B.
     max_x_across: int = 5
     # location to output the results
     out: Optional[str] = None
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_librispeech/task.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abx17/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import pandas as pd
 
 try:
     import libriabx
 except ImportError:
     libriabx = ...
-    warnings.warn("abx module not installed")
+    warnings.warn("abx17 extension not installed")
 
 from .params import ABXParameters, ABXMode, ABXDistanceMode
 from zerospeech.generics import FileListItem, FileItem
 from zerospeech.settings import get_settings
 from zerospeech.out import warning_console
 from zerospeech.tasks import Task
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/params.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abxLS_phoneme/params.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/abx/abx_phoneme/task.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/abx/abxLS_phoneme/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 try:
     import zrc_abx2
     from vdataset import mount, unmount
 except ImportError:
     zrc_abx2 = ...
     mount, unmount = ..., ...
-    warnings.warn("abx2 module not installed")
+    warnings.warn("abxLS extension not installed")
 
 from .params import ABX2Parameters, ABXSpeakerMode, ABXDistanceMode, ContextMode
 from zerospeech.generics import  FileItem, FileListItem
 from zerospeech.settings import get_settings
 from zerospeech.out import warning_console
 from zerospeech.tasks import Task
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/lexical.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/lexical.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/params.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/params.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/prosody.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/prosody.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/semantic.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/semantic.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/lm/syntactic.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/lm/syntactic.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/tasks/tde.py` & `zerospeech-benchmarks-0.9.3/zerospeech/tasks/tde.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/upload/file_split.py` & `zerospeech-benchmarks-0.9.3/zerospeech/upload/file_split.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/upload/submission.py` & `zerospeech-benchmarks-0.9.3/zerospeech/upload/submission.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/upload/user_api.py` & `zerospeech-benchmarks-0.9.3/zerospeech/upload/user_api.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/validators/base_validators.py` & `zerospeech-benchmarks-0.9.3/zerospeech/validators/base_validators.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech/validators/validators.py` & `zerospeech-benchmarks-0.9.3/zerospeech/validators/validators.py`

 * *Files identical despite different names*

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/PKG-INFO` & `zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zerospeech-benchmarks
-Version: 0.9.2
+Version: 0.9.3
 Summary: Toolset for usage of the Zero Resource Challenge Benchmarks.
 Author-email: Nicolas Hamilakis <nicolas.hamilakis@ens.psl.eu>, CoML Team <dev@zerospeech.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,16 +690,16 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: vocolab
 Provides-Extra: tts019
-Provides-Extra: abx
-Provides-Extra: abx2
+Provides-Extra: abx17
+Provides-Extra: abxLS
 Provides-Extra: tde
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # Zero Resource Challenge Benchmark Toolkit  ![BETA](https://img.shields.io/badge/-BETA-blue)
```

### Comparing `zerospeech-benchmarks-0.9.2/zerospeech_benchmarks.egg-info/SOURCES.txt` & `zerospeech-benchmarks-0.9.3/zerospeech_benchmarks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,20 +86,20 @@
 zerospeech/submissions/_model/score_dir.py
 zerospeech/submissions/_model/submission.py
 zerospeech/submissions/_model/validation_context.py
 zerospeech/tasks/__init__.py
 zerospeech/tasks/_model.py
 zerospeech/tasks/tde.py
 zerospeech/tasks/abx/__init__.py
-zerospeech/tasks/abx/abx_librispeech/__init__.py
-zerospeech/tasks/abx/abx_librispeech/params.py
-zerospeech/tasks/abx/abx_librispeech/task.py
-zerospeech/tasks/abx/abx_phoneme/__init__.py
-zerospeech/tasks/abx/abx_phoneme/params.py
-zerospeech/tasks/abx/abx_phoneme/task.py
+zerospeech/tasks/abx/abx17/__init__.py
+zerospeech/tasks/abx/abx17/params.py
+zerospeech/tasks/abx/abx17/task.py
+zerospeech/tasks/abx/abxLS_phoneme/__init__.py
+zerospeech/tasks/abx/abxLS_phoneme/params.py
+zerospeech/tasks/abx/abxLS_phoneme/task.py
 zerospeech/tasks/lm/__init__.py
 zerospeech/tasks/lm/lexical.py
 zerospeech/tasks/lm/params.py
 zerospeech/tasks/lm/prosody.py
 zerospeech/tasks/lm/semantic.py
 zerospeech/tasks/lm/syntactic.py
 zerospeech/upload/__init__.py
```

