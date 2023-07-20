# Comparing `tmp/ctaplot-0.6.2.tar.gz` & `tmp/ctaplot-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctaplot-0.6.2.tar", last modified: Fri Apr  8 09:43:01 2022, max compression
+gzip compressed data, was "ctaplot-0.6.3.tar", last modified: Thu Jul 20 11:06:53 2023, max compression
```

## Comparing `ctaplot-0.6.2.tar` & `ctaplot-0.6.3.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-04-08 09:43:01.728090 ctaplot-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4037 2022-04-08 09:43:01.000000 ctaplot-0.6.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/ana/
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/ana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    48835 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/ana/ana.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/ana/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/ana/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13650 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/ana/tests/test_ana.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/gammaboard/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/gammaboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   399640 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/gammaboard/dashboard.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    57144 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/gammaboard/gammaboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4863 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/gammaboard/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/gammaboard/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/gammaboard/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/gammaboard/tests/test_gammaboard.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/io/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8089 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/io/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/io/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/io/tests/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/plots/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/calib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    70538 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/plots.py
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/style.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot/plots/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/tests/test_calib.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/tests/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    12225 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/tests/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot/plots/tests/test_style.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/ctaplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15453 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-08 09:43:01.000000 ctaplot-0.6.2/ctaplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-04-08 09:43:01.736090 ctaplot-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2022-04-08 09:43:01.000000 ctaplot-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.716090 ctaplot-0.6.2/share/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.712089 ctaplot-0.6.2/share/CTA_Performance/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.720090 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1660 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      772 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-Eres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1667 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-Eres.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.720090 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1670 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-Eres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1653 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      786 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1638 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-Eres.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.724089 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-Eres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      796 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1666 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-Eres.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.724089 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      680 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1655 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1642 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-Eres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      794 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1656 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      790 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      719 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      795 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-Eres.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.724089 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1521 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1590 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      551 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-Eres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1475 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-Angres.txt
--rw-r--r--   0 runner    (1001) docker     (121)      678 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-BackgroundSqdeg.txt
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-DiffSens.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffArea.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1533 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffAreaNoDirectionCut.txt
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-Eres.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.724089 ctaplot-0.6.2/share/CTA_Requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-30m-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-30m-LST-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-30m-MST-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-LST-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-LST-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-LST.dat
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-MST-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-MST-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-MST.dat
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h.dat
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-30m-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-30m-LST-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-30m-MST-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-30m-SST-EffectiveArea.dat
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-LST-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-LST-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      340 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-LST.dat
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-MST-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-MST-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-MST.dat
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-SST-AngRes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-SST-ERes.dat
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-SST.dat
--rw-r--r--   0 runner    (1001) docker     (121)      860 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h.dat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.724089 ctaplot-0.6.2/share/HESSII_Impact/
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Loose_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Safe_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Std_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Stereo.txt
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Loose_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Safe_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Std_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Stereo.txt
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Loose_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Safe_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Std_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Stereo.txt
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Loose_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Safe_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Std_Mono.txt
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Stereo.txt
--rw-r--r--   0 runner    (1001) docker     (121)  3833561 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/gammaboard.gif
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.724089 ctaplot-0.6.2/share/iact_sensitivities/
--rw-r--r--   0 runner    (1001) docker     (121)     6171 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/iact_sensitivities/magic_sensitivity_2014.ecsv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/share/images/
--rw-r--r--   0 runner    (1001) docker     (121)    49252 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/images/CTA_angular_resolution.png
--rw-r--r--   0 runner    (1001) docker     (121)    57237 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/images/CTA_effective_area.png
--rw-r--r--   0 runner    (1001) docker     (121)    49977 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/images/CTA_energy_resolution.png
--rw-r--r--   0 runner    (1001) docker     (121)    74611 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/images/CTA_sensitivity.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/share/simu_mc/
--rw-r--r--   0 runner    (1001) docker     (121)      811 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/simu_mc/gamma_20deg_0deg_cta-prod3-LaPalma_run_header.json
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/simu_mc/gamma_20deg_0deg_cta-prod3_Paranal_run_header.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-08 09:43:01.728090 ctaplot-0.6.2/share/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/styles/ctaplot-notebook
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/styles/ctaplot-paper
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-04-08 09:43:01.000000 ctaplot-0.6.2/share/styles/ctaplot-slides
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-20 11:06:53.710147 ctaplot-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-20 11:06:51.000000 ctaplot-0.6.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/ana/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/ana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/ana/ana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/ana/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/ana/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/ana/tests/test_ana.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/gammaboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/gammaboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   399640 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/gammaboard/dashboard.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    57989 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/gammaboard/gammaboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/gammaboard/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/gammaboard/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/gammaboard/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/gammaboard/tests/test_gammaboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/io/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/io/tests/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70668 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot/plots/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/tests/test_calib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/tests/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12225 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/tests/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-20 11:06:51.000000 ctaplot-0.6.3/ctaplot/plots/tests/test_style.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/ctaplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-07-20 11:06:53.000000 ctaplot-0.6.3/ctaplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-07-20 11:06:53.000000 ctaplot-0.6.3/ctaplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 11:06:53.000000 ctaplot-0.6.3/ctaplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-20 11:06:53.000000 ctaplot-0.6.3/ctaplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 11:06:53.000000 ctaplot-0.6.3/ctaplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 11:06:53.000000 ctaplot-0.6.3/ctaplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 11:06:53.710147 ctaplot-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-20 11:06:51.000000 ctaplot-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.690147 ctaplot-0.6.3/share/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.690147 ctaplot-0.6.3/share/CTA_Performance/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.698147 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-Eres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-Eres.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.698147 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-Eres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-Eres.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.698147 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-Eres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-Eres.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.702147 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-Eres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-Eres.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.702147 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-Eres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-Angres.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-BackgroundSqdeg.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-DiffSens.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffArea.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffAreaNoDirectionCut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-Eres.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.706147 ctaplot-0.6.3/share/CTA_Requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-30m-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-30m-LST-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-30m-MST-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-LST-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-LST-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-LST.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-MST-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-MST-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-MST.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-30m-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-30m-LST-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-30m-MST-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-30m-SST-EffectiveArea.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-LST-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-LST-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-LST.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-MST-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-MST-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-MST.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-SST-AngRes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-SST-ERes.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-SST.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.706147 ctaplot-0.6.3/share/HESSII_Impact/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Loose_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Safe_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Std_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 11:06:51.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Stereo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Loose_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Safe_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Std_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Stereo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Loose_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Safe_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Std_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Stereo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Loose_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Safe_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Std_Mono.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Stereo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  3833561 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/gammaboard.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.706147 ctaplot-0.6.3/share/iact_sensitivities/
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/iact_sensitivities/magic_sensitivity_2014.ecsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.706147 ctaplot-0.6.3/share/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    49252 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/images/CTA_angular_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57237 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/images/CTA_effective_area.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49977 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/images/CTA_energy_resolution.png
+-rw-r--r--   0 runner    (1001) docker     (123)    74611 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/images/CTA_sensitivity.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.706147 ctaplot-0.6.3/share/simu_mc/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/simu_mc/gamma_20deg_0deg_cta-prod3-LaPalma_run_header.json
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/simu_mc/gamma_20deg_0deg_cta-prod3_Paranal_run_header.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 11:06:53.710147 ctaplot-0.6.3/share/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/styles/ctaplot-notebook
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/styles/ctaplot-paper
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 11:06:52.000000 ctaplot-0.6.3/share/styles/ctaplot-slides
```

### Comparing `ctaplot-0.6.2/PKG-INFO` & `ctaplot-0.6.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,145 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ctaplot
-Version: 0.6.2
+Version: 0.6.3
 Summary: Compute and plot CTA IRFs
 Home-page: https://github.com/cta-observatory/ctaplot
 Author: Thomas Vuillaume, Mikael Jacquemont
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 License: MIT
-Description: =======
-        ctaplot
-        =======
-        
-        ctaplot provides low-level reconstruction quality-checks metrics computation and vizualisation for Imaging Atmospheric Cherenkov Telescopes such as CTA
-        
-        .. image:: https://travis-ci.org/cta-observatory/ctaplot.svg?branch=master
-            :target: https://travis-ci.org/cta-observatory/ctaplot
-            :alt: Travis CI
-        
-        .. image:: https://readthedocs.org/projects/ctaplot/badge/?version=latest
-           :target: https://ctaplot.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-            
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-           :target: https://opensource.org/licenses/MIT
-           :alt: License: MIT
-        
-        .. image:: https://mybinder.org/badge_logo.svg
-         :target: https://mybinder.org/v2/gh/cta-observatory/ctaplot/master?filepath=examples%2Fnotebooks
-         
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5833854.svg
-          :target: https://doi.org/10.5281/zenodo.5833853
-        
-        
-        You may find examples in the `documentation <https://ctaplot.readthedocs.io/en/latest/>`_ and run them via mybinder.
-        
-        
-        ----
-        
-        
-        * Code : https://github.com/cta-observatory/ctaplot
-        * Documentation : https://ctaplot.readthedocs.io/en/latest/
-        * Author contact: Thomas Vuillaume - thomas.vuillaume@lapp.in2p3.fr
-        * License: MIT
-        
-        ----
-        
-        The CTA instrument response functions data used in ctaplot come from the CTA Consortium and Observatory and may be found on the `cta-observatory website <http://www.cta-observatory.org/science/cta-performance/>`_ .
-        
-        In cases for which the CTA instrument response functions are used in a research project, we ask to add the following acknowledgement in any resulting publication:    
-        
-        “This research has made use of the CTA instrument response functions provided by the CTA Consortium and Observatory, see http://www.cta-observatory.org/science/cta-performance/ (version prod3b-v2) for more details.”
-        
-        ----
-        
-        
-        Install
-        =======
-        
-        
-        Requirements packages:
-        
-        * python > 3.6
-        * numpy  
-        * scipy>=0.19    
-        * matplotlib>=2.0
-        * astropy
-        
-        We recommend the use of `anaconda <https://www.anaconda.com>`_
-        
-        The package is available through pip:
-        
-        .. code-block:: bash
-        
-           pip install ctaplot
-        
-        
-        .. code-block:: bash
-        
-            export GAMMABOARD_DATA=path_to_the_data_directory
-        
-        
-        We recommend that you add this line to your bash source file (`$HOME/.bashrc` or `$HOME/.bash_profile`)
-        
-        
-        
-        GammaBoard
-        ==========
-        
-        *A dashboard to show them all.*
-        
-        
-        GammaBoard is a simple jupyter dashboard thought to display metrics assessing the reconstructions performances of
-        Imaging Atmospheric Cherenkov Telescopes (IACTs).
-        Deep learning is a lot about bookkeeping and trials and errors. GammaBoard ease this bookkeeping and allows quick
-        comparison of the reconstruction performances of your machine learning experiments.
-        
-        It is a working prototype used especially by the `GammaLearn <https://purl.org/gammalearn>`_ project.
-        
-        
-        Run GammaBoard
-        --------------
-        
-        To launch the dashboard, you can simply try the command:
-        
-        .. code-block:: bash
-        
-            gammaboard
-        
-        This will run a temporary copy of the dashboard (a jupyter notebook).
-        Local changes that you make in the dashboard will be discarded afterwards.
-        
-        GammaBoard is using data in a specific directory storing all your experiments files.
-        This directory is known under `$GAMMABOARD_DATA` by default.
-        However, you can change the path access at any time in the dashboard itself.
-        
-        Demo
-        ----
-        
-        Here is a simple demo of GammaBoard:  
-        
-        * On top the plots (metrics) such as angular resolution and energy resolution.
-        * Below, the list of experiments in the user folder.
-        
-        When an experiment is selected in the list, the data is automatically loaded, the metrics computed and displayed.
-        A list of information provided during the training phase is also displayed.
-        As many experiments results can be overlaid.
-        When an experiment is deselected, it simply is removed from the plots.
-        
-        
-        .. image:: /share/gammaboard.gif
-           :alt: gammaboard_demo
-        
-        
-        Cite
-        ====
-        
-        We would appreciate you cite the version of ctaplot you used using the corresponding Zenodo DOI that cound find here: https://doi.org/10.5281/zenodo.5833853
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
+
+=======
+ctaplot
+=======
+
+ctaplot provides low-level reconstruction quality-checks metrics computation and vizualisation for Imaging Atmospheric Cherenkov Telescopes such as CTA
+
+.. image:: https://travis-ci.org/cta-observatory/ctaplot.svg?branch=master
+    :target: https://travis-ci.org/cta-observatory/ctaplot
+    :alt: Travis CI
+
+.. image:: https://readthedocs.org/projects/ctaplot/badge/?version=latest
+   :target: https://ctaplot.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+    
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: License: MIT
+
+.. image:: https://mybinder.org/badge_logo.svg
+ :target: https://mybinder.org/v2/gh/cta-observatory/ctaplot/master?filepath=examples%2Fnotebooks
+ 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5833854.svg
+  :target: https://doi.org/10.5281/zenodo.5833853
+
+
+You may find examples in the `documentation <https://ctaplot.readthedocs.io/en/latest/>`_ and run them via mybinder.
+
+
+----
+
+
+* Code : https://github.com/cta-observatory/ctaplot
+* Documentation : https://ctaplot.readthedocs.io/en/latest/
+* Author contact: Thomas Vuillaume - thomas.vuillaume@lapp.in2p3.fr
+* License: MIT
+
+----
+
+The CTA instrument response functions data used in ctaplot come from the CTA Consortium and Observatory and may be found on the `cta-observatory website <http://www.cta-observatory.org/science/cta-performance/>`_ .
+
+In cases for which the CTA instrument response functions are used in a research project, we ask to add the following acknowledgement in any resulting publication:    
+
+“This research has made use of the CTA instrument response functions provided by the CTA Consortium and Observatory, see http://www.cta-observatory.org/science/cta-performance/ (version prod3b-v2) for more details.”
+
+----
+
+
+Install
+=======
+
+
+Requirements packages:
+
+* python > 3.6
+* numpy  
+* scipy>=0.19    
+* matplotlib>=2.0
+* astropy
+
+We recommend the use of `anaconda <https://www.anaconda.com>`_
+
+The package is available through pip:
+
+.. code-block:: bash
+
+   pip install ctaplot
+
+
+.. code-block:: bash
+
+    export GAMMABOARD_DATA=path_to_the_data_directory
+
+
+We recommend that you add this line to your bash source file (`$HOME/.bashrc` or `$HOME/.bash_profile`)
+
+
+
+GammaBoard
+==========
+
+*A dashboard to show them all.*
+
+
+GammaBoard is a simple jupyter dashboard thought to display metrics assessing the reconstructions performances of
+Imaging Atmospheric Cherenkov Telescopes (IACTs).
+Deep learning is a lot about bookkeeping and trials and errors. GammaBoard ease this bookkeeping and allows quick
+comparison of the reconstruction performances of your machine learning experiments.
+
+It is a working prototype used especially by the `GammaLearn <https://purl.org/gammalearn>`_ project.
+
+
+Run GammaBoard
+--------------
+
+To launch the dashboard, you can simply try the command:
+
+.. code-block:: bash
+
+    gammaboard
+
+This will run a temporary copy of the dashboard (a jupyter notebook).
+Local changes that you make in the dashboard will be discarded afterwards.
+
+GammaBoard is using data in a specific directory storing all your experiments files.
+This directory is known under `$GAMMABOARD_DATA` by default.
+However, you can change the path access at any time in the dashboard itself.
+
+Demo
+----
+
+Here is a simple demo of GammaBoard:  
+
+* On top the plots (metrics) such as angular resolution and energy resolution.
+* Below, the list of experiments in the user folder.
+
+When an experiment is selected in the list, the data is automatically loaded, the metrics computed and displayed.
+A list of information provided during the training phase is also displayed.
+As many experiments results can be overlaid.
+When an experiment is deselected, it simply is removed from the plots.
+
+
+.. image:: /share/gammaboard.gif
+   :alt: gammaboard_demo
+
+
+Cite
+====
+
+We would appreciate you cite the version of ctaplot you used using the corresponding Zenodo DOI that cound find here: https://doi.org/10.5281/zenodo.5833853
+
+
```

### Comparing `ctaplot-0.6.2/README.rst` & `ctaplot-0.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/ana/ana.py` & `ctaplot-0.6.3/ctaplot/ana/ana.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,15 +614,15 @@
         mask = (reco_energy > bins[i]) & (reco_energy < bins[i + 1])
 
         res_e.append(energy_resolution(true_energy[mask], reco_energy[mask],
                                        percentile=percentile,
                                        confidence_level=confidence_level,
                                        bias_correction=bias_correction))
 
-    return irf.energy_bins, np.array(res_e)
+    return bins, np.array(res_e)
 
 
 @u.quantity_input(true_energy=u.TeV, reco_energy=u.TeV, bins=u.TeV)
 def energy_bias(true_energy, reco_energy, bins=None):
     """
     Compute the true_energy relative bias per true_energy bin.
 
@@ -900,15 +900,15 @@
         irf = irf_cta()
         bins = irf.energy_bins
 
     count_R, bin_R = np.histogram(reco_energy, bins=bins)
     count_S, bin_S = np.histogram(true_energy, bins=bins)
 
     np.seterr(divide='ignore', invalid='ignore')
-    return irf.energy_bins, np.nan_to_num(simu_area * count_R / count_S)
+    return bins, np.nan_to_num(simu_area * count_R / count_S)
 
 
 @u.quantity_input(true_x=u.m, reco_x=u.m, true_y=u.m, reco_y=u.m)
 def impact_parameter_error(true_x, reco_x, true_y, reco_y):
     """
     compute the error distance between true and reconstructed impact parameters
     Parameters
```

### Comparing `ctaplot-0.6.2/ctaplot/ana/tests/test_ana.py` & `ctaplot-0.6.3/ctaplot/ana/tests/test_ana.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/gammaboard/dashboard.ipynb` & `ctaplot-0.6.3/ctaplot/gammaboard/dashboard.ipynb`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/gammaboard/gammaboard.py` & `ctaplot-0.6.3/ctaplot/gammaboard/gammaboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 import matplotlib.pyplot as plt
 from matplotlib.lines import Line2D
 from collections import OrderedDict
 from ipywidgets import HBox, Tab, Output, VBox, FloatSlider, Layout, Button, Dropdown, Text, Label
 from sklearn.metrics import roc_auc_score, precision_recall_curve
 from sklearn.multiclass import LabelBinarizer
-from astropy.table import Table
+from astropy.table import Table, vstack
 import astropy.units as u
 from tqdm.auto import tqdm
 from .. import plots
 from .. import ana
 from ..io.dataset import get
 
 __all__ = ['open_dashboard',
@@ -47,22 +47,25 @@
             filename, ext = os.path.splitext(file)
             filepath = os.path.join(dirname, file)
             if ext == '.h5' and guess_particle_type_from_file(filepath) in [GAMMA_ID, PROTON_ID]:
                 file_set.add(dirname + '/' + file)
     return tuple(file_set)
 
 
-def load_data_from_h5(experiment, experiments_directory, join_type='exact', metadata_conflicts='silent'):
+def load_data_from_h5(experiment, experiments_directory, join_type='inner', metadata_conflicts='silent'):
     """
     Load an hdf5 file containing results from an experiment
 
     Args
         experiment (str): the name of the experiment
         experiments_directory (str): the path to the folder containing the experiment folders
-        join_type (str): 'inner' | 'exact' (default) | 'outer'
+        join_type (str): 'inner' (default) | 'exact' | 'outer'
+            'inner': takes the intersection of all data tables
+            'exact': all data tables must have exactly the same columns
+            'outer': takes union of columns and fill missing values
         metadata_conflicts (str): 'silent' (default) | 'warn' | 'error'
 
     Returns
         `pandas.DataFrame`
     """
     assert experiment in os.listdir(experiments_directory)
 
@@ -76,28 +79,27 @@
 # TODO Find a more suitable naming
 def load_trig_events(experiment, experiments_directory):
     assert experiment in os.listdir(experiments_directory)
 
     result_files = find_data_files(experiment, experiments_directory)
     trig_energies = []
     for file in result_files:
-        try:
-            result_file = tables.open_file(file)
-        except Exception as e:
-            print('Could not open data file {}'.format(file))
-            print(e)
-        else:
+        if guess_particle_type_from_file(file) == GAMMA_ID:
             try:
-                if guess_particle_type_from_file(file) == GAMMA_ID:
-                    result_file.close()
-                    trig_energies.append(pd.read_hdf(file, key='triggered_events'))
-            except:
-                print("Cannot load the number of triggered events for experiment {} file".format(experiment))
-                return None
-    energies = Table.from_pandas(pd.concat(trig_energies))
+                dl1_params = Table.read(file, path='dl1/event/telescope/parameters/LST_LSTCam')
+                _, indices = np.unique(dl1_params[['obs_id', 'event_id']], axis=0, return_index=True)
+                trig_energies = dl1_params['mc_energy'][indices]
+            except OSError:
+                try:
+                    trig_energies.append(Table.from_pandas(pd.read_hdf(file, key='triggered_events')))
+                except KeyError as e:
+                    print("Cannot load the number of triggered events for experiment {} file".format(experiment))
+                    return None
+    energies = vstack(trig_energies)
+    energies.rename_column('mc_energy', 'mc_trig_energies')
     energies['mc_trig_energies'] *= u.TeV
     return energies
 
 
 def guess_particle_type_from_file(file_path):
     """
     Ever changing data formats...
@@ -107,15 +109,15 @@
         file_path (str): path to the file
 
     Returns
         particle id (int): if None, no identified particle type
     """
     def get_id_from_array(array):
         if len(set(array)) == 1:
-            return set(array)[0]
+            return array[0]
         else:
             return None
 
     filename = os.path.basename(file_path)
 
     if 'gamma' in filename:
         return GAMMA_ID
@@ -313,16 +315,16 @@
                 self.gamma_data = self.data
         self.mc_trig_events = load_trig_events(self.name, self.experiments_directory)
         self.run_configs = load_run_configs(self.name, self.experiments_directory)
 
     def update_gammaness_cut(self, new_cut):
 
         self.gammaness_cut = new_cut
-        self.reco_gamma_data = self.gamma_data[self.gamma_data['reco_particle'] >= self.gammaness_cut]
-        noise_mask = (self.data['true_particle'] != GAMMA_ID) & (self.data['reco_particle'] >= self.gammaness_cut)
+        self.reco_gamma_data = self.gamma_data[self.gamma_data['reco_gammaness'] >= self.gammaness_cut]
+        noise_mask = (self.data['true_particle'] != GAMMA_ID) & (self.data['reco_gammaness'] >= self.gammaness_cut)
         self.noise_reco_gamma = self.data[noise_mask]
 
     def get_data(self):
         return self.data
 
     def get_plotted(self):
         return self.plotted
@@ -344,28 +346,31 @@
                                                                        self.gamma_data['reco_azimuth'].quantity,
                                                                        self.gamma_data['true_energy'].quantity,
                                                                        bias_correction=self.bias_correction,
                                                                        ax=ax,
                                                                        label=self.name,
                                                                        color=self.color)
 
+            self.ax_ang_res.legend()
             self.set_plotted(True)
 
     def plot_angular_resolution_reco(self, ax=None):
         if self.get_loaded() and self.reco_gamma_data is not None:
             self.ax_ang_res = plots.plot_angular_resolution_per_energy(self.reco_gamma_data['true_altitude'].quantity,
                                                                        self.reco_gamma_data['reco_altitude'].quantity,
                                                                        self.reco_gamma_data['true_azimuth'].quantity,
                                                                        self.reco_gamma_data['reco_azimuth'].quantity,
                                                                        self.reco_gamma_data['true_energy'].quantity,
                                                                        bias_correction=self.bias_correction,
                                                                        ax=ax,
                                                                        label=self.name + '_reco',
                                                                        color=self.color,
+                                                                       marker='^'
                                                                        )
+            self.ax_ang_res.legend()
 
     def update_angular_resolution_reco(self, ax):
         for c in ax.containers:
             if self.name + '_reco' == c.get_label():
                 c.remove()
                 ax.containers.remove(c)
         self.plot_angular_resolution_reco(ax)
@@ -374,25 +379,28 @@
         if self.get_loaded():
             self.ax_ene_res = plots.plot_energy_resolution(self.gamma_data['true_energy'].quantity,
                                                            self.gamma_data['reco_energy'].quantity,
                                                            bias_correction=self.bias_correction,
                                                            ax=ax,
                                                            label=self.name,
                                                            color=self.color)
+            self.ax_ene_res.legend()
             self.set_plotted(True)
 
     def plot_energy_resolution_reco(self, ax=None):
         if self.get_loaded() and self.reco_gamma_data is not None:
             self.ax_ene_res = plots.plot_energy_resolution(self.reco_gamma_data['true_energy'].quantity,
                                                            self.reco_gamma_data['reco_energy'].quantity,
                                                            bias_correction=self.bias_correction,
                                                            ax=ax,
                                                            label=self.name + '_reco',
                                                            color=self.color,
+                                                           marker='^'
                                                            )
+            self.ax_ene_res.legend()
 
     def update_energy_resolution_reco(self, ax):
         for c in ax.containers:
             if self.name + '_reco' == c.get_label():
                 c.remove()
                 ax.containers.remove(c)
         self.plot_energy_resolution_reco(ax)
@@ -408,28 +416,31 @@
                                                                       ax=ax,
                                                                       label=self.name,
                                                                       color=self.color
                                                                       )
             self.ax_imp_res.set_xscale('log')
             self.ax_imp_res.set_xlabel('Energy [TeV]')
             self.ax_imp_res.set_ylabel('Impact resolution [km]')
+            self.ax_imp_res.legend()
             self.set_plotted(True)
 
     def plot_impact_resolution_reco(self, ax=None):
         if self.get_loaded() and self.reco_gamma_data is not None:
-            self.ax_imp_res = plots.plot_impact_resolution_per_energy(self.gamma_data['true_core_x'].quantity,
-                                                                      self.gamma_data['reco_core_x'].quantity,
-                                                                      self.gamma_data['true_core_y'].quantity,
-                                                                      self.gamma_data['reco_core_y'].quantity,
-                                                                      self.gamma_data['true_energy'].quantity,
+            self.ax_imp_res = plots.plot_impact_resolution_per_energy(self.reco_gamma_data['true_core_x'].quantity,
+                                                                      self.reco_gamma_data['reco_core_x'].quantity,
+                                                                      self.reco_gamma_data['true_core_y'].quantity,
+                                                                      self.reco_gamma_data['reco_core_y'].quantity,
+                                                                      self.reco_gamma_data['true_energy'].quantity,
                                                                       bias_correction=self.bias_correction,
                                                                       ax=ax,
                                                                       label=self.name + '_reco',
                                                                       color=self.color,
+                                                                      marker='^'
                                                                       )
+            self.ax_imp_res.legend()
 
     def update_impact_resolution_reco(self, ax):
         for c in ax.containers:
             if self.name + '_reco' == c.get_label():
                 c.remove()
                 ax.containers.remove(c)
         self.plot_impact_resolution_reco(ax)
```

### Comparing `ctaplot-0.6.2/ctaplot/gammaboard/reader.py` & `ctaplot-0.6.3/ctaplot/gammaboard/reader.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/io/dataset.py` & `ctaplot-0.6.3/ctaplot/io/dataset.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/plots/calib.py` & `ctaplot-0.6.3/ctaplot/plots/calib.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/plots/grid.py` & `ctaplot-0.6.3/ctaplot/plots/grid.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/plots/plots.py` & `ctaplot-0.6.3/ctaplot/plots/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -1511,15 +1511,18 @@
     Returns
     -------
     ax: `matplotlib.pyplot.axis`
     """
 
     ax = plt.gca() if ax is None else ax
     delta_res = new_resolution - reference_resolution
-    delta_res[:, 1:] = 0  # the condidence intervals have no meaning here
+    # delta_res[:, 1:] = 0  # the condidence intervals have no meaning here
+    # the condidence intervals have no meaning here
+    delta_res[:, 1] = delta_res[:, 0]
+    delta_res[:, 2] = delta_res[:, 0]
     with quantity_support():
         plot_resolution(bins, delta_res, ax=ax, **kwargs)
     ax.set_ylabel(r"$\Delta$ res")
     ax.set_title("Resolution difference")
 
     return ax
```

### Comparing `ctaplot-0.6.2/ctaplot/plots/style.py` & `ctaplot-0.6.3/ctaplot/plots/style.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/plots/tests/test_calib.py` & `ctaplot-0.6.3/ctaplot/plots/tests/test_calib.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot/plots/tests/test_plots.py` & `ctaplot-0.6.3/ctaplot/plots/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/ctaplot.egg-info/PKG-INFO` & `ctaplot-0.6.3/ctaplot.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,143 +1,145 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: ctaplot
-Version: 0.6.2
+Version: 0.6.3
 Summary: Compute and plot CTA IRFs
 Home-page: https://github.com/cta-observatory/ctaplot
 Author: Thomas Vuillaume, Mikael Jacquemont
 Author-email: thomas.vuillaume@lapp.in2p3.fr
 License: MIT
-Description: =======
-        ctaplot
-        =======
-        
-        ctaplot provides low-level reconstruction quality-checks metrics computation and vizualisation for Imaging Atmospheric Cherenkov Telescopes such as CTA
-        
-        .. image:: https://travis-ci.org/cta-observatory/ctaplot.svg?branch=master
-            :target: https://travis-ci.org/cta-observatory/ctaplot
-            :alt: Travis CI
-        
-        .. image:: https://readthedocs.org/projects/ctaplot/badge/?version=latest
-           :target: https://ctaplot.readthedocs.io/en/latest/?badge=latest
-           :alt: Documentation Status
-            
-        .. image:: https://img.shields.io/badge/license-MIT-blue.svg
-           :target: https://opensource.org/licenses/MIT
-           :alt: License: MIT
-        
-        .. image:: https://mybinder.org/badge_logo.svg
-         :target: https://mybinder.org/v2/gh/cta-observatory/ctaplot/master?filepath=examples%2Fnotebooks
-         
-        .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5833854.svg
-          :target: https://doi.org/10.5281/zenodo.5833853
-        
-        
-        You may find examples in the `documentation <https://ctaplot.readthedocs.io/en/latest/>`_ and run them via mybinder.
-        
-        
-        ----
-        
-        
-        * Code : https://github.com/cta-observatory/ctaplot
-        * Documentation : https://ctaplot.readthedocs.io/en/latest/
-        * Author contact: Thomas Vuillaume - thomas.vuillaume@lapp.in2p3.fr
-        * License: MIT
-        
-        ----
-        
-        The CTA instrument response functions data used in ctaplot come from the CTA Consortium and Observatory and may be found on the `cta-observatory website <http://www.cta-observatory.org/science/cta-performance/>`_ .
-        
-        In cases for which the CTA instrument response functions are used in a research project, we ask to add the following acknowledgement in any resulting publication:    
-        
-        “This research has made use of the CTA instrument response functions provided by the CTA Consortium and Observatory, see http://www.cta-observatory.org/science/cta-performance/ (version prod3b-v2) for more details.”
-        
-        ----
-        
-        
-        Install
-        =======
-        
-        
-        Requirements packages:
-        
-        * python > 3.6
-        * numpy  
-        * scipy>=0.19    
-        * matplotlib>=2.0
-        * astropy
-        
-        We recommend the use of `anaconda <https://www.anaconda.com>`_
-        
-        The package is available through pip:
-        
-        .. code-block:: bash
-        
-           pip install ctaplot
-        
-        
-        .. code-block:: bash
-        
-            export GAMMABOARD_DATA=path_to_the_data_directory
-        
-        
-        We recommend that you add this line to your bash source file (`$HOME/.bashrc` or `$HOME/.bash_profile`)
-        
-        
-        
-        GammaBoard
-        ==========
-        
-        *A dashboard to show them all.*
-        
-        
-        GammaBoard is a simple jupyter dashboard thought to display metrics assessing the reconstructions performances of
-        Imaging Atmospheric Cherenkov Telescopes (IACTs).
-        Deep learning is a lot about bookkeeping and trials and errors. GammaBoard ease this bookkeeping and allows quick
-        comparison of the reconstruction performances of your machine learning experiments.
-        
-        It is a working prototype used especially by the `GammaLearn <https://purl.org/gammalearn>`_ project.
-        
-        
-        Run GammaBoard
-        --------------
-        
-        To launch the dashboard, you can simply try the command:
-        
-        .. code-block:: bash
-        
-            gammaboard
-        
-        This will run a temporary copy of the dashboard (a jupyter notebook).
-        Local changes that you make in the dashboard will be discarded afterwards.
-        
-        GammaBoard is using data in a specific directory storing all your experiments files.
-        This directory is known under `$GAMMABOARD_DATA` by default.
-        However, you can change the path access at any time in the dashboard itself.
-        
-        Demo
-        ----
-        
-        Here is a simple demo of GammaBoard:  
-        
-        * On top the plots (metrics) such as angular resolution and energy resolution.
-        * Below, the list of experiments in the user folder.
-        
-        When an experiment is selected in the list, the data is automatically loaded, the metrics computed and displayed.
-        A list of information provided during the training phase is also displayed.
-        As many experiments results can be overlaid.
-        When an experiment is deselected, it simply is removed from the plots.
-        
-        
-        .. image:: /share/gammaboard.gif
-           :alt: gammaboard_demo
-        
-        
-        Cite
-        ====
-        
-        We would appreciate you cite the version of ctaplot you used using the corresponding Zenodo DOI that cound find here: https://doi.org/10.5281/zenodo.5833853
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
+
+=======
+ctaplot
+=======
+
+ctaplot provides low-level reconstruction quality-checks metrics computation and vizualisation for Imaging Atmospheric Cherenkov Telescopes such as CTA
+
+.. image:: https://travis-ci.org/cta-observatory/ctaplot.svg?branch=master
+    :target: https://travis-ci.org/cta-observatory/ctaplot
+    :alt: Travis CI
+
+.. image:: https://readthedocs.org/projects/ctaplot/badge/?version=latest
+   :target: https://ctaplot.readthedocs.io/en/latest/?badge=latest
+   :alt: Documentation Status
+    
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+   :target: https://opensource.org/licenses/MIT
+   :alt: License: MIT
+
+.. image:: https://mybinder.org/badge_logo.svg
+ :target: https://mybinder.org/v2/gh/cta-observatory/ctaplot/master?filepath=examples%2Fnotebooks
+ 
+.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.5833854.svg
+  :target: https://doi.org/10.5281/zenodo.5833853
+
+
+You may find examples in the `documentation <https://ctaplot.readthedocs.io/en/latest/>`_ and run them via mybinder.
+
+
+----
+
+
+* Code : https://github.com/cta-observatory/ctaplot
+* Documentation : https://ctaplot.readthedocs.io/en/latest/
+* Author contact: Thomas Vuillaume - thomas.vuillaume@lapp.in2p3.fr
+* License: MIT
+
+----
+
+The CTA instrument response functions data used in ctaplot come from the CTA Consortium and Observatory and may be found on the `cta-observatory website <http://www.cta-observatory.org/science/cta-performance/>`_ .
+
+In cases for which the CTA instrument response functions are used in a research project, we ask to add the following acknowledgement in any resulting publication:    
+
+“This research has made use of the CTA instrument response functions provided by the CTA Consortium and Observatory, see http://www.cta-observatory.org/science/cta-performance/ (version prod3b-v2) for more details.”
+
+----
+
+
+Install
+=======
+
+
+Requirements packages:
+
+* python > 3.6
+* numpy  
+* scipy>=0.19    
+* matplotlib>=2.0
+* astropy
+
+We recommend the use of `anaconda <https://www.anaconda.com>`_
+
+The package is available through pip:
+
+.. code-block:: bash
+
+   pip install ctaplot
+
+
+.. code-block:: bash
+
+    export GAMMABOARD_DATA=path_to_the_data_directory
+
+
+We recommend that you add this line to your bash source file (`$HOME/.bashrc` or `$HOME/.bash_profile`)
+
+
+
+GammaBoard
+==========
+
+*A dashboard to show them all.*
+
+
+GammaBoard is a simple jupyter dashboard thought to display metrics assessing the reconstructions performances of
+Imaging Atmospheric Cherenkov Telescopes (IACTs).
+Deep learning is a lot about bookkeeping and trials and errors. GammaBoard ease this bookkeeping and allows quick
+comparison of the reconstruction performances of your machine learning experiments.
+
+It is a working prototype used especially by the `GammaLearn <https://purl.org/gammalearn>`_ project.
+
+
+Run GammaBoard
+--------------
+
+To launch the dashboard, you can simply try the command:
+
+.. code-block:: bash
+
+    gammaboard
+
+This will run a temporary copy of the dashboard (a jupyter notebook).
+Local changes that you make in the dashboard will be discarded afterwards.
+
+GammaBoard is using data in a specific directory storing all your experiments files.
+This directory is known under `$GAMMABOARD_DATA` by default.
+However, you can change the path access at any time in the dashboard itself.
+
+Demo
+----
+
+Here is a simple demo of GammaBoard:  
+
+* On top the plots (metrics) such as angular resolution and energy resolution.
+* Below, the list of experiments in the user folder.
+
+When an experiment is selected in the list, the data is automatically loaded, the metrics computed and displayed.
+A list of information provided during the training phase is also displayed.
+As many experiments results can be overlaid.
+When an experiment is deselected, it simply is removed from the plots.
+
+
+.. image:: /share/gammaboard.gif
+   :alt: gammaboard_demo
+
+
+Cite
+====
+
+We would appreciate you cite the version of ctaplot you used using the corresponding Zenodo DOI that cound find here: https://doi.org/10.5281/zenodo.5833853
+
+
```

### Comparing `ctaplot-0.6.2/ctaplot.egg-info/SOURCES.txt` & `ctaplot-0.6.3/ctaplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/setup.py` & `ctaplot-0.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     ],
     tests_require=['pytest'],
     classifiers=[
         'Intended Audience :: Science/Research',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Astronomy',
     ],
-    data_files=[('ctaplot', dataset)],
+    data_files=[('ctaplot', dataset), ],
+    package_data={'': ['license.rst']},
     entry_points={
         'console_scripts': [
             'gammaboard = ctaplot.gammaboard:open_dashboard'
         ]
     }
 )
```

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-North-20deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-20deg/CTA-Performance-prod3b-v1-South-20deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-North-40deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v1-40deg/CTA-Performance-prod3b-v1-South-40deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-North-20deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-20deg/CTA-Performance-prod3b-v2-South-20deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-North-40deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-40deg/CTA-Performance-prod3b-v2-South-40deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-North-60deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-05h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-30m-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-Angres.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-Angres.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-BackgroundSqdeg.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-BackgroundSqdeg.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-DiffSens.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-DiffSens.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffArea.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffArea.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffAreaNoDirectionCut.txt` & `ctaplot-0.6.3/share/CTA_Performance/CTA-Performance-prod3b-v2-60deg/CTA-Performance-prod3b-v2-South-60deg-50h-EffAreaNoDirectionCut.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-AngRes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-AngRes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-ERes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-ERes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-MST-AngRes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-MST-AngRes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-MST-ERes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-MST-ERes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h-MST.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h-MST.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_North-50h.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_North-50h.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-AngRes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-AngRes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-ERes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-ERes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-MST-AngRes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-MST-AngRes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-MST-ERes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-MST-ERes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h-SST-AngRes.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h-SST-AngRes.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/CTA_Requirements/cta_requirements_South-50h.dat` & `ctaplot-0.6.3/share/CTA_Requirements/cta_requirements_South-50h.dat`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Loose_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Loose_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Safe_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Safe_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Std_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Std_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Stereo.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Angular_Resolution_Stereo.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Loose_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Loose_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Safe_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Safe_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Std_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Std_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Effective_Area_Stereo.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Effective_Area_Stereo.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Loose_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Loose_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Safe_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Safe_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Bias_Std_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Bias_Std_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Loose_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Loose_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Safe_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Safe_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Std_Mono.txt` & `ctaplot-0.6.3/share/HESSII_Impact/HESS_Impact_Energy_Resolution_Std_Mono.txt`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/gammaboard.gif` & `ctaplot-0.6.3/share/gammaboard.gif`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/iact_sensitivities/magic_sensitivity_2014.ecsv` & `ctaplot-0.6.3/share/iact_sensitivities/magic_sensitivity_2014.ecsv`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/images/CTA_angular_resolution.png` & `ctaplot-0.6.3/share/images/CTA_angular_resolution.png`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/images/CTA_effective_area.png` & `ctaplot-0.6.3/share/images/CTA_effective_area.png`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/images/CTA_energy_resolution.png` & `ctaplot-0.6.3/share/images/CTA_energy_resolution.png`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/images/CTA_sensitivity.png` & `ctaplot-0.6.3/share/images/CTA_sensitivity.png`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/simu_mc/gamma_20deg_0deg_cta-prod3-LaPalma_run_header.json` & `ctaplot-0.6.3/share/simu_mc/gamma_20deg_0deg_cta-prod3-LaPalma_run_header.json`

 * *Files identical despite different names*

### Comparing `ctaplot-0.6.2/share/simu_mc/gamma_20deg_0deg_cta-prod3_Paranal_run_header.json` & `ctaplot-0.6.3/share/simu_mc/gamma_20deg_0deg_cta-prod3_Paranal_run_header.json`

 * *Files identical despite different names*

