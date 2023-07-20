# Comparing `tmp/entsoe-py-0.5.8.tar.gz` & `tmp/entsoe-py-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/entsoe-py/entsoe-py/dist/tmplgwv86o9/entsoe-py-0.5.8.tar", last modified: Sun Aug 21 15:19:44 2022, max compression
+gzip compressed data, was "/home/runner/work/entsoe-py/entsoe-py/dist/.tmp-lmt22jvw/entsoe-py-0.5.9.tar", last modified: Tue Nov 29 14:07:02 2022, max compression
```

## Comparing `entsoe-py-0.5.8.tar` & `entsoe-py-0.5.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      112 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9420 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     8782 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe/
--rw-r--r--   0 runner    (1001) docker     (116)       96 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4611 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/decorators.py
--rw-r--r--   0 runner    (1001) docker     (116)    67567 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/entsoe.py
--rw-r--r--   0 runner    (1001) docker     (116)      250 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe/geo/
--rw-r--r--   0 runner    (1001) docker     (116)       29 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe/geo/geojson/
--rw-r--r--   0 runner    (1001) docker     (116)    47525 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/AT.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    27680 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/BE.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    38425 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/BG.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    32133 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/CH.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    40228 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/CZ.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   133011 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/DE_LU.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    65781 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/DK_1.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    27249 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/DK_2.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    45888 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/EE.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   110461 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/ES.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   141232 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/FI.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   158622 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/FR.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   267088 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/GR.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   102548 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/HR.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    36985 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/HU.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    13255 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_CALA.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    50809 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_CNOR.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    43645 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_CNOR_2020.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    52052 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_CSUD.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    44885 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_CSUD_2020.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    67852 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_NORD.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    30130 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_SARD.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    15873 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_SICI.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    34209 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_SUD.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    37133 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/IT_SUD_2020.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    24634 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/LT.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    23806 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/LV.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    33960 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/NL.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   773550 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/NO_1.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   217427 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/NO_2.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   221446 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/NO_3.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   702723 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/NO_4.geojson
--rw-r--r--   0 runner    (1001) docker     (116)   440492 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/NO_5.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    58106 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/PL.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    39787 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/PT.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    52241 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/RO.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    40937 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/RS.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    42877 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/SE_1.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    40138 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/SE_2.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    96287 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/SE_3.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    26450 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/SE_4.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    22802 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/SI.geojson
--rw-r--r--   0 runner    (1001) docker     (116)    25103 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/geojson/SK.geojson
--rw-r--r--   0 runner    (1001) docker     (116)     1928 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/geo/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)    18340 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/mappings.py
--rw-r--r--   0 runner    (1001) docker     (116)     1977 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)    27832 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1234 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/entsoe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9420 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1796 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       43 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/entsoe_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       43 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2022-08-21 15:19:44.000000 entsoe-py-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2369 2022-08-21 15:19:36.000000 entsoe-py-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      112 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     9420 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     8782 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe/
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4611 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (116)    67768 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/entsoe.py
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe/geo/
+-rw-r--r--   0 runner    (1001) docker     (116)       29 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe/geo/geojson/
+-rw-r--r--   0 runner    (1001) docker     (116)    47525 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/AT.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    27680 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/BE.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    38425 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/BG.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    32133 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/CH.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    40228 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/CZ.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   133011 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/DE_LU.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    65781 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/DK_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    27249 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/DK_2.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    45888 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/EE.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   110461 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/ES.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   141232 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/FI.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   158622 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/FR.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   267088 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/GR.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   102548 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/HR.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    36985 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/HU.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    13255 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_CALA.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    50809 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_CNOR.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    43645 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_CNOR_2020.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    52052 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_CSUD.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    44885 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_CSUD_2020.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    67852 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_NORD.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    30130 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_SARD.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    15873 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_SICI.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    34209 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_SUD.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    37133 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/IT_SUD_2020.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    24634 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/LT.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    23806 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/LV.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    33960 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/NL.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   773550 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/NO_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   217427 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/NO_2.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   221446 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/NO_3.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   702723 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/NO_4.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)   440492 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/NO_5.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    58106 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/PL.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    39787 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/PT.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    52241 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/RO.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    40937 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/RS.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    42877 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/SE_1.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    40138 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/SE_2.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    96287 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/SE_3.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    26450 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/SE_4.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    22802 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/SI.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)    25103 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/geojson/SK.geojson
+-rw-r--r--   0 runner    (1001) docker     (116)     1928 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/geo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)    18651 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1977 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/misc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    27851 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1246 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/entsoe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     9420 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1796 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        7 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/entsoe_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       43 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       79 2022-11-29 14:07:02.000000 entsoe-py-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2369 2022-11-29 14:06:50.000000 entsoe-py-0.5.9/setup.py
```

### Comparing `entsoe-py-0.5.8/LICENSE` & `entsoe-py-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/PKG-INFO` & `entsoe-py-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entsoe-py
-Version: 0.5.8
+Version: 0.5.9
 Summary: A python API wrapper for ENTSO-E
 Home-page: https://github.com/EnergieID/entsoe-py
 Author: EnergieID.be, Frank Boerman
 Author-email: jan@energieid.be, frank@fboerman.nl
 License: MIT
 Keywords: ENTSO-E data api energy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `entsoe-py-0.5.8/README.md` & `entsoe-py-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/decorators.py` & `entsoe-py-0.5.9/entsoe/decorators.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/entsoe.py` & `entsoe-py-0.5.9/entsoe/entsoe.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     parse_water_hydro
 from .decorators import retry, paginated, year_limited, day_limited, documents_limited
 import warnings
 
 warnings.filterwarnings('ignore', category=XMLParsedAsHTMLWarning)
 
 __title__ = "entsoe-py"
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 __author__ = "EnergieID.be, Frank Boerman"
 __license__ = "MIT"
 
 URL = 'https://web-api.tp.entsoe.eu/api'
 
 
 class EntsoeRawClient:
@@ -147,15 +147,15 @@
         Returns
         -------
         str
         """
         if dtm.tzinfo is not None and dtm.tzinfo != pytz.UTC:
             dtm = dtm.tz_convert("UTC")
         fmt = '%Y%m%d%H00'
-        ret_str = dtm.strftime(fmt)
+        ret_str = dtm.round(freq='h').strftime(fmt)
         return ret_str
 
     def query_day_ahead_prices(self, country_code: Union[Area, str],
                                start: pd.Timestamp, end: pd.Timestamp) -> str:
         """
         Parameters
         ----------
@@ -171,15 +171,15 @@
         params = {
             'documentType': 'A44',
             'in_Domain': area.code,
             'out_Domain': area.code
         }
         response = self._base_request(params=params, start=start, end=end)
         return response.text
-    
+
     def query_net_position(self, country_code: Union[Area, str],
                            start: pd.Timestamp, end: pd.Timestamp, dayahead: bool = True) -> str:
         """
         Parameters
         ----------
         country_code : Area|str
         start : pd.Timestamp
@@ -566,15 +566,15 @@
         -------
         str
         """
         return self._query_crossborder(
             country_code_from=country_code_from,
             country_code_to=country_code_to, start=start, end=end,
             doctype="A61", contract_marketagreement_type="A04")
-    
+
     def query_intraday_offered_capacity(
         self, country_code_from: Union[Area, str],
             country_code_to: Union[Area, str], start: pd.Timestamp,
             end: pd.Timestamp, implicit:bool = True,**kwargs) -> str:
         """
         Parameters
         ----------
@@ -631,15 +631,15 @@
     def _query_crossborder(
             self, country_code_from: Union[Area, str],
             country_code_to: Union[Area, str], start: pd.Timestamp,
             end: pd.Timestamp, doctype: str,
             contract_marketagreement_type: Optional[str] = None,
             auction_type: Optional[str] = None, business_type: Optional[str] = None) -> str:
         """
-        Generic function called by query_crossborder_flows, 
+        Generic function called by query_crossborder_flows,
         query_scheduled_exchanges, query_net_transfer_capacity_DA/WA/MA/YA and query_.
 
         Parameters
         ----------
         country_code_from : Area|str
         country_code_to : Area|str
         start : pd.Timestamp
@@ -757,15 +757,15 @@
         if type_marketagreement_type:
             params.update({'type_MarketAgreement.Type': type_marketagreement_type})
         response = self._base_request(params=params, start=start, end=end)
         return response.content
 
     def query_activated_balancing_energy(
             self, country_code: Union[Area, str], start: pd.Timestamp,
-            end: pd.Timestamp, business_type: str, 
+            end: pd.Timestamp, business_type: str,
             psr_type: Optional[str] = None) -> bytes:
         """
         Activated Balancing Energy [17.1.E]
         Parameters
         ----------
         country_code : Area|str
         start : pd.Timestamp
@@ -1048,29 +1048,30 @@
         return series
 
     @year_limited
     def query_day_ahead_prices(
             self, country_code: Union[Area, str],
             start: pd.Timestamp,
             end: pd.Timestamp,
-            resolution: List[Literal['60T', '15T']] = '60T') -> pd.Series:
+            resolution: List[Literal['60T', '30T', '15T']] = '60T') -> pd.Series:
         """
         Parameters
         ----------
-        resolution: either 60T for hourly values or 15T for quarterly values, throws error if type is not available
+        resolution: either 60T for hourly values, 
+            30T for half-hourly values or 15T for quarterly values, throws error if type is not available
         country_code : Area|str
         start : pd.Timestamp
         end : pd.Timestamp
 
         Returns
         -------
         pd.Series
         """
-        if resolution not in ['60T', '15T']:
-            raise InvalidParameterError('Please choose either 60T or 15T')
+        if resolution not in ['60T', '30T', '15T']:
+            raise InvalidParameterError('Please choose either 60T, 30T or 15T')
         area = lookup_area(country_code)
         # we do here extra days at start and end to fix issue 187
         text = super(EntsoePandasClient, self).query_day_ahead_prices(
             country_code=area,
             start=start-pd.Timedelta(days=1),
             end=end+pd.Timedelta(days=1)
         )
@@ -1459,15 +1460,15 @@
             country_code_to=area_to,
             start=start,
             end=end)
         ts = parse_crossborder_flows(text)
         ts = ts.tz_convert(area_from.tz)
         ts = ts.truncate(before=start, after=end)
         return ts
-    
+
     @year_limited
     def query_net_transfer_capacity_yearahead(
             self, country_code_from: Union[Area, str],
             country_code_to: Union[Area, str], start: pd.Timestamp,
             end: pd.Timestamp, **kwargs) -> pd.Series:
         """
         Note: Result will be in the timezone of the origin country
@@ -1567,15 +1568,15 @@
             contract_marketagreement_type=contract_marketagreement_type,
             implicit=implicit,
             offset=offset)
         ts = parse_crossborder_flows(text)
         ts = ts.tz_convert(area_from.tz)
         ts = ts.truncate(before=start, after=end)
         return ts
-    
+
     @year_limited
     def query_imbalance_prices(
             self, country_code: Union[Area, str], start: pd.Timestamp,
             end: pd.Timestamp, psr_type: Optional[str] = None) -> pd.DataFrame:
         """
         Parameters
         ----------
@@ -1655,15 +1656,15 @@
         df = df.tz_convert(area.tz)
         df = df.truncate(before=start, after=end)
         return df
 
     @year_limited
     def query_activated_balancing_energy(
             self, country_code: Union[Area, str], start: pd.Timestamp,
-            end: pd.Timestamp, business_type: str, 
+            end: pd.Timestamp, business_type: str,
             psr_type: Optional[str] = None) -> pd.DataFrame:
         """
         Activated Balancing Energy [17.1.E]
         Parameters
         ----------
         country_code : Area|str
         start : pd.Timestamp
@@ -1675,21 +1676,21 @@
 
         Returns
         -------
         pd.DataFrame
         """
         area = lookup_area(country_code)
         text = super(EntsoePandasClient, self).query_activated_balancing_energy(
-            country_code=area, start=start, end=end, 
+            country_code=area, start=start, end=end,
             business_type=business_type, psr_type=psr_type)
         df = parse_contracted_reserve(text, area.tz, "quantity")
         df = df.tz_convert(area.tz)
         df = df.truncate(before=start, after=end)
         return df
-    
+
     @year_limited
     @paginated
     @documents_limited(100)
     def query_contracted_reserve_prices(
             self,
             country_code: Union[Area, str],
             type_marketagreement_type: str,
@@ -1934,14 +1935,17 @@
             country_code=area, start=start, end=end, psr_type=psr_type)
         df = parse_generation(text, per_plant=True, include_eic=include_eic)
         df.columns = df.columns.set_levels(df.columns.levels[0].str.encode('latin-1').str.decode('utf-8'), level=0)
         df = df.tz_convert(area.tz)
         # Truncation will fail if data is not sorted along the index in rare
         # cases. Ensure the dataframe is sorted:
         df = df.sort_index(axis=0)
+
+        if df.columns.nlevels == 2:
+            df = df.assign(newlevel='Actual Aggregated').set_index('newlevel', append=True).unstack('newlevel')
         df = df.truncate(before=start, after=end)
         return df
 
     def query_import(self, country_code: Union[Area, str], start: pd.Timestamp,
                      end: pd.Timestamp) -> pd.DataFrame:
         """
         Adds together all incoming cross-border flows to a country
```

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/AT.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/AT.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/BE.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/BE.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/BG.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/BG.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/CH.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/CH.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/CZ.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/CZ.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/DE_LU.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/DE_LU.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/DK_1.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/DK_1.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/DK_2.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/DK_2.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/EE.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/EE.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/ES.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/ES.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/FI.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/FI.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/FR.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/FR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/GR.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/GR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/HR.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/HR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/HU.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/HU.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_CALA.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_CALA.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_CNOR.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_CNOR.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_CNOR_2020.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_CNOR_2020.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_CSUD.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_CSUD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_CSUD_2020.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_CSUD_2020.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_NORD.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_NORD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_SARD.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_SARD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_SICI.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_SICI.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_SUD.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_SUD.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/IT_SUD_2020.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/IT_SUD_2020.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/LT.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/LT.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/LV.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/LV.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/NL.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/NL.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/NO_1.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/NO_1.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/NO_2.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/NO_2.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/NO_3.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/NO_3.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/NO_4.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/NO_4.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/NO_5.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/NO_5.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/PL.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/PL.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/PT.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/PT.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/RO.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/RO.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/RS.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/RS.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/SE_1.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/SE_1.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/SE_2.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/SE_2.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/SE_3.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/SE_3.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/SE_4.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/SE_4.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/SI.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/SI.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/geojson/SK.geojson` & `entsoe-py-0.5.9/entsoe/geo/geojson/SK.geojson`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/geo/utils.py` & `entsoe-py-0.5.9/entsoe/geo/utils.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/mappings.py` & `entsoe-py-0.5.9/entsoe/mappings.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     CWE =           '10YDOM-REGION-1V', 'CWE Region',                                   'Europe/Brussels',
     CY =            '10YCY-1001A0003J', 'Cyprus, Cyprus TSO BZ / CA / MBA',             'Asia/Nicosia',
     CZ =            '10YCZ-CEPS-----N', 'Czech Republic, CEPS BZ / CA/ MBA',            'Europe/Prague',
     DE_AT_LU =      '10Y1001A1001A63L', 'DE-AT-LU BZ',                                  'Europe/Berlin',
     DE_LU =         '10Y1001A1001A82H', 'DE-LU BZ / MBA',                               'Europe/Berlin',
     DK =            '10Y1001A1001A65H', 'Denmark',                                      'Europe/Copenhagen',
     DK_1 =          '10YDK-1--------W', 'DK1 BZ / MBA',                                 'Europe/Copenhagen',
+    DK_1_NO_1 =     '46Y000000000007M', 'DK1 NO1 BZ',                                   'Europe/Copenhagen',
     DK_2 =          '10YDK-2--------M', 'DK2 BZ / MBA',                                 'Europe/Copenhagen',
     DK_CA =         '10Y1001A1001A796', 'Denmark, Energinet CA',                        'Europe/Copenhagen',
     EE =            '10Y1001A1001A39I', 'Estonia, Elering BZ / CA / MBA',               'Europe/Tallinn',
     FI =            '10YFI-1--------U', 'Finland, Fingrid BZ / CA / MBA',               'Europe/Helsinki',
     MK =            '10YMK-MEPSO----8', 'Former Yugoslav Republic of Macedonia, MEPSO BZ / CA / MBA', 'Europe/Skopje',
     FR =            '10YFR-RTE------C', 'France, RTE BZ / CA / MBA',                    'Europe/Paris',
     DE =            '10Y1001A1001A83F', 'Germany',                                      'Europe/Berlin'
@@ -106,16 +107,18 @@
     GB =            '10YGB----------A', 'National Grid BZ / CA/ MBA',                   'Europe/London',
     GB_IFA =        '10Y1001C--00098F', 'GB(IFA) BZN',                                  'Europe/London',
     GB_IFA2 =       '17Y0000009369493', 'GB(IFA2) BZ',                                  'Europe/London',
     GB_ELECLINK =   '11Y0-0000-0265-K', 'GB(ElecLink) BZN',                             'Europe/London',
     UK =            '10Y1001A1001A92E', 'United Kingdom',                               'Europe/London',
     NL =            '10YNL----------L', 'Netherlands, TenneT NL BZ / CA/ MBA',          'Europe/Amsterdam',
     NO_1 =          '10YNO-1--------2', 'NO1 BZ / MBA',                                 'Europe/Oslo',
+    NO_1A =         '10Y1001A1001A64J', 'NO1 A BZ',                                     'Europe/Oslo',
     NO_2 =          '10YNO-2--------T', 'NO2 BZ / MBA',                                 'Europe/Oslo',
-    NO_2_NSL =      '50Y0JVU59B4JWQCU', 'NO2 NSL BZ / MBA',                                 'Europe/Oslo',
+    NO_2_NSL =      '50Y0JVU59B4JWQCU', 'NO2 NSL BZ / MBA',                             'Europe/Oslo',
+    NO_2A =         '10Y1001C--001219', 'NO2 A BZ',                                     'Europe/Oslo',
     NO_3 =          '10YNO-3--------J', 'NO3 BZ / MBA',                                 'Europe/Oslo',
     NO_4 =          '10YNO-4--------9', 'NO4 BZ / MBA',                                 'Europe/Oslo',
     NO_5 =          '10Y1001A1001A48H', 'NO5 BZ / MBA',                                 'Europe/Oslo',
     NO =            '10YNO-0--------C', 'Norway, Norway MBA, Stattnet CA',              'Europe/Oslo',
     PL_CZ =         '10YDOM-1001A082L', 'PL-CZ BZA / CA',                               'Europe/Warsaw',
     PL =            '10YPL-AREA-----S', 'Poland, PSE SA BZ / BZA / CA / MBA',           'Europe/Warsaw',
     PT =            '10YPT-REN------W', 'Portugal, REN BZ / CA / MBA',                  'Europe/Lisbon',
```

### Comparing `entsoe-py-0.5.8/entsoe/misc.py` & `entsoe-py-0.5.9/entsoe/misc.py`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/entsoe/parsers.py` & `entsoe-py-0.5.9/entsoe/parsers.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
     Returns
     -------
     pd.Series
     """
     series = {
         '15T': [],
+        '30T': [],
         '60T': []
     }
     for soup in _extract_timeseries(xml_text):
         soup_series = _parse_price_timeseries(soup)
         series[soup_series.index.freqstr].append(soup_series)
 
     for freq, freq_series in series.items():
```

### Comparing `entsoe-py-0.5.8/entsoe/utils.py` & `entsoe-py-0.5.9/entsoe/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # tries to grab all mapping codes from the website and check them against the ones we already know
 def check_new_area_codes():
     # grab the docs page
     r = requests.get('https://transparency.entsoe.eu/content/static_content/Static%20content/web%20api/Guide.html')
     soup = BeautifulSoup(r.text, 'lxml')
     # to select the correct table find a known code and go to the parent table of that cell
     rows = soup.find('p', text='10YNL----------L').parent.parent.parent.find_all('tr')
-    table_area_codes = [[x.text for x in y.find_all('td')] for y in rows]
+    table_area_codes = [[x.text.strip('\n') for x in y.find_all('td')] for y in rows]
     # remove the header row
     del table_area_codes[0]
 
     # grab all codes of our mapping
     mapped_codes = set([x.value for x in Area])
     # grab all codes from the docs
     docs_codes = set([x[0] for x in table_area_codes])
```

### Comparing `entsoe-py-0.5.8/entsoe_py.egg-info/PKG-INFO` & `entsoe-py-0.5.9/entsoe_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entsoe-py
-Version: 0.5.8
+Version: 0.5.9
 Summary: A python API wrapper for ENTSO-E
 Home-page: https://github.com/EnergieID/entsoe-py
 Author: EnergieID.be, Frank Boerman
 Author-email: jan@energieid.be, frank@fboerman.nl
 License: MIT
 Keywords: ENTSO-E data api energy
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `entsoe-py-0.5.8/entsoe_py.egg-info/SOURCES.txt` & `entsoe-py-0.5.9/entsoe_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `entsoe-py-0.5.8/setup.py` & `entsoe-py-0.5.9/setup.py`

 * *Files identical despite different names*

