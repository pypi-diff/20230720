# Comparing `tmp/OpenFisca-Survey-Manager-1.1.1.tar.gz` & `tmp/OpenFisca-Survey-Manager-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-Survey-Manager-1.1.1.tar", last modified: Thu Jul 20 09:16:46 2023, max compression
+gzip compressed data, was "OpenFisca-Survey-Manager-1.1.2.tar", last modified: Thu Jul 20 14:42:07 2023, max compression
```

## Comparing `OpenFisca-Survey-Manager-1.1.1.tar` & `OpenFisca-Survey-Manager-1.1.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.374337 OpenFisca-Survey-Manager-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)    18177 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/LICENSE.AGPL.txt
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.366337 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-20 09:16:46.000000 OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    14274 2023-07-20 09:16:46.374337 OpenFisca-Survey-Manager-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    13360 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.370337 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/aggregates.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.370337 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/
--rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
--rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/coicop.py
--rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/google_colab.py
--rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/input_dataframe_generator.py
--rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/read_dbf.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/read_spss.py
--rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/scenarios.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.370337 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/scripts/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/statshelpers.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/survey_collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tables.py
--rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.374337 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 09:16:46.374337 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/data_files/
--rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/data_files/config_template.ini
--rw-r--r--   0 runner    (1001) docker     (122)     3644 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_calmar.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
--rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_legislation_inflator.py
--rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_matching.py
--rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_quantile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_read_sas.py
--rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_scenario.py
--rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_summarize_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_surveys.py
--rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
--rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_top_bottom_share.py
--rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/variables.py
--rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-20 09:16:46.374337 OpenFisca-Survey-Manager-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-20 09:16:19.000000 OpenFisca-Survey-Manager-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    18399 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    34499 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/LICENSE.AGPL.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.640916 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2469 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-20 14:42:07.000000 OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    14346 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    13432 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.644916 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/
+-rw-r--r--   0 runner    (1001) docker     (122)     2129 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17292 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/aggregates.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     3551 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)      451 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_divisions.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    12096 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)     6262 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9929 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3150 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/coicop.py
+-rw-r--r--   0 runner    (1001) docker     (122)      741 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      836 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/google_colab.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13357 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/input_dataframe_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4591 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1386 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_dbf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_spss.py
+-rw-r--r--   0 runner    (1001) docker     (122)    79765 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scenarios.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10047 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11312 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/statshelpers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5365 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/survey_collections.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10119 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9552 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3302 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-20 14:42:07.648917 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/data_files/
+-rw-r--r--   0 runner    (1001) docker     (122)      381 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/data_files/config_template.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     3591 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2457 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_calmar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5223 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_legislation_inflator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      989 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3556 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4373 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_quantile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_read_sas.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13724 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (122)      716 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_summarize_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_surveys.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1671 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_top_bottom_share.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10433 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2850 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-07-20 14:42:07.652917 OpenFisca-Survey-Manager-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3403 2023-07-20 14:41:39.000000 OpenFisca-Survey-Manager-1.1.2/setup.py
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/CHANGELOG.md` & `OpenFisca-Survey-Manager-1.1.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 ﻿# Changelog
 
+### 1.1.2 [#262](https://github.com/openfisca/openfisca-survey-manager/pull/262)
+
+* Technical changes
+  - Remove old `CircleCI` continuous integration configuration
+  - Set `README` CI badge to current `GitHub Actions` CI
+
 ### 1.1.1 [#261](https://github.com/openfisca/openfisca-survey-manager/pull/261)
 
 * Technical changes
   - Fix `Conda build` step in `publish-to-conda` GitHub Actions job  
     - Define `OpenFisca-Survey-Manager` package dependencies once for `PyPI` and `conda`
       - Use `setup.py` general requirement and extra requirements for `conda` package
       - Adapt `tables` library name to `pytables` for `conda`
@@ -13,15 +19,14 @@
 
 * New features
 - Add options in inflate_parameters and inflate_parameter_leaf:
   - `start_update_instant` : Instant of the year when the inflation should start, if different from January 1st
   - `round_ndigits` : number of digits in the rounded result
 - Adjustment of inflate_parameters to use it with parameter leaf
 
-
 ### 1.0.2 [#259](https://github.com/openfisca/openfisca-survey-manager/pull/259)
 
 * Technical changes
   - A parameter `config_files_directory` exist but it is not used evrywhere, this PR generalize it.
   - Add tests using this parameter.
 
 ### 1.0.1 [#257](https://github.com/openfisca/openfisca-survey-manager/pull/257)
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/LICENSE.AGPL.txt` & `OpenFisca-Survey-Manager-1.1.2/LICENSE.AGPL.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,15 +23,15 @@
 License-File: LICENSE.AGPL.txt
 
 # OpenFisca Survey Manager
 
 [![Newsletter](https://img.shields.io/badge/newsletter-subscribe!-informational.svg?style=flat)](mailto:contact%40openfisca.org?subject=Subscribe%20to%20your%20newsletter%20%7C%20S'inscrire%20%C3%A0%20votre%20newsletter&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0AEnvoyez-nous%20cet%20email%20pour%20que%20l'on%20puisse%20vous%20inscrire%20%C3%A0%20la%20newsletter.%20%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20send%20us%20this%20email%2C%20so%20we%20can%20subscribe%20you%20to%20the%20newsletter.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
 [![Twitter](https://img.shields.io/badge/twitter-follow%20us!-9cf.svg?style=flat)](https://twitter.com/intent/follow?screen_name=openfisca)
 [![Slack](https://img.shields.io/badge/slack-join%20us!-blueviolet.svg?style=flat)](mailto:contact%40openfisca.org?subject=Join%20you%20on%20Slack%20%7C%20Nous%20rejoindre%20sur%20Slack&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0ARacontez-nous%20un%20peu%20de%20vous%2C%20et%20du%20pourquoi%20de%20votre%20int%C3%A9r%C3%AAt%20de%20rejoindre%20la%20communaut%C3%A9%20OpenFisca%20sur%20Slack.%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AN%E2%80%99oubliez%20pas%20de%20nous%20envoyer%20cet%20email%C2%A0!%20Sinon%2C%20on%20ne%20pourra%20pas%20vous%20contacter%20ni%20vous%20inviter%20sur%20Slack.%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20tell%20us%20a%20bit%20about%20you%20and%20why%20you%20want%20to%20join%20the%20OpenFisca%20community%20on%20Slack.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2.%0A%0ADon't%20forget%20to%20send%20us%20this%20email!%20Otherwise%20we%20won't%20be%20able%20to%20contact%20you%20back%2C%20nor%20invite%20you%20on%20Slack.%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
-[![CircleCI](https://img.shields.io/circleci/project/github/openfisca/openfisca-survey-manager/master.svg?style=flat)](https://circleci.com/gh/openfisca/openfisca-survey-manager)
+[![GitHub Actions](https://github.com/openfisca/openfisca-survey-manager/actions/workflows/workflow.yml/badge.svg?branch=master&event=push)](https://github.com/openfisca/openfisca-survey-manager/actions?query=branch%3Amaster)
 [![Coveralls](https://img.shields.io/coveralls/github/openfisca/openfisca-survey-manager/master.svg?style=flat)](https://coveralls.io/github/openfisca/openfisca-survey-manager?branch=master)
 [![Python](https://img.shields.io/pypi/pyversions/openfisca-survey-manager.svg)](https://pypi.python.org/pypi/openfisca-survey-manager)
 [![PyPi](https://img.shields.io/pypi/v/openfisca-survey-manager.svg?style=flat)](https://pypi.python.org/pypi/openfisca-survey-manager)
 
 ## [EN] Introduction
 
 [OpenFisca](https://openfisca.org) is a versatile microsimulation free software. You can check the [online documentation](https://openfisca.org/doc/) for more details.
@@ -269,15 +269,15 @@
 
 To run the entire test suite:
 
 ```sh
 make test
 ```
 
-To run the entire test suite with the same config as in CI:
+To run the entire test suite with the same config as in Continuous Integration (CI):
 
 ```sh
 CI=True make test
 ```
 
 ## Style
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/SOURCES.txt` & `OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/OpenFisca_Survey_Manager.egg-info/requires.txt` & `OpenFisca-Survey-Manager-1.1.2/OpenFisca_Survey_Manager.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/PKG-INFO` & `OpenFisca-Survey-Manager-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenFisca-Survey-Manager
-Version: 1.1.1
+Version: 1.1.2
 Summary: A tool for managing survey/administrative data.
 Home-page: https://github.com/openfisca/openfisca-survey-manager
 Author: OpenFisca Team
 Author-email: contact@openfisca.fr
 License: http://www.fsf.org/licensing/licenses/agpl-3.0.html
 Keywords: survey data
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,15 +23,15 @@
 License-File: LICENSE.AGPL.txt
 
 # OpenFisca Survey Manager
 
 [![Newsletter](https://img.shields.io/badge/newsletter-subscribe!-informational.svg?style=flat)](mailto:contact%40openfisca.org?subject=Subscribe%20to%20your%20newsletter%20%7C%20S'inscrire%20%C3%A0%20votre%20newsletter&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0AEnvoyez-nous%20cet%20email%20pour%20que%20l'on%20puisse%20vous%20inscrire%20%C3%A0%20la%20newsletter.%20%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20send%20us%20this%20email%2C%20so%20we%20can%20subscribe%20you%20to%20the%20newsletter.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
 [![Twitter](https://img.shields.io/badge/twitter-follow%20us!-9cf.svg?style=flat)](https://twitter.com/intent/follow?screen_name=openfisca)
 [![Slack](https://img.shields.io/badge/slack-join%20us!-blueviolet.svg?style=flat)](mailto:contact%40openfisca.org?subject=Join%20you%20on%20Slack%20%7C%20Nous%20rejoindre%20sur%20Slack&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0ARacontez-nous%20un%20peu%20de%20vous%2C%20et%20du%20pourquoi%20de%20votre%20int%C3%A9r%C3%AAt%20de%20rejoindre%20la%20communaut%C3%A9%20OpenFisca%20sur%20Slack.%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AN%E2%80%99oubliez%20pas%20de%20nous%20envoyer%20cet%20email%C2%A0!%20Sinon%2C%20on%20ne%20pourra%20pas%20vous%20contacter%20ni%20vous%20inviter%20sur%20Slack.%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20tell%20us%20a%20bit%20about%20you%20and%20why%20you%20want%20to%20join%20the%20OpenFisca%20community%20on%20Slack.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2.%0A%0ADon't%20forget%20to%20send%20us%20this%20email!%20Otherwise%20we%20won't%20be%20able%20to%20contact%20you%20back%2C%20nor%20invite%20you%20on%20Slack.%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
-[![CircleCI](https://img.shields.io/circleci/project/github/openfisca/openfisca-survey-manager/master.svg?style=flat)](https://circleci.com/gh/openfisca/openfisca-survey-manager)
+[![GitHub Actions](https://github.com/openfisca/openfisca-survey-manager/actions/workflows/workflow.yml/badge.svg?branch=master&event=push)](https://github.com/openfisca/openfisca-survey-manager/actions?query=branch%3Amaster)
 [![Coveralls](https://img.shields.io/coveralls/github/openfisca/openfisca-survey-manager/master.svg?style=flat)](https://coveralls.io/github/openfisca/openfisca-survey-manager?branch=master)
 [![Python](https://img.shields.io/pypi/pyversions/openfisca-survey-manager.svg)](https://pypi.python.org/pypi/openfisca-survey-manager)
 [![PyPi](https://img.shields.io/pypi/v/openfisca-survey-manager.svg?style=flat)](https://pypi.python.org/pypi/openfisca-survey-manager)
 
 ## [EN] Introduction
 
 [OpenFisca](https://openfisca.org) is a versatile microsimulation free software. You can check the [online documentation](https://openfisca.org/doc/) for more details.
@@ -269,15 +269,15 @@
 
 To run the entire test suite:
 
 ```sh
 make test
 ```
 
-To run the entire test suite with the same config as in CI:
+To run the entire test suite with the same config as in Continuous Integration (CI):
 
 ```sh
 CI=True make test
 ```
 
 ## Style
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/README.md` & `OpenFisca-Survey-Manager-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # OpenFisca Survey Manager
 
 [![Newsletter](https://img.shields.io/badge/newsletter-subscribe!-informational.svg?style=flat)](mailto:contact%40openfisca.org?subject=Subscribe%20to%20your%20newsletter%20%7C%20S'inscrire%20%C3%A0%20votre%20newsletter&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0AEnvoyez-nous%20cet%20email%20pour%20que%20l'on%20puisse%20vous%20inscrire%20%C3%A0%20la%20newsletter.%20%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20send%20us%20this%20email%2C%20so%20we%20can%20subscribe%20you%20to%20the%20newsletter.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
 [![Twitter](https://img.shields.io/badge/twitter-follow%20us!-9cf.svg?style=flat)](https://twitter.com/intent/follow?screen_name=openfisca)
 [![Slack](https://img.shields.io/badge/slack-join%20us!-blueviolet.svg?style=flat)](mailto:contact%40openfisca.org?subject=Join%20you%20on%20Slack%20%7C%20Nous%20rejoindre%20sur%20Slack&body=%5BEnglish%20version%20below%5D%0A%0ABonjour%2C%0A%0AVotre%C2%A0pr%C3%A9sence%C2%A0ici%C2%A0nous%C2%A0ravit%C2%A0!%20%F0%9F%98%83%0A%0ARacontez-nous%20un%20peu%20de%20vous%2C%20et%20du%20pourquoi%20de%20votre%20int%C3%A9r%C3%AAt%20de%20rejoindre%20la%20communaut%C3%A9%20OpenFisca%20sur%20Slack.%0A%0AAh%C2%A0!%20Et%20si%20vous%20pouviez%20remplir%20ce%20petit%20questionnaire%2C%20%C3%A7a%20serait%20encore%20mieux%C2%A0!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2F45M0VR1TYKD1RGzX2%0A%0AN%E2%80%99oubliez%20pas%20de%20nous%20envoyer%20cet%20email%C2%A0!%20Sinon%2C%20on%20ne%20pourra%20pas%20vous%20contacter%20ni%20vous%20inviter%20sur%20Slack.%0A%0AAmiti%C3%A9%2C%0AL%E2%80%99%C3%A9quipe%20OpenFisca%0A%0A%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%20ENGLISH%20VERSION%20%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%3D%0A%0AHi%2C%20%0A%0AWe're%20glad%20to%20see%20you%20here!%20%F0%9F%98%83%0A%0APlease%20tell%20us%20a%20bit%20about%20you%20and%20why%20you%20want%20to%20join%20the%20OpenFisca%20community%20on%20Slack.%0A%0AAlso%2C%20if%20you%20can%20fill%20out%20this%20short%20survey%2C%20even%20better!%0Ahttps%3A%2F%2Fgoo.gl%2Fforms%2FsOg8K1abhhm441LG2.%0A%0ADon't%20forget%20to%20send%20us%20this%20email!%20Otherwise%20we%20won't%20be%20able%20to%20contact%20you%20back%2C%20nor%20invite%20you%20on%20Slack.%0A%0ACheers%2C%0AThe%20OpenFisca%20Team)
-[![CircleCI](https://img.shields.io/circleci/project/github/openfisca/openfisca-survey-manager/master.svg?style=flat)](https://circleci.com/gh/openfisca/openfisca-survey-manager)
+[![GitHub Actions](https://github.com/openfisca/openfisca-survey-manager/actions/workflows/workflow.yml/badge.svg?branch=master&event=push)](https://github.com/openfisca/openfisca-survey-manager/actions?query=branch%3Amaster)
 [![Coveralls](https://img.shields.io/coveralls/github/openfisca/openfisca-survey-manager/master.svg?style=flat)](https://coveralls.io/github/openfisca/openfisca-survey-manager?branch=master)
 [![Python](https://img.shields.io/pypi/pyversions/openfisca-survey-manager.svg)](https://pypi.python.org/pypi/openfisca-survey-manager)
 [![PyPi](https://img.shields.io/pypi/v/openfisca-survey-manager.svg?style=flat)](https://pypi.python.org/pypi/openfisca-survey-manager)
 
 ## [EN] Introduction
 
 [OpenFisca](https://openfisca.org) is a versatile microsimulation free software. You can check the [online documentation](https://openfisca.org/doc/) for more details.
@@ -245,15 +245,15 @@
 
 To run the entire test suite:
 
 ```sh
 make test
 ```
 
-To run the entire test suite with the same config as in CI:
+To run the entire test suite with the same config as in Continuous Integration (CI):
 
 ```sh
 CI=True make test
 ```
 
 ## Style
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/__init__.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,35 +24,31 @@
     default_config_files_directory = BaseDirectory.save_config_path('openfisca-survey-manager')
 except pkg_resources.DistributionNotFound:
     france_data_location = None
 
 if france_data_location is None or not os.path.exists(default_config_files_directory):
     default_config_files_directory = None
 
-# Run CI when testing openfisca-survey-manager for example GitHub actions
+# Run CI when testing openfisca-survey-manager for example GitHub Actions
 test_config_files_directory = os.path.join(
     pkg_resources.get_distribution('openfisca-survey-manager').location,
     'openfisca_survey_manager',
     'tests',
     'data_files',
     )
 
 with open(os.path.join(test_config_files_directory, 'config_template.ini')) as file:
     config_ini = file.read()
 
 config_ini = config_ini.format(location = pkg_resources.get_distribution('openfisca-survey-manager').location)
 with open(os.path.join(test_config_files_directory, 'config.ini'), "w+") as file:
     file.write(config_ini)
 
-# GitHub actions test
-if 'CI' in os.environ:
-    is_in_ci = True
-else:
-    is_in_ci = False
-
+# GitHub Actions test
+is_in_ci = 'CI' in os.environ
 
 if is_in_ci and default_config_files_directory is None:
     default_config_files_directory = test_config_files_directory
 
 if default_config_files_directory is None:
     from xdg import BaseDirectory
     default_config_files_directory = BaseDirectory.save_config_path('openfisca-survey-manager')
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/aggregates.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/aggregates.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_groupes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_postes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/assets/nomenclature_coicop_source_by_sous_classes.csv`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/calibration.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calibration.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/calmar.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/coicop.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/coicop.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/config.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/config.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/google_colab.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/google_colab.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/input_dataframe_generator.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/input_dataframe_generator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/matching.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/read_dbf.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_dbf.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/read_sas.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/scenarios.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scenarios.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/scripts/build_collection.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/scripts/build_collection.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/statshelpers.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/statshelpers.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/survey_collections.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/survey_collections.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/surveys.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tables.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/temporary.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/temporary.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_add_survey_to_collection.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_add_survey_to_collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 import pandas as pd
 import pytest
 
 from openfisca_survey_manager.survey_collections import SurveyCollection
 from openfisca_survey_manager.scripts.build_collection import add_survey_to_collection
 from openfisca_survey_manager.input_dataframe_generator import set_table_in_survey
 
-# Travis, Gitlab runner, Gihub Action and circle has env variable "CI" set by default
-if 'CI' in os.environ:
-    is_in_ci = True
-else:
-    is_in_ci = False
+# GitLab Runner and GitHub Actions have env variable "CI" set by default
+is_in_ci = 'CI' in os.environ
 
 
 def test_add_survey_to_collection():
     # if is_in_ci:
     #     return
     name = 'fake'
     survey_name = 'fake_survey'
```

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_calmar.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_calmar.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_create_data_frame_by_entity.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_legislation_inflator.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_legislation_inflator.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_marginal_tax_rate.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_marginal_tax_rate.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_matching.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_quantile.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_quantile.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_read_sas.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_read_sas.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_scenario.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_scenario.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_summarize_variables.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_summarize_variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_surveys.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_surveys.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/tests/test_tax_benefit_system_asof.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/utils.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/utils.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/openfisca_survey_manager/variables.py` & `OpenFisca-Survey-Manager-1.1.2/openfisca_survey_manager/variables.py`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/setup.cfg` & `OpenFisca-Survey-Manager-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `OpenFisca-Survey-Manager-1.1.1/setup.py` & `OpenFisca-Survey-Manager-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 doc_lines = __doc__.split('\n')
 
 
 setup(
     name = 'OpenFisca-Survey-Manager',
-    version = '1.1.1',
+    version = '1.1.2',
     author = 'OpenFisca Team',
     author_email = 'contact@openfisca.fr',
     classifiers = [classifier for classifier in classifiers.split('\n') if classifier],
     description = doc_lines[0],
     keywords = 'survey data',
     license = 'http://www.fsf.org/licensing/licenses/agpl-3.0.html',
     license_files = ("LICENSE.AGPL.txt",),
```

