# Comparing `tmp/OpenFisca-Survey-Manager-1.0.2.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.0.2.tar", last modified: Wed Jul 12 12:01:37 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.1.0.tar", last modified: Thu Jul 20 06:42:36 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.0.2.tar` & `OpenFisca-Survey-Manager-1.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)    17279 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.525532 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-12 12:01:37.000000 OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13360 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     4147 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (122)     8319 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-12 12:01:37.529532 OpenFisca-Survey-Manager-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-07-12 12:01:13.000000 OpenFisca-Survey-Manager-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.333307 OpenFisca-Survey-Manager-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    17676 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.325307 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-20 06:42:36.000000 OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-20 06:42:36.333307 OpenFisca-Survey-Manager-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13360 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.329307 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.329307 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.329307 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.333307 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 06:42:36.333307 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-20 06:42:36.333307 OpenFisca-Survey-Manager-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3197 2023-07-20 06:42:04.000000 OpenFisca-Survey-Manager-1.1.0/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.0.2/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 ﻿# Changelog
 
+### 1.1.0 [#260](https://github.com/openfisca/openfisca-survey-manager/pull/260)
+
+* New features
+
+- Add options in inflate_parameters and inflate_parameter_leaf:
+  - start_update_instant : Instant of the year when the inflation should start, if different from January 1st
+  - round_ndigits : number of digits in the rounded result
+- Adjustment of inflate_parameters to use it with parameter leaf
+
 ### 1.0.2 [#259](https://github.com/openfisca/openfisca-survey-manager/pull/259)
 
 * Technical changes
 - A parameter `config_files_directory` exist but it is not used evrywhere, this PR generalize it.
 - Add tests using this parameter.
 
 ### 1.0.1 [#257](https://github.com/openfisca/openfisca-survey-manager/pull/257)
```

### Comparing `OpenFisca-Survey-Manager-1.0.2/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.1.0/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.1.0/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.0.2
+Version: 1.1.0
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `OpenFisca-Survey-Manager-1.0.2/README.md` & `OpenFisca-Survey-Manager-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/scenarios.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files 21% similar despite different names*

```diff
@@ -80,13 +80,35 @@
             parameters.taxes.social_security_contribution(2016).thresholds
             ):
         assert threshold_2017 == threshold_2016 * 1.3, "{} != {}".format(
             threshold_2017, threshold_2016 * 1.3
             )
 
 
+def test_inflate_start_instant_option():
+    """
+        Test parameters inflator with a specific start_instant
+    """
+    tax_benefit_system = CountryTaxBenefitSystem()
+    parameters = tax_benefit_system.parameters
+    parameters_asof(parameters, instant = periods.instant(2022))  # Remove post 2022 legislation changes
+    inflate_parameters(parameters, inflator = .3, base_year = 2022, last_year = 2023, start_instant="2023-07-01")
+    for (threshold_2023_06, threshold_2023_07, threshold_2022) in zip(
+            parameters.taxes.social_security_contribution('2023-06').thresholds,
+            parameters.taxes.social_security_contribution('2023-07').thresholds,
+            parameters.taxes.social_security_contribution(2022).thresholds
+            ):
+        assert threshold_2023_07 == threshold_2022 * 1.3, "{} != {}".format(
+            threshold_2023_07, threshold_2022 * 1.3
+            )
+        assert threshold_2023_06 == threshold_2022, "{} != {}".format(
+            threshold_2023_06, threshold_2022
+            )
+
+
 if __name__ == '__main__':
     test_inflate_simple_parameter()
     test_inflate_scale()
     test_inflate_scale_with_changing_number_of_brackets()
     test_asof_simple_annual_parameter()
     test_asof_scale_parameters()
+    test_inflate_start_instant_option()
```

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,72 +8,85 @@
 from openfisca_core import periods
 from openfisca_core.parameters import ParameterNode, Scale
 
 
 log = logging.getLogger(__name__)
 
 
-def inflate_parameters(parameters, inflator, base_year, last_year = None, ignore_missing_units = False):
+def inflate_parameters(parameters, inflator, base_year, last_year = None, ignore_missing_units = False,
+                       start_instant = None, round_ndigits = 2):
+    """
+    Inflate a Parameter node or a Parameter lead according for the years between base_year and last_year
+    ::parameters:: af Parameter node or a Parameter leaf
+    ::inflator:: rate used to inflate the parameter. The rate is unique for all the years
+    ::base_year:: base year of the parameter
+    ::last_year::  last year of inflation
+    ::ignore_missing_units:: if True, a parameter leaf without unit in metadata will not be inflate
+    ::start_instant :: Instant of the year when the update should start, if None will be Junuary 1st
+    ::round_ndigits:: Number of digits to keep in the rounded result
+    """
 
     if (last_year is not None) and (last_year > base_year + 1):
-        for year in range(base_year + 1, last_year + 1):
-            inflate_parameters(parameters, inflator, year - 1, last_year = year, ignore_missing_units = ignore_missing_units)
+        for year in range(base_year + 1, last_year + 1):  # For each year we inflate with the same inflator rate. Example : base_year + 1 : paramaters = paramaters * inflator ; base_year + 2 : parameters = parameters * inflator * inflator
+            inflate_parameters(parameters, inflator, year - 1, last_year = year, ignore_missing_units = ignore_missing_units,
+                               start_instant = start_instant, round_ndigits = round_ndigits)
 
     else:
         if last_year is None:
             last_year = base_year + 1
 
         assert last_year == base_year + 1
 
-        for sub_parameter in parameters.children.values():
-            if isinstance(sub_parameter, ParameterNode):
-                inflate_parameters(sub_parameter, inflator, base_year, last_year, ignore_missing_units = ignore_missing_units)
-            else:
-                acceptable_units = [
-                    'rate_unit',
-                    'threshold_unit',
-                    'unit',
-                    ]
-                if ignore_missing_units:
-                    if not hasattr(sub_parameter, 'metadata'):
-                        continue
-                    # Empty intersection: not unit present in metadata
-                    if not bool(set(sub_parameter.metadata.keys()) & set(acceptable_units)):
-                        continue
-
-                assert hasattr(sub_parameter, 'metadata'), "{} doesn't have metadata".format(sub_parameter.name)
-                unit_types = set(sub_parameter.metadata.keys()).intersection(set(acceptable_units))
-                assert unit_types, "No admissible unit in metadata for parameter {}. You may consider using the option 'ignore_missing_units' from the inflate_paramaters() function.".format(
-                    sub_parameter.name)
-                if len(unit_types) > 1:
-                    assert unit_types == set(['threshold_unit', 'rate_unit']), \
-                        "Too much admissible units in metadata for parameter {}".format(
-                            sub_parameter.name)
-                unit_by_type = dict([
-                    (unit_type, sub_parameter.metadata[unit_type]) for unit_type in unit_types
-                    ])
-
-                for unit_type in unit_by_type.keys():
-                    if sub_parameter.metadata[unit_type].startswith("currency"):
-                        inflate_parameter_leaf(sub_parameter, base_year, inflator, unit_type = unit_type)
+        if isinstance(parameters, ParameterNode):
+            for sub_parameter in parameters.children.values():
+                inflate_parameters(sub_parameter, inflator, base_year, last_year, ignore_missing_units = ignore_missing_units,
+                                   start_instant = start_instant, round_ndigits = round_ndigits)
+        else:
+            acceptable_units = [
+                'rate_unit',
+                'threshold_unit',
+                'unit',
+                ]
+            if ignore_missing_units:
+                if not hasattr(parameters, 'metadata'):
+                    return
+                # Empty intersection: not unit present in metadata
+                if not bool(set(parameters.metadata.keys()) & set(acceptable_units)):
+                    return
+            assert hasattr(parameters, 'metadata'), "{} doesn't have metadata".format(parameters.name)
+            unit_types = set(parameters.metadata.keys()).intersection(set(acceptable_units))
+            assert unit_types, "No admissible unit in metadata for parameter {}. You may consider using the option 'ignore_missing_units' from the inflate_paramaters() function.".format(
+                parameters.name)
+            if len(unit_types) > 1:
+                assert unit_types == set(['threshold_unit', 'rate_unit']), \
+                    "Too much admissible units in metadata for parameter {}".format(
+                        parameters.name)
+            unit_by_type = dict([
+                (unit_type, parameters.metadata[unit_type]) for unit_type in unit_types
+                ])
+            for unit_type in unit_by_type.keys():
+                if parameters.metadata[unit_type].startswith("currency"):
+                    inflate_parameter_leaf(parameters, base_year, inflator, unit_type = unit_type, start_instant = start_instant, round_ndigits = round_ndigits)
 
 
-def inflate_parameter_leaf(sub_parameter, base_year, inflator, unit_type = 'unit'):
+def inflate_parameter_leaf(sub_parameter, base_year, inflator, unit_type = 'unit', start_instant = None, round_ndigits = 2):
     """
-    Inflate a Parameter leaf according to unit type
-
-    Basic unit type are supposed by default
-    Other admissible unit types are threshold_unit and rate_unit
+    Inflate a Parameter leaf according to unit type for the year after base_year
+    ::sub_parameter:: af Parameter leaf
+    ::base_year:: base year of the parameter
+    ::inflator:: rate used to inflate the parameter
+    ::unit_type:: unit supposed by default. Other admissible unit types are threshold_unit and rate_unit
+    ::start_instant:: Instant of the year when the update should start, if None will be Junuary 1st
+    ::round_ndigits:: Number of digits to keep in the rounded result
     """
-
     if isinstance(sub_parameter, Scale):
         if unit_type == 'threshold_unit':
             for bracket in sub_parameter.brackets:
                 threshold = bracket.children['threshold']
-                inflate_parameter_leaf(threshold, base_year, inflator)
+                inflate_parameter_leaf(threshold, base_year, inflator, start_instant = start_instant, round_ndigits = round_ndigits)
             return
     else:
         # Remove new values for year > base_year
         kept_instants_str = [
             parameter_at_instant.instant_str
             for parameter_at_instant in sub_parameter.values_list
             if periods.instant(parameter_at_instant.instant_str).year <= base_year
@@ -82,44 +95,56 @@
             return
 
         last_admissible_instant_str = max(kept_instants_str)
         sub_parameter.update(
             start = last_admissible_instant_str,
             value = sub_parameter(last_admissible_instant_str)
             )
-        restricted_to_base_year_value_list = [
-            parameter_at_instant for parameter_at_instant in sub_parameter.values_list
-            if periods.instant(parameter_at_instant.instant_str).year == base_year
-            ]
-        # When value is changed in the base year
-        if restricted_to_base_year_value_list:
-            for parameter_at_instant in reversed(restricted_to_base_year_value_list):
-                if parameter_at_instant.instant_str.startswith(str(base_year)):
-                    value = (
-                        parameter_at_instant.value * (1 + inflator)
-                        if parameter_at_instant.value is not None
-                        else None
-                        )
-                    sub_parameter.update(
-                        start = parameter_at_instant.instant_str.replace(
-                            str(base_year), str(base_year + 1)
-                            ),
-                        value = value,
-                        )
-        # Or use the value at that instant even when it is defined earlier tahn the base year
-        else:
+        if start_instant is not None:
+            assert periods.instant(start_instant).year == (base_year + 1), "Year of start_instant should be base_year + 1"
             value = (
-                sub_parameter("{}-12-31".format(base_year)) * (1 + inflator)
+                round(sub_parameter("{}-12-31".format(base_year)) * (1 + inflator), round_ndigits)
                 if sub_parameter("{}-12-31".format(base_year)) is not None
                 else None
                 )
             sub_parameter.update(
-                start = "{}-01-01".format(base_year + 1),
-                value = value
+                start = start_instant,
+                value = value,
                 )
+        else:
+            restricted_to_base_year_value_list = [
+                parameter_at_instant for parameter_at_instant in sub_parameter.values_list
+                if periods.instant(parameter_at_instant.instant_str).year == base_year
+                ]
+            # When value is changed in the base year
+            if restricted_to_base_year_value_list:
+                for parameter_at_instant in reversed(restricted_to_base_year_value_list):
+                    if parameter_at_instant.instant_str.startswith(str(base_year)):
+                        value = (
+                            round(parameter_at_instant.value * (1 + inflator), round_ndigits)
+                            if parameter_at_instant.value is not None
+                            else None
+                            )
+                        sub_parameter.update(
+                            start = parameter_at_instant.instant_str.replace(
+                                str(base_year), str(base_year + 1)
+                                ),
+                            value = value,
+                            )
+            # Or use the value at that instant even when it is defined earlier tahn the base year
+            else:
+                value = (
+                    round(sub_parameter("{}-12-31".format(base_year)) * (1 + inflator), round_ndigits)
+                    if sub_parameter("{}-12-31".format(base_year)) is not None
+                    else None
+                    )
+                sub_parameter.update(
+                    start = "{}-01-01".format(base_year + 1),
+                    value = value,
+                    )
 
 
 def asof(tax_benefit_system, instant):
     parameters = tax_benefit_system.parameters
     parameters_asof(parameters, instant)
     variables_asof(tax_benefit_system, instant)
```

### Comparing `OpenFisca-Survey-Manager-1.0.2/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.1.0/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/setup.cfg` & `OpenFisca-Survey-Manager-1.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.0.2/setup.py` & `OpenFisca-Survey-Manager-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.0.2',
+    version = '1.1.0',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

