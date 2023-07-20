# Comparing `tmp/joseki-2.2.0.tar.gz` & `tmp/joseki-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joseki-2.2.0.tar", last modified: Tue Jul 18 07:38:20 2023, max compression
+gzip compressed data, was "joseki-2.3.0.tar", last modified: Thu Jul 20 12:59:04 2023, max compression
```

## Comparing `joseki-2.2.0.tar` & `joseki-2.3.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
--rw-r--r--   0        0        0     1075 2023-07-18 07:37:59.771823 joseki-2.2.0/LICENSE
--rw-r--r--   0        0        0     2042 2023-07-18 07:37:59.771823 joseki-2.2.0/README.md
--rw-r--r--   0        0        0     1813 2023-07-18 07:37:59.775823 joseki-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      401 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/__init__.py
--rw-r--r--   0        0        0     3769 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/__main__.py
--rw-r--r--   0        0        0       22 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/__version__.py
--rw-r--r--   0        0        0    15568 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/accessor.py
--rw-r--r--   0        0        0     1741 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/constants.py
--rw-r--r--   0        0        0     2899 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/core.py
--rw-r--r--   0        0        0       92 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/README.md
--rw-r--r--   0        0        0       22 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/__init__.py
--rw-r--r--   0        0        0      396 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/README.md
--rw-r--r--   0        0        0       84 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/__init__.py
--rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1a.csv
--rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1b.csv
--rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1c.csv
--rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1d.csv
--rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1e.csv
--rw-r--r--   0        0        0     3871 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_1f.csv
--rw-r--r--   0        0        0     3422 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2a.csv
--rw-r--r--   0        0        0     3423 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2b.csv
--rw-r--r--   0        0        0     3426 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2c.csv
--rw-r--r--   0        0        0     3429 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/afgl_1986/table_2d.csv
--rw-r--r--   0        0        0      151 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/ecmwf/README.md
--rw-r--r--   0        0        0     4542 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/ecmwf/model_levels_60.csv
--rw-r--r--   0        0        0     1788 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/README.md
--rw-r--r--   0        0        0       93 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/__init__.py
--rw-r--r--   0        0        0     5683 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/extra.atm
--rw-r--r--   0        0        0    42274 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_day.atm
--rw-r--r--   0        0        0    42276 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_night.atm
--rw-r--r--   0        0        0    42270 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/polar_summer.atm
--rw-r--r--   0        0        0    42270 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/polar_winter.atm
--rw-r--r--   0        0        0    42270 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/data/mipas_2007/tropical.atm
--rw-r--r--   0        0        0      789 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/profiles/__init__.py
--rw-r--r--   0        0        0    13295 2023-07-18 07:37:59.775823 joseki-2.2.0/src/joseki/profiles/afgl_1986.py
--rw-r--r--   0        0        0    27398 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/cams.py
--rw-r--r--   0        0        0    13343 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/core.py
--rw-r--r--   0        0        0     1921 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/factory.py
--rw-r--r--   0        0        0    11728 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/mipas_2007.py
--rw-r--r--   0        0        0    10466 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/schema.py
--rw-r--r--   0        0        0     2887 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/ussa_1976.py
--rw-r--r--   0        0        0     4404 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/profiles/util.py
--rw-r--r--   0        0        0      393 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/tests_util.py
--rw-r--r--   0        0        0     3325 2023-07-18 07:37:59.779823 joseki-2.2.0/src/joseki/units.py
--rw-r--r--   0        0        0       41 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2168 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc
--rw-r--r--   0        0        0    11316 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip
--rw-r--r--   0        0        0    54028 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc
--rw-r--r--   0        0        0     1496 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc
--rw-r--r--   0        0        0    55752 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip
--rw-r--r--   0        0        0     2046 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/README.md
--rw-r--r--   0        0        0        0 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/data/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/__init__.py
--rw-r--r--   0        0        0     1556 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_afgl_1986.py
--rw-r--r--   0        0        0     7227 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_cams.py
--rw-r--r--   0        0        0     7018 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_core.py
--rw-r--r--   0        0        0      160 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_factory.py
--rw-r--r--   0        0        0     6159 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_mipas_2007.py
--rw-r--r--   0        0        0      233 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_ussa_1976.py
--rw-r--r--   0        0        0      767 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/profiles/test_util.py
--rw-r--r--   0        0        0     7066 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_accessor.py
--rw-r--r--   0        0        0     4582 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_core.py
--rw-r--r--   0        0        0     2918 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_main.py
--rw-r--r--   0        0        0     1972 2023-07-18 07:37:59.779823 joseki-2.2.0/tests/test_units.py
--rw-r--r--   0        0        0     2754 1970-01-01 00:00:00.000000 joseki-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-20 12:58:45.952765 joseki-2.3.0/LICENSE
+-rw-r--r--   0        0        0     2048 2023-07-20 12:58:45.952765 joseki-2.3.0/README.md
+-rw-r--r--   0        0        0     1813 2023-07-20 12:58:45.960763 joseki-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      421 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/__init__.py
+-rw-r--r--   0        0        0     3769 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/__main__.py
+-rw-r--r--   0        0        0       22 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/__version__.py
+-rw-r--r--   0        0        0    15568 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/accessor.py
+-rw-r--r--   0        0        0     1741 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/constants.py
+-rw-r--r--   0        0        0     5034 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/core.py
+-rw-r--r--   0        0        0       92 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/README.md
+-rw-r--r--   0        0        0       22 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/README.md
+-rw-r--r--   0        0        0       84 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/__init__.py
+-rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1a.csv
+-rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1b.csv
+-rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1c.csv
+-rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1d.csv
+-rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1e.csv
+-rw-r--r--   0        0        0     3871 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_1f.csv
+-rw-r--r--   0        0        0     3422 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2a.csv
+-rw-r--r--   0        0        0     3423 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2b.csv
+-rw-r--r--   0        0        0     3426 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2c.csv
+-rw-r--r--   0        0        0     3429 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/afgl_1986/table_2d.csv
+-rw-r--r--   0        0        0      151 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/ecmwf/README.md
+-rw-r--r--   0        0        0     4542 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/ecmwf/model_levels_60.csv
+-rw-r--r--   0        0        0     1788 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/README.md
+-rw-r--r--   0        0        0       93 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/__init__.py
+-rw-r--r--   0        0        0     5683 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/extra.atm
+-rw-r--r--   0        0        0    42274 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_day.atm
+-rw-r--r--   0        0        0    42276 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_night.atm
+-rw-r--r--   0        0        0    42270 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/polar_summer.atm
+-rw-r--r--   0        0        0    42270 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/polar_winter.atm
+-rw-r--r--   0        0        0    42270 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/data/mipas_2007/tropical.atm
+-rw-r--r--   0        0        0      789 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/__init__.py
+-rw-r--r--   0        0        0    13295 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/afgl_1986.py
+-rw-r--r--   0        0        0    27728 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/cams.py
+-rw-r--r--   0        0        0    13343 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/core.py
+-rw-r--r--   0        0        0     1921 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/factory.py
+-rw-r--r--   0        0        0    11728 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/mipas_2007.py
+-rw-r--r--   0        0        0    10466 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/schema.py
+-rw-r--r--   0        0        0     2887 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/ussa_1976.py
+-rw-r--r--   0        0        0     4404 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/profiles/util.py
+-rw-r--r--   0        0        0      393 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/tests_util.py
+-rw-r--r--   0        0        0     3325 2023-07-20 12:58:45.960763 joseki-2.3.0/src/joseki/units.py
+-rw-r--r--   0        0        0       41 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2168 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc
+-rw-r--r--   0        0        0    11316 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip
+-rw-r--r--   0        0        0    56340 2023-07-20 12:58:45.960763 joseki-2.3.0/tests/data/774f1fd2-63c5-4b59-b23d-eadcad7d6b83.zip
+-rw-r--r--   0        0        0    29668 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/86dbfcd6-9e0b-40df-8ea7-aa2e328339dc.zip
+-rw-r--r--   0        0        0    54028 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc
+-rw-r--r--   0        0        0     1496 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc
+-rw-r--r--   0        0        0    55752 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip
+-rw-r--r--   0        0        0     3617 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/__init__.py
+-rw-r--r--   0        0        0     1556 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_afgl_1986.py
+-rw-r--r--   0        0        0     7227 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_cams.py
+-rw-r--r--   0        0        0     7023 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_core.py
+-rw-r--r--   0        0        0      160 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_factory.py
+-rw-r--r--   0        0        0     6159 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_mipas_2007.py
+-rw-r--r--   0        0        0      233 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_ussa_1976.py
+-rw-r--r--   0        0        0      767 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/profiles/test_util.py
+-rw-r--r--   0        0        0     7066 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_accessor.py
+-rw-r--r--   0        0        0     4832 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_core.py
+-rw-r--r--   0        0        0     2918 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_main.py
+-rw-r--r--   0        0        0     1972 2023-07-20 12:58:45.964763 joseki-2.3.0/tests/test_units.py
+-rw-r--r--   0        0        0     2760 1970-01-01 00:00:00.000000 joseki-2.3.0/PKG-INFO
```

### Comparing `joseki-2.2.0/LICENSE` & `joseki-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/README.md` & `joseki-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 ```shell
 conda install -c conda-forge joseki
 ```
 
 ## Documentation
 
-Visit https://nollety.github.io/joseki/.
+Visit https://nollety.github.io/joseki/latest.
 
 ## Ikigai
 
 *Joseki* was born in the context of the development of the 
 [Eradiate](https://github.com/eradiate/eradiate) radiative transfer model, from
 the need to collect, document and trace, integrate and modify *popular* 
 thermophysical profiles.
```

### Comparing `joseki-2.2.0/pyproject.toml` & `joseki-2.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "xarray>=2022.12.0",
     "ussa1976>=0.3.4",
     "attrs>=22.2.0",
     "importlib-resources>=5.10.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-version = "2.2.0"
+version = "2.3.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Changelog = "https://github.com/nollety/joseki/blob/main/docs/changelog.md"
 homepage = "https://github.com/nollety/joseki"
```

### Comparing `joseki-2.2.0/src/joseki/__main__.py` & `joseki-2.3.0/src/joseki/__main__.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/accessor.py` & `joseki-2.3.0/src/joseki/accessor.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/constants.py` & `joseki-2.3.0/src/joseki/constants.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_1a.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_1a.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_1b.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_1b.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_1c.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_1c.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_1d.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_1d.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_1e.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_1e.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_1f.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_1f.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_2a.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_2a.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_2b.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_2b.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_2c.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_2c.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/afgl_1986/table_2d.csv` & `joseki-2.3.0/src/joseki/data/afgl_1986/table_2d.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/ecmwf/model_levels_60.csv` & `joseki-2.3.0/src/joseki/data/ecmwf/model_levels_60.csv`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/README.md` & `joseki-2.3.0/src/joseki/data/mipas_2007/README.md`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/extra.atm` & `joseki-2.3.0/src/joseki/data/mipas_2007/extra.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_day.atm` & `joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_day.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/midlatitude_night.atm` & `joseki-2.3.0/src/joseki/data/mipas_2007/midlatitude_night.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/polar_summer.atm` & `joseki-2.3.0/src/joseki/data/mipas_2007/polar_summer.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/polar_winter.atm` & `joseki-2.3.0/src/joseki/data/mipas_2007/polar_winter.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/data/mipas_2007/tropical.atm` & `joseki-2.3.0/src/joseki/data/mipas_2007/tropical.atm`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/__init__.py` & `joseki-2.3.0/src/joseki/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/afgl_1986.py` & `joseki-2.3.0/src/joseki/profiles/afgl_1986.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/cams.py` & `joseki-2.3.0/src/joseki/profiles/cams.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     lat: float | pint.Quantity,
     lon: float | pint.Quantity,
     molecules: list[str] | None = None,
     missing_molecules_from: xr.Dataset | None = None,
     extrapolate: dict | None = None,
     regularize: bool | dict | None = None,
     extract_dir : Path | None = None,
-    pressure_data : str | None = "model_level_60",
+    pressure_data : str | None = "surface_pressure",
 ) -> xr.Dataset:
     """Convert CAMS reanalysis data to a profile.
 
     Args:
         data: Path to CAMS data archive file or list of paths to CAMS datasets 
             or path to directory where CAMS datasets are located.
         identifier: `'EAC4'` for a *CAMS reanalysis of atmospheric composition* 
@@ -156,19 +156,31 @@
 
     level_dataset, surface_dataset = identify(datasets)
 
     if level_dataset is None:  # pragma: no cover
         raise ValueError("Could not find a multi-level dataset.") 
 
     # Select in time and space
-    selected = select(level_dataset, time, longitude.m, latitude.m)
+    interpolated = interp_time_space(
+        level_dataset,
+        time,
+        longitude.m,
+        latitude.m,
+    )
+
+    pressure_data = "surface_pressure" if pressure_data is None else pressure_data
 
     # Read surface pressure if available
     if surface_dataset is not None:
-        surface_selected = select(surface_dataset, time, longitude.m, latitude.m)
+        surface_selected = interp_time_space(
+            surface_dataset,
+            time,
+            longitude.m,
+            latitude.m,
+        )
         if "sp" in surface_selected:
             surface_pressure = to_quantity(surface_selected["sp"])
         else:
             if pressure_data == "surface_pressure":  # pragma: no cover
                 raise ValueError(
                     "Could not found a 'sp' surface pressure data variable "
                     "in the surface dataset."
@@ -188,15 +200,15 @@
             surface_pressure = None  # pragma: no cover
 
     if surface_pressure is not None:  # pragma: no cover
         logger.info("Surface pressure: %s", f"{surface_pressure:~P}")
 
     # Translate model levels into altitude values (and add pressure data)
     altitude_dataset = model_level_to_altitude(
-        selected,
+        interpolated,
         pressure_data=pressure_data,
         surface_pressure=surface_pressure,
     )
 
     # Create a data structure storing mole fractions
     data = mole_fractions(altitude_dataset)
 
@@ -514,34 +526,41 @@
             level_dataset = dataset
         else:
             surface_dataset = dataset
     
     return level_dataset, surface_dataset
 
 
-def select(
+def interp_time_space(
     ds: xr.Dataset,
     datetime: str | datetime.datetime | np.datetime64,
     lon: float,
     lat: float,
 ):
-    """Select a CAMS dataset at specific datetime, longitude and latitude.
+    """Interpolate a CAMS dataset at specific datetime, longitude and latitude.
     
     Args:
         ds: CAMS Dataset.
         datetime: Datetime.
         lon: Longitude [degrees].
         lat: Latitude [degrees].
 
     Notes:
-        The dataset is selected using the nearest method.
+        The dataset is interpolated using the linear method.
     """
-    _ds = ds.sel(time=datetime, method="nearest", drop=True)
-    _ds = _ds.sel(latitude=lat, longitude=lon, method="nearest", drop=True)
-    return _ds
+    return ds.interp(
+        time=datetime,
+        method="linear",
+        kwargs={"bounds_error": True},
+    ).interp(
+        latitude=lat,
+        longitude=lon,
+        method="linear",
+        kwargs={"bounds_error": True},
+    )
 
 
 def getpath(filename: str) -> Path:
     """
     Get path for data file.
 
     Args:
@@ -766,15 +785,15 @@
         )
     ]
     logger.debug("Opened %d datasets.", len(datasets))
 
     _, surface_dataset = identify(datasets)
 
     # Select in time and space
-    selected = select(surface_dataset, time, longitude.m, latitude.m)
+    selected = interp_time_space(surface_dataset, time, longitude.m, latitude.m)
 
     amount = {}
     for dv in selected.data_vars:
         try:
             m = MOLECULE_TOTALS[dv]
         except KeyError:  # pragma: no cover
             pass
```

### Comparing `joseki-2.2.0/src/joseki/profiles/core.py` & `joseki-2.3.0/src/joseki/profiles/core.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/factory.py` & `joseki-2.3.0/src/joseki/profiles/factory.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/mipas_2007.py` & `joseki-2.3.0/src/joseki/profiles/mipas_2007.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/schema.py` & `joseki-2.3.0/src/joseki/profiles/schema.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/ussa_1976.py` & `joseki-2.3.0/src/joseki/profiles/ussa_1976.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/profiles/util.py` & `joseki-2.3.0/src/joseki/profiles/util.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/src/joseki/units.py` & `joseki-2.3.0/src/joseki/units.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc` & `joseki-2.3.0/tests/data/232f85b4-b3e9-47a7-a52d-9f955c38b9f6.nc`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip` & `joseki-2.3.0/tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc` & `joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_ml.nc`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc` & `joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb/levtype_sfc.nc`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip` & `joseki-2.3.0/tests/data/97da7a58-674a-4a1f-a92b-534cb95d07bb.zip`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/profiles/test_afgl_1986.py` & `joseki-2.3.0/tests/profiles/test_afgl_1986.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/profiles/test_cams.py` & `joseki-2.3.0/tests/profiles/test_cams.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,15 +220,15 @@
         to_paths(42)
 
 def test_from_cams_reanalysis_pressure_data():
     """Surface pressure data is used to rescale the pressure profile."""
     ds = from_cams_reanalysis(
         data="tests/data/25b63a29-3eab-4599-92f4-7bba42ec6add.zip",
         identifier="EAC4",
-        time="2020-04-01T12:00:00",
-        lat=28.0,
-        lon=86.0,
+        time="2021-04-01T12:00:00",
+        lat=27.5,
+        lon=86.5,
         pressure_data="surface_pressure",
     )
 
     surface_pressure = to_quantity(ds.p.isel(z=0))
     assert np.abs(surface_pressure - 1013.25 * ureg.hPa).magnitude > 1.0
```

### Comparing `joseki-2.2.0/tests/profiles/test_core.py` & `joseki-2.3.0/tests/profiles/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,13 +240,13 @@
     assert "H2O" in selected.joseki.molecules
     assert "CO2" in selected.joseki.molecules
     assert "O3" not in selected.joseki.molecules
 
 def test_select_molecules_invalid(test_data_set: xr.Dataset):
     """Raise when selected molecules are not available."""
     molecules = ["SO2", "NO2"]
-    ds = test_data_set.drop([f"x_{m}" for m in molecules])
+    ds = test_data_set.drop_vars([f"x_{m}" for m in molecules])
     with pytest.raises(ValueError):
         select_molecules(
             ds=ds,
             molecules=["H2O", "CO2", "SO2", "NO2"],
         )
```

### Comparing `joseki-2.2.0/tests/profiles/test_mipas_2007.py` & `joseki-2.3.0/tests/profiles/test_mipas_2007.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/profiles/test_util.py` & `joseki-2.3.0/tests/profiles/test_util.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/test_accessor.py` & `joseki-2.3.0/tests/test_accessor.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/test_core.py` & `joseki-2.3.0/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Test cases for the core module."""
 import numpy as np
 import pytest
 import xarray as xr
 from numpy.testing import assert_approx_equal
 
 from joseki import unit_registry as ureg
-from joseki.core import make, open_dataset, load_dataset, identifiers
+from joseki.core import make, open_dataset, load_dataset, merge, identifiers
 
 
 def test_make():
     """Returns xr.Dataset."""
     assert isinstance(make(identifier="afgl_1986-tropical"), xr.Dataset)
 
 
@@ -144,10 +144,16 @@
     """Returns xr.Dataset."""
     ds = make(identifier="afgl_1986-tropical")
     path = tmpdir.join("test.nc")
     ds.to_netcdf(path)
     ds2 = load_dataset(path)
     assert ds2.joseki.is_valid
 
+def test_merge_1():
+    ds1 = make(identifier="afgl_1986-tropical", molecules=["H2O", "CO2"])
+    ds2 = make(identifier="afgl_1986-tropical", molecules=["O3"])
+    ds = merge([ds1, ds2])
+    assert ds.joseki.molecules == ["H2O", "CO2", "O3"]
+
 def test_identifiers():
     """Returns list of identifiers."""
     assert isinstance(identifiers(), list)
```

### Comparing `joseki-2.2.0/tests/test_main.py` & `joseki-2.3.0/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/tests/test_units.py` & `joseki-2.3.0/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `joseki-2.2.0/PKG-INFO` & `joseki-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joseki
-Version: 2.2.0
+Version: 2.3.0
 Summary: Reference atmosphere's thermophysical profiles for radiative transfer applications in Earth's atmosphere.
 License: MIT
 Author-email: Yvan Nollet <yvan.nollet@rayference.eu>
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -62,15 +62,15 @@
 
 ```shell
 conda install -c conda-forge joseki
 ```
 
 ## Documentation
 
-Visit https://nollety.github.io/joseki/.
+Visit https://nollety.github.io/joseki/latest.
 
 ## Ikigai
 
 *Joseki* was born in the context of the development of the 
 [Eradiate](https://github.com/eradiate/eradiate) radiative transfer model, from
 the need to collect, document and trace, integrate and modify *popular* 
 thermophysical profiles.
```

