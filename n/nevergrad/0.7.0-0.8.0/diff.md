# Comparing `tmp/nevergrad-0.7.0.tar.gz` & `tmp/nevergrad-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nevergrad-0.7.0.tar", last modified: Fri Jun 16 09:57:59 2023, max compression
+gzip compressed data, was "dist/nevergrad-0.8.0.tar", last modified: Thu Jul  6 19:13:36 2023, max compression
```

## Comparing `nevergrad-0.7.0.tar` & `nevergrad-0.8.0.tar`

### file list

```diff
@@ -1,232 +1,236 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1086 2023-06-16 09:52:50.000000 nevergrad-0.7.0/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-16 09:52:50.000000 nevergrad-0.7.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4076 2023-06-16 09:57:59.000000 nevergrad-0.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-06-16 09:52:50.000000 nevergrad-0.7.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/benchmark/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      271 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4910 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11376 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4979 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/execution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    95004 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/experiments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/exporttable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11579 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/frozenexperiments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13529 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/gymexperiments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8693 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/optgroups.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41063 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/plotting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3826 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_execution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6658 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_experiments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8519 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_plotting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2231 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5902 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/test_xpbase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4175 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13468 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/benchmark/xpbase.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2450 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/decorators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/test_decorators.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3458 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/test_testing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2468 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/test_tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5710 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/testing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/tools.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2135 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/common/typing.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/ac/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/ac/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/ac/ac.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      506 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/ac/test_ac.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3700 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1957 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/arcoating/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18068 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/base.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4136 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/causaldiscovery/test_core.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/control/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/mujoco.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/control/test_mujoco.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13026 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/corefuncs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/cycling/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/cycling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5024 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/cyclist.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4296 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/mensteampursuit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1436 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/simulationresult.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4942 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/teampursuit.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      564 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/test_cycling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3691 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/cycling/womensteampursuit.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/fishing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/fishing/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/fishing/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/fishing/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15194 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/functionlib.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/games/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/games/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17992 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/games/game.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/games/test_game.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/gym/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30916 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/multigym.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/test_multigym.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-06-16 09:52:50.000000 nevergrad-0.7.0/nevergrad/functions/gym/tuple_gym_env.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5735 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14277 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5594 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/imagelosses.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1311 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2138 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/images/test_imagelosses.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      276 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6141 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2396 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/iohprofiler/test_core.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      468 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mixsimulator/test_core.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/ml/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/ml/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15750 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/ml/mlfunctionlib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3145 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/ml/test_mlfunctionlib.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/mlda/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      372 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3757 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/datasets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10034 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/problems.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3322 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/test_datasets.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4334 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/mlda/test_problems.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/multiobjective/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/multiobjective/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4355 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1670 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/olympussurfaces/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5637 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pbt.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/photonics/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8008 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15293 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/photonics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6864 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/photonics/test_core.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13522 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/powersystems/test_core.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8360 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3463 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2859 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/pyomo/test_pyomo_doc.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/rl/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7070 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/agents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9742 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5317 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/envs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3016 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/test_agents.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3538 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rl/test_envs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/rocket/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rocket/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12181 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rocket/rocket.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/rocket/test_rocket.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/stsp/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/stsp/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/stsp/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/stsp/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8614 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3746 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_corefuncs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_functionlib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/test_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3453 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/unitcommitment/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/functions/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/ops/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/ops/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3824 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/ops/constraints.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/ops/test_constraints.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/optimization/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41000 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14126 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/callbacks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17988 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/differentialevolution.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6295 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/es.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20000 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/experimentalvariants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9958 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/externalbo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1537 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/families.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3664 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/metamodel.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12534 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13167 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/hypervolume.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9935 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/nsga2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5561 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9883 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_hypervolume.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5819 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_nsga2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6561 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/mutations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20194 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/oneshot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   138230 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/optimizerlib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18010 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/recaster.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20594 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/recastlib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/requirements_check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8616 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/sequences.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8138 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6692 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_callbacks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7557 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_doc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5143 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_externalbo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_mutations.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38904 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_optimizerlib.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6927 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_recaster.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_sa.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3756 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_sequences.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_special.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4609 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_suggest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2405 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_tabu.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5267 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14309 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/optimization/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad/parametrization/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14333 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/_datalayers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10997 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/_layering.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10415 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/choice.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9435 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/container.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21684 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21250 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5375 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/discretization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9664 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12840 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/instantiate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/mutation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1101 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/parameter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2166 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_discretization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_instantiate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5599 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_layers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4599 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_mutation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_param_doc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16652 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_parameter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6548 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_parameters_legacy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3994 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_transforms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11025 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10944 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/transforms.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9987 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/parametrization/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:52:51.000000 nevergrad-0.7.0/nevergrad/py.typed
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4076 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1876 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-06-16 09:57:59.000000 nevergrad-0.7.0/nevergrad.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-06-16 09:52:51.000000 nevergrad-0.7.0/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-16 09:57:59.000000 nevergrad-0.7.0/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      827 2023-06-16 09:52:51.000000 nevergrad-0.7.0/requirements/bench.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-06-16 09:52:51.000000 nevergrad-0.7.0/requirements/dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-06-16 09:52:51.000000 nevergrad-0.7.0/requirements/main.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-16 09:57:59.000000 nevergrad-0.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3131 2023-06-16 09:52:51.000000 nevergrad-0.7.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1086 2023-07-06 19:08:22.000000 nevergrad-0.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-06 19:08:22.000000 nevergrad-0.8.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4076 2023-07-06 19:13:36.000000 nevergrad-0.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3325 2023-07-06 19:08:22.000000 nevergrad-0.8.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      623 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/benchmark/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      271 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4910 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11376 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4979 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/execution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   107214 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/experiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2941 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/exporttable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11579 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/frozenexperiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13529 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/gymexperiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8638 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/optgroups.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41886 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/plotting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6365 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3826 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/test_execution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6658 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/test_experiments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8519 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/test_plotting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2231 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5902 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/test_xpbase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4196 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13468 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/benchmark/xpbase.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2450 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/decorators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2584 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1653 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/test_decorators.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3458 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/test_testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2468 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5710 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2135 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/common/typing.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      615 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/ac/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/ac/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/ac/ac.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      506 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/ac/test_ac.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/arcoating/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/arcoating/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3700 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/arcoating/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1957 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/arcoating/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18393 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/base.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/causaldiscovery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/causaldiscovery/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4136 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/causaldiscovery/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/causaldiscovery/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/control/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/control/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/control/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/control/mujoco.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2270 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/control/test_mujoco.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13026 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/corefuncs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/cycling/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      247 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/cycling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5024 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/cyclist.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4296 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/mensteampursuit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1436 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/simulationresult.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4942 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/teampursuit.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      564 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/test_cycling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3691 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/cycling/womensteampursuit.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/fishing/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/fishing/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2059 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/fishing/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/fishing/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15194 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/functionlib.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/games/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/games/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17992 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/games/game.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      936 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/games/test_game.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/gym/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/gym/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30916 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/gym/multigym.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/gym/test_multigym.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1569 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/gym/tuple_gym_env.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5735 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      268 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/images/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14277 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/images/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5610 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/images/imagelosses.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1311 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/images/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2138 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/images/test_imagelosses.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/iohprofiler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      276 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/iohprofiler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6141 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/iohprofiler/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2396 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/iohprofiler/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/mixsimulator/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mixsimulator/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mixsimulator/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      468 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mixsimulator/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/ml/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/ml/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15750 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/ml/mlfunctionlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3145 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/ml/test_mlfunctionlib.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/mlda/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      372 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mlda/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3757 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mlda/datasets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10034 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mlda/problems.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3322 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mlda/test_datasets.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4334 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/mlda/test_problems.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/multiobjective/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1147 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/multiobjective/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/olympussurfaces/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      284 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/olympussurfaces/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4355 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/olympussurfaces/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1670 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/olympussurfaces/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5637 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/pbt.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/photonics/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      221 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/photonics/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8013 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/photonics/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15293 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/photonics/photonics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6864 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/photonics/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/powersystems/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      225 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/powersystems/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13522 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/powersystems/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/powersystems/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/pyomo/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      213 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/pyomo/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8360 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/pyomo/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3463 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/pyomo/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2859 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/pyomo/test_pyomo_doc.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/rl/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rl/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7070 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rl/agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9742 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rl/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5317 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rl/envs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3016 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rl/test_agents.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3538 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rl/test_envs.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/rocket/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rocket/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12181 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rocket/rocket.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/rocket/test_rocket.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/stsp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      211 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/stsp/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1757 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/stsp/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      562 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/stsp/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8614 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3746 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/test_corefuncs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9269 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/test_functionlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/topology_optimization/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      207 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/topology_optimization/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1891 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/topology_optimization/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/topology_optimization/test_core.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/functions/unitcommitment/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/unitcommitment/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3453 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/unitcommitment/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/unitcommitment/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1371 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/functions/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/ops/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/ops/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3824 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/ops/constraints.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1025 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/ops/test_constraints.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/optimization/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      319 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41000 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14126 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/callbacks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20420 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/differentialevolution.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6295 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/es.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20000 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/experimentalvariants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9958 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/externalbo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1537 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/families.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3664 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/metamodel.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12534 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13167 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/hypervolume.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9935 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/nsga2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5561 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/test_core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9883 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/test_hypervolume.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5819 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/multiobjective/test_nsga2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6561 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/mutations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20194 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/oneshot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   143628 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/optimizerlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18010 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/recaster.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21626 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/recastlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/requirements_check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8616 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/sequences.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8138 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6692 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_callbacks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7557 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_doc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5143 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_externalbo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3191 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_mutations.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41818 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_optimizerlib.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6927 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_recaster.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1389 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_sa.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3756 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_sequences.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_special.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4655 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_suggest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2405 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_tabu.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5267 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14309 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/optimization/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad/parametrization/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14333 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/_datalayers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10997 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/_layering.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10415 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/choice.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9435 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/container.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21684 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21250 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5375 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/discretization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9664 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12840 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/instantiate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/mutation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1101 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/parameter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2166 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_discretization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6133 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_instantiate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5599 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_layers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4599 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_mutation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3098 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_param_doc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16652 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_parameter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6548 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_parameters_legacy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3994 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_transforms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11025 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10944 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/transforms.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9987 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/parametrization/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:08:22.000000 nevergrad-0.8.0/nevergrad/py.typed
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4076 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7515 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1872 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-07-06 19:13:36.000000 nevergrad-0.8.0/nevergrad.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-07-06 19:08:22.000000 nevergrad-0.8.0/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-06 19:13:36.000000 nevergrad-0.8.0/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      825 2023-07-06 19:08:22.000000 nevergrad-0.8.0/requirements/bench.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2023-07-06 19:08:22.000000 nevergrad-0.8.0/requirements/dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-07-06 19:08:22.000000 nevergrad-0.8.0/requirements/main.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-06 19:13:36.000000 nevergrad-0.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3131 2023-07-06 19:08:22.000000 nevergrad-0.8.0/setup.py
```

### Comparing `nevergrad-0.7.0/LICENSE` & `nevergrad-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/PKG-INFO` & `nevergrad-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nevergrad
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python toolbox for performing gradient-free optimization
 Home-page: https://github.com/facebookresearch/nevergrad
 Author: Facebook AI Research
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -16,15 +16,15 @@
 Provides-Extra: benchmark
 License-File: LICENSE
 
 [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine) [![CircleCI](https://circleci.com/gh/facebookresearch/nevergrad/tree/main.svg?style=svg)](https://circleci.com/gh/facebookresearch/nevergrad/tree/main)
 
 # Nevergrad - A gradient-free optimization platform
 
-![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/Nevergrad-LogoMark.png)
+![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.8.0/docs/resources/Nevergrad-LogoMark.png)
 
 
 `nevergrad` is a Python 3.6+ library. It can be installed with:
 
 ```
 pip install nevergrad
 ```
@@ -74,15 +74,15 @@
 # show the recommended keyword arguments of the function
 print(recommendation.kwargs)
 >>> {'learning_rate': 0.1998, 'batch_size': 4, 'architecture': 'conv'}
 ```
 
 Learn more on parametrization in the [**documentation**](https://facebookresearch.github.io/nevergrad/)!
 
-![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/TwoPointsDE.gif)
+![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.8.0/docs/resources/TwoPointsDE.gif)
 
 *Convergence of a population of points to the minima with two-points DE.*
 
 
 ## Documentation
 
 Check out our [**documentation**](https://facebookresearch.github.io/nevergrad/)! It's still a work in progress, don't hesitate to submit issues and/or PR to update it and make it clearer!
@@ -99,9 +99,9 @@
     journal = {GitHub repository},
     howpublished = {\url{https://GitHub.com/FacebookResearch/Nevergrad}},
 }
 ```
 
 ## License
 
-`nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.7.0/LICENSE) for additional details about it.
+`nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.8.0/LICENSE) for additional details about it.
 See also our [Terms of Use](https://opensource.facebook.com/legal/terms) and [Privacy Policy](https://opensource.facebook.com/legal/privacy).
```

### Comparing `nevergrad-0.7.0/README.md` & `nevergrad-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/__init__.py` & `nevergrad-0.8.0/nevergrad/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from .common import errors as errors
 from . import ops as ops
 
 
 __all__ = ["optimizers", "families", "callbacks", "p", "typing", "errors", "ops"]
 
 
-__version__ = "0.7.0"
+__version__ = "0.8.0"
```

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/__main__.py` & `nevergrad-0.8.0/nevergrad/benchmark/__main__.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/core.py` & `nevergrad-0.8.0/nevergrad/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/execution.py` & `nevergrad-0.8.0/nevergrad/benchmark/execution.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/experiments.py` & `nevergrad-0.8.0/nevergrad/benchmark/experiments.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from nevergrad.functions import mlda as _mlda
 from nevergrad.functions.photonics import Photonics
 from nevergrad.functions.arcoating import ARCoating
 from nevergrad.functions import images as imagesxp
 from nevergrad.functions.powersystems import PowerSystem
 from nevergrad.functions.ac import NgAquacrop
 from nevergrad.functions.stsp import STSP
+from nevergrad.functions.topology_optimization import TO
 from nevergrad.functions.rocket import Rocket
 from nevergrad.functions.mixsimulator import OptimizeMix
 from nevergrad.functions.unitcommitment import UnitCommitmentProblem
 from nevergrad.functions import control
 from nevergrad.functions import rl
 from nevergrad.functions.games import game
 from nevergrad.functions import iohprofiler
@@ -74,97 +75,170 @@
             # Most points violate the constraint.
             value = float(np.sum(np.square(data)) - len(data) - np.sqrt(len(data)))
         else:
             raise NotImplementedError(f"Unknown function {self.name}")
         return value > 0 if self.as_bool else value
 
 
+@registry.register
 def keras_tuning(
-    seed: tp.Optional[int] = None, overfitter: bool = False, seq: bool = False
+    seed: tp.Optional[int] = None,
+    overfitter: bool = False,
+    seq: bool = False,
+    veryseq: bool = False,
 ) -> tp.Iterator[Experiment]:
     """Machine learning hyperparameter tuning experiment. Based on Keras models."""
     seedg = create_seed_generator(seed)
     # Continuous case,
 
     # First, a few functions with constraints.
-    optims: tp.List[str] = ["PSO", "OnePlusOne"] + get_optimizers("basics", seed=next(seedg))  # type: ignore
+    # optims: tp.List[str] = ["PSO", "OnePlusOne"] + get_optimizers("basics", seed=next(seedg))  # type: ignore
+    optims = ["OnePlusOne", "BO", "RandomSearch", "CMA", "DE", "TwoPointsDE", "HyperOpt", "PCABO", "Cobyla"]
+    optims = [
+        "OnePlusOne",
+        "RandomSearch",
+        "CMA",
+        "DE",
+        "TwoPointsDE",
+        "HyperOpt",
+        "Cobyla",
+        "MetaModel",
+        "MetaModelOnePlusOne",
+        "RFMetaModel",
+        "RFMetaModelOnePlusOne",
+    ]
+    optims = ["OnePlusOne", "RandomSearch", "Cobyla"]
+    optims = ["DE", "TwoPointsDE", "HyperOpt", "MetaModelOnePlusOne"]
+    optims = get_optimizers("oneshot", seed=next(seedg))  # type: ignore
+    optims = [
+        "MetaTuneRecentering",
+        "MetaRecentering",
+        "HullCenterHullAvgCauchyScrHammersleySearch",
+        "LHSSearch",
+        "LHSCauchySearch",
+    ]
+    optims = ["NGOpt", "NGOptRW", "QODE"]
+    optims = ["NGOpt"]
     datasets = ["kerasBoston", "diabetes", "auto-mpg", "red-wine", "white-wine"]
     for dimension in [None]:
         for dataset in datasets:
             function = MLTuning(
                 regressor="keras_dense_nn", data_dimension=dimension, dataset=dataset, overfitter=overfitter
             )
             for budget in [150, 500]:
                 for num_workers in (
                     [1, budget // 4] if seq else [budget]
                 ):  # Seq for sequential optimization experiments.
+                    if veryseq and num_workers > 1:
+                        continue
                     for optim in optims:
                         xp = Experiment(
                             function, optim, num_workers=num_workers, budget=budget, seed=next(seedg)
                         )
                         skip_ci(reason="too slow")
                         if not xp.is_incoherent:
                             yield xp
 
 
+@registry.register
 def mltuning(
     seed: tp.Optional[int] = None,
     overfitter: bool = False,
     seq: bool = False,
+    veryseq: bool = False,
     nano: bool = False,
 ) -> tp.Iterator[Experiment]:
     """Machine learning hyperparameter tuning experiment. Based on scikit models."""
     seedg = create_seed_generator(seed)
-    optims: tp.List[str] = get_optimizers("basics", seed=next(seedg))  # type: ignore
-    if not seq:
-        optims = get_optimizers("oneshot", seed=next(seedg))  # type: ignore
+    # optims: tp.List[str] = get_optimizers("basics", seed=next(seedg))  # type: ignore
+    # if not seq:
+    #    optims = get_optimizers("oneshot", seed=next(seedg))  # type: ignore
+    optims = ["OnePlusOne", "BO", "RandomSearch", "CMA", "DE", "TwoPointsDE", "PCABO", "HyperOpt", "Cobyla"]
+    optims = [
+        "OnePlusOne",
+        "RandomSearch",
+        "CMA",
+        "DE",
+        "TwoPointsDE",
+        "HyperOpt",
+        "Cobyla",
+        "MetaModel",
+        "MetaModelOnePlusOne",
+        "RFMetaModel",
+        "RFMetaModelOnePlusOne",
+    ]
+    optims = ["OnePlusOne", "RandomSearch", "Cobyla"]
+    optims = ["DE", "TwoPointsDE", "HyperOpt", "MetaModelOnePlusOne"]
+    optims = get_optimizers("oneshot", seed=next(seedg))  # type: ignore
+    optims = [
+        "MetaTuneRecentering",
+        "MetaRecentering",
+        "HullCenterHullAvgCauchyScrHammersleySearch",
+        "LHSSearch",
+        "LHSCauchySearch",
+    ]
+    optims = ["NGOpt", "NGOptRW", "QODE"]
+    optims = ["NGOpt"]
     for dimension in [None, 1, 2, 3]:
         if dimension is None:
             datasets = ["boston", "diabetes", "auto-mpg", "red-wine", "white-wine"]
         else:
             datasets = ["artificialcos", "artificial", "artificialsquare"]
         for regressor in ["mlp", "decision_tree", "decision_tree_depth"]:
             for dataset in datasets:
                 function = MLTuning(
                     regressor=regressor, data_dimension=dimension, dataset=dataset, overfitter=overfitter
                 )
                 for budget in [150, 500] if not nano else [80, 160]:
                     # Seq for sequential optimization experiments.
                     parallelization = [1, budget // 4] if seq else [budget]
                     for num_workers in parallelization:
+                        if veryseq and num_workers > 1:
+                            continue
 
                         for optim in optims:
                             xp = Experiment(
                                 function, optim, num_workers=num_workers, budget=budget, seed=next(seedg)
                             )
                             skip_ci(reason="too slow")
                             if not xp.is_incoherent:
                                 yield xp
 
 
+@registry.register
 def naivemltuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Counterpart of mltuning with overfitting of valid loss, i.e. train/valid/valid instead of train/valid/test."""
     return mltuning(seed, overfitter=True)
 
 
-# We register only the sequential counterparts for the moment.
+@registry.register
+def veryseq_keras_tuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Iterative counterpart of keras tuning."""
+    return keras_tuning(seed, overfitter=False, seq=True, veryseq=True)
+
+
 @registry.register
 def seq_keras_tuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Iterative counterpart of keras tuning."""
     return keras_tuning(seed, overfitter=False, seq=True)
 
 
-# We register only the sequential counterparts for the moment.
 @registry.register
 def naive_seq_keras_tuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Naive counterpart (no overfitting, see naivemltuning)of seq_keras_tuning."""
     return keras_tuning(seed, overfitter=True, seq=True)
 
 
 @registry.register
+def naive_veryseq_keras_tuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Naive counterpart (no overfitting, see naivemltuning)of seq_keras_tuning."""
+    return keras_tuning(seed, overfitter=True, seq=True, veryseq=True)
+
+
+@registry.register
 def oneshot_mltuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """One-shot counterpart of Scikit tuning."""
     return mltuning(seed, overfitter=False, seq=False)
 
 
 # We register only the (almost) sequential counterparts for the moment.
 @registry.register
@@ -176,14 +250,27 @@
 @registry.register
 def nano_seq_mltuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Iterative counterpart of seq_mltuning with smaller budget."""
     return mltuning(seed, overfitter=False, seq=True, nano=True)
 
 
 @registry.register
+def nano_veryseq_mltuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Iterative counterpart of seq_mltuning with smaller budget."""
+    return mltuning(seed, overfitter=False, seq=True, nano=True, veryseq=True)
+
+
+@registry.register
+def nano_naive_veryseq_mltuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Iterative counterpart of mltuning with overfitting of valid loss, i.e. train/valid/valid instead of train/valid/test,
+    and with lower budget."""
+    return mltuning(seed, overfitter=True, seq=True, nano=True, veryseq=True)
+
+
+@registry.register
 def nano_naive_seq_mltuning(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Iterative counterpart of mltuning with overfitting of valid loss, i.e. train/valid/valid instead of train/valid/test,
     and with lower budget."""
     return mltuning(seed, overfitter=True, seq=True, nano=True)
 
 
 @registry.register
@@ -238,18 +325,17 @@
         for split in [True, False]  # period 2
     ][
         ::37
     ]  # 37 is coprime with all periods above so we sample correctly the possibilities.
     assert len(functions) == 21, f"{len(functions)} problems instead of 21. Yawidebbob should be standard."
     # This problem is intended as a stable basis forever.
     # The list of optimizers should contain only the basic for comparison and "baselines".
-    optims: tp.List[str] = ["NGOpt10"] + get_optimizers("baselines", seed=next(seedg))  # type: ignore
-    optims = ["NGOptRW", "NGOpt", "CMandAS2", "Shiwa", "CMA", "DE", "DiscreteLenglerOnePlusOne"]
-    np.random.shuffle(optims)
-    optims = optims[:2]
+    # optims: tp.List[str] = ["NGOpt10"] + get_optimizers("baselines", seed=next(seedg))  # type: ignore
+    optims = ["NGOptRW", "NGOpt", "RandomSearch", "CMA", "DE", "DiscreteLenglerOnePlusOne"]
+    # optims = optims[:2]
     index = 0
     for function in functions:
         for budget in [50, 1500, 25000]:
             for nw in [1, budget] + ([] if budget <= 300 else [300]):
                 index += 1
                 if index % 5 == 0:
                     total_xp_per_optim += 1
@@ -325,15 +411,16 @@
 
 
 # pylint: disable=redefined-outer-name
 @registry.register
 def parallel_small_budget(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Parallel optimization with small budgets"""
     seedg = create_seed_generator(seed)
-    optims: tp.List[str] = get_optimizers("basics", seed=next(seedg))  # type: ignore
+    # optims: tp.List[str] = get_optimizers("basics", seed=next(seedg))  # type: ignore
+    optims = ["DE", "TwoPointsDE", "CMA", "NGOpt", "PSO", "OnePlusOne", "RandomSearch"]
     names = ["hm", "rastrigin", "griewank", "rosenbrock", "ackley", "multipeak"]
     names += ["sphere", "cigar", "ellipsoid", "altellipsoid"]
     names += ["deceptiveillcond", "deceptivemultimodal", "deceptivepath"]
     # funcs
     functions = [
         ArtificialFunction(name, block_dimension=d, rotation=rotation)
         for name in names
@@ -362,15 +449,22 @@
 @registry.register
 def instrum_discrete(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Comparison of optimization algorithms equipped with distinct instrumentations.
     Onemax, Leadingones, Jump function."""
     # Discrete, unordered.
 
     seedg = create_seed_generator(seed)
-    optims = get_optimizers("small_discrete", seed=next(seedg))
+    # optims = get_optimizers("small_discrete", seed=next(seedg))
+    optims = ["DiscreteOnePlusOne", "NGOpt", "CMA", "TwoPointsDE", "DiscreteLenglerOnePlusOne"]
+    optims = ["RFMetaModelOnePlusOne"]
+    optims = ["FastGADiscreteOnePlusOne"]
+    optims = ["DoubleFastGADiscreteOnePlusOne"]
+    optims = ["DiscreteOnePlusOne"]
+    optims = ["OnePlusOne"]
+    optims = ["DiscreteLenglerOnePlusOne"]
     for nv in [10, 50, 200, 1000, 5000]:
         for arity in [2, 3, 7, 30]:
             for instrum_str in ["Unordered", "Softmax", "Ordered"]:
                 if instrum_str == "Softmax":
                     instrum: ng.p.Parameter = ng.p.Choice(range(arity), repetitions=nv)
                 else:
                     assert instrum_str in ("Ordered", "Unordered")
@@ -378,68 +472,106 @@
                         range(arity), repetitions=nv, ordered=instrum_str == "Ordered"
                     )
                 for name in ["onemax", "leadingones", "jump"]:
                     dfunc = ExperimentFunction(
                         corefuncs.DiscreteFunction(name, arity), instrum.set_name(instrum_str)
                     )
                     dfunc.add_descriptors(arity=arity)
+                    dfunc.add_descriptors(nv=nv)
+                    dfunc.add_descriptors(instrum_str=instrum_str)
                     for optim in optims:
                         for nw in [1, 10]:
                             for budget in [50, 500, 5000]:
                                 yield Experiment(
                                     dfunc, optim, num_workers=nw, budget=budget, seed=next(seedg)
                                 )
 
 
 @registry.register
 def sequential_instrum_discrete(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Sequential counterpart of instrum_discrete."""
 
     seedg = create_seed_generator(seed)
     # Discrete, unordered.
-    optims = get_optimizers("discrete", seed=next(seedg))
+    # optims = get_optimizers("discrete", seed=next(seedg))
+    optims = ["DiscreteOnePlusOne", "NGOpt", "CMA", "TwoPointsDE", "DiscreteLenglerOnePlusOne"]
+    optims = ["OnePlusOne"]
+    optims = ["DiscreteLenglerOnePlusOne"]
     for nv in [10, 50, 200, 1000, 5000]:
         for arity in [2, 3, 7, 30]:
             for instrum_str in ["Unordered", "Softmax", "Ordered"]:
                 if instrum_str == "Softmax":
                     instrum: ng.p.Parameter = ng.p.Choice(range(arity), repetitions=nv)
                 else:
                     instrum = ng.p.TransitionChoice(
                         range(arity), repetitions=nv, ordered=instrum_str == "Ordered"
                     )
                 for name in ["onemax", "leadingones", "jump"]:
                     dfunc = ExperimentFunction(
                         corefuncs.DiscreteFunction(name, arity), instrum.set_name(instrum_str)
                     )
                     dfunc.add_descriptors(arity=arity)
+                    dfunc.add_descriptors(nv=nv)
+                    dfunc.add_descriptors(instrum_str=instrum_str)
                     for optim in optims:
                         for budget in [50, 500, 5000, 50000]:
                             yield Experiment(dfunc, optim, budget=budget, seed=next(seedg))
 
 
 @registry.register
 def deceptive(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Very difficult objective functions: one is highly multimodal (infinitely many local optima),
     one has an infinite condition number, one has an infinitely long path towards the optimum.
     Looks somehow fractal."""
     seedg = create_seed_generator(seed)
     names = ["deceptivemultimodal", "deceptiveillcond", "deceptivepath"]
     optims = get_optimizers("basics", seed=next(seedg))
+    optims = ["CMA", "DE", "TwoPointsDE", "PSO", "OnePlusOne", "RandomSearch", "NGOptRW"]
+    optims = [
+        "BFGS",
+        "LBFGSB",
+        "DE",
+        "TwoPointsDE",
+        "RandomSearch",
+        "OnePlusOne",
+        "PSO",
+        "CMA",
+        "ChainMetaModelSQP",
+        "MemeticDE",
+        "MetaModel",
+        "RFMetaModel",
+        "MetaModelDE",
+        "RFMetaModelDE",
+    ]
     functions = [
         ArtificialFunction(
             name, block_dimension=2, num_blocks=n_blocks, rotation=rotation, aggregator=aggregator
         )
         for name in names
         for rotation in [False, True]
         for n_blocks in [1, 2, 8, 16]
         for aggregator in ["sum", "max"]
     ]
     for func in functions:
         for optim in optims:
-            for budget in [25, 37, 50, 75, 87] + list(range(100, 20001, 500)):
+            for budget in [
+                25,
+                37,
+                50,
+                75,
+                87,
+                100,
+                200,
+                400,
+                800,
+                1600,
+                3200,
+                6400,
+                12800,
+            ]:  # + list(range(100, 20001, 500)):
                 yield Experiment(func, optim, budget=budget, num_workers=1, seed=next(seedg))
 
 
 @registry.register
 def parallel(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Parallel optimization on 3 classical objective functions: sphere, rastrigin, cigar.
     The number of workers is 20 % of the budget.
@@ -573,37 +705,71 @@
     """
     seedg = create_seed_generator(seed)
     names = ["hm", "rastrigin", "griewank", "rosenbrock", "ackley", "lunacek", "deceptivemultimodal"]
     # Keep in mind that Rosenbrock is multimodal in high dimension http://ieeexplore.ieee.org/document/6792472/.
     optims = get_optimizers("basics", seed=next(seedg))
     if not para:
         optims += get_optimizers("scipy", seed=next(seedg))
+    optims = [
+        "BFGS",
+        "LBFGSB",
+        "DE",
+        "TwoPointsDE",
+        "RandomSearch",
+        "OnePlusOne",
+        "PSO",
+        "CMA",
+        "ChainMetaModelSQP",
+        "MemeticDE",
+        "MetaModel",
+        "RFMetaModel",
+        "MetaModelDE",
+        "RFMetaModelDE",
+    ]
     # + list(sorted(x for x, y in ng.optimizers.registry.items() if "Chain" in x or "BO" in x))
     functions = [
         ArtificialFunction(name, block_dimension=bd, useless_variables=bd * uv_factor)
         for name in names
         for bd in [3, 25]
         for uv_factor in [0, 5]
     ]
     for func in functions:
         for optim in optims:
             for budget in [3000, 10000, 30000, 100000]:
                 for nw in [1000] if para else [1]:
-                    yield Experiment(func, optim, budget=budget, num_workers=nw, seed=next(seedg))
+                    xp = Experiment(func, optim, budget=budget, num_workers=nw, seed=next(seedg))
+                    if not xp.is_incoherent:
+                        yield xp
 
 
 @registry.register
 def hdmultimodal(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Experiment on multimodal functions, namely hm, rastrigin, griewank, rosenbrock, ackley, lunacek,
     deceptivemultimodal. Similar to multimodal, but dimension 20 or 100 or 1000. Budget 1000 or 10000, sequential."""
     seedg = create_seed_generator(seed)
     names = ["hm", "rastrigin", "griewank", "rosenbrock", "ackley", "lunacek", "deceptivemultimodal"]
     # Keep in mind that Rosenbrock is multimodal in high dimension http://ieeexplore.ieee.org/document/6792472/.
 
     optims = get_optimizers("basics", "multimodal", seed=next(seedg))
+    optims = [
+        "BFGS",
+        "LBFGSB",
+        "DE",
+        "TwoPointsDE",
+        "RandomSearch",
+        "OnePlusOne",
+        "PSO",
+        "CMA",
+        "ChainMetaModelSQP",
+        "MemeticDE",
+        "MetaModel",
+        "RFMetaModel",
+        "MetaModelDE",
+        "RFMetaModelDE",
+    ]
     functions = [
         ArtificialFunction(name, block_dimension=bd)
         for name in names
         for bd in [
             1000,
             6000,
             36000,
@@ -626,36 +792,47 @@
 def bonnans(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     seedg = create_seed_generator(seed)
     instrum = ng.p.TransitionChoice(range(2), repetitions=100, ordered=False)
     softmax_instrum: ng.p.Parameter = ng.p.Choice(range(2), repetitions=100)
     optims = [
         "RotatedTwoPointsDE",
         "DiscreteLenglerOnePlusOne",
+        "DiscreteLengler2OnePlusOne",
+        "DiscreteLengler3OnePlusOne",
+        "DiscreteLenglerHalfOnePlusOne",
+        "DiscreteLenglerFourthOnePlusOne",
         "PortfolioDiscreteOnePlusOne",
         "FastGADiscreteOnePlusOne",
         "DiscreteDoerrOnePlusOne",
         "DiscreteBSOOnePlusOne",
+        "DiscreteOnePlusOne",
         "AdaptiveDiscreteOnePlusOne",
         "GeneticDE",
         "DE",
         "TwoPointsDE",
         "DiscreteOnePlusOne",
         "CMA",
         "SQP",
         "MetaModel",
         "DiagonalCMA",
     ]
+    optims = ["RFMetaModelOnePlusOne"]
+    optims = ["MemeticDE", "cGA", "DoubleFastGADiscreteOnePlusOne", "FastGADiscreteOnePlusOne"]
     for i in range(21):
         bonnans = corefuncs.BonnansFunction(index=i)
         for optim in optims:
+            instrum_str = "TransitionChoice" if "Discrete" in optim else "Softmax"
             dfunc = ExperimentFunction(
                 bonnans,
-                instrum.set_name("bitmap") if "Discrete" in optim else softmax_instrum.set_name("softmax"),
+                instrum.set_name("") if instrum_str == "TransitionChoice" else softmax_instrum.set_name(""),
             )
-            for budget in [20, 50, 100]:
+            dfunc.add_descriptors(index=i)
+            dfunc.add_descriptors(instrum_str=instrum_str)
+            # dfunc._descriptors = {'index': i}
+            for budget in [20, 30, 40, 50, 60, 70, 80, 90, 100]:
                 yield Experiment(dfunc, optim, num_workers=1, budget=budget, seed=next(seedg))
 
 
 # pylint: disable=redefined-outer-name,too-many-arguments
 @registry.register
 def yabbob(
     seed: tp.Optional[int] = None,
@@ -703,44 +880,138 @@
     # Parametrizing the noise level.
     if noise:
         noise_level = 100000 if hd else 100
     else:
         noise_level = 0
 
     # Choosing the list of optimizers.
-    optims: tp.List[str] = get_optimizers("competitive", seed=next(seedg))  # type: ignore
+    # optims: tp.List[str] = get_optimizers("competitive", seed=next(seedg))  # type: ignore
+    optims = [
+        "OnePlusOne",
+        "MetaModel",
+        "CMA",
+        "DE",
+        "PSO",
+        "TwoPointsDE",
+        "RandomSearch",
+        "ChainMetaModelSQP",
+        "NeuralMetaModel",
+        "MetaModelDE",
+        "MetaModelOnePlusOne",
+    ]
     if noise:
         optims += ["TBPSA", "SQP", "NoisyDiscreteOnePlusOne"]
     if hd:
         optims += ["OnePlusOne"]
         optims += get_optimizers("splitters", seed=next(seedg))  # type: ignore
 
     if hd and small:
-        optims = ["BO", "CMA", "PSO", "DE"]
-
+        optims += ["BO", "PCABO", "CMA", "PSO", "DE"]
+    if small and not hd:
+        optims += ["PCABO", "BO", "Cobyla"]
+    optims = [
+        "MetaModelDE",
+        "MetaModelOnePlusOne",
+        "OnePlusOne",
+        "ChainMetaModelSQP",
+        "RFMetaModel",
+        "RFMetaModelDE",
+    ]
     # if bounded:
     #    optims = ["BO", "PCABO", "BayesOptimBO", "CMA", "PSO", "DE"]
     # if box:
     #    optims = ["DiagonalCMA", "Cobyla", "NGOpt16", "NGOpt15", "CMandAS2", "OnePlusOne"]
     # List of objective functions.
+    optims = [
+        "MetaModelDE",
+        "NeuralMetaModelDE",
+        "SVMMetaModelDE",
+        "RFMetaModelDE",
+        "MetaModelTwoPointsDE",
+        "NeuralMetaModelTwoPointsDE",
+        "SVMMetaModelTwoPointsDE",
+        "RFMetaModelTwoPointsDE",
+        "GeneticDE",
+    ]
+    optims = ["LargeCMA", "TinyCMA", "OldCMA", "MicroCMA"]
+    optims = ["BFGS", "LBFGSB"]
+    optims = get_optimizers("oneshot", seed=next(seedg))  # type: ignore
+    optims = [
+        "MetaTuneRecentering",
+        "MetaRecentering",
+        "HullCenterHullAvgCauchyScrHammersleySearch",
+        "LHSSearch",
+        "LHSCauchySearch",
+    ]
+    optims = [
+        "BFGS",
+        "LBFGSB",
+        "MicroCMA",
+        "RandomSearch",
+        "NoisyDiscreteOnePlusOne",
+        "TBPSA",
+        "TinyCMA",
+        "CMA",
+        "ChainMetaModelSQP",
+        "OnePlusOne",
+        "MetaModel",
+        "RFMetaModel",
+        "DE",
+    ]
+    optims = ["NGOpt", "NGOptRW"]
+    optims = ["QrDE", "QODE", "LhsDE"]
+    optims = ["NGOptRW"]
+    if noise:
+        optims = [
+            #        "MicroCMA",
+            #        "TinyCMA",
+            #            "SQP",
+            #            "NoisyDiscreteOnePlusOne",
+            #            "TBPSA",
+            #        "RecombiningOptimisticNoisyDiscreteOnePlusOne",
+            #
+            #            "CMA",
+            #            "TinyCMA",
+            # "LPCMA",
+            # "VLPCMA",
+            # "MetaTuneRecentering",
+            # "MetaRecentering",
+            # "SPSA",
+            # "TinySQP",
+            # "MicroSQP",
+            # "TinySPSA",
+            # "MetaModel",
+            # "RFMetaModel",
+            # "RFMetaModelOnePlusOne",
+            "NoisyOnePlusOne",
+            # "MicroSPSA",
+        ]
+    else:
+        optims = ["MetaModelPSO", "RFMetaModelPSO", "SVMMetaModelPSO"]
     functions = [
         ArtificialFunction(
             name,
             block_dimension=d,
             rotation=rotation,
             noise_level=noise_level,
             split=split,
             num_blocks=num_blocks,
             bounded=bounded or box,
         )
         for name in names
         for rotation in [True, False]
         for num_blocks in ([1] if not split else [7, 12])
         for d in (
-            [100, 1000, 3000] if hd else ([2, 5, 10, 15] if tuning else ([40] if bounded else [2, 10, 50]))
+            [100, 1000, 3000]
+            if hd
+            else (
+                [2, 5, 10, 15]
+                if tuning
+                else ([40] if bounded else ([2, 3, 5, 10, 15, 20, 50] if noise else [2, 10, 50]))
+            )
         )
     ]
 
     assert reduction_factor in [1, 7, 13, 17]  # needs to be a cofactor
     functions = functions[::reduction_factor]
 
     # We possibly add constraints.
@@ -794,15 +1065,15 @@
                 func.constraint_violation += [
                     constraint
                 ]  # Just for storing, we will move it to the experiment soon
 
     budgets = (
         [40000, 80000, 160000, 320000]
         if (big and not noise)
-        else ([50, 200, 800, 3200, 12800] if not noise else [3200, 12800])
+        else ([50, 200, 800, 3200, 12800] if not noise else [3200, 12800, 51200, 102400])
     )
     if small and not noise:
         budgets = [10, 20, 40]
     if bounded:
         budgets = [10, 20, 40, 100, 300]
     for optim in optims:
         for function in functions:
@@ -1095,14 +1366,19 @@
         "OnePointDE",
         "GeneticDE",
         "TwoPointsDE",
         "PSO",
         "NGOptRW",
         "NGOpt",
     ]
+    optims = ["ChainMetaModelSQP", "MetaModelOnePlusOne", "MetaModelDE"]
+    optims = ["LargeCMA", "TinyCMA", "OldCMA", "MicroCMA"]
+    optims = ["BFGS", "LBFGSB", "MemeticDE"]
+    optims = ["QrDE", "QODE", "LhsDE", "NGOpt", "NGOptRW"]
+    optims = ["TinyCMA", "QODE", "MetaModelOnePlusOne", "LhsDE", "TinyLhsDE", "TinyQODE"]
     dims = [40, 20]
     functions = [
         ArtificialFunction(name, block_dimension=d, rotation=rotation, expo=expo)
         for name in ["cigar", "sphere", "rastrigin", "hm", "deceptivemultimodal"]
         for rotation in [True]
         for expo in [1.0, 3.0, 5.0, 7.0, 9.0]
         for d in dims
@@ -1359,14 +1635,16 @@
     """Some optimizers on a noisy optimization problem. This benchmark is based on the noisy benchmark.
     Budget 500, 1000, 2000, 4000, ... doubling... 128000.
     Rotation or not.
     Sphere, Sphere4, Cigar.
     """
     seedg = create_seed_generator(seed)
     optims: tp.List[str] = get_optimizers("spsa", seed=next(seedg))  # type: ignore
+    optims += ["CMA", "OnePlusOne", "DE", "PSO"]
+    optims = ["SQP", "NoisyDiscreteOnePlusOne", "NoisyBandit"]
     for budget in [500, 1000, 2000, 4000, 8000, 16000, 32000, 64000, 128000]:
         for optim in optims:
             for rotation in [True, False]:
                 for name in ["sphere", "sphere4", "cigar"]:
                     function = ArtificialFunction(
                         name=name, rotation=rotation, block_dimension=20, noise_level=10
                     )
@@ -1437,14 +1715,15 @@
 @registry.register
 def aquacrop_fao(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """FAO Crop simulator. Maximize yield."""
 
     funcs = [NgAquacrop(i, 300.0 + 150.0 * np.cos(i)) for i in range(3, 7)]
     seedg = create_seed_generator(seed)
     optims = get_optimizers("basics", seed=next(seedg))
+    optims = ["BFGS", "LBFGSB", "MemeticDE"]
     for budget in [25, 50, 100, 200, 400, 800, 1600]:
         for num_workers in [1, 30]:
             if num_workers < budget:
                 for algo in optims:
                     for fu in funcs:
                         xp = Experiment(fu, algo, budget, num_workers=num_workers, seed=next(seedg))
                         if not xp.is_incoherent:
@@ -1453,14 +1732,15 @@
 
 @registry.register
 def fishing(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Lotka-Volterra equations"""
     funcs = [OptimizeFish(i) for i in [17, 35, 52, 70, 88, 105]]
     seedg = create_seed_generator(seed)
     optims = get_optimizers("basics", seed=next(seedg))
+    optims += ["NGOpt", "NGOptRW", "ChainMetaModelSQP"]
     for budget in [25, 50, 100, 200, 400, 800, 1600]:
         for algo in optims:
             for fu in funcs:
                 xp = Experiment(fu, algo, budget, seed=next(seedg))
                 if not xp.is_incoherent:
                     yield xp
 
@@ -1469,14 +1749,19 @@
 def rocket(seed: tp.Optional[int] = None, seq: bool = False) -> tp.Iterator[Experiment]:
     """Rocket simulator. Maximize max altitude by choosing the thrust schedule, given a total thrust.
     Budget 25, 50, ..., 1600.
     Sequential or 30 workers."""
     funcs = [Rocket(i) for i in range(17)]
     seedg = create_seed_generator(seed)
     optims = get_optimizers("basics", seed=next(seedg))
+    optims += ["NGOpt", "NGOptRW", "ChainMetaModelSQP"]
+    optims = ["BFGS", "LBFGSB", "MemeticDE"]
+    optims = ["CMA", "PSO", "QODE", "QRDE", "MetaModelPSO"]
+    if seq:
+        optims += ["BFGS", "LBFGSB", "MemeticDE"]
     for budget in [25, 50, 100, 200, 400, 800, 1600]:
         for num_workers in [1] if seq else [1, 30]:
             if num_workers < budget:
                 for algo in optims:
                     for fu in funcs:
                         xp = Experiment(fu, algo, budget, num_workers=num_workers, seed=next(seedg))
                         skip_ci(reason="Too slow")
@@ -1536,15 +1821,15 @@
             array.set_mutation(sigma=sigma)  # type: ignore
         param.set_name(f"sigma={sigma}")
 
         f.parametrization = param
         f.parametrization.freeze()
         funcs2.append(f)
     optims = get_optimizers("basics")
-
+    optims = ["NGOpt", "PSO", "CMA"]
     for budget in [50, 75, 100, 150, 200, 250, 300, 400, 500, 1000, 3000, 5000, 8000, 16000, 32000, 64000]:
         for algo in optims:
             for fu in funcs2:
                 xp = Experiment(fu, algo, budget, num_workers=1, seed=next(seedg))
                 if not xp.is_incoherent:
                     yield xp
 
@@ -1563,15 +1848,15 @@
             control.Walker2d,
             control.Ant,
             control.Humanoid,
         ]
     ]
 
     optims = ["CMA", "NGOpt4", "DiagonalCMA", "NGOpt8", "MetaModel", "ChainCMAPowell"]
-
+    optims = ["NGOpt", "CMA", "PSO"]
     for budget in [50, 500, 5000, 10000, 20000, 35000, 50000, 100000, 200000]:
         for algo in optims:
             for fu in funcs:
                 xp = Experiment(fu, algo, budget, num_workers=1, seed=next(seedg))
                 if not xp.is_incoherent:
                     yield xp
 
@@ -1586,14 +1871,15 @@
         for k in range(2, 5):
             for noise in ["GaussianNoise", "UniformNoise", "GammaNoise"]:
                 for noise_scale in [0.5, 1]:
                     funcs.append(OlympusSurface(kind, 10**k, noise, noise_scale))
 
     seedg = create_seed_generator(seed)
     optims = get_optimizers("basics", "noisy", seed=next(seedg))
+    optims = ["NGOpt", "CMA"]
     for budget in [25, 50, 100, 200, 400, 800, 1600, 3200, 6400, 12800, 25600]:
         for num_workers in [1]:  # , 10, 100]:
             if num_workers < budget:
                 for algo in optims:
                     for fu in funcs:
                         xp = Experiment(fu, algo, budget, num_workers=num_workers, seed=next(seedg))
                         if not xp.is_incoherent:
@@ -1608,25 +1894,50 @@
     funcs = []
     for dataset_kind in OlympusEmulator.DATASETS:
         for model_kind in ["BayesNeuralNet", "NeuralNet"]:
             funcs.append(OlympusEmulator(dataset_kind, model_kind))
 
     seedg = create_seed_generator(seed)
     optims = get_optimizers("basics", "noisy", seed=next(seedg))
+    optims = ["NGOpt", "CMA"]
     for budget in [25, 50, 100, 200, 400, 800, 1600, 3200, 6400, 12800, 25600]:
         for num_workers in [1]:  # , 10, 100]:
             if num_workers < budget:
                 for algo in optims:
                     for fu in funcs:
                         xp = Experiment(fu, algo, budget, num_workers=num_workers, seed=next(seedg))
                         if not xp.is_incoherent:
                             yield xp
 
 
 @registry.register
+def topology_optimization(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    seedg = create_seed_generator(seed)
+    funcs = [TO(i) for i in [10, 20, 30, 40]]
+    optims = ["CMA", "GeneticDE", "TwoPointsDE", "VoronoiDE", "DE", "PSO", "RandomSearch", "OnePlusOne"]
+    for budget in [10, 20, 40, 80, 160, 320, 640, 1280, 2560, 5120, 10240, 20480, 40960]:
+        for optim in optims:
+            for f in funcs:
+                for nw in [1, 30]:
+                    yield Experiment(f, optim, budget, num_workers=nw, seed=next(seedg))
+
+
+@registry.register
+def sequential_topology_optimization(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    seedg = create_seed_generator(seed)
+    funcs = [TO(i) for i in [10, 20, 30, 40]]
+    optims = ["CMA", "GeneticDE", "TwoPointsDE", "VoronoiDE", "DE", "PSO", "RandomSearch", "OnePlusOne"]
+    for budget in [10, 20, 40, 80, 160, 320, 640, 1280, 2560, 5120, 10240, 20480, 40960]:
+        for optim in optims:
+            for f in funcs:
+                for nw in [1, 30]:
+                    yield Experiment(f, optim, budget, num_workers=nw, seed=next(seedg))
+
+
+@registry.register
 def simple_tsp(seed: tp.Optional[int] = None, complex_tsp: bool = False) -> tp.Iterator[Experiment]:
     """Simple TSP problems. Please note that the methods we use could be applied or complex variants, whereas
     specialized methods can not always do it; therefore this comparisons from a black-box point of view makes sense
     even if white-box methods are not included though they could do this more efficiently.
     10, 100, 1000, 10000 cities.
     Budgets doubling from 25, 50, 100, 200, ... up  to 25600
 
@@ -1733,14 +2044,16 @@
     funcs: tp.List[ExperimentFunction] = [
         _mlda.Clustering.from_mlda(name, num, rescale)
         for name, num in [("Ruspini", 5), ("German towns", 10), ("Ruspini", 50), ("German towns", 100)]
         for rescale in [True, False]
     ]
     seedg = create_seed_generator(seed)
     optims = get_optimizers("splitters", "progressive", seed=next(seedg))
+    optims += ["DE", "CMA", "PSO", "TwoPointsDE", "RandomSearch"]
+    optims = ["QODE", "QRDE"]
     for budget in [1000, 10000]:
         for num_workers in [1, 10, 100]:
             if num_workers < budget:
                 for algo in optims:
                     for func in funcs:
                         xp = Experiment(func, algo, budget, num_workers=num_workers, seed=next(seedg))
                         if not xp.is_incoherent:
@@ -1987,15 +2300,24 @@
     modules = {"mono": rl.agents.Perceptron, "multi": rl.agents.DenseNet}
     agents = {
         a: rl.agents.TorchAgent.from_module_maker(base_env, m, deterministic=False)
         for a, m in modules.items()
     }
     env = base_env.with_agent(player_0=random_agent).as_single_agent()
     dde = ng.optimizers.DifferentialEvolution(crossover="dimension").set_name("DiscreteDE")
-    optimizers: tp.List[tp.Any] = ["PSO", dde, "MetaTuneRecentering", "DiagonalCMA"]
+    optimizers: tp.List[tp.Any] = [
+        "PSO",
+        dde,
+        "MetaTuneRecentering",
+        "DiagonalCMA",
+        "TBPSA",
+        "SPSA",
+        "RecombiningOptimisticNoisyDiscreteOnePlusOne",
+        "MetaModelPSO",
+    ]
     for num_repetitions in [1, 10, 100]:
         for archi in ["mono", "multi"]:
             for optim in optimizers:
                 for env_budget in [5000, 10000, 20000, 40000]:
                     for num_workers in [1, 10, 100]:
                         # careful, not threadsafe
                         runner = rl.EnvironmentRunner(
@@ -2027,14 +2349,16 @@
     optims += [
         ng.families.DifferentialEvolution(multiobjective_adaptation=False).set_name("DE-noadapt"),
         ng.families.DifferentialEvolution(crossover="twopoints", multiobjective_adaptation=False).set_name(
             "TwoPointsDE-noadapt"
         ),
     ]
     optims += ["DiscreteOnePlusOne", "DiscreteLenglerOnePlusOne"]
+    optims = ["PymooNSGA2", "PymooBatchNSGA2", "LPCMA", "VLPCMA", "CMA"]
+    optims = ["LPCMA", "VLPCMA", "CMA"]
     popsizes = [20, 40, 80]
     optims += [
         ng.families.EvolutionStrategy(
             recombination_ratio=recomb, only_offsprings=only, popsize=pop, offsprings=pop * 5
         )
         for only in [True, False]
         for recomb in [0.1, 0.5]
@@ -2137,35 +2461,92 @@
     for func in FarOptimumFunction.itercases():
         for optim in optims:
             for budget in [100, 400, 1000, 4000, 10000]:
                 yield Experiment(func, optim, budget=budget, seed=next(seedg))
 
 
 @registry.register
-def photonics(seed: tp.Optional[int] = None, as_tuple: bool = False) -> tp.Iterator[Experiment]:
+def photonics(
+    seed: tp.Optional[int] = None,
+    as_tuple: bool = False,
+    small: bool = False,
+    ultrasmall: bool = False,
+) -> tp.Iterator[Experiment]:
     """Too small for being interesting: Bragg mirror + Chirped + Morpho butterfly."""
     seedg = create_seed_generator(seed)
+    divider = 2 if small else 1
+    if ultrasmall:
+        divider = 4
     optims = get_optimizers("es", "basics", "splitters", seed=next(seedg))  # type: ignore
+    optims = [
+        "MemeticDE",
+        "PSO",
+        "DE",
+        "CMA",
+        "OnePlusOne",
+        "TwoPointsDE",
+        "GeneticDE",
+        "ChainMetaModelSQP",
+        "MetaModelDE",
+        "SVMMetaModelDE",
+        "RFMetaModelDE",
+        "BFGS",
+        "LBFGSB",
+    ]
+    optims = ["QrDE", "QODE", "RFMetaModelDE"]
     for method in ["clipping", "tanh"]:  # , "arctan"]:
-        for name in ["bragg", "chirped", "morpho", "cf_photosic_realistic", "cf_photosic_reference"]:
-            func = Photonics(name, 60 if name == "morpho" else 80, bounding_method=method, as_tuple=as_tuple)
-            for budget in [1e3, 1e4, 1e5, 1e6]:
+        for name in (
+            ["bragg"]
+            if ultrasmall
+            else ["bragg", "chirped", "morpho", "cf_photosic_realistic", "cf_photosic_reference"]
+        ):
+            func = Photonics(
+                name,
+                4 * ((60 // divider) // 4) if name == "morpho" else 80 // divider,
+                bounding_method=method,
+                as_tuple=as_tuple,
+            )
+            for budget in [1e1, 1e2, 1e3]:
                 for algo in optims:
                     xp = Experiment(func, algo, int(budget), num_workers=1, seed=next(seedg))
                     if not xp.is_incoherent:
                         yield xp
 
 
 @registry.register
 def photonics2(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Counterpart of yabbob with higher dimensions."""
     return photonics(seed, as_tuple=True)
 
 
 @registry.register
+def ultrasmall_photonics(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Counterpart of yabbob with higher dimensions."""
+    return photonics(seed, as_tuple=False, small=True, ultrasmall=True)
+
+
+@registry.register
+def ultrasmall_photonics2(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Counterpart of yabbob with higher dimensions."""
+    return photonics(seed, as_tuple=True, small=True, ultrasmall=True)
+
+
+@registry.register
+def small_photonics(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Counterpart of yabbob with higher dimensions."""
+    return photonics(seed, as_tuple=False, small=True)
+
+
+@registry.register
+def small_photonics2(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
+    """Counterpart of yabbob with higher dimensions."""
+    return photonics(seed, as_tuple=True, small=True)
+
+
+@registry.register
 def adversarial_attack(seed: tp.Optional[int] = None) -> tp.Iterator[Experiment]:
     """Pretrained ResNes50 under black-box attacked.
     Square attacks:
     100 queries ==> 0.1743119266055046
     200 queries ==> 0.09043250327653997
     300 queries ==> 0.05111402359108781
     400 queries ==> 0.04325032765399738
@@ -2217,17 +2598,18 @@
         ]
     for dim in [16, 64, 100]:
         for fid in range(1, 24):
             for iid in range(1, 5):
                 index += 1
                 if reduced and index % 13:
                     continue
-                for instrumentation in ["Unordered"] if reduced else ["Softmax", "Ordered", "Unordered"]:
+                for instrumentation in ["Softmax", "Ordered", "Unordered"]:
                     try:
                         func = iohprofiler.PBOFunction(fid, iid, dim, instrumentation=instrumentation)
+                        func.add_descriptors(instrum_str=instrumentation)
                     except ModuleNotFoundError as e:
                         raise fbase.UnsupportedExperiment("IOHexperimenter needs to be installed") from e
                     for optim in list_optims:
                         for nw in [1, 10]:
                             for budget in [100, 1000, 10000]:
                                 yield Experiment(func, optim, num_workers=nw, budget=budget, seed=next(seedg))  # type: ignore
```

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/exporttable.py` & `nevergrad-0.8.0/nevergrad/benchmark/exporttable.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         f.write("\\lccode`3=`3\n")
         f.write("\\lccode`4=`4\n")
         f.write("\\lccode`5=`5\n")
         f.write("\\lccode`6=`6\n")
         f.write("\\lccode`7=`7\n")
         f.write("\\lccode`8=`8\n")
         f.write("\\lccode`9=`9\n")
-        f.write(r"\\newcolumntype{P}[1]{>{\hspace{0pt}}p{#1}}\n")
+        f.write(r"\newcolumntype{P}[1]{>{\hspace{0pt}}p{#1}}")
+        f.write("\n")
         f.write("\\begin{document}\n")
         f.write("\\scriptsize\n")
         f.write("\\renewcommand{\\arraystretch}{1.5}\n")
         f.write("\\sloppy\n")
         p = str(1.0 / (2 + len(cols)))
         # f.write("\\begin{landscape}\n")
         f.write(
```

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/frozenexperiments.py` & `nevergrad-0.8.0/nevergrad/benchmark/frozenexperiments.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/gymexperiments.py` & `nevergrad-0.8.0/nevergrad/benchmark/gymexperiments.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/optgroups.py` & `nevergrad-0.8.0/nevergrad/benchmark/optgroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,14 @@
         np.random.RandomState(seed).shuffle(optims)  # type: ignore
     return optims
 
 
 @registry.register
 def large() -> tp.Sequence[Optim]:
     return [
-        "NGO",
-        "Shiwa",
-        "DiagonalCMA",
         "CMA",
         "PSO",
         "DE",
         "MiniDE",
         "QrDE",
         "MiniQrDE",
         "LhsDE",
```

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/plotting.py` & `nevergrad-0.8.0/nevergrad/benchmark/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from . import utils
 from .exporttable import export_table
 
 # pylint: disable=too-many-locals
 
 
 _DPI = 250
+pure_algorithms = []
 
 # %% Basic tools
 
 
 def compactize(name: str) -> str:
     if len(name) < 70:
         return name
@@ -252,15 +253,22 @@
             "num_workers",
             "dimension",
             "useful_dimensions",
             "num_blocks",
             "block_dimension",
             "num_objectives",
         ):
-            df[col] = df[col].astype(float).astype(int)
+            try:
+                df[col] = df[col].astype(float).astype(int)
+            except Exception as e1:
+                try:
+                    for i in range(len(df[col])):
+                        float(df[col][i])
+                except Exception as e2:
+                    assert False, f"Fails at row {i+2}, Exceptions: {e1}, {e2}"
         elif col != "loss":
             df[col] = df[col].astype(str)
             df[col] = df[col].replace(r"\.[0]*$", "", regex=True)
             try:
                 df.loc[:, col] = pd.to_numeric(df.loc[:, col])
             except:
                 pass
@@ -378,14 +386,16 @@
                 casedf, fight_descriptors, num_rows=num_rows, complete_runs_only=True
             )
             fplotter = FightPlotter(data_df)
             if name == "fight_all.png":
                 with open(str(output_folder / name) + ".cp.txt", "w") as f:
                     f.write(fullname)
                     f.write("ranking:\n")
+                    global pure_algorithms
+                    pure_algorithms = list(data_df.columns[:])
                     for i, algo in enumerate(data_df.columns[:58]):
                         f.write(f"  algo {i}: {algo}\n")
             if name == "fight_all.png":
                 fplotter.save(str(output_folder / "fight_all_pure.png"), dpi=_DPI)
             else:
                 fplotter.save(str(output_folder / name) + "_pure.png", dpi=_DPI)
             if order == 2 and competencemaps and best_algo:  # With order 2 we can create a competence map.
@@ -401,15 +411,17 @@
     name_style = NameStyle()  # keep the same style for each algorithm
     cases = df.unique(descriptors)
     if not cases:
         cases = [()]
     # Average normalized plot with everything.
     out_filepath = output_folder / "xpresults_all.png"
     data = XpPlotter.make_data(df, normalized_loss=True)
-    xpplotter = XpPlotter(data, title=os.path.basename(output_folder), name_style=name_style, xaxis=xpaxis)
+    xpplotter = XpPlotter(
+        data, title=os.path.basename(output_folder), name_style=name_style, xaxis=xpaxis, pure_only=True
+    )
     xpplotter.save(out_filepath)
     # Now one xp plot per case.
     for case in cases:
         subdf = df.select_and_drop(**dict(zip(descriptors, case)))
         description = ",".join("{}:{}".format(x, y) for x, y in zip(descriptors, case))
         full_description = description
         description = compactize(description)
@@ -475,26 +487,34 @@
 
     def __init__(
         self,
         optim_vals: tp.Dict[str, tp.Dict[str, np.ndarray]],
         title: str,
         name_style: tp.Optional[tp.Dict[str, tp.Any]] = None,
         xaxis: str = "budget",
+        pure_only: bool = False,
     ) -> None:
         if name_style is None:
             name_style = NameStyle()
         upperbound = max(
             np.max(vals["loss"]) for vals in optim_vals.values() if np.max(vals["loss"]) < np.inf
         )
         for optim, vals in optim_vals.items():
             if optim.lower() in ["stupid", "idiot"] or optim in ["Zero", "StupidRandom"]:
                 upperbound = min(upperbound, np.max(vals["loss"]))
         # plot from best to worst
         lowerbound = np.inf
         sorted_optimizers = sorted(optim_vals, key=lambda x: optim_vals[x]["loss"][-1], reverse=True)
+        if pure_only:
+            assert len(pure_algorithms) > 0
+            # print(sorted_optimizers, " merged with ", pure_algorithms)
+            sorted_optimizers = [
+                o for o in sorted_optimizers if o + " " in [p[: (len(o) + 1)] for p in pure_algorithms]
+            ]
+            # print("Leads to ", sorted_optimizers)
         self._fig = plt.figure()
         self._ax = self._fig.add_subplot(111)
         # use log plot? yes, if no negative value
         logplot = not any(
             x <= 0 or x > 10**8 for ov in optim_vals.values() for x in ov["loss"]
         )  # if x < np.inf)
         if logplot:
```

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/test_core.py` & `nevergrad-0.8.0/nevergrad/benchmark/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/test_execution.py` & `nevergrad-0.8.0/nevergrad/benchmark/test_execution.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/test_experiments.py` & `nevergrad-0.8.0/nevergrad/benchmark/test_experiments.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/test_plotting.py` & `nevergrad-0.8.0/nevergrad/benchmark/test_plotting.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/test_utils.py` & `nevergrad-0.8.0/nevergrad/benchmark/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/test_xpbase.py` & `nevergrad-0.8.0/nevergrad/benchmark/test_xpbase.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/utils.py` & `nevergrad-0.8.0/nevergrad/benchmark/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             assert not df.isnull().values.any(), "Cannot work with NaN values"
             return set(tuple(row) for row in df.itertuples(index=False))
         else:
             raise NotImplementedError("Only strings, lists and tuples are allowed")
 
     @classmethod
     def read_csv(cls, path: tp.PathLike) -> "Selector":
-        return cls(pd.read_csv(str(path)))
+        return cls(pd.read_csv(str(path), on_bad_lines="skip"))
 
     def assert_equivalent(self, other: pd.DataFrame, err_msg: str = "") -> None:
         """Asserts that two selectors are equal, up to row and column permutations
 
         Note
         ----
         Use sparsely, since it is quite slow to test
```

### Comparing `nevergrad-0.7.0/nevergrad/benchmark/xpbase.py` & `nevergrad-0.8.0/nevergrad/benchmark/xpbase.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/decorators.py` & `nevergrad-0.8.0/nevergrad/common/decorators.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/errors.py` & `nevergrad-0.8.0/nevergrad/common/errors.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/test_decorators.py` & `nevergrad-0.8.0/nevergrad/common/test_decorators.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/test_testing.py` & `nevergrad-0.8.0/nevergrad/common/test_testing.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/test_tools.py` & `nevergrad-0.8.0/nevergrad/common/test_tools.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/testing.py` & `nevergrad-0.8.0/nevergrad/common/testing.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/tools.py` & `nevergrad-0.8.0/nevergrad/common/tools.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/common/typing.py` & `nevergrad-0.8.0/nevergrad/common/typing.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/__init__.py` & `nevergrad-0.8.0/nevergrad/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/ac/ac.py` & `nevergrad-0.8.0/nevergrad/functions/ac/ac.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/arcoating/core.py` & `nevergrad-0.8.0/nevergrad/functions/arcoating/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/arcoating/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/arcoating/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/base.py` & `nevergrad-0.8.0/nevergrad/functions/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,19 @@
             boundargs.apply_defaults()  # make sure we get the default non-provided arguments
             callargs = dict(boundargs.arguments)
             callargs.pop("self")
         inst._auto_init = callargs
         inst._descriptors = {
             x: y for x, y in callargs.items() if isinstance(y, (str, tuple, int, float, bool))
         }
+        # if "bonnans" in str(cls.__name__) or "discrete" in str(cls.__name__) or "pbo" in str(cls.__name__):
+        #    inst._descriptors = {
+        #        x: y for x, y in callargs.items() if isinstance(y, (str, tuple, int, float, bool)) and "dimension" not
+        #        in x and "paramet" not in x
+        #    }
         inst._descriptors["function_class"] = cls.__name__
         return inst  # type: ignore
 
     def __init__(
         self: EF,
         function: tp.Callable[..., tp.Loss],
         parametrization: p.Parameter,
```

### Comparing `nevergrad-0.7.0/nevergrad/functions/causaldiscovery/core.py` & `nevergrad-0.8.0/nevergrad/functions/causaldiscovery/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/causaldiscovery/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/causaldiscovery/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/control/core.py` & `nevergrad-0.8.0/nevergrad/functions/control/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/control/mujoco.py` & `nevergrad-0.8.0/nevergrad/functions/control/mujoco.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/control/test_mujoco.py` & `nevergrad-0.8.0/nevergrad/functions/control/test_mujoco.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/corefuncs.py` & `nevergrad-0.8.0/nevergrad/functions/corefuncs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/cycling.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/cycling.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/cyclist.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/cyclist.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/mensteampursuit.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/mensteampursuit.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/simulationresult.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/simulationresult.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/teampursuit.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/teampursuit.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/test_cycling.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/test_cycling.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/cycling/womensteampursuit.py` & `nevergrad-0.8.0/nevergrad/functions/cycling/womensteampursuit.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/fishing/core.py` & `nevergrad-0.8.0/nevergrad/functions/fishing/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/functionlib.py` & `nevergrad-0.8.0/nevergrad/functions/functionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/games/game.py` & `nevergrad-0.8.0/nevergrad/functions/games/game.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/games/test_game.py` & `nevergrad-0.8.0/nevergrad/functions/games/test_game.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/gym/multigym.py` & `nevergrad-0.8.0/nevergrad/functions/gym/multigym.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/gym/test_multigym.py` & `nevergrad-0.8.0/nevergrad/functions/gym/test_multigym.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/gym/tuple_gym_env.py` & `nevergrad-0.8.0/nevergrad/functions/gym/tuple_gym_env.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/helpers.py` & `nevergrad-0.8.0/nevergrad/functions/helpers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/images/core.py` & `nevergrad-0.8.0/nevergrad/functions/images/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/images/imagelosses.py` & `nevergrad-0.8.0/nevergrad/functions/images/imagelosses.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     REQUIRES_REFERENCE = False
 
     def __call__(self, img: np.ndarray) -> float:
         assert img.shape[2] == 3
         assert len(img.shape) == 3
         img = np.asarray(img, dtype=np.float64)
-        return -float(cv2.Laplacian(img, cv2.CV_64F).var())
+        return -float(cv2.Laplacian(img, cv2.CV_64F).var())  # type: ignore
 
 
 @registry.register
 class Brisque(ImageLoss):
     """
     This estimates the Brisque score (lower is better).
     """
```

### Comparing `nevergrad-0.7.0/nevergrad/functions/images/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/images/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/images/test_imagelosses.py` & `nevergrad-0.8.0/nevergrad/functions/images/test_imagelosses.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/iohprofiler/core.py` & `nevergrad-0.8.0/nevergrad/functions/iohprofiler/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/iohprofiler/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/iohprofiler/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/mixsimulator/core.py` & `nevergrad-0.8.0/nevergrad/functions/mixsimulator/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/ml/mlfunctionlib.py` & `nevergrad-0.8.0/nevergrad/functions/ml/mlfunctionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/ml/test_mlfunctionlib.py` & `nevergrad-0.8.0/nevergrad/functions/ml/test_mlfunctionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/mlda/datasets.py` & `nevergrad-0.8.0/nevergrad/functions/mlda/datasets.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/mlda/problems.py` & `nevergrad-0.8.0/nevergrad/functions/mlda/problems.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/mlda/test_datasets.py` & `nevergrad-0.8.0/nevergrad/functions/mlda/test_datasets.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/mlda/test_problems.py` & `nevergrad-0.8.0/nevergrad/functions/mlda/test_problems.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/multiobjective/__init__.py` & `nevergrad-0.8.0/nevergrad/functions/multiobjective/__init__.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/olympussurfaces/core.py` & `nevergrad-0.8.0/nevergrad/functions/olympussurfaces/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/olympussurfaces/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/olympussurfaces/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/pbt.py` & `nevergrad-0.8.0/nevergrad/functions/pbt.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/photonics/core.py` & `nevergrad-0.8.0/nevergrad/functions/photonics/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     divisor = max(2, len(bounds))
     assert not dimension % divisor, f"points length should be a multiple of {divisor}, got {dimension}"
     assert (
         shape[0] * shape[1] == dimension
     ), f"Cannot work with dimension {dimension} for {name}: not divisible by {shape[0]}."
     b_array = np.array(bounds)
     assert b_array.shape[0] == shape[0]  # pylint: disable=unsubscriptable-object
-    ones = np.ones((1, shape[1]))
+    ones = np.ones((1, int(shape[1])))
     init = np.sum(b_array, axis=1, keepdims=True).dot(ones) / 2  # type: ignore
     if as_tuple:
         instrum = ng.p.Instrumentation(
             *[
                 ng.p.Array(init=init[:, i]).set_bounds(
                     b_array[:, 0], b_array[:, 1], method=bounding_method, full_range_sampling=True
                 )
```

### Comparing `nevergrad-0.7.0/nevergrad/functions/photonics/photonics.py` & `nevergrad-0.8.0/nevergrad/functions/photonics/photonics.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/photonics/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/photonics/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/powersystems/core.py` & `nevergrad-0.8.0/nevergrad/functions/powersystems/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/powersystems/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/powersystems/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/pyomo/core.py` & `nevergrad-0.8.0/nevergrad/functions/pyomo/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/pyomo/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/pyomo/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/pyomo/test_pyomo_doc.py` & `nevergrad-0.8.0/nevergrad/functions/pyomo/test_pyomo_doc.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/rl/agents.py` & `nevergrad-0.8.0/nevergrad/functions/rl/agents.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/rl/base.py` & `nevergrad-0.8.0/nevergrad/functions/rl/base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/rl/envs.py` & `nevergrad-0.8.0/nevergrad/functions/rl/envs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/rl/test_agents.py` & `nevergrad-0.8.0/nevergrad/functions/rl/test_agents.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/rl/test_envs.py` & `nevergrad-0.8.0/nevergrad/functions/rl/test_envs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/rocket/rocket.py` & `nevergrad-0.8.0/nevergrad/functions/rocket/rocket.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/stsp/core.py` & `nevergrad-0.8.0/nevergrad/functions/stsp/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/stsp/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/stsp/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/test_base.py` & `nevergrad-0.8.0/nevergrad/functions/test_base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/test_corefuncs.py` & `nevergrad-0.8.0/nevergrad/functions/test_corefuncs.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/test_functionlib.py` & `nevergrad-0.8.0/nevergrad/functions/test_functionlib.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/test_utils.py` & `nevergrad-0.8.0/nevergrad/functions/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/unitcommitment/core.py` & `nevergrad-0.8.0/nevergrad/functions/unitcommitment/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/unitcommitment/test_core.py` & `nevergrad-0.8.0/nevergrad/functions/unitcommitment/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/functions/utils.py` & `nevergrad-0.8.0/nevergrad/functions/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/ops/constraints.py` & `nevergrad-0.8.0/nevergrad/ops/constraints.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/ops/test_constraints.py` & `nevergrad-0.8.0/nevergrad/ops/test_constraints.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/base.py` & `nevergrad-0.8.0/nevergrad/optimization/base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/callbacks.py` & `nevergrad-0.8.0/nevergrad/optimization/callbacks.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/differentialevolution.py` & `nevergrad-0.8.0/nevergrad/optimization/differentialevolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,33 +9,41 @@
 from nevergrad.parametrization import parameter as p
 from . import metamodel
 from . import base
 from . import oneshot
 
 
 class Crossover:
-    def __init__(self, random_state: np.random.RandomState, crossover: tp.Union[str, float]):
+    def __init__(
+        self,
+        random_state: np.random.RandomState,
+        crossover: tp.Union[str, float],
+        parameter: tp.Optional[p.Parameter] = None,
+    ):
         self.CR = 0.5
         self.crossover = crossover
         self.random_state = random_state
         if isinstance(crossover, float):
             self.CR = crossover
         elif crossover == "random":
             self.CR = self.random_state.uniform(0.0, 1.0)
-        elif crossover not in ["twopoints", "onepoint", "rotated_twopoints"]:
+        elif crossover not in ["twopoints", "onepoint", "rotated_twopoints", "voronoi"]:
             raise ValueError(f'Unknown crossover "{crossover}"')
+        self.shape = np.array(parameter.value).shape if parameter is not None else None
 
     def apply(self, donor: np.ndarray, individual: np.ndarray) -> None:
         dim = donor.size
         if self.crossover == "twopoints" and dim >= 4:
             return self.twopoints(donor, individual)
         elif self.crossover == "rotated_twopoints" and dim >= 4:
             return self.rotated_twopoints(donor, individual)
         elif self.crossover == "onepoint" and dim >= 3:
             return self.onepoint(donor, individual)
+        elif self.crossover == "voronoi":
+            return self.voronoi(donor, individual)
         else:
             return self.variablewise(donor, individual)
 
     def variablewise(self, donor: np.ndarray, individual: np.ndarray) -> None:
         R = self.random_state.randint(donor.size)
         # the following could be updated to vectorial uniform sampling (changes recomms)
         transfer = np.array(
@@ -65,14 +73,37 @@
         if bounds[1] == donor.size and not bounds[0]:  # make sure there is at least one point crossover
             bounds[self.random_state.randint(2)] = self.random_state.randint(1, donor.size)
         bounds2 = [self.random_state.choice(donor.size + 1 - bounds[1] + bounds[0])]
         bounds2.append(bounds2[0] + bounds[1] - bounds[0])
         assert bounds[1] < donor.size + 1
         donor[bounds[0] : bounds[1]] = individual[bounds2[0] : bounds2[1]]
 
+    def voronoi(self, donor: np.ndarray, individual: np.ndarray) -> None:
+        shape = self.shape
+        if shape is None or len(shape) < 2:
+            warnings.warn("Voronoi DE needs a shape.")
+            self.twopoints(donor, individual)
+            return
+        local_donor = donor.reshape(shape)
+        local_individual = individual.reshape(shape)
+        x1 = np.array([np.random.randint(shape[i]) for i in range(len(shape))])
+        x2 = np.array([np.random.randint(shape[i]) for i in range(len(shape))])
+        x3 = np.array([np.random.randint(shape[i]) for i in range(len(shape))])
+        x4 = np.array([np.random.randint(shape[i]) for i in range(len(shape))])
+        it = np.nditer(local_donor, flags=["multi_index"])
+        for _ in it:
+            d1 = np.linalg.norm(np.array(it.multi_index) - x1)
+            d2 = np.linalg.norm(np.array(it.multi_index) - x2)
+            d3 = np.linalg.norm(np.array(it.multi_index) - x3)
+            d4 = np.linalg.norm(np.array(it.multi_index) - x4)
+            if min([d1, d2, d3]) > d4:
+                local_donor[it.multi_index] = local_individual[it.multi_index]
+        donor[:] = local_donor.flatten()[:]
+        individual[:] = local_individual.flatten()[:]
+
 
 class _DE(base.Optimizer):
     """Differential evolution.
 
     Default pop size equal to 30
     We return the mean of the individuals with fitness better than median, which might be stupid sometimes.
     CR =.5, F1=.8, F2=.8, curr-to-best.
@@ -140,26 +171,37 @@
         with p.helpers.deterministic_sampling(out):
             out.set_standardized_data(data)
         return out
 
     def _internal_ask_candidate(self) -> p.Parameter:
         if len(self.population) < self.llambda:  # initialization phase
             init = self._config.initialization
+            if self.sampler is None and init == "QO":
+                self.sampler = oneshot.SamplingSearch(
+                    sampler="Hammersley", scrambled=True, opposition_mode="quasi"
+                )(self.parametrization, budget=self.llambda)
             if self.sampler is None and init not in ["gaussian", "parametrization"]:
                 assert init in ["LHS", "QR"]
                 self.sampler = oneshot.SamplingSearch(
                     sampler=init if init == "LHS" else "Hammersley", scrambled=init == "QR", scale=self.scale
                 )(
                     self.parametrization,
                     budget=self.llambda,
                 )
             if init == "parametrization":
                 candidate = self.parametrization.sample()
             elif self.sampler is not None:
                 candidate = self.sampler.ask()
+            elif self._config.crossover == "voronoi":
+                new_guy = (
+                    self.scale * self._rng.normal(0, 1, self.dimension)
+                    if len(self.population) > self.llambda / 6
+                    else self.scale * self._rng.normal() * np.ones(self.dimension)
+                )
+                candidate = self.parametrization.spawn_child().set_standardized_data(new_guy)
             else:
                 new_guy = self.scale * self._rng.normal(0, 1, self.dimension)
                 candidate = self.parametrization.spawn_child().set_standardized_data(new_guy)
             candidate.heritage["lineage"] = candidate.uid  # new lineage
             self.population[candidate.uid] = candidate
             self._uid_queue.asked.add(candidate.uid)
             return candidate
@@ -188,15 +230,17 @@
         donor = data + self._config.F1 * (data_a - data_b) + self._config.F2 * (data_best - data)
         candidate.parents_uids.extend([i.uid for i in (a, b)])
         # apply crossover
         co = self._config.crossover
         if co == "parametrization":
             candidate.recombine(self.parametrization.spawn_child().set_standardized_data(donor))
         else:
-            crossovers = Crossover(self._rng, 1.0 / self.dimension if co == "dimension" else co)
+            crossovers = Crossover(
+                self._rng, 1.0 / self.dimension if co == "dimension" else co, self.parametrization
+            )
             crossovers.apply(donor, data)
             candidate.set_standardized_data(donor, reference=self.parametrization)
         return candidate
 
     def _internal_tell_candidate(self, candidate: p.Parameter, loss: tp.FloatLoss) -> None:
         uid = candidate.heritage["lineage"]
         if uid not in self.population:  # parent was removed, revert to tell_not_asked
@@ -262,15 +306,15 @@
     which might be stupid sometimes though.
 
     Default settings are CR =.5, F1=.8, F2=.8, curr-to-best, pop size is 30
     Initial population: pure random.
 
     Parameters
     ----------
-    initialization: "parametrization", "LHS" or "QR"
+    initialization: "parametrization", "LHS" or "QR" or "QO"
         algorithm/distribution used for the initialization phase. If "parametrization", this uses the
         sample method of the parametrization.
     scale: float or str
         scale of random component of the updates
     recommendation: "pessimistic", "optimistic", "mean" or "noisy"
         choice of the criterion for the best point to recommend
     crossover: float or str
@@ -307,25 +351,26 @@
         popsize: tp.Union[str, int] = "standard",
         propagate_heritage: bool = False,  # experimental
         multiobjective_adaptation: bool = True,
         high_speed: bool = False,
     ) -> None:
         super().__init__(_DE, locals(), as_config=True)
         assert recommendation in ["optimistic", "pessimistic", "noisy", "mean"]
-        assert initialization in ["gaussian", "LHS", "QR", "parametrization"]
+        assert initialization in ["gaussian", "LHS", "QO", "QR", "parametrization"]
         assert isinstance(scale, float) or scale == "mini"
         if not isinstance(popsize, int):
             assert popsize in ["large", "dimension", "standard"]
         assert isinstance(crossover, float) or crossover in [
             "onepoint",
             "twopoints",
             "rotated_twopoints",
             "dimension",
             "random",
             "parametrization",
+            "voronoi",
         ]
         self.initialization = initialization
         self.scale = scale
         self.high_speed = high_speed
         self.recommendation = recommendation
         self.propagate_heritage = propagate_heritage
         self.F1 = F1
@@ -333,20 +378,22 @@
         self.crossover = crossover
         self.popsize = popsize
         self.multiobjective_adaptation = multiobjective_adaptation
 
 
 DE = DifferentialEvolution().set_name("DE", register=True)
 TwoPointsDE = DifferentialEvolution(crossover="twopoints").set_name("TwoPointsDE", register=True)
+VoronoiDE = DifferentialEvolution(crossover="voronoi").set_name("VoronoiDE", register=True)
 RotatedTwoPointsDE = DifferentialEvolution(crossover="rotated_twopoints").set_name(
     "RotatedTwoPointsDE", register=True
 )
 
 LhsDE = DifferentialEvolution(initialization="LHS").set_name("LhsDE", register=True)
 QrDE = DifferentialEvolution(initialization="QR").set_name("QrDE", register=True)
+QODE = DifferentialEvolution(initialization="QO").set_name("QODE", register=True)
 NoisyDE = DifferentialEvolution(recommendation="noisy").set_name("NoisyDE", register=True)
 AlmostRotationInvariantDE = DifferentialEvolution(crossover=0.9).set_name(
     "AlmostRotationInvariantDE", register=True
 )
 RotationInvariantDE = DifferentialEvolution(crossover=1.0, popsize="dimension").set_name(
     "RotationInvariantDE", register=True
 )
```

### Comparing `nevergrad-0.7.0/nevergrad/optimization/es.py` & `nevergrad-0.8.0/nevergrad/optimization/es.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/experimentalvariants.py` & `nevergrad-0.8.0/nevergrad/optimization/experimentalvariants.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/externalbo.py` & `nevergrad-0.8.0/nevergrad/optimization/externalbo.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/families.py` & `nevergrad-0.8.0/nevergrad/optimization/families.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/helpers.py` & `nevergrad-0.8.0/nevergrad/optimization/helpers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/metamodel.py` & `nevergrad-0.8.0/nevergrad/optimization/metamodel.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/multiobjective/core.py` & `nevergrad-0.8.0/nevergrad/optimization/multiobjective/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/multiobjective/hypervolume.py` & `nevergrad-0.8.0/nevergrad/optimization/multiobjective/hypervolume.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/multiobjective/nsga2.py` & `nevergrad-0.8.0/nevergrad/optimization/multiobjective/nsga2.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_core.py` & `nevergrad-0.8.0/nevergrad/optimization/multiobjective/test_core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_hypervolume.py` & `nevergrad-0.8.0/nevergrad/optimization/multiobjective/test_hypervolume.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/multiobjective/test_nsga2.py` & `nevergrad-0.8.0/nevergrad/optimization/multiobjective/test_nsga2.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/mutations.py` & `nevergrad-0.8.0/nevergrad/optimization/mutations.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/oneshot.py` & `nevergrad-0.8.0/nevergrad/optimization/oneshot.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/optimizerlib.py` & `nevergrad-0.8.0/nevergrad/optimization/optimizerlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,14 +139,18 @@
             "rls",
             "doublefastga",
             "adaptive",
             "coordinatewise_adaptive",
             "portfolio",
             "discreteBSO",
             "lengler",
+            "lengler2",
+            "lengler3",
+            "lenglerhalf",
+            "lenglerfourth",
             "doerr",
         ], f"Unkwnown mutation: '{mutation}'"
         if mutation == "adaptive":
             self._adaptive_mr = 0.5
         if mutation == "coordinatewise_adaptive":
             self._velocity = self._rng.uniform(size=self.dimension) * arity / 4.0
             self._modified_variables = np.array([True] * self.dimension)
@@ -267,14 +271,46 @@
                 alpha = 1.54468
                 intensity = int(max(1, self.dimension * (alpha * np.log(self.num_ask) / self.num_ask)))
                 data = mutator.portfolio_discrete_mutation(
                     pessimistic_data,
                     intensity=intensity,
                     arity=self.arity_for_discrete_mutation,
                 )
+            elif mutation == "lengler2":
+                alpha = 3.0
+                intensity = int(max(1, self.dimension * (alpha * np.log(self.num_ask) / self.num_ask)))
+                data = mutator.portfolio_discrete_mutation(
+                    pessimistic_data,
+                    intensity=intensity,
+                    arity=self.arity_for_discrete_mutation,
+                )
+            elif mutation == "lengler3":
+                alpha = 9.0
+                intensity = int(max(1, self.dimension * (alpha * np.log(self.num_ask) / self.num_ask)))
+                data = mutator.portfolio_discrete_mutation(
+                    pessimistic_data,
+                    intensity=intensity,
+                    arity=self.arity_for_discrete_mutation,
+                )
+            elif mutation == "lenglerfourth":
+                alpha = 0.4
+                intensity = int(max(1, self.dimension * (alpha * np.log(self.num_ask) / self.num_ask)))
+                data = mutator.portfolio_discrete_mutation(
+                    pessimistic_data,
+                    intensity=intensity,
+                    arity=self.arity_for_discrete_mutation,
+                )
+            elif mutation == "lenglerhalf":
+                alpha = 0.8
+                intensity = int(max(1, self.dimension * (alpha * np.log(self.num_ask) / self.num_ask)))
+                data = mutator.portfolio_discrete_mutation(
+                    pessimistic_data,
+                    intensity=intensity,
+                    arity=self.arity_for_discrete_mutation,
+                )
             elif mutation == "doerr":
                 # Selection, either random, or greedy, or a mutation rate.
                 assert self._doerr_index == -1, "We should have used this index in tell."
                 if self._rng.uniform() < self._doerr_epsilon:
                     index = self._rng.choice(range(len(self._doerr_mutation_rates)))
                     self._doerr_index = index
                 else:
@@ -380,14 +416,15 @@
         - `"discreteBSO"`: as in brainstorm optimization, we slowly decrease the mutation rate from 1 to 1/d.
         - `"fastga"`: FastGA mutations from the current best
         - `"doublefastga"`: double-FastGA mutations from the current best (Doerr et al, Fast Genetic Algorithms, 2017)
         - `"rls"`: Randomized Local Search (randomly mutate one and only one variable).
         - `"portfolio"`: Random number of mutated bits (called niform mixing in
           Dang & Lehre "Self-adaptation of Mutation Rates in Non-elitist Population", 2016)
         - `"lengler"`: specific mutation rate chosen as a function of the dimension and iteration index.
+        - `"lengler{2|3|half|fourth}"`: variant of Lengler
     crossover: bool
         whether to add a genetic crossover step every other iteration.
     use_pareto: bool
         whether to restart from a random pareto element in multiobjective mode, instead of the last one added
     sparse: bool
         whether we have random mutations setting variables to 0.
     smoother: bool
@@ -458,14 +495,26 @@
 )
 PortfolioDiscreteOnePlusOneT = ParametrizedOnePlusOne(tabu_length=10000, mutation="portfolio").set_name(
     "PortfolioDiscreteOnePlusOneT", register=True
 )
 DiscreteLenglerOnePlusOne = ParametrizedOnePlusOne(mutation="lengler").set_name(
     "DiscreteLenglerOnePlusOne", register=True
 )
+DiscreteLengler2OnePlusOne = ParametrizedOnePlusOne(mutation="lengler2").set_name(
+    "DiscreteLengler2OnePlusOne", register=True
+)
+DiscreteLengler3OnePlusOne = ParametrizedOnePlusOne(mutation="lengler3").set_name(
+    "DiscreteLengler3OnePlusOne", register=True
+)
+DiscreteLenglerHalfOnePlusOne = ParametrizedOnePlusOne(mutation="lenglerhalf").set_name(
+    "DiscreteLenglerHalfOnePlusOne", register=True
+)
+DiscreteLenglerFourthOnePlusOne = ParametrizedOnePlusOne(mutation="lenglerfourth").set_name(
+    "DiscreteLenglerFourthOnePlusOne", register=True
+)
 DiscreteLenglerOnePlusOneT = ParametrizedOnePlusOne(tabu_length=10000, mutation="lengler").set_name(
     "DiscreteLenglerOnePlusOneT", register=True
 )
 AdaptiveDiscreteOnePlusOne = ParametrizedOnePlusOne(mutation="adaptive").set_name(
     "AdaptiveDiscreteOnePlusOne", register=True
 )
 AnisotropicAdaptiveDiscreteOnePlusOne = ParametrizedOnePlusOne(mutation="coordinatewise_adaptive").set_name(
@@ -522,16 +571,18 @@
         super().__init__(parametrization, budget=budget, num_workers=num_workers)
         self.algorithm = algorithm
         self._config = ParametrizedCMA() if config is None else config
         pop = self._config.popsize
         self._popsize = (
             max(num_workers, 4 + int(self._config.popsize_factor * np.log(self.dimension)))
             if pop is None
-            else pop
+            else max(pop, num_workers)
         )
+        if self._config.elitist:
+            self._popsize = max(self._popsize, self.num_workers + 1)
         # internal attributes
         self._to_be_asked: tp.Deque[np.ndarray] = deque()
         self._to_be_told: tp.List[p.Parameter] = []
         self._num_spawners = self._popsize // 2  # experimental, for visualization
         self._parents = [self.parametrization]
         # delay initialization to ease implementation of variants
         self._es: tp.Any = None
@@ -754,14 +805,16 @@
         return out
 
     def enable_pickling(self) -> None:
         self.optim.enable_pickling()
 
 
 OldCMA = ParametrizedCMA().set_name("OldCMA", register=True)
+LargeCMA = ParametrizedCMA(scale=3.0).set_name("LargeCMA", register=True)
+TinyCMA = ParametrizedCMA(scale=0.33).set_name("TinyCMA", register=True)
 CMA = ParametrizedCMA().set_name("CMA", register=True)
 CMAbounded = ParametrizedCMA(
     scale=1.5884, popsize_factor=1, elitist=True, diagonal=True, fcmaes=False
 ).set_name("CMAbounded", register=True)
 CMAsmall = ParametrizedCMA(
     scale=0.3607, popsize_factor=3, elitist=False, diagonal=False, fcmaes=False
 ).set_name("CMAsmall", register=True)
@@ -1346,14 +1399,24 @@
         base_optimizer: base.OptCls = MetaCMA,
         scale: tp.Optional[float] = None,
     ) -> None:
         super().__init__(_Rescaled, locals())
 
 
 RescaledCMA = Rescaled().set_name("RescaledCMA", register=True)
+TinyLhsDE = Rescaled(base_optimizer=LhsDE, scale=1e-3).set_name("TinyLhsDE", register=True)
+TinyQODE = Rescaled(base_optimizer=QODE, scale=1e-3).set_name("TinyQODE", register=True)
+TinySQP = Rescaled(base_optimizer=SQP, scale=1e-3).set_name("TinySQP", register=True)
+MicroSQP = Rescaled(base_optimizer=SQP, scale=1e-6).set_name("MicroSQP", register=True)
+TinySQP.no_parallelization = True
+MicroSQP.no_parallelization = True
+TinySPSA = Rescaled(base_optimizer=SPSA, scale=1e-3).set_name("TinySPSA", register=True)
+MicroSPSA = Rescaled(base_optimizer=SPSA, scale=1e-6).set_name("MicroSPSA", register=True)
+TinySPSA.no_parallelization = True
+MicroSPSA.no_parallelization = True
 
 
 class SplitOptimizer(base.Optimizer):
     """Combines optimizers, each of them working on their own variables. (use ConfSplitOptimizer)"""
 
     def __init__(
         self,
@@ -1697,14 +1760,16 @@
 PolyCMA = ConfPortfolio(
     optimizers=[ParametrizedCMA(random_init=True) for _ in range(20)], warmup_ratio=0.33
 ).set_name("PolyCMA", register=True)
 MultiScaleCMA = ConfPortfolio(
     optimizers=[ParametrizedCMA(random_init=True, scale=scale) for scale in [1.0, 1e-3, 1e-6]],
     warmup_ratio=0.33,
 ).set_name("MultiScaleCMA", register=True)
+LPCMA = ParametrizedCMA(popsize_factor=10.0).set_name("LPCMA", register=True)
+VLPCMA = ParametrizedCMA(popsize_factor=100.0).set_name("VLPCMA", register=True)
 
 
 class _MetaModel(base.Optimizer):
     def __init__(
         self,
         parametrization: IntOrParameter,
         budget: tp.Optional[int] = None,
@@ -1713,18 +1778,17 @@
         multivariate_optimizer: tp.Optional[base.OptCls] = None,
         frequency_ratio: float = 0.9,
         algorithm: str,  # Quad or NN or SVR
     ) -> None:
         super().__init__(parametrization, budget=budget, num_workers=num_workers)
         self.frequency_ratio = frequency_ratio
         self.algorithm = algorithm
+        elitist = self.dimension < 3
         if multivariate_optimizer is None:
-            multivariate_optimizer = (
-                ParametrizedCMA(elitist=(self.dimension < 3)) if self.dimension > 1 else OnePlusOne
-            )
+            multivariate_optimizer = ParametrizedCMA(elitist=elitist) if self.dimension > 1 else OnePlusOne
         self._optim = multivariate_optimizer(
             self.parametrization, budget, num_workers
         )  # share parametrization and its rng
 
     def _internal_ask_candidate(self) -> p.Parameter:
         # We request a bit more points than what is really necessary for our dimensionality (+dimension).
         sample_size = int((self.dimension * (self.dimension - 1)) / 2 + 2 * self.dimension + 1)
@@ -1778,14 +1842,48 @@
 MetaModel = ParametrizedMetaModel().set_name("MetaModel", register=True)
 NeuralMetaModel = ParametrizedMetaModel(algorithm="neural").set_name("NeuralMetaModel", register=True)
 SVMMetaModel = ParametrizedMetaModel(algorithm="svr").set_name("SVMMetaModel", register=True)
 RFMetaModel = ParametrizedMetaModel(algorithm="rf").set_name("RFMetaModel", register=True)
 MetaModelOnePlusOne = ParametrizedMetaModel(multivariate_optimizer=OnePlusOne).set_name(
     "MetaModelOnePlusOne", register=True
 )
+RFMetaModelOnePlusOne = ParametrizedMetaModel(multivariate_optimizer=OnePlusOne, algorithm="rf").set_name(
+    "RFMetaModelOnePlusOne", register=True
+)
+MetaModelPSO = ParametrizedMetaModel(multivariate_optimizer=PSO).set_name("MetaModelPSO", register=True)
+RFMetaModelPSO = ParametrizedMetaModel(multivariate_optimizer=PSO, algorithm="rf").set_name(
+    "RFMetaModelPSO", register=True
+)
+SVMMetaModelPSO = ParametrizedMetaModel(multivariate_optimizer=PSO, algorithm="svr").set_name(
+    "SVMMetaModelPSO", register=True
+)
+
+MetaModelDE = ParametrizedMetaModel(multivariate_optimizer=DE).set_name("MetaModelDE", register=True)
+NeuralMetaModelDE = ParametrizedMetaModel(algorithm="neural", multivariate_optimizer=DE).set_name(
+    "NeuralMetaModelDE", register=True
+)
+SVMMetaModelDE = ParametrizedMetaModel(algorithm="svr", multivariate_optimizer=DE).set_name(
+    "SVMMetaModelDE", register=True
+)
+RFMetaModelDE = ParametrizedMetaModel(algorithm="rf", multivariate_optimizer=DE).set_name(
+    "RFMetaModelDE", register=True
+)
+
+MetaModelTwoPointsDE = ParametrizedMetaModel(multivariate_optimizer=TwoPointsDE).set_name(
+    "MetaModelTwoPointsDE", register=True
+)
+NeuralMetaModelTwoPointsDE = ParametrizedMetaModel(
+    algorithm="neural", multivariate_optimizer=TwoPointsDE
+).set_name("NeuralMetaModelTwoPointsDE", register=True)
+SVMMetaModelTwoPointsDE = ParametrizedMetaModel(algorithm="svr", multivariate_optimizer=TwoPointsDE).set_name(
+    "SVMMetaModelTwoPointsDE", register=True
+)
+RFMetaModelTwoPointsDE = ParametrizedMetaModel(algorithm="rf", multivariate_optimizer=TwoPointsDE).set_name(
+    "RFMetaModelTwoPointsDE", register=True
+)
 
 
 @registry.register
 class SQPCMA(Portfolio):
     """Passive portfolio of MetaCMA and many SQP."""
 
     def __init__(
@@ -2254,22 +2352,24 @@
         # Either we have the budget for each algorithm, or the last algorithm uses the rest of the budget, so:
         self.optimizers: tp.List[base.Optimizer] = []
         converter = {
             "num_workers": self.num_workers,
             "dimension": self.dimension,
             "half": self.budget // 2 if self.budget else self.num_workers,
             "third": self.budget // 3 if self.budget else self.num_workers,
+            "fourth": self.budget // 4 if self.budget else self.num_workers,
             "tenth": self.budget // 10 if self.budget else self.num_workers,
             "sqrt": int(np.sqrt(self.budget)) if self.budget else self.num_workers,
         }
         self.budgets = [max(1, converter[b]) if isinstance(b, str) else b for b in budgets]
         last_budget = None if self.budget is None else max(4, self.budget - sum(self.budgets))
         assert len(optimizers) == len(self.budgets) + 1
         assert all(
-            x in ("third", "half", "tenth", "dimension", "num_workers", "sqrt") or x > 0 for x in self.budgets
+            x in ("fourth", "third", "half", "tenth", "dimension", "num_workers", "sqrt") or x > 0
+            for x in self.budgets
         ), str(self.budgets)
         for opt, optbudget in zip(optimizers, self.budgets + [last_budget]):  # type: ignore
             self.optimizers.append(opt(self.parametrization, budget=optbudget, num_workers=self.num_workers))
         if self.name.startswith("chain"):
             warnings.warn(
                 "Chain optimizers are renamed with a capital C for consistency. "
                 "Eg: chainCMAPowell becomes ChainCMAPowell",
@@ -2324,14 +2424,20 @@
         super().__init__(_Chain, locals())
 
 
 # new names
 GeneticDE = Chaining([RotatedTwoPointsDE, TwoPointsDE], [200]).set_name(
     "GeneticDE", register=True
 )  # Also known as CGDE
+MemeticDE = Chaining([RotatedTwoPointsDE, TwoPointsDE, DE, SQP], ["fourth", "fourth", "fourth"]).set_name(
+    "MemeticDE", register=True
+)
+QNDE = Chaining([QODE, BFGS], ["half"]).set_name("QNDE", register=True)
+QNDE.no_parallelization = True
+MemeticDE.no_parallelization = True
 discretememetic = Chaining(
     [RandomSearch, DiscreteLenglerOnePlusOne, DiscreteOnePlusOne], ["third", "third"]
 ).set_name("discretememetic", register=True)
 # discretememeticT = Chaining(
 #     [RandomSearch, DiscreteLenglerOnePlusOneT, DiscreteOnePlusOneT], ["tenth", "third"]
 # ).set_name("discretememeticT", register=True)
 ChainCMAPowell = Chaining([MetaCMA, Powell], ["half"]).set_name("ChainCMAPowell", register=True)
```

### Comparing `nevergrad-0.7.0/nevergrad/optimization/recaster.py` & `nevergrad-0.8.0/nevergrad/optimization/recaster.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/recastlib.py` & `nevergrad-0.8.0/nevergrad/optimization/recastlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,15 @@
                 "CmaFmin2",
                 "Nelder-Mead",
                 "COBYLA",
                 "SLSQP",
                 "Powell",
             ]
             or "NLOPT" in method
+            or "BFGS" in method
         ), f"Unknown method '{method}'"
         self.method = method
         self.random_restart = random_restart
         # The following line rescales to [0, 1] if fully bounded.
 
         if method == "CmaFmin2" or "NLOPT" in method:
             normalizer = p.helpers.Normalizer(self.parametrization)
@@ -208,14 +209,16 @@
 
 
 NelderMead = NonObjectOptimizer(method="Nelder-Mead").set_name("NelderMead", register=True)
 CmaFmin2 = NonObjectOptimizer(method="CmaFmin2").set_name("CmaFmin2", register=True)
 NLOPT = NonObjectOptimizer(method="NLOPT").set_name("NLOPT", register=True)
 Powell = NonObjectOptimizer(method="Powell").set_name("Powell", register=True)
 RPowell = NonObjectOptimizer(method="Powell", random_restart=True).set_name("RPowell", register=True)
+BFGS = NonObjectOptimizer(method="BFGS", random_restart=True).set_name("BFGS", register=True)
+LBFGSB = NonObjectOptimizer(method="L-BFGS-B", random_restart=True).set_name("LBFGSB", register=True)
 Cobyla = NonObjectOptimizer(method="COBYLA").set_name("Cobyla", register=True)
 RCobyla = NonObjectOptimizer(method="COBYLA", random_restart=True).set_name("RCobyla", register=True)
 SQP = NonObjectOptimizer(method="SLSQP").set_name("SQP", register=True)
 SLSQP = SQP  # Just so that people who are familiar with SLSQP naming are not lost.
 RSQP = NonObjectOptimizer(method="SLSQP", random_restart=True).set_name("RSQP", register=True)
 RSLSQP = RSQP  # Just so that people who are familiar with SLSQP naming are not lost.
 NEWUOA = NonObjectOptimizer(method="NLOPT_LN_NEWUOA_BOUND").set_name("NEWUOA", register=True)
@@ -262,16 +265,34 @@
         #     "moead",
         #     "ctaea",
         # ]:  # algorithms that require reference points or reference directions
         #     the appropriate n_partitions must be looked into
         #     ref_dirs = get_reference_directions("das-dennis", self.num_objectives, n_partitions=12)
         #     algorithm = get_pymoo_algorithm(self.algorithm, ref_dirs)
         # else:
-        algorithm = get_pymoo_algorithm(weakself.algorithm)
         problem = _create_pymoo_problem(weakself, objective_function)
+        if weakself.algorithm == "CMAES":
+            from pymoo.algorithms.soo.nonconvex.cmaes import CMAES
+
+            algorithm = CMAES(x0=np.random.random(problem.n_var), maxfevals=weakself.budget)
+        elif weakself.algorithm == "BIPOP":
+            from pymoo.algorithms.soo.nonconvex.cmaes import CMAES
+
+            algorithm = CMAES(
+                x0=np.random.random(problem.n_var),
+                sigma=0.5,
+                restarts=2,
+                maxfevals=weakself.budget,
+                tolfun=1e-6,
+                tolx=1e-6,
+                restart_from_best=True,
+                bipop=True,
+            )
+        else:
+            algorithm = get_pymoo_algorithm(weakself.algorithm)
         pymoooptimize.minimize(problem, algorithm, seed=weakself._initial_seed)
         return None
 
     def _internal_ask_candidate(self) -> p.Parameter:
         """
         Special version to make sure that num_objectives has been set before
         the proper _internal_ask_candidate, in our parent class, is called.
@@ -500,9 +521,11 @@
             # pylint:disable=unused-argument
             # pymoo is supplying us with bounded parameters in [-pi/2,pi/2]. Nevergrad wants unbounded reals from us.
             out["F"] = self.objective_function(np.tan(X))
 
     return _PymooProblem(optimizer, objective_function)
 
 
+PymooCMAES = Pymoo(algorithm="CMAES").set_name("PymooCMAES", register=True)
+PymooBIPOP = Pymoo(algorithm="BIPOP").set_name("PymooBIPOP", register=True)
 PymooNSGA2 = Pymoo(algorithm="nsga2").set_name("PymooNSGA2", register=True)
 PymooBatchNSGA2 = PymooBatch(algorithm="nsga2").set_name("PymooBatchNSGA2", register=False)
```

### Comparing `nevergrad-0.7.0/nevergrad/optimization/requirements_check.py` & `nevergrad-0.8.0/nevergrad/optimization/requirements_check.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/sequences.py` & `nevergrad-0.8.0/nevergrad/optimization/sequences.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_base.py` & `nevergrad-0.8.0/nevergrad/optimization/test_base.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_callbacks.py` & `nevergrad-0.8.0/nevergrad/optimization/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_doc.py` & `nevergrad-0.8.0/nevergrad/optimization/test_doc.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_externalbo.py` & `nevergrad-0.8.0/nevergrad/optimization/test_externalbo.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_mutations.py` & `nevergrad-0.8.0/nevergrad/optimization/test_mutations.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_optimizerlib.py` & `nevergrad-0.8.0/nevergrad/optimization/test_optimizerlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 #
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
+import os
 import re
 import sys
 import time
 import random
 import inspect
 import logging
 import platform
@@ -16,14 +17,15 @@
 from functools import partial
 from unittest import SkipTest
 from unittest.mock import patch
 import pytest
 import numpy as np
 import pandas as pd
 from scipy import stats
+from scipy.ndimage import gaussian_filter
 from bayes_opt.util import acq_max
 
 # from bayes_opt.util import NotUniqueError
 import nevergrad as ng
 import nevergrad.common.typing as tp
 from nevergrad.common import testing
 from nevergrad.common import errors
@@ -206,22 +208,28 @@
         )
 
 
 @skip_win_perf  # type: ignore
 @pytest.mark.parametrize("name", registry)  # type: ignore
 def test_optimizers(name: str) -> None:
     """Checks that each optimizer is able to converge on a simple test case"""
-    if sum([ord(c) for c in name]) % 4 > 0 and name not in [
-        "DE",
-        "CMA",
-        "OnePlusOne",
-        "Cobyla",
-        "DiscreteLenglerOnePlusOne",
-        "PSO",
-    ]:
+    if (
+        sum([ord(c) for c in name]) % 4 > 0
+        and name
+        not in [
+            "DE",
+            "CMA",
+            "OnePlusOne",
+            "Cobyla",
+            "DiscreteLenglerOnePlusOne",
+            "PSO",
+        ]
+        or "Tiny" in name
+        or "Micro" in name
+    ):
         raise SkipTest("Too expensive: we randomly skip 3/4 of these tests.")
     if name in ["CMAbounded", "NEWUOA"]:  # Not a general purpose optimization method.
         return
     if "BO" in name:  # Bayesian Optimization is rarely good, let us save up time.
         return
     optimizer_cls = registry[name]
     if isinstance(optimizer_cls, base.ConfiguredOptimizer):
@@ -955,14 +963,81 @@
     x = ng.p.Array(shape=(5, 5)).set_integer_casting()
     assert (
         optlib.smooth_copy(x).get_standardized_data(reference=x).shape
         == x.get_standardized_data(reference=x).shape
     )
 
 
+@pytest.mark.parametrize("n", [5, 10, 15, 25, 40])  # type: ignore
+@pytest.mark.parametrize("b_per_dim", [1, 10, 20])  # type: ignore
+def test_voronoide(n, b_per_dim) -> None:
+    if n < 25 or b_per_dim < 1 and not os.environ.get("CIRCLECI", False):  # Outside CircleCI, only the big.
+        raise SkipTest("Only big things outside CircleCI.")
+
+    list_optims = ["CMA", "DE", "PSO", "RandomSearch", "TwoPointsDE", "OnePlusOne"]
+    if os.environ.get("CIRCLECI", False) and (n > 10 or n * b_per_dim > 100):  # In CircleCI, only the small.
+        raise SkipTest("Topology optimization too slow in CircleCI")
+    if os.environ.get("CIRCLECI", False) or (n < 10 or b_per_dim < 20):
+        list_optims = ["CMA", "PSO", "OnePlusOne"]
+    if n > 20:
+        list_optims = ["DE", "TwoPointsDE"]
+    fails = {}
+    for o in list_optims:
+        fails[o] = 0
+    size = n * n
+    sqrtsize = n
+    b = b_per_dim * size  # budget
+    nw = 20  # parallel workers
+
+    num_tests = 20
+    array = ng.p.Array(shape=(n, n), lower=-1.0, upper=1.0)
+    for idx in range(num_tests):
+        xa = idx % 3
+        xb = 2 - xa
+        xs = 1.5 * (
+            np.array([float(np.cos(xa * i + xb * j) < 0.0) for i in range(n) for j in range(n)]).reshape(n, n)
+            - 0.5
+        )
+        if (idx // 3) % 2 > 0:
+            xs = np.transpose(xs)
+        if (idx // 6) % 2 > 0:
+            xs = -xs
+
+        def f(x):
+            # return np.linalg.norm(x - xs) + np.linalg.norm(x - gaussian_filter(x, sigma=1))
+            return (
+                5.0 * np.sum(np.abs(x - xs) > 0.3) / size
+                + 13.0 * np.linalg.norm(x - gaussian_filter(x, sigma=3)) / sqrtsize
+            )
+
+        VoronoiDE = ng.optimizers.VoronoiDE(array, budget=b, num_workers=nw)
+        vde = f(VoronoiDE.minimize(f).value)
+        for o in list_optims:
+            try:
+                other = ng.optimizers.registry[o](array, budget=b, num_workers=nw)
+                val = f(other.minimize(f).value)
+            except:
+                print(f"crash in {o}")
+                val = float(1.0e7)
+            # print(o, val / vde)
+            if val < vde:
+                fails[o] += 1
+        # Remove both lines below. TODO
+        # ratio = min([(idx + 1 - fails[o]) / (0.001 + fails[o]) for o in list_optims])
+        # print(f"temporary: {ratio}", idx + 1, fails, f"({n}-{b_per_dim})")
+    ratio = min([(num_tests - fails[o]) / (0.001 + fails[o]) for o in list_optims])
+    print(f"VoronoiDE for DO: {ratio}", num_tests, fails, f"({n}-{b_per_dim})")
+
+    for o in list_optims:
+        ratio = 3.0 if "DE" not in "o" else 2.0
+        assert (
+            num_tests - fails[o] > ratio * fails[o]
+        ), f"Failure {o}: {fails[o]} / {num_tests}    ({n}-{b_per_dim})"
+
+
 def test_weighted_moo_de() -> None:
     for _ in range(1):  # Yes this is cheaper.
         D = 2
         N = 3
         DE = ng.optimizers.TwoPointsDE(D, budget=600)
         index = np.random.choice(range(N))
         w = np.ones(N)
```

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_recaster.py` & `nevergrad-0.8.0/nevergrad/optimization/test_recaster.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_sa.py` & `nevergrad-0.8.0/nevergrad/optimization/test_sa.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_sequences.py` & `nevergrad-0.8.0/nevergrad/optimization/test_sequences.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_special.py` & `nevergrad-0.8.0/nevergrad/optimization/test_special.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_suggest.py` & `nevergrad-0.8.0/nevergrad/optimization/test_suggest.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         "PortfolioDiscreteOne",
         "FastGADiscreteOne",
     ]
     return not any(k in name for k in keywords)
 
 
 @skip_win_perf  # type: ignore
-@pytest.mark.parametrize("name", [r for r in registry if "iscre" in r and good_at_suggest(r)])  # type: ignore
+@pytest.mark.parametrize("name", [r for r in registry if "iscre" in r and good_at_suggest(r) and ("Lengler" not in r or "LenglerOne" in r)])  # type: ignore
 def test_harder_suggest_optimizers(name: str) -> None:
     """Checks that discrete optimizers are good when a suggestion is nearby."""
     instrum = ng.p.Array(shape=(100,)).set_bounds(0.0, 1.0)
     instrum.set_integer_casting()
     optimum = np.asarray([0] * 17 + [1] * 17 + [0] * 66)
     target = lambda x: min(3, np.sum((np.asarray(x, dtype=int) - optimum) ** 2))
     suggestion = np.asarray([0] * 17 + [1] * 16 + [0] * 67)
```

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_tabu.py` & `nevergrad-0.8.0/nevergrad/optimization/test_tabu.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/test_utils.py` & `nevergrad-0.8.0/nevergrad/optimization/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/optimization/utils.py` & `nevergrad-0.8.0/nevergrad/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/_datalayers.py` & `nevergrad-0.8.0/nevergrad/parametrization/_datalayers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/_layering.py` & `nevergrad-0.8.0/nevergrad/parametrization/_layering.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/choice.py` & `nevergrad-0.8.0/nevergrad/parametrization/choice.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/container.py` & `nevergrad-0.8.0/nevergrad/parametrization/container.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/core.py` & `nevergrad-0.8.0/nevergrad/parametrization/core.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/data.py` & `nevergrad-0.8.0/nevergrad/parametrization/data.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/discretization.py` & `nevergrad-0.8.0/nevergrad/parametrization/discretization.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/helpers.py` & `nevergrad-0.8.0/nevergrad/parametrization/helpers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/instantiate.py` & `nevergrad-0.8.0/nevergrad/parametrization/instantiate.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/mutation.py` & `nevergrad-0.8.0/nevergrad/parametrization/mutation.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/parameter.py` & `nevergrad-0.8.0/nevergrad/parametrization/parameter.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_discretization.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_discretization.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_instantiate.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_layers.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_layers.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_mutation.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_mutation.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_param_doc.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_param_doc.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_parameter.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_parameter.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_parameters_legacy.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_parameters_legacy.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_transforms.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_transforms.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/test_utils.py` & `nevergrad-0.8.0/nevergrad/parametrization/test_utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/transforms.py` & `nevergrad-0.8.0/nevergrad/parametrization/transforms.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad/parametrization/utils.py` & `nevergrad-0.8.0/nevergrad/parametrization/utils.py`

 * *Files identical despite different names*

### Comparing `nevergrad-0.7.0/nevergrad.egg-info/PKG-INFO` & `nevergrad-0.8.0/nevergrad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nevergrad
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Python toolbox for performing gradient-free optimization
 Home-page: https://github.com/facebookresearch/nevergrad
 Author: Facebook AI Research
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
@@ -16,15 +16,15 @@
 Provides-Extra: benchmark
 License-File: LICENSE
 
 [![Support Ukraine](https://img.shields.io/badge/Support-Ukraine-FFD500?style=flat&labelColor=005BBB)](https://opensource.fb.com/support-ukraine) [![CircleCI](https://circleci.com/gh/facebookresearch/nevergrad/tree/main.svg?style=svg)](https://circleci.com/gh/facebookresearch/nevergrad/tree/main)
 
 # Nevergrad - A gradient-free optimization platform
 
-![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/Nevergrad-LogoMark.png)
+![Nevergrad](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.8.0/docs/resources/Nevergrad-LogoMark.png)
 
 
 `nevergrad` is a Python 3.6+ library. It can be installed with:
 
 ```
 pip install nevergrad
 ```
@@ -74,15 +74,15 @@
 # show the recommended keyword arguments of the function
 print(recommendation.kwargs)
 >>> {'learning_rate': 0.1998, 'batch_size': 4, 'architecture': 'conv'}
 ```
 
 Learn more on parametrization in the [**documentation**](https://facebookresearch.github.io/nevergrad/)!
 
-![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.7.0/docs/resources/TwoPointsDE.gif)
+![Example of optimization](https://raw.githubusercontent.com/facebookresearch/nevergrad/0.8.0/docs/resources/TwoPointsDE.gif)
 
 *Convergence of a population of points to the minima with two-points DE.*
 
 
 ## Documentation
 
 Check out our [**documentation**](https://facebookresearch.github.io/nevergrad/)! It's still a work in progress, don't hesitate to submit issues and/or PR to update it and make it clearer!
@@ -99,9 +99,9 @@
     journal = {GitHub repository},
     howpublished = {\url{https://GitHub.com/FacebookResearch/Nevergrad}},
 }
 ```
 
 ## License
 
-`nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.7.0/LICENSE) for additional details about it.
+`nevergrad` is released under the MIT license. See [LICENSE](https://github.com/facebookresearch/nevergrad/blob/0.8.0/LICENSE) for additional details about it.
 See also our [Terms of Use](https://opensource.facebook.com/legal/terms) and [Privacy Policy](https://opensource.facebook.com/legal/privacy).
```

### Comparing `nevergrad-0.7.0/nevergrad.egg-info/SOURCES.txt` & `nevergrad-0.8.0/nevergrad.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,17 @@
 nevergrad/functions/rl/test_envs.py
 nevergrad/functions/rocket/__init__.py
 nevergrad/functions/rocket/rocket.py
 nevergrad/functions/rocket/test_rocket.py
 nevergrad/functions/stsp/__init__.py
 nevergrad/functions/stsp/core.py
 nevergrad/functions/stsp/test_core.py
+nevergrad/functions/topology_optimization/__init__.py
+nevergrad/functions/topology_optimization/core.py
+nevergrad/functions/topology_optimization/test_core.py
 nevergrad/functions/unitcommitment/__init__.py
 nevergrad/functions/unitcommitment/core.py
 nevergrad/functions/unitcommitment/test_core.py
 nevergrad/ops/__init__.py
 nevergrad/ops/constraints.py
 nevergrad/ops/test_constraints.py
 nevergrad/optimization/__init__.py
```

### Comparing `nevergrad-0.7.0/nevergrad.egg-info/requires.txt` & `nevergrad-0.8.0/nevergrad.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 tensorflow>=2.7.0
 image-quality>=1.2.7
 keras>=2.4.3
 pymoo==0.5.0
 Keras-Preprocessing
 silence_tensorflow
 tensorflow_probability
-bayes-optim==0.2.5.5
+bayes-optim==0.3.0
 nlopt
 pybullet>=3.2.2
 box2d-py>=2.3.5
 glfw
 mujoco
 
 [all:sys_platform == "linux"]
@@ -90,15 +90,15 @@
 tensorflow>=2.7.0
 image-quality>=1.2.7
 keras>=2.4.3
 pymoo==0.5.0
 Keras-Preprocessing
 silence_tensorflow
 tensorflow_probability
-bayes-optim==0.2.5.5
+bayes-optim==0.3.0
 nlopt
 pybullet>=3.2.2
 box2d-py>=2.3.5
 glfw
 mujoco
 
 [benchmark:sys_platform == "linux"]
```

### Comparing `nevergrad-0.7.0/requirements/bench.txt` & `nevergrad-0.8.0/requirements/bench.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 image-quality>=1.2.7
 keras>=2.4.3
 pymoo==0.5.0
 olymp==0.0.1b0 ; sys_platform == "linux"
 Keras-Preprocessing
 silence_tensorflow  # for olymp
 tensorflow_probability  # for olymp
-bayes-optim==0.2.5.5
+bayes-optim==0.3.0
 nlopt
 pybullet>=3.2.2
 box2d-py>=2.3.5
 glfw
 mujoco
```

### Comparing `nevergrad-0.7.0/setup.py` & `nevergrad-0.8.0/setup.py`

 * *Files identical despite different names*

