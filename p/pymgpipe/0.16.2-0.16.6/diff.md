# Comparing `tmp/pymgpipe-0.16.2.tar.gz` & `tmp/pymgpipe-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymgpipe-0.16.2.tar", last modified: Tue Jul  4 00:20:21 2023, max compression
+gzip compressed data, was "pymgpipe-0.16.6.tar", last modified: Thu Jul  6 18:20:19 2023, max compression
```

## Comparing `pymgpipe-0.16.2.tar` & `pymgpipe-0.16.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.407652 pymgpipe-0.16.2/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.379306 pymgpipe-0.16.2/.github/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.382350 pymgpipe-0.16.2/.github/workflows/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1038 2023-04-27 18:57:29.000000 pymgpipe-0.16.2/.github/workflows/docs.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2945 2023-07-03 23:03:04.000000 pymgpipe-0.16.2/.github/workflows/python-package.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1144 2023-04-27 19:33:13.000000 pymgpipe-0.16.2/.github/workflows/tests.yml
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2059 2023-06-30 20:10:42.000000 pymgpipe-0.16.2/.gitignore
--rw-r--r--   0 yolimeydan   (501) staff       (20)    11389 2023-05-16 14:54:10.000000 pymgpipe-0.16.2/LICENSE
--rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-04 00:20:21.406953 pymgpipe-0.16.2/PKG-INFO
--rw-r--r--   0 yolimeydan   (501) staff       (20)    14257 2023-07-03 22:41:47.000000 pymgpipe-0.16.2/README.md
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.383517 pymgpipe-0.16.2/docs/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1162 2023-05-05 20:21:07.000000 pymgpipe-0.16.2/docs/conf.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      451 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/docs/index.rst
--rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/docs/modules.rst
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1212 2023-05-11 17:45:24.000000 pymgpipe-0.16.2/docs/pymgpipe.rst
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.384311 pymgpipe-0.16.2/examples/
--rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-05-11 17:28:05.000000 pymgpipe-0.16.2/examples/test_diet.csv
--rw-r--r--   0 yolimeydan   (501) staff       (20)    47496 2023-07-04 00:16:04.000000 pymgpipe-0.16.2/examples/workflow.ipynb
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.387719 pymgpipe-0.16.2/pymgpipe/
--rw-r--r--   0 yolimeydan   (501) staff       (20)      149 2023-07-03 21:57:55.000000 pymgpipe-0.16.2/pymgpipe/__init__.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2206 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/coupling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    14625 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/diet.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     9847 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/fva.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     5283 2023-07-03 21:59:54.000000 pymgpipe-0.16.2/pymgpipe/io.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      341 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/logger.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    12371 2023-06-30 20:03:36.000000 pymgpipe-0.16.2/pymgpipe/main.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1254 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/metrics.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     8900 2023-07-04 00:14:08.000000 pymgpipe-0.16.2/pymgpipe/modeling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     6417 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/nmpc.py
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.379912 pymgpipe-0.16.2/pymgpipe/resources/
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.392590 pymgpipe-0.16.2/pymgpipe/resources/diets/
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2656 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/AverageEuropeanDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2681 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/DACHDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2616 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/GlutenFreeDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2639 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/HighFatLowCarbDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2669 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/HighFiberDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2685 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/HighProteinDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2675 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/MediterraneanDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2657 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/Type2DiabetesDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2655 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/UnhealthyDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2624 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/VeganDiet.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2659 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/diets/VegetarianDiet.txt
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.393697 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaA.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaB.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaC.xml.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaD.xml.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.400041 pymgpipe-0.16.2/pymgpipe/resources/models/
--rw-r--r--   0 yolimeydan   (501) staff       (20)   319554 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.json
--rw-r--r--   0 yolimeydan   (501) staff       (20)   636272 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.mat
--rw-r--r--   0 yolimeydan   (501) staff       (20)  1624449 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml
--rw-r--r--   0 yolimeydan   (501) staff       (20)    75498 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.403927 pymgpipe-0.16.2/pymgpipe/resources/problems/
--rw-r--r--   0 yolimeydan   (501) staff       (20)   113023 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp
--rw-r--r--   0 yolimeydan   (501) staff       (20)    19492 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp.gz
--rw-r--r--   0 yolimeydan   (501) staff       (20)   185852 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps
--rw-r--r--   0 yolimeydan   (501) staff       (20)    24457 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps.gz
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.406528 pymgpipe-0.16.2/pymgpipe/tests/
--rw-r--r--   0 yolimeydan   (501) staff       (20)      592 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/conftest.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2092 2023-05-11 17:36:33.000000 pymgpipe-0.16.2/pymgpipe/tests/test_build.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1606 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_coupling.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     2550 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_diet.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     6096 2023-06-30 20:03:36.000000 pymgpipe-0.16.2/pymgpipe/tests/test_e2e.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1430 2023-04-27 19:31:46.000000 pymgpipe-0.16.2/pymgpipe/tests/test_fva.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1920 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_io.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)      723 2023-04-27 18:09:14.000000 pymgpipe-0.16.2/pymgpipe/tests/test_utils.py
--rw-r--r--   0 yolimeydan   (501) staff       (20)    11375 2023-05-18 15:36:12.000000 pymgpipe-0.16.2/pymgpipe/utils.py
-drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-04 00:20:21.388505 pymgpipe-0.16.2/pymgpipe.egg-info/
--rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/PKG-INFO
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1837 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/SOURCES.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)        1 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/dependency_links.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)       55 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/requires.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)        9 2023-07-04 00:20:21.000000 pymgpipe-0.16.2/pymgpipe.egg-info/top_level.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)      226 2023-06-30 20:03:34.000000 pymgpipe-0.16.2/requirements.txt
--rw-r--r--   0 yolimeydan   (501) staff       (20)       38 2023-07-04 00:20:21.407710 pymgpipe-0.16.2/setup.cfg
--rw-r--r--   0 yolimeydan   (501) staff       (20)     1608 2023-07-04 00:20:01.000000 pymgpipe-0.16.2/setup.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.440775 pymgpipe-0.16.6/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.400416 pymgpipe-0.16.6/.github/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.403140 pymgpipe-0.16.6/.github/workflows/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1038 2023-04-27 18:57:29.000000 pymgpipe-0.16.6/.github/workflows/docs.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2945 2023-07-03 23:03:04.000000 pymgpipe-0.16.6/.github/workflows/python-package.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1144 2023-04-27 19:33:13.000000 pymgpipe-0.16.6/.github/workflows/tests.yml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2059 2023-06-30 20:10:42.000000 pymgpipe-0.16.6/.gitignore
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    11389 2023-05-16 14:54:10.000000 pymgpipe-0.16.6/LICENSE
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-06 18:20:19.438650 pymgpipe-0.16.6/PKG-INFO
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    14257 2023-07-03 22:41:47.000000 pymgpipe-0.16.6/README.md
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.404300 pymgpipe-0.16.6/docs/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1162 2023-05-05 20:21:07.000000 pymgpipe-0.16.6/docs/conf.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      451 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/docs/index.rst
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/docs/modules.rst
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1212 2023-05-11 17:45:24.000000 pymgpipe-0.16.6/docs/pymgpipe.rst
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.404972 pymgpipe-0.16.6/examples/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       61 2023-05-11 17:28:05.000000 pymgpipe-0.16.6/examples/test_diet.csv
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    10097 2023-07-06 15:37:56.000000 pymgpipe-0.16.6/examples/workflow.ipynb
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.408430 pymgpipe-0.16.6/pymgpipe/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      149 2023-07-06 15:56:00.000000 pymgpipe-0.16.6/pymgpipe/__init__.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     3093 2023-07-06 15:20:02.000000 pymgpipe-0.16.6/pymgpipe/coupling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15530 2023-07-06 15:29:25.000000 pymgpipe-0.16.6/pymgpipe/diet.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     9849 2023-07-06 15:54:48.000000 pymgpipe-0.16.6/pymgpipe/fva.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     5731 2023-07-06 15:41:31.000000 pymgpipe-0.16.6/pymgpipe/io.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      341 2023-05-18 15:36:12.000000 pymgpipe-0.16.6/pymgpipe/logger.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    12373 2023-07-06 15:34:31.000000 pymgpipe-0.16.6/pymgpipe/main.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1255 2023-07-06 15:34:41.000000 pymgpipe-0.16.6/pymgpipe/metrics.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     8900 2023-07-04 00:14:08.000000 pymgpipe-0.16.6/pymgpipe/modeling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     6417 2023-05-18 15:36:12.000000 pymgpipe-0.16.6/pymgpipe/nmpc.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.401107 pymgpipe-0.16.6/pymgpipe/resources/
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.412429 pymgpipe-0.16.6/pymgpipe/resources/diets/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2656 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/AverageEuropeanDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2681 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/DACHDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2616 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/GlutenFreeDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2639 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/HighFatLowCarbDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2669 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/HighFiberDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2685 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/HighProteinDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2675 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/MediterraneanDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2657 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/Type2DiabetesDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2655 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/UnhealthyDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2624 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/VeganDiet.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2659 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/diets/VegetarianDiet.txt
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.420278 pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaA.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaB.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaC.xml.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    18688 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaD.xml.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.432703 pymgpipe-0.16.6/pymgpipe/resources/models/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   319554 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.json
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   636272 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.mat
+-rw-r--r--   0 yolimeydan   (501) staff       (20)  1624449 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.xml
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    75498 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.xml.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.436398 pymgpipe-0.16.6/pymgpipe/resources/problems/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   113023 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.lp
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    19492 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.lp.gz
+-rw-r--r--   0 yolimeydan   (501) staff       (20)   185852 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.mps
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    24457 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.mps.gz
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.438318 pymgpipe-0.16.6/pymgpipe/tests/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      592 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/tests/conftest.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2092 2023-05-11 17:36:33.000000 pymgpipe-0.16.6/pymgpipe/tests/test_build.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1606 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/tests/test_coupling.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     2550 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/tests/test_diet.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     6094 2023-07-06 15:56:38.000000 pymgpipe-0.16.6/pymgpipe/tests/test_e2e.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1430 2023-04-27 19:31:46.000000 pymgpipe-0.16.6/pymgpipe/tests/test_fva.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1920 2023-04-27 18:09:14.000000 pymgpipe-0.16.6/pymgpipe/tests/test_io.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      767 2023-07-06 16:44:07.000000 pymgpipe-0.16.6/pymgpipe/tests/test_utils.py
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    14813 2023-07-06 16:02:55.000000 pymgpipe-0.16.6/pymgpipe/utils.py
+drwxr-xr-x   0 yolimeydan   (501) staff       (20)        0 2023-07-06 18:20:19.409497 pymgpipe-0.16.6/pymgpipe.egg-info/
+-rw-r--r--   0 yolimeydan   (501) staff       (20)    15186 2023-07-06 18:20:19.000000 pymgpipe-0.16.6/pymgpipe.egg-info/PKG-INFO
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1837 2023-07-06 18:20:19.000000 pymgpipe-0.16.6/pymgpipe.egg-info/SOURCES.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)        1 2023-07-06 18:20:19.000000 pymgpipe-0.16.6/pymgpipe.egg-info/dependency_links.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       55 2023-07-06 18:20:19.000000 pymgpipe-0.16.6/pymgpipe.egg-info/requires.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)        9 2023-07-06 18:20:19.000000 pymgpipe-0.16.6/pymgpipe.egg-info/top_level.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)      226 2023-06-30 20:03:34.000000 pymgpipe-0.16.6/requirements.txt
+-rw-r--r--   0 yolimeydan   (501) staff       (20)       38 2023-07-06 18:20:19.440913 pymgpipe-0.16.6/setup.cfg
+-rw-r--r--   0 yolimeydan   (501) staff       (20)     1608 2023-07-06 18:18:04.000000 pymgpipe-0.16.6/setup.py
```

### Comparing `pymgpipe-0.16.2/.github/workflows/docs.yml` & `pymgpipe-0.16.6/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/.github/workflows/python-package.yml` & `pymgpipe-0.16.6/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/.github/workflows/tests.yml` & `pymgpipe-0.16.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/.gitignore` & `pymgpipe-0.16.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/LICENSE` & `pymgpipe-0.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/PKG-INFO` & `pymgpipe-0.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymgpipe
-Version: 0.16.2
+Version: 0.16.6
 Summary: Community level microbiome metabolic modeling in Python
 Home-page: https://github.com/korem-lab/pymgpipe
 Author: Yoli Meydan, Federico Baldini, Tal Korem
 Author-email: ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0
 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/issues
 Project-URL: Source, https://github.com/korem-lab/pymgpipe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.2 Summary: Community level
+Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.6 Summary: Community level
 microbiome metabolic modeling in Python Home-page: https://github.com/korem-
 lab/pymgpipe Author: Yoli Meydan, Federico Baldini, Tal Korem Author-email:
 ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/
 issues Project-URL: Source, https://github.com/korem-lab/pymgpipe Project-URL:
 Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `pymgpipe-0.16.2/README.md` & `pymgpipe-0.16.6/README.md`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/docs/conf.py` & `pymgpipe-0.16.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/docs/pymgpipe.rst` & `pymgpipe-0.16.6/docs/pymgpipe.rst`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/diet.py` & `pymgpipe-0.16.6/pymgpipe/diet.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     set_reaction_bounds,
     get_reaction_bounds,
 )
 from .io import load_model
 from .logger import logger
 
 def get_available_diets():
+    """Returns all diets that come pre-packaged with pymgpipe"""
     return [f.split('.txt')[0] for f in os.listdir(resource_filename("pymgpipe", "resources/diets/"))]
 
-def get_adapted_diet(
+def _get_adapted_diet(
     diet, essential_metabolites=None, micronutrients=None, vaginal=False, threshold=0.8
 ):
     if not isinstance(diet, pd.DataFrame):
         raise Exception(
             "Diet needs to be of type pd.DataFrame, received %s" % type(diet)
         )
 
@@ -398,22 +399,24 @@
 
     adapted_diet.index = adapted_diet.index.str.split("\(e\)").str[0]
     return adapted_diet
 
 
 # Removes any diet
 def remove_diet(model):
+    """Removes existing diet from model"""
     model = load_model(model)
     print("Removing diet from model...")
     for d in get_reactions(model, regex="Diet_EX_.*"):
         set_reaction_bounds(model, d, -1000, 1000)
 
 
 # Finds diet current set in model
 def get_diet(model):
+    """Returns existing diet from model"""
     model = load_model(model)
     print("Fetching diet from model...")
 
     diet = []
     for f in get_reactions(model, regex="Diet_EX_.*"):
         lower, upper = get_reaction_bounds(model, f)
         diet.append({"id": f.name, "lb": lower, "ub": upper})
@@ -426,14 +429,25 @@
     force_uptake=True,
     essential_metabolites=None,
     micronutrients=None,
     vaginal=False,
     threshold=0.8,
     check=True
 ):
+    """Add pymgpipe-adapated diet to model as defined by original mgPipe paper (see README for more details)
+
+    Args:
+        model (optlang.interface.model): LP problem
+        diet (pandas.DataFrame | str): Path to diet or dataframe
+        essential_metabolites (list): Custom of essential metabolites  (uses pre-defined list by default)
+        micronutrients (list): Custom list of micronutrients (uses pre-defined list by default)
+        vaginal (bool): Whether or not this is a vaginal diet
+        threshold (float): Value between 0 and 1 that defines how strict the diet constraints are (with 1 being the least strict)
+        check (bool): Check whether or not this diet is feasible (can take some time depending on size of model)
+    """
     model = load_model(model)
 
     print("\nAttempting to add diet...")
     if isinstance(diet, str) and os.path.exists(diet):
         if diet.endswith(".csv"):
             diet_df = load_dataframe(diet)
         elif diet.endswith(".txt"):
@@ -491,15 +505,15 @@
     diet_df = diet_df[diet_df.columns[0]].to_frame()
 
     if essential_metabolites is not None:
         print("Using custom set of essential metabolites...")
     if micronutrients is not None:
         print("Using custom set of micronutrients...")
 
-    d = get_adapted_diet(diet_df, essential_metabolites, micronutrients, vaginal, threshold)
+    d = _get_adapted_diet(diet_df, essential_metabolites, micronutrients, vaginal, threshold)
 
     logger.info("Adding %s diet to model..." % diet)
     added = []
 
     diet_reactions = {
         f.name.split("[d]")[0].split("Diet_")[-1]: f for f in diet_reactions
     }
```

### Comparing `pymgpipe-0.16.2/pymgpipe/fva.py` & `pymgpipe-0.16.6/pymgpipe/fva.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from functools import partial
 from optlang.interface import Objective
 from pathlib import Path
 from .utils import (
     load_model,
     Constants,
     get_reactions,
-    get_reverse_id,
+    _get_reverse_id,
     solve_model,
     load_dataframe,
 )
 from .io import suppress_stdout
 from .logger import logger
 from enum import Enum
 
@@ -250,15 +250,15 @@
 def _optlang_worker(threshold, metabolites):
     global global_model
 
     result = []
     for m in metabolites:
         net = global_model.variables[m]
 
-        reverse_id = get_reverse_id(m)
+        reverse_id = _get_reverse_id(m)
         if reverse_id in global_model.variables:
             net -= global_model.variables[reverse_id]
 
         global_model.objective = Objective(net, direction="max")
         max_sol = solve_model(model=global_model, reactions=[m]).to_dict()[
             global_model.name
         ][m]
```

### Comparing `pymgpipe-0.16.2/pymgpipe/io.py` & `pymgpipe-0.16.6/pymgpipe/io.py`

 * *Files 11% similar despite different names*

```diff
@@ -68,41 +68,49 @@
             % solver
         )
 
 
 # Loads cobra file and returns cobrapy model
 # RETURNS- cobra model
 def load_cobra_model(file, solver="gurobi"):
+    """Loads and returns COBRA model"""
     _, ext = path.splitext(file)
     read_func = _read_funcs[ext]
     try:
         with suppress_stdout():
             model = read_func(file)
     except Exception:
         raise Exception("Error reading cobra model at %s" % file)
     model.name = file.split("/")[-1].split(".")[0]
     model.solver = solver
 
     return model
 
 
-# Warning- COBRA won't save any additional custom constraints to the model (i.e. coupling constraints)
 def write_cobra_model(model, file):
+    """Writes COBRA model to file
+    
+    Warning: COBRA won't save any custom modifications added to the model (i.e. coupling constraints, diet, etc). For this reason, we recommend working and using the corresponding optlang LP problems.
+    """
     _, ext = path.splitext(file)
     write_func = _write_funcs[ext]
     try:
         with suppress_stdout():
             write_func(model, file)
     except Exception:
         raise Exception("Error writing cobra model to %s" % file)
 
 
 # Loads either LP file or cobra file and returns optlang model representing underlying optimization problem
 # RETURNS- optlang model
 def load_model(path, solver="gurobi"):
+    """Loads optlang.interface.Model from either an LP file (.lp or .mps) or any of the available COBRA file types (.xml, .mat, etc)
+    
+    Returns: optlang.interface.Model
+    """
     if isinstance(path, cobra.Model):
         path.solver.name = path.name
         return path.solver
     elif isinstance(path, optlang.interface.Model):
         return path
     elif not isinstance(path, str):
         raise Exception("Expected string, received %s" % type(path))
@@ -132,14 +140,15 @@
         optlang_model.solver.name = path.split("/")[-1].split(".")[0]
         return optlang_model.solver
 
     return optlang_model
 
 
 def write_lp_problem(model, out_file=None, compress=True, force=True):
+    """Writes optlang.interface.Model out to file (will compress by default)"""
     out_file = "./" + model.name + ".xml" if out_file is None else out_file
 
     if compress and not (out_file.endswith(".gz") or out_file.endswith(".7z")):
         out_file = out_file + ".gz"
     if not force and os.path.basename(out_file).split(".")[0] in [
         f.split(".")[0] for f in os.listdir(os.path.dirname(out_file))
     ]:
```

### Comparing `pymgpipe-0.16.2/pymgpipe/main.py` & `pymgpipe-0.16.6/pymgpipe/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from multiprocessing import Pool
 from functools import partial
 from .modeling import build
 from .diet import add_diet_to_model
 from .io import load_cobra_model, write_lp_problem, write_cobra_model, suppress_stdout
 from .utils import load_dataframe, remove_reverse_vars
 from .coupling import add_coupling_constraints
-from .metrics import compute_diversity_metrics
+from .metrics import _compute_diversity_metrics
 from .logger import logger
 
 cobra_config = Configuration()
 cobra_config.lower_bound = -1000
 cobra_config.upper_bound = 1000
 
 
@@ -262,15 +262,15 @@
                 diet_fecal_compartments=diet_fecal_compartments,
                 solver=solver
             )
         force = True 
         write_cobra_model(pymgpipe_model, model_out)
 
     if compute_metrics:
-        metrics = compute_diversity_metrics(pymgpipe_model)
+        metrics = _compute_diversity_metrics(pymgpipe_model)
         if metrics is None or len(metrics)==0:
             logger.warning('Unable to compute diversity metrics for %s'%pymgpipe_model.name)
 
     if force or (not os.path.exists(lp_out) and not os.path.exists(lp_out+'.gz') and not os.path.exists(lp_out+'.7z')):
         # ----- START OPTLANG MODIFICATIONS -----
         if remove_reverse_vars_from_lp:
             try:
```

### Comparing `pymgpipe-0.16.2/pymgpipe/metrics.py` & `pymgpipe-0.16.6/pymgpipe/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .utils import get_abundances
 import cobra
 
-def compute_diversity_metrics(model):
+def _compute_diversity_metrics(model):
     assert isinstance(model, cobra.Model), '`model` needs to be COBRA model to compute diversity metrics.'
     print('Computing metrics for %s...'%model.name)
 
     taxa = get_abundances(model)[model.name].to_dict()
     unique_reactions = set(r.id.split('__')[0] for r in model.reactions if 
         'EX' not in r.id and 
         'biomass' not in r.id and
```

### Comparing `pymgpipe-0.16.2/pymgpipe/modeling.py` & `pymgpipe-0.16.6/pymgpipe/modeling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/nmpc.py` & `pymgpipe-0.16.6/pymgpipe/nmpc.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/AverageEuropeanDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/AverageEuropeanDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/DACHDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/DACHDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/GlutenFreeDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/GlutenFreeDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/HighFatLowCarbDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/HighFatLowCarbDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/HighFiberDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/HighFiberDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/HighProteinDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/HighProteinDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/MediterraneanDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/MediterraneanDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/Type2DiabetesDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/Type2DiabetesDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/UnhealthyDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/UnhealthyDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/VeganDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/VeganDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/diets/VegetarianDiet.txt` & `pymgpipe-0.16.6/pymgpipe/resources/diets/VegetarianDiet.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaA.xml.gz` & `pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaA.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaB.xml.gz` & `pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaB.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaC.xml.gz` & `pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaC.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/miniTaxa/TaxaD.xml.gz` & `pymgpipe-0.16.6/pymgpipe/resources/miniTaxa/TaxaD.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.json` & `pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.json`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.mat` & `pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.mat`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml` & `pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.xml`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/models/mini_model.xml.gz` & `pymgpipe-0.16.6/pymgpipe/resources/models/mini_model.xml.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp` & `pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.lp`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.lp.gz` & `pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.lp.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps` & `pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.mps`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/resources/problems/mini_model.mps.gz` & `pymgpipe-0.16.6/pymgpipe/resources/problems/mini_model.mps.gz`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/conftest.py` & `pymgpipe-0.16.6/pymgpipe/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_build.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_coupling.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_coupling.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_diet.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_diet.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_e2e.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_e2e.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from pymgpipe import (
     add_coupling_constraints,
     compute_nmpcs,
     get_abundances,
     build_models,
     remove_reverse_vars,
     load_dataframe,
-    get_reverse_id,
+    build
 )
-from pymgpipe.modeling import build
+from pymgpipe.utils import _get_reverse_id
 from pytest_check import check
 import re
 import tempfile
 
 
 def test_build_models():
     samples = ["sample%s" % i for i in range(5)]
@@ -160,15 +160,15 @@
     pymgpipe_model = build(
         sample_data,
         sample='sample1',
         taxa_directory=taxa_directory,
         diet_fecal_compartments=True
     )
     some_var = pymgpipe_model.variables[100]
-    reverse_var_id = get_reverse_id(some_var.name)
+    reverse_var_id = _get_reverse_id(some_var.name)
 
     res1 = compute_nmpcs(samples=pymgpipe_model, write_to_file=False, threads=-1, objective_percent=None).nmpc
     remove_reverse_vars(pymgpipe_model, hard_remove=False)
     
     assert pymgpipe_model.variables[reverse_var_id].lb == 0 and pymgpipe_model.variables[reverse_var_id].ub == 0
     
     res2 = compute_nmpcs(samples=pymgpipe_model, write_to_file=False, threads=-1, objective_percent=None).nmpc
```

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_fva.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_fva.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_io.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/pymgpipe/tests/test_utils.py` & `pymgpipe-0.16.6/pymgpipe/tests/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pymgpipe import *
+from pymgpipe.utils import _get_reverse_id
 
 def test_remove_reverse_reactions(mini_optlang_model):
     num_reactions = len(mini_optlang_model.variables)
     some_var = mini_optlang_model.variables[100]
-    reverse_var_id = get_reverse_id(some_var.name)
+    reverse_var_id = _get_reverse_id(some_var.name)
     assert reverse_var_id in mini_optlang_model.variables
 
     remove_reverse_vars(mini_optlang_model,hard_remove=False)
     assert len(mini_optlang_model.variables) == num_reactions and \
         mini_optlang_model.variables[reverse_var_id].lb == 0 and mini_optlang_model.variables[reverse_var_id].ub == 0
 
     remove_reverse_vars(mini_optlang_model,hard_remove=True)
```

### Comparing `pymgpipe-0.16.2/pymgpipe.egg-info/PKG-INFO` & `pymgpipe-0.16.6/pymgpipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymgpipe
-Version: 0.16.2
+Version: 0.16.6
 Summary: Community level microbiome metabolic modeling in Python
 Home-page: https://github.com/korem-lab/pymgpipe
 Author: Yoli Meydan, Federico Baldini, Tal Korem
 Author-email: ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0
 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/issues
 Project-URL: Source, https://github.com/korem-lab/pymgpipe
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.2 Summary: Community level
+Metadata-Version: 2.1 Name: pymgpipe Version: 0.16.6 Summary: Community level
 microbiome metabolic modeling in Python Home-page: https://github.com/korem-
 lab/pymgpipe Author: Yoli Meydan, Federico Baldini, Tal Korem Author-email:
 ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu
 License: Apache-2.0 Project-URL: Issues, https://github.com/korem-lab/pymgpipe/
 issues Project-URL: Source, https://github.com/korem-lab/pymgpipe Project-URL:
 Readme, https://github.com/korem-lab/pymgpipe/blob/main/README.md Classifier:
 Intended Audience :: Healthcare Industry Classifier: Intended Audience ::
```

### Comparing `pymgpipe-0.16.2/pymgpipe.egg-info/SOURCES.txt` & `pymgpipe-0.16.6/pymgpipe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymgpipe-0.16.2/setup.py` & `pymgpipe-0.16.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     author="Yoli Meydan, Federico Baldini, Tal Korem",
     author_email="ym2877@cumc.columbia.edu, fb2557@cumc.columbia.edu, tk2829@cumc.columbia.edu",
     name="pymgpipe",
     description="Community level microbiome metabolic modeling in Python",
-    version="v0.16.2",
+    version="v0.16.6",
     classifiers=[
         "Intended Audience :: Healthcare Industry",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3",
         "Topic :: Scientific/Engineering",
```

