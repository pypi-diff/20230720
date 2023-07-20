# Comparing `tmp/eu_cbm_hat-0.6.4.tar.gz` & `tmp/eu_cbm_hat-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eu_cbm_hat-0.6.4.tar", last modified: Wed Jun 28 10:15:34 2023, max compression
+gzip compressed data, was "eu_cbm_hat-0.6.5.tar", last modified: Thu Jul 20 09:58:26 2023, max compression
```

## Comparing `eu_cbm_hat-0.6.4.tar` & `eu_cbm_hat-0.6.5.tar`

### file list

```diff
@@ -1,151 +1,142 @@
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.336535 eu_cbm_hat-0.6.4/
--rw-r--r--   0 paul      (1000) paul      (1000)    13862 2022-12-07 14:55:14.000000 eu_cbm_hat-0.6.4/LICENCE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       92 2022-12-07 14:57:34.000000 eu_cbm_hat-0.6.4/MANIFEST.in
--rw-r--r--   0 paul      (1000) paul      (1000)    57674 2022-12-07 16:29:26.000000 eu_cbm_hat-0.6.4/NOTICE.txt
--rw-r--r--   0 paul      (1000) paul      (1000)     8078 2023-06-28 10:15:34.336535 eu_cbm_hat-0.6.4/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     7649 2023-05-16 17:40:14.000000 eu_cbm_hat-0.6.4/README.md
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.300535 eu_cbm_hat-0.6.4/eu_cbm_hat/
--rw-r--r--   0 paul      (1000) paul      (1000)     1618 2023-06-28 10:15:02.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/__init__.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.304535 eu_cbm_hat-0.6.4/eu_cbm_hat/cbm/
--rw-r--r--   0 paul      (1000) paul      (1000)       72 2022-12-09 09:42:16.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/cbm/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)    31577 2023-06-27 16:23:38.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/cbm/dynamic.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5853 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/cbm/simulation.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.308535 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/
--rw-r--r--   0 paul      (1000) paul      (1000)     3604 2023-06-20 08:59:59.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5199 2023-06-20 14:08:29.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/base_combo.py
--rw-r--r--   0 paul      (1000) paul      (1000)      905 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/harvest_test.py
--rw-r--r--   0 paul      (1000) paul      (1000)      825 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/hat.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2091 2022-12-07 10:05:35.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/historical.py
--rw-r--r--   0 paul      (1000) paul      (1000)      833 2023-06-20 07:57:49.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/ia_2040.py
--rw-r--r--   0 paul      (1000) paul      (1000)      791 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/no_market_forcing.py
--rw-r--r--   0 paul      (1000) paul      (1000)      719 2023-06-20 08:23:58.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/pikbau.py
--rw-r--r--   0 paul      (1000) paul      (1000)      721 2023-06-20 08:01:12.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/pikfair.py
--rw-r--r--   0 paul      (1000) paul      (1000)      793 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/potencia_baseline.py
--rw-r--r--   0 paul      (1000) paul      (1000)      805 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/potencia_necp_bme_up100.py
--rw-r--r--   0 paul      (1000) paul      (1000)      805 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/potencia_necp_bme_up200.py
--rw-r--r--   0 paul      (1000) paul      (1000)      807 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/potencia_necp_bms_down50.py
--rw-r--r--   0 paul      (1000) paul      (1000)      807 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/potencia_necp_bms_down90.py
--rw-r--r--   0 paul      (1000) paul      (1000)      777 2023-02-14 09:33:00.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/reference.py
--rw-r--r--   0 paul      (1000) paul      (1000)      845 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/reference_crf.py
--rw-r--r--   0 paul      (1000) paul      (1000)      835 2022-12-21 16:03:35.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/skewfcth.py
--rw-r--r--   0 paul      (1000) paul      (1000)      818 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/combos/special.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.312535 eu_cbm_hat-0.6.4/eu_cbm_hat/core/
--rw-r--r--   0 paul      (1000) paul      (1000)      618 2022-12-09 09:35:23.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/core/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2743 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/core/continent.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5672 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/core/country.py
--rw-r--r--   0 paul      (1000) paul      (1000)     8949 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/core/runner.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.312535 eu_cbm_hat-0.6.4/eu_cbm_hat/info/
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5226 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/aidb.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5983 2022-12-15 15:55:50.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/fluxes.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5456 2022-12-07 10:05:35.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/harvest.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5224 2023-05-16 16:03:15.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/input_data.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2573 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/internal_data.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4019 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/orig_data.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7534 2023-06-26 11:09:26.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/output_data.py
--rw-r--r--   0 paul      (1000) paul      (1000)    14668 2022-12-15 16:30:06.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/info/silviculture.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.312535 eu_cbm_hat-0.6.4/eu_cbm_hat/launch/
--rw-r--r--   0 paul      (1000) paul      (1000)      167 2022-12-09 09:56:16.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/launch/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3287 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/launch/associations.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3743 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/launch/create_json.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.316535 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/
--rw-r--r--   0 paul      (1000) paul      (1000)       84 2022-12-09 10:01:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1059 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/classifiers.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1401 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/column_order.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3287 2023-05-16 16:06:20.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/long_or_wide.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1803 2023-06-26 16:35:35.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/post_processor.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3659 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/pump/pre_processor.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.316535 eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/
--rw-r--r--   0 paul      (1000) paul      (1000)     1150 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/__init__.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1694 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/aidb.py
--rw-r--r--   0 paul      (1000) paul      (1000)     7382 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/expected_provided.py
--rw-r--r--   0 paul      (1000) paul      (1000)     3226 2022-12-07 10:05:35.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/input_years.py
--rw-r--r--   0 paul      (1000) paul      (1000)     5958 2022-12-15 15:59:43.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/silviculture.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.320535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/
--rw-r--r--   0 paul      (1000) paul      (1000)      895 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/copy_data.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.300535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.320535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/combos/
--rw-r--r--   0 paul      (1000) paul      (1000)     3775 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/combos/reference.yaml
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.320535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/common/
--rw-r--r--   0 paul      (1000) paul      (1000)      999 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/common/country_codes.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      267 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/common/reference_years.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.296535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.300535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.300535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.320535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/events.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/growth_curves.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/inventory.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/transitions.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.324535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/events.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/growth_curves.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/inventory.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/transitions.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.324535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/
--rw-r--r--   0 paul      (1000) paul      (1000)     3418 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/events.csv
--rw-r--r--   0 paul      (1000) paul      (1000)    13415 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/growth_curves.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     6835 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/inventory.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      843 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/transitions.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.324535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/events.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/growth_curves.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/inventory.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/transitions.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.324535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/
--rw-r--r--   0 paul      (1000) paul      (1000)     1649 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/events.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/growth_curves.csv
--rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/inventory.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      631 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/transitions.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.328535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/
--rw-r--r--   0 paul      (1000) paul      (1000)      586 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/age_classes.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      833 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/classifiers.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      585 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/disturbance_types.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.328535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/config/
--rw-r--r--   0 paul      (1000) paul      (1000)     2098 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/config/associations.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.328535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/
--rw-r--r--   0 paul      (1000) paul      (1000)     6303 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/events_templates.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     2632 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/harvest_factors.csv
--rw-r--r--   0 paul      (1000) paul      (1000)     4603 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/irw_frac_by_dist.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      104 2023-04-26 17:02:44.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/vol_to_mass_coefs.csv
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.300535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.328535 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/
--rw-r--r--   0 paul      (1000) paul      (1000)   145505 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/fw_harvest.csv
--rw-r--r--   0 paul      (1000) paul      (1000)   134895 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/irw_harvest.csv
--rw-r--r--   0 paul      (1000) paul      (1000)      299 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/test_qaqc.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1489 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/test_salvage.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2041 2023-02-14 09:33:00.000000 eu_cbm_hat-0.6.4/eu_cbm_hat/tests/test_silviculture.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.304535 eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/
--rw-r--r--   0 paul      (1000) paul      (1000)     8078 2023-06-28 10:15:34.000000 eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/PKG-INFO
--rw-r--r--   0 paul      (1000) paul      (1000)     5028 2023-06-28 10:15:34.000000 eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/SOURCES.txt
--rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-06-28 10:15:34.000000 eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/dependency_links.txt
--rw-r--r--   0 paul      (1000) paul      (1000)      134 2023-06-28 10:15:34.000000 eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/requires.txt
--rw-r--r--   0 paul      (1000) paul      (1000)       46 2023-06-28 10:15:34.000000 eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/top_level.txt
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.300535 eu_cbm_hat-0.6.4/scripts/
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.332535 eu_cbm_hat-0.6.4/scripts/conversion/
--rw-r--r--   0 paul      (1000) paul      (1000)     5120 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/conversion/add_indicators_to_aidb.py
--rw-r--r--   0 paul      (1000) paul      (1000)     4140 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/conversion/convert_aidb.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2355 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/conversion/merge_growth_curves.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1765 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/conversion/rename_all_classifiers.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1436 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/conversion/rename_associations.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1954 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/conversion/update_input_classif.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.332535 eu_cbm_hat-0.6.4/scripts/running/
--rw-r--r--   0 paul      (1000) paul      (1000)      718 2023-05-31 09:20:18.000000 eu_cbm_hat-0.6.4/scripts/running/run_at.py
--rw-r--r--   0 paul      (1000) paul      (1000)      648 2023-06-20 09:22:23.000000 eu_cbm_hat-0.6.4/scripts/running/run_ee.py
--rw-r--r--   0 paul      (1000) paul      (1000)      454 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/scripts/running/run_fi.py
--rw-r--r--   0 paul      (1000) paul      (1000)      542 2023-06-05 13:51:32.000000 eu_cbm_hat-0.6.4/scripts/running/run_fr.py
--rw-r--r--   0 paul      (1000) paul      (1000)      607 2023-05-16 15:21:25.000000 eu_cbm_hat-0.6.4/scripts/running/run_hu.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1059 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/scripts/running/run_lu.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2208 2023-06-21 16:44:21.000000 eu_cbm_hat-0.6.4/scripts/running/run_scenario_combo.py
--rw-r--r--   0 paul      (1000) paul      (1000)      539 2023-06-27 15:03:33.000000 eu_cbm_hat-0.6.4/scripts/running/run_se.py
--rw-r--r--   0 paul      (1000) paul      (1000)      607 2023-06-27 15:04:10.000000 eu_cbm_hat-0.6.4/scripts/running/run_si.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1353 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/scripts/running/run_zz.py
--rw-r--r--   0 paul      (1000) paul      (1000)     1542 2022-12-07 10:05:35.000000 eu_cbm_hat-0.6.4/scripts/running/run_zz_in_temp_dir_without_eu_cbm_data.py
-drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-06-28 10:15:34.336535 eu_cbm_hat-0.6.4/scripts/setup/
--rw-r--r--   0 paul      (1000) paul      (1000)    11109 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/setup/activities_creation.py
--rw-r--r--   0 paul      (1000) paul      (1000)      463 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/setup/aidb_symlink.py
--rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.4/scripts/setup/copy_zz_from_libcbm_data.py
--rw-r--r--   0 paul      (1000) paul      (1000)      572 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/setup/make_interface.py
--rw-r--r--   0 paul      (1000) paul      (1000)      572 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.4/scripts/setup/save_interface.py
--rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-06-28 10:15:34.336535 eu_cbm_hat-0.6.4/setup.cfg
--rw-r--r--   0 paul      (1000) paul      (1000)     1436 2023-06-28 10:15:02.000000 eu_cbm_hat-0.6.4/setup.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.530458 eu_cbm_hat-0.6.5/
+-rw-r--r--   0 paul      (1000) paul      (1000)    13862 2022-12-07 14:55:14.000000 eu_cbm_hat-0.6.5/LICENCE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       92 2022-12-07 14:57:34.000000 eu_cbm_hat-0.6.5/MANIFEST.in
+-rw-r--r--   0 paul      (1000) paul      (1000)    57674 2022-12-07 16:29:26.000000 eu_cbm_hat-0.6.5/NOTICE.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)     8078 2023-07-20 09:58:26.530458 eu_cbm_hat-0.6.5/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     7649 2023-05-16 17:40:14.000000 eu_cbm_hat-0.6.5/README.md
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.482457 eu_cbm_hat-0.6.5/eu_cbm_hat/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1722 2023-07-20 09:57:39.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/__init__.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.482457 eu_cbm_hat-0.6.5/eu_cbm_hat/cbm/
+-rw-r--r--   0 paul      (1000) paul      (1000)       72 2022-12-09 09:42:16.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/cbm/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    31694 2023-07-19 09:15:44.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/cbm/dynamic.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5853 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/cbm/simulation.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.486457 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3057 2023-07-19 10:29:06.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     6364 2023-07-12 15:47:15.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/base_combo.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      825 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/hat.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2091 2022-12-07 10:05:35.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/historical.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      833 2023-06-20 07:57:49.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/ia_2040.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      777 2023-02-14 09:33:00.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/combos/reference.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.494457 eu_cbm_hat-0.6.5/eu_cbm_hat/core/
+-rw-r--r--   0 paul      (1000) paul      (1000)      618 2022-12-09 09:35:23.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/core/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3464 2023-06-29 15:43:05.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/core/continent.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5672 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/core/country.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     8943 2023-07-19 15:20:51.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/core/runner.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.498457 eu_cbm_hat-0.6.5/eu_cbm_hat/info/
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5226 2023-07-11 12:48:44.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/aidb.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5983 2022-12-15 15:55:50.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/fluxes.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5456 2023-06-28 14:20:29.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/harvest.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5224 2023-05-16 16:03:15.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/input_data.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2573 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/internal_data.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4019 2023-07-11 12:48:44.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/orig_data.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7534 2023-06-26 11:09:26.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/output_data.py
+-rw-r--r--   0 paul      (1000) paul      (1000)    14730 2023-07-11 13:31:35.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/info/silviculture.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.498457 eu_cbm_hat-0.6.5/eu_cbm_hat/launch/
+-rw-r--r--   0 paul      (1000) paul      (1000)      167 2022-12-09 09:56:16.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/launch/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3287 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/launch/associations.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3743 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/launch/create_json.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.502457 eu_cbm_hat-0.6.5/eu_cbm_hat/post_processor/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1803 2023-06-26 16:35:35.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/post_processor/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      889 2023-07-20 09:03:16.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/post_processor/harvest.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3892 2023-07-19 16:25:06.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/post_processor/sink.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.502457 eu_cbm_hat-0.6.5/eu_cbm_hat/pump/
+-rw-r--r--   0 paul      (1000) paul      (1000)       84 2022-12-09 10:01:44.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/pump/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1059 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/pump/classifiers.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1401 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/pump/column_order.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3287 2023-05-16 16:06:20.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/pump/long_or_wide.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3659 2023-07-11 12:48:44.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/pump/pre_processor.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.506457 eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1150 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/__init__.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3106 2023-06-29 14:32:20.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/aidb.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     7382 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/expected_provided.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     3226 2022-12-07 10:05:35.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/input_years.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     5958 2022-12-15 15:59:43.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/silviculture.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.518458 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/
+-rw-r--r--   0 paul      (1000) paul      (1000)      895 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/copy_data.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.478457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.518458 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/combos/
+-rw-r--r--   0 paul      (1000) paul      (1000)     4231 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/combos/reference.yaml
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.518458 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)      999 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/common/country_codes.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      267 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/common/reference_years.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.478457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.478457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.478457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.518458 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1259 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/events.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      591 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/growth_curves.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      288 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/inventory.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      448 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/transitions.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.518458 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1573 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/events.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/growth_curves.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/inventory.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      446 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/deforestation/transitions.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.522457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8178 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/events.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)    13415 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/growth_curves.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     6835 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/inventory.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      847 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/transitions.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.522457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/events.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/growth_curves.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/inventory.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_nsr/transitions.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.522457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/
+-rw-r--r--   0 paul      (1000) paul      (1000)     1466 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/events.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/growth_curves.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)        0 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/inventory.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      631 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/transitions.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.522457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/
+-rw-r--r--   0 paul      (1000) paul      (1000)      586 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/age_classes.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      833 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/classifiers.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      578 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/disturbance_types.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.526457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/config/
+-rw-r--r--   0 paul      (1000) paul      (1000)     2065 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/config/associations.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.526457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/
+-rw-r--r--   0 paul      (1000) paul      (1000)     3583 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/events_templates.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     4863 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/harvest_factors.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)     2278 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/irw_frac_by_dist.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      104 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/vol_to_mass_coefs.csv
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.478457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.526457 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/
+-rw-r--r--   0 paul      (1000) paul      (1000)   145240 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/fw_harvest.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)   140902 2023-07-19 10:08:02.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/irw_harvest.csv
+-rw-r--r--   0 paul      (1000) paul      (1000)      290 2023-07-19 14:44:38.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/test_qaqc.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1481 2023-07-19 14:51:09.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/test_salvage.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2033 2023-07-19 14:43:15.000000 eu_cbm_hat-0.6.5/eu_cbm_hat/tests/test_silviculture.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.482457 eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/
+-rw-r--r--   0 paul      (1000) paul      (1000)     8078 2023-07-20 09:58:26.000000 eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/PKG-INFO
+-rw-r--r--   0 paul      (1000) paul      (1000)     4658 2023-07-20 09:58:26.000000 eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/SOURCES.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)        1 2023-07-20 09:58:26.000000 eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/dependency_links.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)      134 2023-07-20 09:58:26.000000 eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/requires.txt
+-rw-r--r--   0 paul      (1000) paul      (1000)       46 2023-07-20 09:58:26.000000 eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/top_level.txt
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.478457 eu_cbm_hat-0.6.5/scripts/
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.526457 eu_cbm_hat-0.6.5/scripts/conversion/
+-rw-r--r--   0 paul      (1000) paul      (1000)     5120 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/conversion/add_indicators_to_aidb.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     4140 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/conversion/convert_aidb.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2355 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/conversion/merge_growth_curves.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1765 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/conversion/rename_all_classifiers.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1436 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/conversion/rename_associations.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1954 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/conversion/update_input_classif.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.530458 eu_cbm_hat-0.6.5/scripts/running/
+-rw-r--r--   0 paul      (1000) paul      (1000)      718 2023-07-11 12:48:44.000000 eu_cbm_hat-0.6.5/scripts/running/run_at.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      648 2023-06-20 09:22:23.000000 eu_cbm_hat-0.6.5/scripts/running/run_ee.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      454 2023-05-04 16:10:28.000000 eu_cbm_hat-0.6.5/scripts/running/run_fi.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      542 2023-06-05 13:51:32.000000 eu_cbm_hat-0.6.5/scripts/running/run_fr.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      607 2023-05-16 15:21:25.000000 eu_cbm_hat-0.6.5/scripts/running/run_hu.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      943 2023-07-12 14:16:18.000000 eu_cbm_hat-0.6.5/scripts/running/run_lu.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2208 2023-06-21 16:44:21.000000 eu_cbm_hat-0.6.5/scripts/running/run_scenario_combo.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      539 2023-06-27 15:03:33.000000 eu_cbm_hat-0.6.5/scripts/running/run_se.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      591 2023-07-19 08:43:46.000000 eu_cbm_hat-0.6.5/scripts/running/run_si.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1353 2023-07-19 15:02:08.000000 eu_cbm_hat-0.6.5/scripts/running/run_zz.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     1548 2023-07-19 15:01:48.000000 eu_cbm_hat-0.6.5/scripts/running/run_zz_in_temp_dir_without_eu_cbm_data.py
+drwxr-xr-x   0 paul      (1000) paul      (1000)        0 2023-07-20 09:58:26.530458 eu_cbm_hat-0.6.5/scripts/setup/
+-rw-r--r--   0 paul      (1000) paul      (1000)    11109 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/setup/activities_creation.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      463 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/setup/aidb_symlink.py
+-rw-r--r--   0 paul      (1000) paul      (1000)     2711 2023-07-19 10:07:31.000000 eu_cbm_hat-0.6.5/scripts/setup/copy_zz_from_libcbm_data.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      572 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/setup/make_interface.py
+-rw-r--r--   0 paul      (1000) paul      (1000)      572 2022-11-24 14:36:18.000000 eu_cbm_hat-0.6.5/scripts/setup/save_interface.py
+-rw-r--r--   0 paul      (1000) paul      (1000)       38 2023-07-20 09:58:26.530458 eu_cbm_hat-0.6.5/setup.cfg
+-rw-r--r--   0 paul      (1000) paul      (1000)     1436 2023-07-20 09:57:39.000000 eu_cbm_hat-0.6.5/setup.py
```

### Comparing `eu_cbm_hat-0.6.4/LICENCE.txt` & `eu_cbm_hat-0.6.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/NOTICE.txt` & `eu_cbm_hat-0.6.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/PKG-INFO` & `eu_cbm_hat-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eu_cbm_hat
-Version: 0.6.4
+Version: 0.6.5
 Summary: eu_cbm_hat is a python package for running carbon budget simulations.
 Home-page: https://gitlab.com/bioeconomy/eu_cbm/eu_cbm_hat
 Author: Lucas Sinclair
 Author-email: lucas.sinclair@me.com
 Maintainer: Paul Rougieux
 License: EUPL
 Requires-Python: >=3.8
```

### Comparing `eu_cbm_hat-0.6.4/README.md` & `eu_cbm_hat-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/__init__.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,18 +13,20 @@
 feedback under [issue
 50](https://gitlab.com/bioeconomy/eu_cbm/eu_cbm_hat/-/issues/50) ).
 - The Harvest Allocation Tool is implemented in `eu_cbm_hat.cbm.dynamic`.
 
 """
 
 # Special variables #
-__version__ = '0.6.4'
+__version__ = '0.6.5'
 
 # Built-in modules #
-import os, sys
+import os
+import sys
+import pathlib
 
 # First party modules #
 from autopaths import Path
 from autopaths.dir_path import DirectoryPath
 from plumbing.git import GitRepo
 
 # Constants #
@@ -44,13 +46,16 @@
 # Where is the data, default case #
 eu_cbm_data_dir = DirectoryPath("~/eu_cbm/eu_cbm_data/")
 
 # But you can override that with an environment variable #
 if os.environ.get("EU_CBM_DATA"):
     eu_cbm_data_dir = DirectoryPath(os.environ['EU_CBM_DATA'])
 
+# Prepare the move to pathlib
+eu_cbm_data_pathlib = pathlib.Path(eu_cbm_data_dir)
+
 # Where are the AIDBs, default case
 eu_cbm_aidb_dir = DirectoryPath("~/eu_cbm/eu_cbm_aidb/")
 
 # But you can override that with an environment variable #
 if os.environ.get("EU_CBM_AIDB"):
     eu_cbm_aidb_dir = DirectoryPath(os.environ['EU_CBM_AIDB'])
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/cbm/dynamic.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/cbm/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -614,18 +614,20 @@
 
         # Select which events columns appear in the output record
         # Note: dist_type_name is already an input dist id (not an internal dist id)
         # It will not be converted by the outputdata.__setitem__() method
         cols += ['dist_type_name', 'product_created', 'dist_interval_bias',
                  'using_id', 'sw_start', 'sw_end', 'hw_start', 'hw_end',
                  'min_since_last_dist', 'max_since_last_dist', 'last_dist_id',
-                 'sort_type', 'measurement_type', 'efficiency', 'skew', 'wood_density',
+                 'sort_type', 'measurement_type', 'efficiency', 'wood_density',
                  'bark_frac', 'irw_avail', 'fw_avail',
                  'irw_norm', 'irw_need', 'irw_frac',
                  'fw_colat', 'fw_norm', 'fw_need', 'amount']
+        if 'skew' in df.columns:
+            cols += ['skew']
         # Write the events to an output file for the record
         self.runner.output.events = pandas.concat([self.runner.output.events, df[cols]])
 
         # Get only the right columns in the dataframe to send to `libcbm` #
         cols = self.runner.input_data['events'].columns
         df = df[cols].copy()
 
@@ -675,8 +677,9 @@
             # Convert other values
             mapping = {v:k for k,v in str_to_id.items()}
             df[classif_name] = df[classif_name].map(mapping)
         # Return #
         return df
 
     def out_var(self, key, value):
+        """Store summary information into output extras.csv"""
         self.runner.output.extras.loc[self.year, key] = value
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/cbm/simulation.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/cbm/simulation.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/combos/base_combo.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/combos/base_combo.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from autopaths      import Path
 from plumbing.cache import property_cached
 from plumbing.timer import Timer
 
 # Internal modules #
 from eu_cbm_hat import eu_cbm_data_dir
 from eu_cbm_hat.core.runner import Runner
+from eu_cbm_hat.cbm.dynamic       import DynamicRunner
 
 # Constant directory for all the data #
 yaml_dir = eu_cbm_data_dir + 'combos/'
 
 ###############################################################################
 class Combination(object):
     """
@@ -52,23 +53,25 @@
         >>> r.run(True, True, True)
 
     You can then check the output pools:
 
         >>> r.output.load('pools')
     """
 
-    short_name = None
-
-    def __init__(self, continent):
+    def __init__(self, continent, short_name=None):
+        self.short_name = short_name
         # Save parent #
         self.continent = continent
         # The combos dir used for all output #
         self.output_dir = self.continent.output_dir
         # The base dir for our output #
         self.base_dir = Path(self.output_dir + self.short_name + '/')
+        # The path to our specific YAML file #
+        self.yaml_path = yaml_dir + self.short_name + '.yaml'
+
 
     def __repr__(self):
         return '%s object with %i runners' % (self.__class__, len(self))
 
     def __iter__(self): return iter(self.runners.values())
     def __len__(self):  return len(self.runners.values())
 
@@ -79,18 +82,16 @@
     #----------------------------- Properties --------------------------------#
     @property_cached
     def config(self):
         """
         The values chosen by the user in the YAML file which decide on every
         scenario choice for every activity and silvicultural practice.
         """
-        # The path to our specific YAML file #
-        yaml_path = yaml_dir + self.short_name + '.yaml'
         # Read it with a third party library #
-        with open(yaml_path, "r") as handle:
+        with open(self.yaml_path, "r") as handle:
             result = yaml.safe_load(handle)
         # Convert silvicultural choices to dataframes #
         key = 'harvest'
         value = result[key]
         if not isinstance(value, str):
             df = pandas.DataFrame.from_dict(value,
                                             orient  = 'index',
@@ -102,15 +103,38 @@
 
     @property_cached
     def runners(self):
         """
         A dictionary of country codes as keys with a list of runners as
         values.
         """
-        return {c.iso2_code: [Runner(self, c, 0)] for c in self.continent}
+        accepted_runner_types = ["base_runner", "dynamic_runner"]
+
+        # Error message to be reused by diverse errors
+        msg = f"The yaml file at {self.yaml_path} "
+        msg += "should contain a 'runner_type' field with values:"
+        msg += "\nrunner_type: "
+        msg += "\n# or\nrunner_type: ".join(accepted_runner_types)
+
+        # If runner_type is not defined in the yaml file raise an error
+        if "runner_type" not in self.config.keys():
+            raise ValueError(msg)
+
+        if self.config["runner_type"] not in accepted_runner_types:
+            msg_2 = f"runner_type: {self.config['runner_type']} "
+            msg_2 += "is not an accepted value.\n"
+            raise ValueError(msg_2 + msg)
+
+        # If it's defined as "base_runner", return base runners
+        if self.config["runner_type"] == "base_runner":
+            return {c.iso2_code: [Runner(self, c, 0)] for c in self.continent}
+
+        # If it's defined as "dynamic_runner" return dynamic runners
+        if self.config["runner_type"] == "dynamic_runner":
+            return {c.iso2_code: [DynamicRunner(self, c, 0)] for c in self.continent}
 
     #------------------------------- Methods ---------------------------------#
     def __call__(self, parallel=False, timer=True):
         """A method to run a combo by simulating all countries."""
         # Message #
         print("Running combo '%s'." % self.short_name)
         # Timer start #
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/combos/harvest_test.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/combos/hat.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,20 @@
 from plumbing.cache import property_cached
 
 # Internal modules #
 from eu_cbm_hat.combos.base_combo import Combination
 from eu_cbm_hat.cbm.dynamic       import DynamicRunner
 
 ###############################################################################
-class HarvestTest(Combination):
+class Hat(Combination):
     """
-    An integration test for the dynamic creation of disturbances during
-    the model run. Especially aimed at country `ZZ`.
+    A Combination used for the Harvest Allocation Tool (HAT).
     """
 
-    short_name = 'harvest_test'
+    short_name = 'hat'
 
     @property_cached
     def runners(self):
         """
         A dictionary of country codes as keys with a list of runners as
         values.
         """
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/combos/hat.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/combos/ia_2040.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 from plumbing.cache import property_cached
 
 # Internal modules #
 from eu_cbm_hat.combos.base_combo import Combination
 from eu_cbm_hat.cbm.dynamic       import DynamicRunner
 
 ###############################################################################
-class Hat(Combination):
+class IA_2040(Combination):
     """
     A Combination used for the Harvest Allocation Tool (HAT).
     """
 
-    short_name = 'hat'
+    short_name = 'ia_2040'
 
     @property_cached
     def runners(self):
         """
         A dictionary of country codes as keys with a list of runners as
         values.
         """
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/combos/historical.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/combos/historical.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/combos/ia_2040.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/combos/reference.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-#!/usr/bin/env python3
 # -*- coding: utf-8 -*-
-
 """
-Written by Lucas Sinclair and Paul Rougieux.
+Created on Wed Jun 29 16:09:00 2022
 
-JRC Biomass Project.
-Unit D1 Bioeconomy.
+@author: blujd
 """
 
 # Built-in modules #
 
 # First party modules #
 from plumbing.cache import property_cached
 
 # Internal modules #
 from eu_cbm_hat.combos.base_combo import Combination
 from eu_cbm_hat.cbm.dynamic       import DynamicRunner
 
 ###############################################################################
-class IA_2040(Combination):
+class Reference(Combination):
     """
     A Combination used for the Harvest Allocation Tool (HAT).
     """
 
-    short_name = 'ia_2040'
+    short_name = 'reference'
 
     @property_cached
     def runners(self):
         """
         A dictionary of country codes as keys with a list of runners as
         values.
         """
         return {c.iso2_code: [DynamicRunner(self, c, 0)]
-                for c in self.continent}
+                for c in self.continent}
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/core/__init__.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/core/continent.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/core/continent.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 # First party modules #
 from autopaths.auto_paths import AutoPaths
 from plumbing.cache       import property_cached
 
 # Internal modules #
 from eu_cbm_hat import eu_cbm_data_dir
 from eu_cbm_hat.core.country import Country
-from eu_cbm_hat.combos       import combo_classes
+from eu_cbm_hat.combos       import combo_classes_dict
+from eu_cbm_hat.combos.base_combo import Combination
+from eu_cbm_hat import eu_cbm_data_pathlib
+
 
 ###############################################################################
 class Continent(object):
     """
     Entry object to the pipeline.
 
     Aggregates countries together and enables access to a data frame containing
@@ -66,15 +69,25 @@
         all_countries = [Country(self, d)
                          for d in self.countries_dir.flat_directories]
         return {c.iso2_code: c for c in all_countries}
 
     @property_cached
     def combos(self):
         """Return a dictionary of combination names to Combination objects."""
-        all_combos = [combo(self) for combo in combo_classes]
+        combo_dir = eu_cbm_data_pathlib / "combos"
+        # List hard coded combo classes
+        hard_coded_combos = [combo(self, short_name) for short_name, combo in combo_classes_dict.items()]
+        # List yaml files
+        yaml_short_names = [x.stem for x in combo_dir.glob('**/*.yaml')]
+        # Remove short_names which correspond to hard coded combos
+        yaml_short_names = list(set(yaml_short_names) - set(combo_classes_dict.keys()))
+        # Create combos from yaml files
+        combos_from_yaml_files = [Combination(self, short_name) for short_name in yaml_short_names]
+        # List all combos
+        all_combos = hard_coded_combos + combos_from_yaml_files
         return {s.short_name: s for s in all_combos}
 
     #------------------------------- Methods ---------------------------------#
     def get_runner(self, combo, country, step):
         """Return a runner based on combo, country and step."""
         return self.combos[combo].runners[country][step]
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/core/country.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/core/country.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/core/runner.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/core/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from eu_cbm_hat.info.harvest         import Demand
 from eu_cbm_hat.info.fluxes         import Fluxes
 from eu_cbm_hat.info.input_data     import InputData
 from eu_cbm_hat.info.internal_data  import InternalData
 from eu_cbm_hat.info.output_data    import OutputData
 from eu_cbm_hat.info.silviculture   import Silviculture
 from eu_cbm_hat.launch.create_json  import CreateJSON
-from eu_cbm_hat.pump.post_processor import PostProcessor
+from eu_cbm_hat.post_processor import PostProcessor
 from eu_cbm_hat.pump.pre_processor  import PreProcessor
 from eu_cbm_hat.qaqc                import Qaqc
 import eu_cbm_hat
 
 # Third party modules
 
 ###############################################################################
@@ -39,15 +39,15 @@
     from a few input tables, such as an inventory and a list of disturbances
     and to bring this data all the way to the predicted carbon stock and
     fluxes.
 
     You can run a combo like this:
 
         >>> from eu_cbm_hat.core.continent import continent
-        >>> combo  = continent.combos['historical']
+        >>> combo  = continent.combos['reference']
         >>> runner = combo.runners['LU'][0]
         >>> runner.run()
 
     The runner has an attribute `output` that only deals with final output
     data that can be reached after closing and reopening your interpreter.
 
     The runner has an attribute `internal` that only deals with getting the
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/aidb.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/aidb.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/fluxes.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/fluxes.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/harvest.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/harvest.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/input_data.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/input_data.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/internal_data.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/internal_data.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/orig_data.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/orig_data.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/output_data.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/output_data.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/info/silviculture.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/info/silviculture.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 """
 
 # Built-in modules #
 
 # Third party modules #
 import pandas
+import numpy as np
 
 # First party modules #
 from plumbing.cache import property_cached
 
 # Internal modules #
 
 def keep_clfrs_without_question_marks(df, classifiers):
@@ -403,10 +404,11 @@
                 msg += f"Check column: {col} in scenario {df_wrong.index.to_list()}"
                 raise ValueError(msg)
         # Check that the skew factors sum to one by scenario and product group
         df_long = self.raw.melt(id_vars = self.cols + ["scenario"])
         index = ["scenario", "product_created", "variable"]
         df_long["value_sum"] = df_long.groupby(index)["value"].transform(sum)
         df_long_irw = df_long.query("product_created=='irw_and_fw'")
-        if not all(df_long_irw["value_sum"] == 1):
+        selector = np.isclose(df_long_irw["value_sum"], 1,  atol=1e-08)
+        if not all(selector):
             msg = "The following skew factors do not sum to one"
-            raise ValueError(msg, df_long_irw.query("value_sum !=1"))
+            raise ValueError(msg, df_long_irw.loc[~selector])
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/launch/associations.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/launch/associations.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/launch/create_json.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/launch/create_json.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/pump/classifiers.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/pump/classifiers.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/pump/column_order.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/pump/column_order.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/pump/long_or_wide.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/pump/long_or_wide.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/pump/post_processor.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/post_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/pump/pre_processor.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/pump/pre_processor.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/__init__.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/__init__.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/expected_provided.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/expected_provided.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/input_years.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/input_years.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/qaqc/silviculture.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/qaqc/silviculture.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/copy_data.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/copy_data.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/common/country_codes.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/common/country_codes.csv`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/growth_curves.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/growth_curves.csv`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/inventory.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/inventory.csv`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/transitions.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/mgmt/transitions.csv`

 * *Files 3% similar despite different names*

```diff
@@ -1,6 +1,6 @@
 scenario,from_status,from_forest_type,from_region,from_mgmt_type,from_mgmt_strategy,from_climate,from_con_broad,from_site_index,from_growth_period,using_id,sw_start,sw_end,hw_start,hw_end,dist_type_name,to_status,to_forest_type,to_region,to_mgmt_type,to_mgmt_strategy,to_climate,to_con_broad,to_site_index,to_growth_period,regen_delay,reset_age,percent
 reference,For,DF,LU00,H,E,?,con,1,Cur,FALSE,71,90,71,90,22,For,DF,LU00,H,E,?,con,1,Cur,0,0,100
 reference,For,OB,LU00,H,E,?,broad,1,Cur,FALSE,80,210,80,210,21,For,OB,LU00,H,E,?,broad,1,Cur,0,0,100
 reference,For,OC,LU00,H,E,?,con,1,Cur,FALSE,60,80,60,80,22,For,OC,LU00,H,E,?,con,1,Cur,0,0,100
 reference,For,QR,LU00,C,E,?,broad,1,Cur,FALSE,20,210,20,210,21,For,QR,LU00,C,E,?,broad,1,Cur,0,0,100
-reference,For,FS,LU00,H,U,?,broad,1,Cur,FALSE,20,40,20,40,15,For,FS,LU00,H,U,?,broad,1,Cur,0,1,30
+uneven_aged,For,FS,LU00,H,U,?,broad,1,Cur,FALSE,20,40,20,40,15,For,FS,LU00,H,U,?,broad,1,Cur,0,30,100
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/events.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/afforestation/events.csv`

 * *Files 26% similar despite different names*

```diff
@@ -1,3 +1,2 @@
-scenario,status,forest_type,region,mgmt_type,mgmt_strategy,climate,con_broad,site_index,growth_period,using_id,sw_start,sw_end,hw_start,hw_end,min_since_last_dist,max_since_last_dist,last_dist_id,min_tot_biom_c,max_tot_biom_c,min_merch_soft_biom_c,max_merch_soft_biom_c,min_merch_hard_biom_c,max_merch_hard_biom_c,min_tot_stem_snag_c,max_tot_stem_snag_c,min_tot_soft_stem_snag_c,max_tot_soft_stem_snag_c,min_tot_hard_stem_snag_c,max_tot_hard_stem_snag_c,min_tot_merch_stem_snag_c,max_tot_merch_stem_snag_c,min_tot_merch_soft_stem_snag_c,max_tot_merch_soft_stem_snag_c,min_tot_merch_hard_stem_snag_c,max_tot_merch_hard_stem_snag_c,efficiency,sort_type,measurement_type,dist_type_name,amount_2021,amount_2022,amount_2023,amount_2024,amount_2025,amount_2026,amount_2027,amount_2028,amount_2029,amount_2030,amount_2031,amount_2032,amount_2033,amount_2034,amount_2035,amount_2036,amount_2037,amount_2038,amount_2039,amount_2040,amount_2041,amount_2042,amount_2043,amount_2044,amount_2045,amount_2046,amount_2047,amount_2048,amount_2049,amount_2050,amount_2051,amount_2052,amount_2053,amount_2054,amount_2055,amount_2056,amount_2057,amount_2058,amount_2059,amount_2060,amount_2061,amount_2062,amount_2063,amount_2064,amount_2065,amount_2066,amount_2067,amount_2068,amount_2069,amount_2070
-reference,For,PA,LU00,?,?,35,con,1,Cur,FALSE,50,200,50,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,6,A,4,,,,100,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-reference,For,PA,LU00,?,?,45,con,1,Cur,FALSE,50,200,50,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,6,A,4,,,,100,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
+scenario,status,forest_type,region,mgmt_type,mgmt_strategy,climate,con_broad,site_index,growth_period,using_id,sw_start,sw_end,hw_start,hw_end,min_since_last_dist,max_since_last_dist,last_dist_id,min_tot_biom_c,max_tot_biom_c,min_merch_soft_biom_c,max_merch_soft_biom_c,min_merch_hard_biom_c,max_merch_hard_biom_c,min_tot_stem_snag_c,max_tot_stem_snag_c,min_tot_soft_stem_snag_c,max_tot_soft_stem_snag_c,min_tot_hard_stem_snag_c,max_tot_hard_stem_snag_c,min_tot_merch_stem_snag_c,max_tot_merch_stem_snag_c,min_tot_merch_soft_stem_snag_c,max_tot_merch_soft_stem_snag_c,min_tot_merch_hard_stem_snag_c,max_tot_merch_hard_stem_snag_c,efficiency,sort_type,measurement_type,dist_type_name,amount_2021,amount_2022,amount_2023,amount_2024,amount_2025,amount_2026,amount_2027,amount_2028,amount_2029,amount_2030,amount_2031,amount_2032,amount_2033,amount_2034,amount_2035,amount_2036,amount_2037,amount_2038,amount_2039,amount_2040,amount_2041,amount_2042,amount_2043,amount_2044,amount_2045,amount_2046,amount_2047,amount_2048,amount_2049,amount_2050
+reference,NF,NF_OC,?,?,?,?,con,1,Cur,FALSE,0,200,0,200,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1,3,A,8,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/transitions.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/activities/nd_sr/transitions.csv`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/age_classes.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/age_classes.csv`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/classifiers.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/classifiers.csv`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/disturbance_types.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/common/disturbance_types.csv`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 dist_type_name,dist_desc_input,silv_practice
 2,Wild Fire,#NA
-4,"Windstorm, with some salvage logging in the initial year",sr
+4,Windstorm (for CP),sr
 5,Generic 60% (INSECTS widespread),nr
 7,Deforestation,d
 8,Afforestation,ar
 11,Generic 15%,th
 12,15% commercial thinning,th
 14,20% commercial thinning,th
 15,Generic 20%,th
 16,30% commercial thinning,th
 18,35% commercial thinning,th
 21,Clearcut  with slash burn (broad based on area),fc
 22,Generic 90 % mortality (clearcut conif on area),fc
 29,Salvage year 1 post-windstorm,sr
 30,Salvage year 2 post-windstorm,sr
 42,Insects with salvage logging (within year),nr
+49,Windstorm (for projection),sr
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/config/associations.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/config/associations.csv`

 * *Files 11% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 MapDisturbanceType,Wild Fire,Wild Fire
 MapDisturbanceType,Deforestation,Deforestation
 MapDisturbanceType,Afforestation,Afforestation
 MapDisturbanceType,Generic 15%,generic 15% mortality
 MapDisturbanceType,Generic 20%,generic 20% mortality
 MapDisturbanceType,Generic 25%,generic 25% mortality
 MapDisturbanceType,Generic 60% (INSECTS widespread),generic 60% mortality
-MapDisturbanceType,"Windstorm, with some salvage logging in the initial year","Windstorm, with some salvage logging in the initial year"
+MapDisturbanceType,Windstorm (for CP),Windstorm
+MapDisturbanceType,Windstorm (for projection),Windstorm
 MapDisturbanceType,Generic 90 % mortality (clearcut conif on area),generic 90% mortality
 MapDisturbanceType,Salvage year 1 post-windstorm,Salvage year 1 post-windstorm
 MapDisturbanceType,Salvage year 2 post-windstorm,Salvage year 2 post-windstorm
 MapDisturbanceType,Clearcut  with slash burn (broad based on area),Clearcut with slash-burn
 MapDisturbanceType,10% commercial thinning,10% Commercial thinning
 MapDisturbanceType,15% commercial thinning,15% Commercial thinning
 MapDisturbanceType,20% commercial thinning,20% Commercial thinning
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/events_templates.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/countries/ZZ/silv/events_templates.csv`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,18 @@
 scenario,status,forest_type,region,mgmt_type,mgmt_strategy,climate,con_broad,site_index,growth_period,product_created,dist_interval_bias,using_id,sw_start,sw_end,hw_start,hw_end,min_since_last_dist,max_since_last_dist,last_dist_id,sort_type,disturbance_type,dist_type_name,min_tot_biom_c,max_tot_biom_c,min_merch_soft_biom_c,max_merch_soft_biom_c,min_merch_hard_biom_c,max_merch_hard_biom_c,min_tot_stem_snag_c,max_tot_stem_snag_c,min_tot_soft_stem_snag_c,max_tot_soft_stem_snag_c,min_tot_hard_stem_snag_c,max_tot_hard_stem_snag_c,min_tot_merch_stem_snag_c,max_tot_merch_stem_snag_c,min_tot_merch_soft_stem_snag_c,max_tot_merch_soft_stem_snag_c,min_tot_merch_hard_stem_snag_c,max_tot_merch_hard_stem_snag_c,efficiency
-reference,For,OB,LU00,H,E,35,broad,1,Cur,fw_only,5,FALSE,61,50,61,50,5,-1,-1,3,11,Generic 15%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,QR,LU00,H,E,35,broad,1,Cur,fw_only,5,FALSE,36,117,36,117,5,-1,-1,3,11,Generic 15%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OB,LU00,H,E,45,broad,1,Cur,fw_only,5,FALSE,61,50,61,50,5,-1,-1,3,11,Generic 15%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,QR,LU00,H,E,45,broad,1,Cur,fw_only,5,FALSE,36,117,36,117,5,-1,-1,3,11,Generic 15%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OB,LU00,H,E,35,broad,1,Cur,fw_only,5,FALSE,20,50,20,50,5,-1,-1,3,18,35% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OB,LU00,H,E,45,broad,1,Cur,irw_and_fw,15,FALSE,20,50,20,50,5,-1,-1,3,18,35% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OB,LU00,H,E,35,broad,1,Cur,irw_and_fw,10,FALSE,51,210,51,210,5,-1,-1,3,21,Clearcut  with slash burn (broad based on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,QR,LU00,C,E,35,broad,1,Cur,irw_and_fw,5,FALSE,21,210,21,210,5,-1,-1,3,21,Clearcut  with slash burn (broad based on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OB,LU00,H,E,45,broad,1,Cur,irw_and_fw,10,FALSE,51,210,51,210,5,-1,-1,3,21,Clearcut  with slash burn (broad based on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,QR,LU00,C,E,45,broad,1,Cur,irw_and_fw,10,FALSE,21,210,21,210,5,-1,-1,3,21,Clearcut  with slash burn (broad based on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,DF,LU00,H,E,35,con,1,Cur,fw_only,5,FALSE,36,50,36,50,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OC,LU00,H,E,35,con,1,Cur,fw_only,5,FALSE,26,40,26,40,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,35,con,1,Cur,fw_only,5,FALSE,26,40,26,40,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,DF,LU00,H,E,45,con,1,Cur,fw_only,5,FALSE,36,50,36,50,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OC,LU00,H,E,45,con,1,Cur,fw_only,5,FALSE,26,40,26,40,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,45,con,1,Cur,fw_only,5,FALSE,26,40,26,40,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,DF,LU00,H,E,35,con,1,Cur,fw_only,5,FALSE,51,90,51,90,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OC,LU00,H,E,35,con,1,Cur,fw_only,5,FALSE,41,60,41,60,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,35,con,1,Cur,irw_and_fw,10,FALSE,41,60,41,60,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,DF,LU00,H,E,45,con,1,Cur,irw_and_fw,10,FALSE,51,90,51,90,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OC,LU00,H,E,45,con,1,Cur,irw_and_fw,10,FALSE,41,60,41,60,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,45,con,1,Cur,irw_and_fw,10,FALSE,41,60,41,60,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,DF,LU00,H,E,35,con,1,Cur,irw_and_fw,10,FALSE,91,210,91,210,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OC,LU00,H,E,35,con,1,Cur,irw_and_fw,10,FALSE,61,210,61,210,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,35,con,1,Cur,irw_and_fw,10,FALSE,61,200,61,200,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,DF,LU00,H,E,45,con,1,Cur,irw_and_fw,10,FALSE,91,210,91,210,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,OC,LU00,H,E,45,con,1,Cur,irw_and_fw,10,FALSE,61,210,61,210,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,45,con,1,Cur,irw_and_fw,10,FALSE,61,200,61,200,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,35,con,1,Cur,irw_and_fw,1,FALSE,1,2,1,2,-1,-1,4,7,29,Salvage year 1 post-windstorm,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,35,con,1,Cur,irw_and_fw,1,FALSE,0,2,0,2,-1,-1,29,7,30,Salvage year 2 post-windstorm,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,45,con,1,Cur,irw_and_fw,1,FALSE,1,2,1,2,-1,-1,4,7,29,Salvage year 1 post-windstorm,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,PA,LU00,H,E,45,con,1,Cur,irw_and_fw,1,FALSE,0,2,0,2,-1,-1,29,7,30,Salvage year 2 post-windstorm,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
-reference,For,FS,LU00,H,U,?,?,1,Cur,irw_and_fw,6,FALSE,20,40,20,40,1,-1,-1,3,15,Generic 20%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,QR,LU00,H,E,?,broad,1,Cur,irw_and_fw,5,FALSE,36,117,36,117,5,-1,-1,3,11,Generic 15%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,OB,LU00,H,E,?,broad,1,Cur,irw_and_fw,5,FALSE,61,50,61,50,5,-1,-1,3,11,Generic 15%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,OB,LU00,H,E,?,broad,1,Cur,irw_and_fw,5,FALSE,20,50,20,50,5,-1,-1,3,18,35% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,OB,LU00,H,E,?,broad,1,Cur,irw_and_fw,10,FALSE,51,210,51,210,5,-1,-1,3,21,Clearcut  with slash burn (broad based on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,QR,LU00,C,E,?,broad,1,Cur,fw_only,5,FALSE,21,210,21,210,5,-1,-1,3,21,Clearcut  with slash burn (broad based on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,DF,LU00,H,E,?,con,1,Cur,fw_only,5,FALSE,36,50,36,50,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,OC,LU00,H,E,?,con,1,Cur,fw_only,5,FALSE,26,40,26,40,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,PA,LU00,H,E,?,con,1,Cur,fw_only,5,FALSE,26,40,26,40,5,-1,-1,3,12,15% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,DF,LU00,H,E,?,con,1,Cur,irw_and_fw,10,FALSE,51,90,51,90,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,OC,LU00,H,E,?,con,1,Cur,irw_and_fw,10,FALSE,41,60,41,60,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,PA,LU00,H,E,?,con,1,Cur,irw_and_fw,10,FALSE,41,60,41,60,5,-1,-1,3,14,20% commercial thinning,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,DF,LU00,H,E,?,con,1,Cur,irw_and_fw,10,FALSE,91,210,91,210,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,OC,LU00,H,E,?,con,1,Cur,irw_and_fw,10,FALSE,61,210,61,210,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,PA,LU00,H,E,?,con,1,Cur,irw_and_fw,10,FALSE,61,200,61,200,5,-1,-1,3,22,Generic 90 % mortality (clearcut conif on area),-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,PA,LU00,H,E,?,con,1,Cur,irw_and_fw,1,FALSE,1,2,1,2,-1,-1,49,7,29,Salvage year 1 post-windstorm,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+reference,For,PA,LU00,H,E,?,con,1,Cur,irw_and_fw,1,FALSE,0,2,0,2,-1,-1,29,7,30,Salvage year 2 post-windstorm,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
+uneven_aged,For,FS,LU00,H,U,?,broad,1,Cur,irw_and_fw,6,FALSE,20,40,20,40,1,-1,-1,3,15,Generic 20%,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,-1,1
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/fw_harvest.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/fw_harvest.csv`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 faostat_name,element,unit,country,value_1992,value_1993,value_1994,value_1995,value_1996,value_1997,value_1998,value_1999,value_2000,value_2001,value_2002,value_2003,value_2004,value_2005,value_2006,value_2007,value_2008,value_2009,value_2010,value_2011,value_2012,value_2013,value_2014,value_2015,value_2016,value_2017,value_2018,value_2019,value_2020,value_2021,value_2022,value_2023,value_2024,value_2025,value_2026,value_2027,value_2028,value_2029,value_2030,value_2031,value_2032,value_2033,value_2034,value_2035,value_2036,value_2037,value_2038,value_2039,value_2040,value_2041,value_2042,value_2043,value_2044,value_2045,value_2046,value_2047,value_2048,value_2049,value_2050,value_2051,value_2052,value_2053,value_2054,value_2055,value_2056,value_2057,value_2058,value_2059,value_2060,value_2061,value_2062,value_2063,value_2064,value_2065,value_2066,value_2067,value_2068,value_2069,value_2070
-Fuelwood,Production,1000m3,Austria,2994,3149,3259,3059,3797,3423,3175,3095,2860,2905,3036,3336,3540,3685,4705,4796.377,5023.689,4583.553,4549.512,5065.139,5189.462,4956.972,5058.84,4979.064,4589.952,4908.713,5243.22,5579.035,5327.115,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333
+Fuelwood,Production,1000m3,Austria,2994,3149,3259,3059,3797,3423,3175,3095,2860,2905,3036,3336,3540,3685,4705,4796.377,5023.689,4583.553,4549.512,5065.139,5189.462,4956.972,5058.84,4979.064,4589.952,4908.713,5243.22,5579.035,5327.115,4899.508,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333,5383.123333
 Fuelwood,Production,1000m3,Belgium,0,0,0,0,0,0,0,0,550,550,550,550,600,650,670,740,700,725,713.525,892.753,892.753,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75,892.75
-Fuelwood,Production,1000m3,Bulgaria,1870,1710,887,874,1185,1179,1388.333,1101,2107,1635,2187,2187,2909,2678,2885,2526,2692,2375,2657,2841,2915.785,2778.358,2533.66,2848.199,2928.212,2989.255,2849.214,2709.256,2332.449,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333
-Fuelwood,Production,1000m3,Croatia,568,711,1012,860,832,1006,1107,1094,976,747,755,979,954,908,915,761,763,862,1056,1422,1557,1400,1652.811,1768.741,1768.454,2389,2175.341,2205.259,2206.911,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837
-Fuelwood,Production,1000m3,Cyprus,11.2,13.9,11.1,10.9,9.9,9.7,8.315,8.039,5.42,6.55,5.21,4.271,3.287,3.857,2.864,7.73,6.701,3.718,3.628,3.545,6.523,5.666,4.83,7.488,12.875,13.618,8.84,7.385,6.356,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527
-Fuelwood,Production,1000m3,Czechia,0,700,778,649,718,610,820,840,940,1010,1007,1180,1190,1225,1345,1770,1880,1733,1965,1914,2020,2182,2111,2336,2344,2376,4246,5922,6726,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333,5631.333333
+Fuelwood,Production,1000m3,Bulgaria,1870,1710,887,874,1185,1179,1388.333,1101,2107,1635,2187,2187,2909,2678,2885,2526,2692,2375,2657,2841,2915.785,2778.358,2533.66,2848.199,2928.212,2989.255,2849.214,2709.256,2332.449,2356.632,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333,2630.306333
+Fuelwood,Production,1000m3,Croatia,568,711,1012,860,832,1006,1107,1094,976,747,755,979,954,908,915,761,763,862,1056,1422,1557,1400,1652.811,1768.741,1768.454,2389,2175.341,2205.259,2206.911,2130.105,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837,2195.837
+Fuelwood,Production,1000m3,Cyprus,11.2,13.9,11.1,10.9,9.9,9.7,8.315,8.039,5.42,6.55,5.21,4.271,3.287,3.857,2.864,7.73,6.701,3.718,3.628,3.545,6.523,5.666,4.83,7.488,12.875,13.618,8.84,7.385,6.356,7.178,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527,7.527
+Fuelwood,Production,1000m3,Czechia,0,700,778,649,718,610,820,840,940,1010,1007,1180,1190,1225,1345,1770,1880,1733,1965,1914,2020,2182,2111,2336,2344,2376,4246,5922,6726,6726,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667,2263.666667
 Fuelwood,Production,1000m3,Denmark,485.3,541.3,555.9,560.6,627.4,625.3,546.9,556.5,699.2,685.2,730.1,907.4,949.7,1280.9,1155.2,1094.8,1056.1,1391.1,1362.2,1416.6,1827.7,2218,2068.7,2278.2,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1,2061.1
-Fuelwood,Production,1000m3,Estonia,807,1048,544,573,604,1370,693,804,1640,1880,1900,2100,1300,1050,1100,990,1152,1856.682,2520.77,2645.708,2744.63,2820.48,2579.036,3075,3191.667,4456.44,4755.909,4271.969,4135.531,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803
-Fuelwood,Production,1000m3,Finland,2878,4161,4101,4095,4094,4041,4119.117,4044,4114.782,4483,4859.566,4994.434,5117.407,5134.197,5290.309,5206.454,5471.4,6006.6,6705,7251.7,7695.371,7660.176,7831.82,7964.445,7107.138,7949.091,7758.731,8013.23,8937.012,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333
-Fuelwood,Production,1000m3,France,39403,37953,36397,35567,35029,33979,32890,31873,31046,30528,29917,29521,29082,24555.016,24675.001,20232,21714,23000,26756,22267,24924,27837,23626,25421,27099,24896,24148.187,24186.118,23444.464,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633
-Fuelwood,Production,1000m3,Germany,3795,3795,3795,7128,10850,8201,7397,6814,8803.793,13326.689,10615.997,13922.658,15727.768,18106.449,20136.061,21027.267,24502.186,22798.435,27295.11,25340.92,28562.698,28753.149,23610,23344.834,22162.428,22388.937,22358.98,23697.485,22261.463,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267
-Fuelwood,Production,1000m3,Greece,1637,1519,1354,1330,1338,1236,1197,1403,1601.407,1400.59,1093,1073.608,1225,1004.33,1099.88,794.84,794.84,747.273,711.481,857.179,794.84,1192.5,1065,1065,1065,1064.482,998.081,946.849,946.849,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333
-Fuelwood,Production,1000m3,Hungary,2175,2230,2066,1948,1853,1909,1871,2575.8,2596.9,2319,2398.2,2781,2672,3136,3246,2879,2561,2879.3,2993.983,3214.856,2958.918,2858.473,2679.404,2679.171,2636.15,2826.927,2817.977,2683.815,2683.815,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667
-Fuelwood,Production,1000m3,Ireland,50,57,60,64,66,63,73,73,73,32,34,30.1,19.546,19,16,32,52,167.273,181.021,194.543,204.765,209.37,206.257,202.795,316.364,166,186,286,285,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333
+Fuelwood,Production,1000m3,Estonia,807,1048,544,573,604,1370,693,804,1640,1880,1900,2100,1300,1050,1100,990,1152,1856.682,2520.77,2645.708,2744.63,2820.48,2579.036,3075,3191.667,4456.44,4755.909,4271.969,4390.378,4147.576,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803,4387.803
+Fuelwood,Production,1000m3,Finland,2878,4161,4101,4095,4094,4041,4119.117,4044,4114.782,4483,4859.566,4994.434,5117.407,5134.197,5290.309,5206.454,5471.4,6006.6,6705,7251.7,7695.371,7660.176,7831.82,7964.445,7107.138,7949.091,7758.731,8013.23,8937.012,8911.046,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333,8236.324333
+Fuelwood,Production,1000m3,France,39403,37953,36397,35567,35029,33979,32890,31873,31046,30528,29917,29521,29082,24555.016,24675.001,20232,21714,23000,26756,22267,24924,27837,23626,25421,27099,24896,24148.187,24186.118,23323.764,26725.681,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633,23926.25633
+Fuelwood,Production,1000m3,Germany,3795,3795,3795,7128,10850,8201,7397,6814,8803.793,13326.689,10615.997,13922.658,15727.768,18106.449,20136.061,21027.267,24502.186,22798.435,27295.11,25340.92,28562.698,28753.149,23610,23344.834,22162.428,22388.937,22358.98,23697.485,20237.358,23223.901,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267,22772.64267
+Fuelwood,Production,1000m3,Greece,1637,1519,1354,1330,1338,1236,1197,1403,1601.407,1400.59,1093,1073.608,1225,1004.33,1099.88,794.84,794.84,747.273,711.481,857.179,794.84,1192.5,1065,1065,1065,1064.482,998.081,946.849,946.849,946.849,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333,963.9263333
+Fuelwood,Production,1000m3,Hungary,2175,2230,2066,1948,1853,1909,1871,2575.8,2596.9,2319,2398.2,2781,2672,3136,3246,2879,2561,2879.3,2993.983,3214.856,2958.918,2858.473,2679.404,2679.171,2636.15,2826.927,2817.977,2683.815,2515.545,2515.545,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667,2728.535667
+Fuelwood,Production,1000m3,Ireland,50,57,60,64,66,63,73,73,73,32,34,30.1,19.546,19,16,32,52,167.273,181.021,194.543,204.765,209.37,206.257,202.795,316.364,166,186,286,285,285,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333,252.3333333
 Fuelwood,Production,1000m3,Italy,4832,4698,5481,5263,4958,9319,8891,10235,9187,9232,7887,8103,8438,9452,8783,9577,10349,9340,11429,10245,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839,10839
-Fuelwood,Production,1000m3,Latvia,700,1100,1110,1210,2530,2864,2845,2490,1680,1580,1198,990.81,970,950,979,1028,598.42,1736.28,2312,1184.384,1173,1258.298,1299,1200,1700,2200,2200,2555,2620,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333
-Fuelwood,Production,1000m3,Lithuania,1376,1780,1736,1090,1230,1149,1170,1124,1450,1480,1295,1320,1260,1130,1230,1305,1381.805,1782.809,1942.998,1658,2200,2431,2316,2110,2085,2015,1829,1771,1994,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667
-Fuelwood,Production,1000m3,Luxembourg,0,0,0,0,0,0,0,0,27.711,34.605,29.508,37.365,39.309,40.351,53.136,59.285,55.433,61.768,81.576,76.684,78.676,64.692,64.905,67.979,64.731,69.83,84.518,65.188,59.003,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667
+Fuelwood,Production,1000m3,Latvia,700,1100,1110,1210,2530,2864,2845,2490,1680,1580,1198,990.81,970,950,979,1028,598.42,1736.28,2312,1184.384,1173,1258.298,1299,1200,1700,2200,2200,2555,2620,2940,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333,2458.333333
+Fuelwood,Production,1000m3,Lithuania,1376,1780,1736,1090,1230,1149,1170,1124,1450,1480,1295,1320,1260,1130,1230,1305,1381.805,1782.809,1942.998,1658,2200,2431,2316,2110,2085,2015,1829,1771,1994,1885,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667,1864.666667
+Fuelwood,Production,1000m3,Luxembourg,0,0,0,0,0,0,0,0,27.711,34.605,29.508,37.365,39.309,40.351,53.136,59.285,55.433,61.768,81.576,76.684,78.676,64.692,64.905,67.979,64.731,69.83,84.518,65.188,59,45.7,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667,69.56966667
 Fuelwood,Production,1000m3,Malta ,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
-Fuelwood,Production,1000m3,Netherlands,161,175,180,163,123,123,150,162,160,136,136,290,290,290,290,290,290,290,290,290,290,290,357,1397,2301,2332,2378,2325.7,2323,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333,2342.233333
-Fuelwood,Production,1000m3,Poland,3882,3401,3041,2299,2442.5,2545.4,2246.1,2363.5,2464.4,2593.1,3211,3632,3396,3413.2,3617.2,3473.604,3803.834,4153.916,4124.416,4979.775,5043.141,5143.794,5184.868,5497,5295.143,5248.213,5358.506,5068.902,4720,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136
-Fuelwood,Production,1000m3,Portugal,500,500,500,500,550,550,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,1092.029,1047.65,1287.232,1243.714,1618.144,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03
-Fuelwood,Production,1000m3,Romania,2000,1100,2285,2163,2809,3692,3020,3220,3032.2,2618,3062,2903,3015,2959,4516,3769,4149.7,3969.2,2563.588,4014.177,5037.575,5103.239,4859.293,5079.301,5163.781,4913.883,5553.105,5641.341,4581.996,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814
-Fuelwood,Production,1000m3,Slovakia,0,490,628,436,505,339,249,261,277,268,259,304,304,297,307.074,416.622,554.515,586.098,509.893,642.995,587.073,689.79,560.06,559.794,515.173,591.109,523.62,599.63,523.73,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333
-Fuelwood,Production,1000m3,Slovenia,520,107,235,227,362,546,539,505,532,295,280,359,725,943.341,983.56,788.277,928.292,982.6,1104.045,1336.169,1120.99,1127.017,1588.66,1242.229,1271.712,1038.843,1118.134,1116.909,1076.511,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333
-Fuelwood,Production,1000m3,Spain,2300,2338,2317,3078,3198,3198,1710,1650,1600,1855,1989,2030,2055,2180,1607,1982,2600,2080,5120,3900,3030,3435,3709,4522.871,2923.306,2268.594,3506.321,2951.198,2951.198,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239
-Fuelwood,Production,1000m3,Sweden,3800,3800,3800,3800,3800,3800,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,7000,6900,6600,5466,5460,5460,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462
+Fuelwood,Production,1000m3,Netherlands,161,175,180,163,123,123,150,162,160,136,136,290,290,290,290,290,290,290,290,290,290,290,357,1397,2301,2332,2378,2325.7,2303.52,2362.278,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75,1596.75
+Fuelwood,Production,1000m3,Poland,3882,3401,3041,2299,2442.5,2545.4,2246.1,2363.5,2464.4,2593.1,3211,3632,3396,3413.2,3617.2,3473.604,3803.834,4153.916,4124.416,4979.775,5043.141,5143.794,5184.868,5497,5295.143,5248.213,5358.506,5068.902,4713.304,4512,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136,5049.136
+Fuelwood,Production,1000m3,Portugal,500,500,500,500,550,550,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,600,1092.029,1047.65,1287.232,1243.714,1716.005,1762.427,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03,1383.03
+Fuelwood,Production,1000m3,Romania,2000,1100,2285,2163,2809,3692,3020,3220,3032.2,2618,3062,2903,3015,2959,4516,3769,4149.7,3969.2,2563.588,4014.177,5037.575,5103.239,4859.293,5079.301,5163.781,4913.883,5553.105,5641.341,6419.848,5163.98,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814,5258.814
+Fuelwood,Production,1000m3,Slovakia,0,490,628,436,505,339,249,261,277,268,259,304,304,297,307.074,416.622,554.515,586.098,509.893,642.995,587.073,689.79,560.06,559.794,515.173,591.109,523.62,599.63,523.73,495.054,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333,548.9933333
+Fuelwood,Production,1000m3,Slovenia,520,107,235,227,362,546,539,505,532,295,280,359,725,943.341,983.56,788.277,928.292,982.6,1104.045,1336.169,1120.99,1127.017,1588.66,1242.229,1271.712,1038.843,1118.134,1116.909,1073.65,1053.79,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333,1103.851333
+Fuelwood,Production,1000m3,Spain,2300,2338,2317,3078,3198,3198,1710,1650,1600,1855,1989,2030,2055,2180,1607,1982,2600,2080,5120,3900,3030,3435,3709,4522.871,2923.306,2268.594,3506.321,1615.429,2000.371,2000.371,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239,3136.239
+Fuelwood,Production,1000m3,Sweden,3800,3800,3800,3800,3800,3800,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,5900,7000,6900,6600,5466,5400,5400,5400,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462,5462
 Fuelwood,Production,1000m3,ZZ,0,0,0,0,0,0,0,0,28,35,30,37,39,40,53,59,55,62,82,77,79,65,65,68,65,70,73,74.00354108,75.10433091,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733,74.03595733
 Fuelwood,Production,1000m3,Algeria,5949,6151,6324,6430,6550,6713,6825,6948,7074,7188,7305,7424,7545,7669,7767,7867,7968,8072,8176,8246,8317,8388,8460,8533,8584,8635,8635,8598.12457,8672.821554,8734.997091,8796.933631,8854.942523,8914.30383,8973.170042,9032.238318,9091.453365,9150.472897,9209.567432,9268.618039,9342.555668,9431.043955,9515.308295,9601.922454,9688.627458,9776.248091,9864.490775,9953.469488,10043.08088,10133.39932,10224.43649,10316.19593,10408.67975,10501.89575,10595.84184,10665.78737,10742.27458,10817.18477,10892.93328,10970.6601,11046.5832,11123.89027,11201.31817,11279.36603,11357.81957,11436.77438,11516.08781,11595.90019,11676.18614,11756.95813,11838.21558,11919.96219,12002.74737,12084.89936,12167.95255,12251.20942,12333.27142,12418.85608,12502.94646,12588.37201
 Fuelwood,Production,1000m3,Angola,2484,2745,2791,2810,2840,2903,2982,3071,3163,3241,3320,3402,3487,3574,3656,3741,3828,3917,4009,4101,4194,4291,4390,4492,4583,4677,4677,4674.449762,4705.70361,4728.755931,4754.881641,4779.475583,4804.568501,4829.451346,4854.391713,4879.368487,4904.251282,4929.143682,4954.000666,4963.009181,4977.275032,4989.694246,5002.736177,5015.555384,5028.455976,5041.327832,5054.2108,5067.065723,5079.917786,5092.769327,5105.619728,5118.467893,5131.314708,5144.157614,5175.614679,5209.361106,5242.594981,5276.149704,5310.417629,5344.096758,5378.284692,5412.546939,5447.055283,5481.736229,5516.622743,5551.666062,5586.914482,5622.359452,5658.005394,5693.852263,5729.901477,5766.340902,5802.59953,5839.201813,5875.909768,5912.246938,5949.821805,5986.924393,6024.518984
 Fuelwood,Production,1000m3,Benin,5676,5737,5783,5828,5860,5894,5882,5896,5910,5937,5966,5996,6028,6061,6101,6141,6184,6228,6275,6318,6363,6409,6457,6507,6536,6568,6568,6572.875124,6599.820929,6621.564533,6649.584676,6676.666745,6704.093242,6731.417381,6758.808054,6786.252188,6813.66825,6841.121605,6868.584352,6895.838182,6926.49281,6956.096151,6986.198971,7016.269924,7046.501009,7076.823123,7107.26186,7137.792757,7168.432163,7199.18196,7230.042155,7261.012443,7292.093792,7323.284958,7352.8407,7383.857359,7414.537262,7445.41395,7476.735953,7507.675307,7538.929453,7570.222559,7601.663087,7633.204398,7664.867024,7696.620181,7728.493953,7760.482747,7792.589089,7824.812711,7857.154256,7889.729498,7922.185602,7954.846336,7987.5649,8020.049762,8053.285582,8086.225686,8119.459061
 Fuelwood,Production,1000m3,Botswana,603,613,617,624,627,630,628,631,635,640,645,650,655,661,665,669,674,679,683,686,690,693,696,699,699,699,699,700.1738527,703.7662303,706.8099385,711.2729533,715.650889,720.0809191,724.5152287,728.9720096,733.449938,737.940264,742.4501074,746.9765039,750.2323426,753.8607412,757.3773854,760.9510578,764.5239251,768.1169141,771.7225111,775.3435211,778.977291,782.625619,786.2887259,789.9666282,793.6593083,797.3668876,801.0892458,803.5730416,806.2110274,808.8066656,811.4182143,814.0726821,816.6798749,819.3157149,821.9501653,824.594988,827.2450919,829.902678,832.5643875,835.2334527,837.9092416,840.5920003,843.2816726,845.9783009,848.694312,851.3917246,854.105346,856.8193759,859.5025618,862.2604104,864.9807416,867.7265982
 Fuelwood,Production,1000m3,Burkina Faso,9625,9908,10187,10357,10489,10635,10782,7228,7402,7402,6009,6152,8040,10533,11060,11573,12418,12600,12785,12963,13145,13331,13520,13714,13870,14030,14030,14156.99516,14344.54394,14522.93756,14688.98569,14854.58028,15022.56829,15191.97166,15363.18474,15536.19595,15710.83498,15887.26781,16065.44652,16290.429,16526.42731,16762.97938,17003.82614,17247.7343,17495.21748,17746.15329,18000.65319,18258.70372,18520.39506,18785.78197,19054.9151,19327.84494,19604.62605,19885.30778,20198.61788,20520.59722,20846.39209,21177.55619,21514.89315,21856.10337,22203.27507,22555.68884,22913.74846,23277.40049,23646.79372,24021.92079,24402.96363,24789.99579,25183.11765,25582.42218,25988.00677,26400.3561,26818.38589,27243.27819,27674.63513,28111.52872,28557.51652,29009.02216,29468.24197
 Fuelwood,Production,1000m3,Burundi,5998,6184,6475,6684,7023,7205,7390,5252,5420,7952,8095,8241,8390,8542,8681,8822,8965,9111,9259,9397,5743,6007,5999,5999,5999,5999,5999,5963.764491,5944.823089,5921.191127,5886.592436,5851.270427,5816.364404,5781.482744,5746.773035,5712.223792,5677.766904,5643.458204,5609.275116,5586.588858,5566.642338,5545.82047,5525.372255,5504.872844,5484.474088,5464.121332,5443.834218,5423.593709,5403.412148,5383.290664,5363.228956,5343.226503,5323.283722,5303.399416,5283.263774,5264.1623,5244.799406,5225.556957,5206.60641,5187.369419,5168.332221,5149.303416,5130.357107,5111.461144,5092.629039,5073.840019,5055.113805,5036.446331,5017.838881,4999.290911,4980.802468,4962.446094,4943.999263,4925.665825,4907.353859,4888.885929,4870.863079,4852.646979,4834.59434
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/irw_harvest.csv` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/eu_cbm_data/domestic_harvest/reference/irw_harvest.csv`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 faostat_name,element,unit,country,value_1992,value_1993,value_1994,value_1995,value_1996,value_1997,value_1998,value_1999,value_2000,value_2001,value_2002,value_2003,value_2004,value_2005,value_2006,value_2007,value_2008,value_2009,value_2010,value_2011,value_2012,value_2013,value_2014,value_2015,value_2016,value_2017,value_2018,value_2019,value_2020,value_2021,value_2022,value_2023,value_2024,value_2025,value_2026,value_2027,value_2028,value_2029,value_2030,value_2031,value_2032,value_2033,value_2034,value_2035,value_2036,value_2037,value_2038,value_2039,value_2040,value_2041,value_2042,value_2043,value_2044,value_2045,value_2046,value_2047,value_2048,value_2049,value_2050,value_2051,value_2052,value_2053,value_2054,value_2055,value_2056,value_2057,value_2058,value_2059,value_2060,value_2061,value_2062,value_2063,value_2064,value_2065,value_2066,value_2067,value_2068,value_2069,value_2070
-Industrial roundwood,Production,1000m3,Austria,9855,9708,11701,11346,11812,11902,10858,10988,10416,10562,11810,13719,12943,12786,14430,16520.964,16771.739,12143.885,13281.444,13630.532,12831.218,12432.763,12029.72,12570.462,12173.081,12738.405,13948.84,13324.68,11462.455,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167
+Industrial roundwood,Production,1000m3,Austria,9855,9708,11701,11346,11812,11902,10858,10988,10416,10562,11810,13719,12943,12786,14430,16520.964,16771.739,12143.885,13281.444,13630.532,12831.218,12432.763,12029.72,12570.462,12173.081,12738.405,13948.84,13324.68,11462.455,13520.757,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167,12911.99167
 Industrial roundwood,Production,1000m3,Belgium,0,0,0,0,0,0,0,0,3960,3665,3950,4215,4250,4300,4405,4275,4000,3670,4113.9,4235.248,4235.248,4619.39,4519.39,4519.39,4519.39,4519.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39,4319.39
-Industrial roundwood,Production,1000m3,Bulgaria,1675,1837,1798,1970,2020,1862,1842.667,3250.667,2676.89,2356.89,2645.89,2645.89,3076.67,3183.67,3107,3170,3379,2224,3011,3364,3056.725,3025.914,3036.38,3523.903,3481.45,3416.013,3679.901,3454.443,3071.712,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Croatia,1421,1741,1804,1744,1710,2044,2291,2392,2693,2721,2886,2868,2887,3110,3537,3449,3706,3380,3421,3836,4157,4036,3343.779,3409.73,3396.825,2985.5,3214.38,3194.838,3026.956,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Cyprus,33.9,39.2,35.4,37.1,35.2,31.3,27.027,28.412,15.16,11.76,10.22,7.719,6.771,5.799,4.573,11.942,13.13,6.16,5.33,4.95,4.467,3.733,3.98,3.107,2.863,1.911,2.111,1.981,2.259,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Czechia,0,9706,11172,11716,11882,12881,13171,13363,13501,13364,13534,13960,14411,14285,16333,16738,14307,13769,14771,13467,13041,13149,13365,13827,15273,17011,21443,26664,26621,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334,24909.33334
+Industrial roundwood,Production,1000m3,Bulgaria,1675,1837,1798,1970,2020,1862,1842.667,3250.667,2676.89,2356.89,2645.89,2645.89,3076.67,3183.67,3107,3170,3379,2224,3011,3364,3056.725,3025.914,3036.38,3523.903,3481.45,3416.013,3679.901,3454.443,3071.712,3172.243,3402.018667,3347.646889,3330.172111,3422.150407,3359.945889,3366.656469,3370.756136,3382.917588,3365.786165,3373.443398,3373.153296,3374.04905,3370.794286,3373.548581,3372.665544,3372.797306,3372.336137,3373.003811,3372.599663,3372.712418,3372.646537,3372.771964,3372.652872,3372.710306,3372.690458,3372.711714,3372.684545,3372.704159,3372.695572,3372.70014,3372.694759,3372.699957,3372.696824,3372.698285,3372.69718,3372.698355,3372.69743,3372.69794,3372.697655,3372.697908,3372.697675,3372.697835,3372.697746,3372.697806,3372.697752,3372.697796,3372.697768,3372.697784,3372.697772
+Industrial roundwood,Production,1000m3,Croatia,1421,1741,1804,1744,1710,2044,2291,2392,2693,2721,2886,2868,2887,3110,3537,3449,3706,3380,3421,3836,4157,4036,3343.779,3409.73,3396.825,2985.5,3214.38,3194.838,3026.956,2855.686,3145.391333,3117.788889,3101.306667,3131.584296,3121.49563,3116.893284,3118.128864,3123.324403,3118.839259,3119.44885,3120.097509,3120.537504,3119.461873,3120.027955,3120.032295,3120.009111,3119.840708,3120.02312,3119.960705,3119.957646,3119.941511,3119.98049,3119.953287,3119.959882,3119.958429,3119.964553,3119.9572,3119.960955,3119.960061,3119.960903,3119.959405,3119.960639,3119.960123,3119.960316,3119.960056,3119.960359,3119.960165,3119.960244,3119.960193,3119.960256,3119.960201,3119.960231,3119.960217,3119.960229,3119.960216,3119.960226,3119.960221,3119.960224,3119.960221
+Industrial roundwood,Production,1000m3,Cyprus,33.9,39.2,35.4,37.1,35.2,31.3,27.027,28.412,15.16,11.76,10.22,7.719,6.771,5.799,4.573,11.942,13.13,6.16,5.33,4.95,4.467,3.733,3.98,3.107,2.863,1.911,2.111,1.981,2.259,2.855,2.117,2.080333333,2.125666667,2.066111111,2.107666667,2.090703704,2.099814815,2.088160494,2.099395062,2.092893004,2.095790123,2.093482853,2.096026063,2.094055327,2.09509968,2.094521414,2.095060357,2.094558807,2.094893817,2.094713526,2.09483766,2.09472205,2.094815001,2.094757745,2.09479157,2.094764932,2.094788106,2.094771416,2.094781536,2.094774818,2.094780353,2.094775923,2.094778902,2.094777031,2.094778393,2.094777286,2.094778109,2.09477757,2.094777929,2.094777655,2.094777869,2.094777718,2.094777818,2.094777747,2.094777802,2.094777761,2.094777789,2.09477777,2.094777784
+Industrial roundwood,Production,1000m3,Czechia,0,9706,11172,11716,11882,12881,13171,13363,13501,13364,13534,13960,14411,14285,16333,16738,14307,13769,14771,13467,13041,13149,13365,13827,15273,17011,21443,26664,26621,26621,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155,14155
 Industrial roundwood,Production,1000m3,Denmark,1430.199,1236.499,1296.498,1365.2,1248.9,1192.201,1298.5,1413.1,3961.4,1506.6,1139.9,1192.3,1225.5,2285.5,1641.4,1915.7,1808.2,1322.2,1695.3,1478.3,1592.6,1644.6,2097.5,2033.1,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781,1781
-Industrial roundwood,Production,1000m3,Estonia,1339,1391,3006,3137,3297,4023,5368,5900,7270,8320,8600,8400,5500,4450,4300,3510,3708,3779.372,4969.158,5352.137,6299.793,6227.542,6229.207,6440.031,7027.273,7002.197,7469.621,6715.001,6502.046,6895.556,6704.201,6700.601,6766.786,6723.862667,6730.416556,6740.355074,6731.544765,6734.105465,6735.335102,6733.661777,6734.367448,6734.454776,6734.161334,6734.327852,6734.314654,6734.267947,6734.303484,6734.295362,6734.288931,6734.295926,6734.293406,6734.292754,6734.294029,6734.293396,6734.293393,6734.293606,6734.293465,6734.293488,6734.29352,6734.293491,6734.2935,6734.293503,6734.293498,6734.2935,6734.293501,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935
-Industrial roundwood,Production,1000m3,Finland,35604,38083,44644,46124,42503,47288,49540.863,49593,50147.073,47727,48529,49246,49280.858,47115.985,45521.308,51405.725,45460.2,36151.2,45419.6,45526.2,44614.134,49331.404,49201.63,51446.439,54326.736,55330.267,60530.434,55653.634,51296.256,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467
-Industrial roundwood,Production,1000m3,France,29286,26597,29228,30205,27593,28924,29424,29855,39476,33792,29384,27459,28187,27943.721,28591.795,29816.654,27651.1,29080.771,29302.9,28387.152,24945.18,24451.174,25750.288,24998.331,25085.919,25360.656,25720.647,25444.856,24258.629,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Germany,29159,29357,36018,37314,39087,41366,42118,41905,49221.754,41291.965,41947.182,45468.297,50319.04,56019.19,58177.907,70582.738,50312.967,41366.014,47136.967,49876.845,45851.363,44699.687,45386,45653.67,44016.425,43328.442,52873.678,54123.509,61789.517,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466
-Industrial roundwood,Production,1000m3,Greece,684,699,737,631,674,508,495,811,643.528,514.932,498.297,599.248,468.678,518.527,461.96,948.076,948.076,286.624,336.481,339.147,816.822,393.9,367,367,367,571.644,455.12,412.256,412.256,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Hungary,2831,2266,2461,2383,1800,2332,2296,2655,3305.1,3492,3438.2,3004,2988.3,2804,2667,2761,2715,2364.7,2746.292,3017.594,2987.197,3168.729,3118.758,3064.798,2950.019,2862.443,3038.027,2891.608,2891.608,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Ireland,1910,1764,1958,2140,2225,2117,2193,2511,2600.1,2423,2612.1,2653.2,2542.489,2629,2655,2678,2180,2261.499,2436.975,2440.783,2375.654,2550.253,2621.729,2705.195,2734.059,3513,3578,3677,3627,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Italy,3525,4120,3984,4473,4163,3924,4367,4213,3649,2949,2628,2639,2883.316,3017.392,3012.753,2991.113,2993.678,2728.08,2647.228,2402.1,2176.5,2182.144,2245.5,2238.8,2218.5,2212.8,2206.6,7527.548,5002.077,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Latvia,1771,3831,4590,5690,5550,5833,7185,11518,12624,11261,12267.9,11925,11784,11892.6,11865.6,11144.9,8207.33,8706.03,10221.818,11649.108,11356.587,10983.572,11586.344,11094.416,11351.406,10696.149,10742.17,12267.065,12726.704,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967
-Industrial roundwood,Production,1000m3,Lithuania,1784,2728,2256,4870,4310,4000,3709,3800,4050,4220,4820,4955,4860,4915,4640,4890,4212.576,3676.722,5153.862,5346,4721,4622,5035,4304,4662,4780,5153,4917,4372,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814
-Industrial roundwood,Production,1000m3,Luxembourg,0,0,0,0,0,0,0,0,226.13,227.743,224.552,229.317,217.371,237.101,263.918,300.168,299.243,295.374,420.593,361.355,315.239,238.018,279.852,304.41,259.981,297.93,363.382,319.697,290.604,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561
+Industrial roundwood,Production,1000m3,Estonia,1339,1391,3006,3137,3297,4023,5368,5900,7270,8320,8600,8400,5500,4450,4300,3510,3708,3779.372,4969.158,5352.137,6299.793,6227.542,6229.207,6440.031,7027.273,7002.197,7469.621,6715.001,6897.955,6519.773,6704.201,6700.601,6766.786,6723.862667,6730.416556,6740.355074,6731.544765,6734.105465,6735.335102,6733.661777,6734.367448,6734.454776,6734.161334,6734.327852,6734.314654,6734.267947,6734.303484,6734.295362,6734.288931,6734.295926,6734.293406,6734.292754,6734.294029,6734.293396,6734.293393,6734.293606,6734.293465,6734.293488,6734.29352,6734.293491,6734.2935,6734.293503,6734.293498,6734.2935,6734.293501,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935,6734.2935
+Industrial roundwood,Production,1000m3,Finland,35604,38083,44644,46124,42503,47288,49540.863,49593,50147.073,47727,48529,49246,49280.858,47115.985,45521.308,51405.725,45460.2,36151.2,45419.6,45526.2,44614.134,49331.404,49201.63,51446.439,54326.736,55330.267,60530.434,55653.634,51190.924,57802.85,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467,55826.77467
+Industrial roundwood,Production,1000m3,France,29286,26597,29228,30205,27593,28924,29424,29855,39476,33792,29384,27459,28187,27943.721,28591.795,29816.654,27651.1,29080.771,29302.9,28387.152,24945.18,24451.174,25750.288,24998.331,25085.919,25360.656,25720.647,25444.856,24064.28,26188.525,25141.37733,25070.73489,24969.57533,25240.2773,25060.56252,25093.52917,25090.13838,25131.45633,25081.41002,25105.04129,25101.00158,25105.96922,25095.81763,25104.00403,25100.92948,25101.93029,25100.25038,25102.28793,25101.03672,25101.48954,25101.19168,25101.60473,25101.23931,25101.42865,25101.34524,25101.42423,25101.33773,25101.39937,25101.36907,25101.38711,25101.36872,25101.38518,25101.37497,25101.38034,25101.37629,25101.38016,25101.3772,25101.37893,25101.37788,25101.37876,25101.378,25101.37853,25101.37822,25101.37843,25101.37825,25101.37839,25101.3783,25101.37836,25101.37831
+Industrial roundwood,Production,1000m3,Germany,29159,29357,36018,37314,39087,41366,42118,41905,49221.754,41291.965,41947.182,45468.297,50319.04,56019.19,58177.907,70582.738,50312.967,41366.014,47136.967,49876.845,45851.363,44699.687,45386,45653.67,44016.425,43328.442,52873.678,54123.509,58436.086,59187.467,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466,56262.23466
+Industrial roundwood,Production,1000m3,Greece,684,699,737,631,674,508,495,811,643.528,514.932,498.297,599.248,468.678,518.527,461.96,948.076,948.076,286.624,336.481,339.147,816.822,393.9,367,367,367,571.644,455.12,412.256,412.256,412.256,426.544,434.7284444,439.4911111,446.9819259,433.5878519,440.4004938,440.0202963,440.3234239,438.0028807,440.2480713,439.4488669,439.524792,439.233273,439.7405767,439.4023106,439.4995472,439.4587201,439.5474782,439.453526,439.5019152,439.4865748,439.5009731,439.480672,439.4964877,439.4894066,439.4927109,439.4888554,439.4928684,439.4903243,439.4914783,439.4906827,439.491557,439.4908284,439.4912393,439.4910227,439.4912083,439.4910302,439.4911568,439.491087,439.4911317,439.4910913,439.4911252,439.4911034,439.4911161,439.4911066,439.4911149,439.4911087,439.4911125,439.4911101
+Industrial roundwood,Production,1000m3,Hungary,2831,2266,2461,2383,1800,2332,2296,2655,3305.1,3492,3438.2,3004,2988.3,2804,2667,2761,2715,2364.7,2746.292,3017.594,2987.197,3168.729,3118.758,3064.798,2950.019,2862.443,3038.027,2891.608,2456.875,2456.875,2940.414333,2904.636222,2920.905,2925.247741,2921.985185,2916.929654,2922.712642,2921.387527,2920.542494,2920.343274,2921.547554,2920.757765,2920.811107,2920.882865,2921.038809,2920.817246,2920.910927,2920.912973,2920.922327,2920.880382,2920.915409,2920.905227,2920.906039,2920.900339,2920.908892,2920.903869,2920.90509,2920.904367,2920.90595,2920.904442,2920.905136,2920.90492,2920.905176,2920.904832,2920.905077,2920.904976,2920.905028,2920.904962,2920.905027,2920.904989,2920.905006,2920.904993,2920.905007,2920.904996,2920.905002,2920.904999,2920.905002,2920.904999,2920.905001
+Industrial roundwood,Production,1000m3,Ireland,1910,1764,1958,2140,2225,2117,2193,2511,2600.1,2423,2612.1,2653.2,2542.489,2629,2655,2678,2180,2261.499,2436.975,2440.783,2375.654,2550.253,2621.729,2705.195,2734.059,3513,3578,3677,3627,3627,3627.333333,3631.111111,3614.555556,3615.925926,3624.333333,3620.530864,3618.271605,3620.263374,3621.045267,3619.688615,3619.860082,3620.332419,3620.197988,3619.960372,3620.130163,3620.163593,3620.096174,3620.084709,3620.129977,3620.114826,3620.10362,3620.109837,3620.116141,3620.109428,3620.109866,3620.111802,3620.111812,3620.110365,3620.11116,3620.111326,3620.111112,3620.11095,3620.111199,3620.11113,3620.111087,3620.111093,3620.111139,3620.111103,3620.111106,3620.111112,3620.111116,3620.111107,3620.111111,3620.111112,3620.111112,3620.11111,3620.111112,3620.111111,3620.111111
+Industrial roundwood,Production,1000m3,Italy,3525,4120,3984,4473,4163,3924,4367,4213,3649,2949,2628,2639,2883.316,3017.392,3012.753,2991.113,2993.678,2728.08,2647.228,2402.1,2176.5,2182.144,2245.5,2238.8,2218.5,2212.8,2206.6,7527.548,5002.077,5002.077,4912.075,5503.980333,4632.156,4799.457111,5016.070444,4978.531148,4815.894519,4931.352901,4936.832037,4908.592856,4894.693152,4925.592598,4913.372682,4909.626202,4911.219477,4916.197161,4911.40612,4912.347613,4912.940919,4913.316965,4912.231551,4912.868499,4912.829812,4912.805672,4912.643287,4912.834661,4912.75959,4912.761207,4912.745846,4912.785153,4912.755548,4912.764068,4912.762182,4912.768256,4912.760599,4912.764836,4912.763679,4912.764564,4912.763038,4912.76436,4912.76376,4912.763987,4912.763719,4912.764036,4912.763822,4912.763914,4912.763859,4912.763924,4912.763865
+Industrial roundwood,Production,1000m3,Latvia,1771,3831,4590,5690,5550,5833,7185,11518,12624,11261,12267.9,11925,11784,11892.6,11865.6,11144.9,8207.33,8706.03,10221.818,11649.108,11356.587,10983.572,11586.344,11094.416,11351.406,10696.149,10742.17,12267.065,12726.7,13003,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967,11911.97967
+Industrial roundwood,Production,1000m3,Lithuania,1784,2728,2256,4870,4310,4000,3709,3800,4050,4220,4820,4955,4860,4915,4640,4890,4212.576,3676.722,5153.862,5346,4721,4622,5035,4304,4662,4780,5153,4917,4372,4729,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814,4814
+Industrial roundwood,Production,1000m3,Luxembourg,0,0,0,0,0,0,0,0,226.13,227.743,224.552,229.317,217.371,237.101,263.918,300.168,299.243,295.374,420.593,361.355,315.239,238.018,279.852,304.41,259.981,297.93,363.382,319.697,290.7,216.7,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561,324.561
 Industrial roundwood,Production,1000m3,Malta,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
-Industrial roundwood,Production,1000m3,Netherlands,1092,900,863,941,829,986,873,882,879,729,703,754,735.724,820,816.676,732.046,827.099,726.133,790.593,691.8,664.7,818.2,894.14,848.7,952.305,818.886,766.406,742,740,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667
-Industrial roundwood,Production,1000m3,Poland,18155,18229,18881,20193,19615,20951.4,22670.7,23654.3,25194.7,24078.3,25746,27204,29337,28531.3,28766.8,32460.959,30469.587,30475.256,31343.001,32200.207,32972.29,33795.049,35677.17,35878.282,37106.089,40064.42,41352.719,38199.031,35864,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667
-Industrial roundwood,Production,1000m3,Portugal,9778,9707,9319,8850,8428,8428,7948,8378,10231,8346,8142,9073,10269,10146.238,10204.638,10222.886,9568.749,8964.069,9048.36,10361.419,10110.813,10009.589,10552.372,10799.677,12011.4,12517.166,12045.609,12274.169,11692.4,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Romania,10440,7740,9640,10015,9441,9837,8629,9483.5,10116,9806,12092,12537,12794,11542,9454,11572,9517.3,8587.3,10548.052,10344.452,11050.337,10091.483,10470.62,10235.399,9952.933,9577.752,10436.1,10185.905,10947.587,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733
-Industrial roundwood,Production,1000m3,Slovakia,0,4759,4690,4887,4955,4606,5270,5534,5886,5519.9,5523,6051,6936,9005,7561.435,7714.864,8714.041,8500.893,9089.175,8569.912,7614.601,7372.797,8607.92,8434.81,8751.695,8770.383,9079.234,8357.244,6924.129,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Slovenia,1151,958,1709,1639,1629,1662,1594,1563,1721,1962,2003,2232,1826,1789.481,2195.566,2093.373,2061.77,1947.616,1841.404,2051.698,2220.099,2288.16,3510.68,3812.214,4109.679,3470.205,3921.157,3501.25,2804.466,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Spain,11624,11429,12988,12997,12433,12433,13164,13160,12721,13276,13850,14075,14235,13351,14109,12546,14427.374,11900.035,10969.399,11527.772,11626.795,12124.298,12686.343,12904.619,13324.989,14642.343,15457.14,15404.728,15356.347,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,,
-Industrial roundwood,Production,1000m3,Sweden,49720,50200,52500,59800,52500,56400,54700,52800,57400,57300,60700,61200,61400,92300,58700,72300,64900,59200,66300,66000,63599,63700,67400,67300,67900,67580,67712,70012,70600,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333
+Industrial roundwood,Production,1000m3,Netherlands,1092,900,863,941,829,986,873,882,879,729,703,754,735.724,820,816.676,732.046,827.099,726.133,790.593,691.8,664.7,818.2,894.14,848.7,952.305,818.886,766.406,742,662.4,647.934,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667,749.4686667
+Industrial roundwood,Production,1000m3,Poland,18155,18229,18881,20193,19615,20951.4,22670.7,23654.3,25194.7,24078.3,25746,27204,29337,28531.3,28766.8,32460.959,30469.587,30475.256,31343.001,32200.207,32972.29,33795.049,35677.17,35878.282,37106.089,40064.42,41352.719,38199.031,35859.476,38498,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667,38471.91667
+Industrial roundwood,Production,1000m3,Portugal,9778,9707,9319,8850,8428,8428,7948,8378,10231,8346,8142,9073,10269,10146.238,10204.638,10222.886,9568.749,8964.069,9048.36,10361.419,10110.813,10009.589,10552.372,10799.677,12011.4,12517.166,12045.609,12256.202,11031.919,11883.014,12004.05933,12081.85011,11991.81356,12121.63026,12025.90767,12065.09798,12046.45049,12070.87863,12045.81871,12060.80903,12054.38261,12059.16879,12053.67012,12058.12015,12055.74051,12056.98635,12055.84359,12056.949,12056.19015,12056.59298,12056.32758,12056.57738,12056.37024,12056.49931,12056.42507,12056.48231,12056.43154,12056.4689,12056.44631,12056.46092,12056.44891,12056.45871,12056.45205,12056.45618,12056.45322,12056.45564,12056.45382,12056.45501,12056.45423,12056.45482,12056.45435,12056.45469,12056.45447,12056.45462,12056.4545,12056.45459,12056.45453,12056.45457,12056.45454
+Industrial roundwood,Production,1000m3,Romania,10440,7740,9640,10015,9441,9837,8629,9483.5,10116,9806,12092,12537,12794,11542,9454,11572,9517.3,8587.3,10548.052,10344.452,11050.337,10091.483,10470.62,10235.399,9952.933,9577.752,10436.1,10185.905,11628.68,12247.036,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733,10523.19733
+Industrial roundwood,Production,1000m3,Slovakia,0,4759,4690,4887,4955,4606,5270,5534,5886,5519.9,5523,6051,6936,9005,7561.435,7714.864,8714.041,8500.893,9089.175,8569.912,7614.601,7372.797,8607.92,8434.81,8751.695,8770.383,9079.234,8357.244,6924.129,7169.702,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104,8867.104
+Industrial roundwood,Production,1000m3,Slovenia,1151,958,1709,1639,1629,1662,1594,1563,1721,1962,2003,2232,1826,1789.481,2195.566,2093.373,2061.77,1947.616,1841.404,2051.698,2220.099,2288.16,3510.68,3812.214,4109.679,3470.205,3921.157,3501.25,2817.133,2656.408,3408.957667,3312.195556,3281.431444,3450.67463,3334.194889,3348.100543,3355.433654,3377.656687,3345.909695,3360.396962,3359.666679,3361.321115,3355.324445,3360.461585,3358.770746,3359.035715,3358.185592,3359.422682,3358.664018,3358.88133,3358.757431,3358.989343,3358.767593,3358.876035,3358.838122,3358.877657,3358.82725,3358.863938,3358.847676,3358.856282,3358.846288,3358.855965,3358.850082,3358.852845,3358.850778,3358.852964,3358.851235,3358.852196,3358.851659,3358.852132,3358.851697,3358.851996,3358.851829,3358.851941,3358.851841,3358.851922,3358.85187,3358.851901,3358.851878
+Industrial roundwood,Production,1000m3,Spain,11624,11429,12988,12997,12433,12433,13164,13160,12721,13276,13850,14075,14235,13351,14109,12546,14427.374,11900.035,10969.399,11527.772,11626.795,12124.298,12686.343,12904.619,13324.989,14642.343,15457.14,15404.728,13880.625,13785.816,15406.07167,15309.71511,15310.163,15294.61904,15341.98326,15304.83238,15315.58843,15313.81156,15320.80136,15311.41079,15316.73378,15315.34124,15316.31531,15314.49527,15316.13011,15315.38394,15315.6469,15315.33644,15315.72032,15315.45576,15315.56788,15315.50417,15315.58132,15315.50927,15315.55113,15315.53159,15315.54724,15315.53066,15315.54332,15315.5365,15315.54041,15315.53682,15315.54007,15315.53791,15315.5391,15315.53827,15315.53903,15315.53843,15315.5388,15315.53857,15315.53875,15315.5386,15315.53871,15315.53864,15315.53869,15315.53865,15315.53868,15315.53866,15315.53867
+Industrial roundwood,Production,1000m3,Sweden,49720,50200,52500,59800,52500,56400,54700,52800,57400,57300,60700,61200,61400,92300,58700,72300,64900,59200,66300,66000,63599,63700,67400,67300,67900,67580,67712,69000,69000,69000,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333,69441.33333
 Industrial roundwood,Production,1000m3,ZZ,0,0,0,0,0,0,0,0,226,228,225,229,217,237,264,300,299,295,421,361,315,238,280,304,260,298,316,307.3328671,324.0349445,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706,315.7892706
 Industrial roundwood,Production,1000m3,Algeria,351,446,391,390,428,438,444,451,162,208,208,100,122,73,75,103,103,103,145,139,139,139,139,139,139,139,139,161.9165133,172.9430373,181.9518533,193.6622646,207.1881138,226.9264427,262.6594525,110.5819441,106.2174588,101.6781606,96.95058289,92.03529489,85.61642279,78.25072041,70.70219912,62.67009529,54.2432165,45.36631911,36.03837509,26.23689374,18.9094258,11.83332619,4.451923625,0,0,0,0.149352043,0.151034367,0.154086945,0.156696989,0.159405007,0.162464797,0.165025992,0.167804312,0.170515254,0.173270677,0.176021849,0.178789812,0.181541932,0.184309348,0.187085824,0.189873656,0.192672388,0.195484437,0.198446686,0.201165731,0.203989298,0.206758646,0.209155755,0.212251792,0.214906855,0.217763422
 Industrial roundwood,Production,1000m3,Angola,897,927,958,969,1000,1032,1064,1096,1096,1096,1096,1096,1096,1096,1096,1096,1096,1107,1127,1134,1141,1151,1165,1213,1220,1220,1220,1226.818447,1232.233352,1234.506757,1238.02354,1240.973184,1244.181394,1247.355429,1250.605183,1253.933647,1257.287046,1260.71308,1264.198895,1264.629476,1267.265756,1269.136376,1271.278225,1273.334986,1275.436481,1277.535642,1279.649858,1281.762521,1283.884736,1286.017831,1288.161834,1290.316228,1292.482983,1294.650682,1294.862753,1295.926731,1296.596439,1297.235971,1298.012155,1298.345567,1298.713766,1298.919071,1299.029993,1299.006766,1298.855588,1298.546889,1298.092067,1297.477093,1296.692678,1295.726577,1294.474627,1293.189072,1291.51079,1289.651061,1289.628465,1291.68804,1294.205822,1296.442547,1298.813689
 Industrial roundwood,Production,1000m3,Benin,296,303,310,300,304,315,326,332,332,357,387,387,387,387,512,427,427,427,467,467,522,471,498,292,385,385,385,388.558882,396.7912737,402.3650263,409.0435001,415.3250579,422.0730035,428.9592384,436.0888404,443.4644811,451.037903,458.866011,466.9349908,468.6806957,472.833959,476.1839786,479.8599228,483.4706361,487.1601902,490.8753375,494.6355592,498.4217842,502.2465844,506.1114341,510.016334,513.9609939,517.9462998,521.9282478,523.4261444,526.062003,528.3323655,530.685791,533.3333416,535.5679099,537.9846547,540.3468701,542.7476821,545.1464994,547.5608603,549.9635335,552.3804933,554.8065344,557.2435745,559.6912435,562.1516783,564.7401894,567.1266154,569.6021149,572.0336898,574.154488,576.8630996,579.2031826,581.7139394
 Industrial roundwood,Production,1000m3,Botswana,89,92,95,97,99,102,103,105,105,105,105,105,105,105,105,105,105,105,105,105,105,105,105,105,105,105,105,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0,0
 Industrial roundwood,Production,1000m3,Burkina Faso,421,433,449,463,475,490,501,592,594,594,1183,1185,1171,1171,1171,1171,1171,1171,1171,1171,1171,1171,1171,1171,1171,1171,1171,1179.442775,1212.848085,1231.467418,1253.810012,1273.209557,1293.398385,1313.067885,1332.725158,1352.3399,1371.668011,1390.915609,1410.00208,1425.663457,1451.899724,1474.564055,1498.634226,1522.388936,1546.459542,1570.619335,1594.955867,1619.387254,1643.97041,1668.71343,1693.617889,1718.68414,1743.916985,1769.312923,1794.875966,1825.76487,1855.373474,1885.683225,1917.666126,1948.145041,1979.806821,2011.584215,2043.908234,2076.598163,2109.741096,2143.214649,2177.146346,2211.517732,2246.344109,2281.629116,2317.380319,2354.114719,2390.275982,2427.298079,2464.527859,2500.61766,2540.107483,2578.167835,2617.543369
 Industrial roundwood,Production,1000m3,Burundi,615,615,615,688,688,688,688,688,767,767,767,845,845,883,883,883,883,883,883,883,617,625,625,625,625,625,625,623.331001,623.9981065,623.8770706,623.9792268,623.929139,623.9222036,623.8900803,623.8581658,623.8248154,623.7781186,623.7282586,623.6713139,623.4431812,623.7018001,623.787208,623.9286663,624.0477664,624.172752,624.2934088,624.4134479,624.5292686,624.6432236,624.7555501,624.8662126,624.9751303,625.0824097,625.1867592,625.2270907,625.4590022,625.6251888,625.8018334,626.0239121,626.1741393,626.3511995,626.5160968,626.6840511,626.8484656,627.0121659,627.1708236,627.3285832,627.4846184,627.6392288,627.7923319,627.9440134,628.1103251,628.2427135,628.3853887,628.5183166,628.6021286,628.7698562,628.8800996,629.012207
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/test_salvage.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/test_salvage.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 
 Inspired by the use in pandas
 https://github.com/pandas-dev/pandas/blob/main/pandas/tests/strings/test_find_replace.py
 """
 
 from eu_cbm_hat.core.continent import continent
 
-combo  = continent.combos['hat']
-runner = combo.runners['ZZ'][-1]
+runner = continent.combos['reference'].runners['ZZ'][-1]
 
-# runner.num_timesteps = 30
-# runner.run(keep_in_ram=True, verbose=True, interrupt_on_error=True)
 
 def test_dist_4_followed_by_29():
     """Disturbance 4 followed by disturbance 29 salvage logging. Prepare input
     data for ZZ Trying to overwrite as much as possible of the input data with
     these data frames """
     # Overwrite the natural disturbance activity
     # events, inventory, growth curves and transitions
@@ -32,15 +29,16 @@
     # Some files are transformed from wide to long format in this process.
 
     # Overwrite the events template
     # reference	For	PA	LU00	H	E	35	con	1	Cur	irw_and_fw	1	FALSE	0	5	0	5
     # reference	For	PA	LU00	H	E	45	con	1	Cur	irw_and_fw	1	FALSE	0	5	0	5
 
     # Run the model
-
+    runner.num_timesteps = 30
+    runner.run(keep_in_ram=True, verbose=True, interrupt_on_error=True)
 
     # Check output
     print(runner.input_data["events"])
 
     # assert [1,2] == [1,2]
     # assert (np.array([1,2]) == np.array([1,2])).all()
     # np.testing.assert_allclose(np.array([1,2]),np.array([1,3]))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat/tests/test_silviculture.py` & `eu_cbm_hat-0.6.5/eu_cbm_hat/tests/test_silviculture.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 
 """
 
 import numpy as np
 import pandas
 import pytest
 from eu_cbm_hat.core.continent import continent
-combo  = continent.combos['hat']
-runner = combo.runners['ZZ'][-1]
+
+runner = continent.combos['reference'].runners['ZZ'][-1]
 
 harvest_factors_1 = {'scenario': ['reference', 'reference', 'reference', 'no_skew', 'no_skew'],
                      'product_created': ['irw_and_fw', 'irw_and_fw', 'fw_only', 'irw_and_fw', 'fw_only'],
                      'forest_type': np.nan,
                      'silv_practice': np.nan,
                      'mgmt_type': np.nan,
                      'con_broad': ['con', 'broad', np.nan, np.nan, np.nan],
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/PKG-INFO` & `eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eu-cbm-hat
-Version: 0.6.4
+Version: 0.6.5
 Summary: eu_cbm_hat is a python package for running carbon budget simulations.
 Home-page: https://gitlab.com/bioeconomy/eu_cbm/eu_cbm_hat
 Author: Lucas Sinclair
 Author-email: lucas.sinclair@me.com
 Maintainer: Paul Rougieux
 License: EUPL
 Requires-Python: >=3.8
```

### Comparing `eu_cbm_hat-0.6.4/eu_cbm_hat.egg-info/SOURCES.txt` & `eu_cbm_hat-0.6.5/eu_cbm_hat.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,30 +10,18 @@
 eu_cbm_hat.egg-info/requires.txt
 eu_cbm_hat.egg-info/top_level.txt
 eu_cbm_hat/cbm/__init__.py
 eu_cbm_hat/cbm/dynamic.py
 eu_cbm_hat/cbm/simulation.py
 eu_cbm_hat/combos/__init__.py
 eu_cbm_hat/combos/base_combo.py
-eu_cbm_hat/combos/harvest_test.py
 eu_cbm_hat/combos/hat.py
 eu_cbm_hat/combos/historical.py
 eu_cbm_hat/combos/ia_2040.py
-eu_cbm_hat/combos/no_market_forcing.py
-eu_cbm_hat/combos/pikbau.py
-eu_cbm_hat/combos/pikfair.py
-eu_cbm_hat/combos/potencia_baseline.py
-eu_cbm_hat/combos/potencia_necp_bme_up100.py
-eu_cbm_hat/combos/potencia_necp_bme_up200.py
-eu_cbm_hat/combos/potencia_necp_bms_down50.py
-eu_cbm_hat/combos/potencia_necp_bms_down90.py
 eu_cbm_hat/combos/reference.py
-eu_cbm_hat/combos/reference_crf.py
-eu_cbm_hat/combos/skewfcth.py
-eu_cbm_hat/combos/special.py
 eu_cbm_hat/core/__init__.py
 eu_cbm_hat/core/continent.py
 eu_cbm_hat/core/country.py
 eu_cbm_hat/core/runner.py
 eu_cbm_hat/info/__init__.py
 eu_cbm_hat/info/aidb.py
 eu_cbm_hat/info/fluxes.py
@@ -42,19 +30,21 @@
 eu_cbm_hat/info/internal_data.py
 eu_cbm_hat/info/orig_data.py
 eu_cbm_hat/info/output_data.py
 eu_cbm_hat/info/silviculture.py
 eu_cbm_hat/launch/__init__.py
 eu_cbm_hat/launch/associations.py
 eu_cbm_hat/launch/create_json.py
+eu_cbm_hat/post_processor/__init__.py
+eu_cbm_hat/post_processor/harvest.py
+eu_cbm_hat/post_processor/sink.py
 eu_cbm_hat/pump/__init__.py
 eu_cbm_hat/pump/classifiers.py
 eu_cbm_hat/pump/column_order.py
 eu_cbm_hat/pump/long_or_wide.py
-eu_cbm_hat/pump/post_processor.py
 eu_cbm_hat/pump/pre_processor.py
 eu_cbm_hat/qaqc/__init__.py
 eu_cbm_hat/qaqc/aidb.py
 eu_cbm_hat/qaqc/expected_provided.py
 eu_cbm_hat/qaqc/input_years.py
 eu_cbm_hat/qaqc/silviculture.py
 eu_cbm_hat/tests/copy_data.py
```

### Comparing `eu_cbm_hat-0.6.4/scripts/conversion/add_indicators_to_aidb.py` & `eu_cbm_hat-0.6.5/scripts/conversion/add_indicators_to_aidb.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/conversion/convert_aidb.py` & `eu_cbm_hat-0.6.5/scripts/conversion/convert_aidb.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/conversion/merge_growth_curves.py` & `eu_cbm_hat-0.6.5/scripts/conversion/merge_growth_curves.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/conversion/rename_all_classifiers.py` & `eu_cbm_hat-0.6.5/scripts/conversion/rename_all_classifiers.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/conversion/rename_associations.py` & `eu_cbm_hat-0.6.5/scripts/conversion/rename_associations.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/conversion/update_input_classif.py` & `eu_cbm_hat-0.6.5/scripts/conversion/update_input_classif.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_at.py` & `eu_cbm_hat-0.6.5/scripts/running/run_at.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_ee.py` & `eu_cbm_hat-0.6.5/scripts/running/run_ee.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_fr.py` & `eu_cbm_hat-0.6.5/scripts/running/run_fr.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_hu.py` & `eu_cbm_hat-0.6.5/scripts/running/run_hu.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_lu.py` & `eu_cbm_hat-0.6.5/scripts/running/run_lu.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,24 +13,20 @@
 
      ipython3 -i -- ~/deploy/eu_cbm_hat/scripts/running/run_lu.py
 
 """
 
 from eu_cbm_hat.core.continent import continent
 
-
 #############################################
 # Declare which scenario combination to run #
 #############################################
-# Scenario combination defined in the yaml file 
+# Scenario combination defined in yaml files
 # `~/repos/eu_cbm_data/combos/harvest_test.yaml`
-# Scenario itself is defined as code in 
-# `~/repos/eu_cbm_hat/eu_cbm_hat/combos/harvest_test.py`
-combo   = continent.combos['hat']
-runner  = combo.runners['LU'][-1]
+runner = continent.combos['pikfair'].runners['LU'][-1]
 runner.num_timesteps = 25
 
 # Run the model
 output = runner.run(keep_in_ram=True, verbose=True, interrupt_on_error=True)
 
 # Input events sent to libcbm
 events_input = runner.input_data["events"]
```

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_scenario_combo.py` & `eu_cbm_hat-0.6.5/scripts/running/run_scenario_combo.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_se.py` & `eu_cbm_hat-0.6.5/scripts/running/run_se.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_si.py` & `eu_cbm_hat-0.6.5/scripts/running/run_si.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,16 +12,15 @@
 
 from eu_cbm_hat.core.continent import continent
 
 
 #############################################
 # Declare which scenario combination to run #
 #############################################
-combo   = continent.combos['reference']
-runner  = combo.runners['SI'][-1]
+runner  = continent.combos['reference'].runners['SI'][-1]
 runner.num_timesteps = 50
 
 # Run the model
 output = runner.run(keep_in_ram=True, verbose=True, interrupt_on_error=True)
```

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_zz.py` & `eu_cbm_hat-0.6.5/scripts/running/run_zz.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/running/run_zz_in_temp_dir_without_eu_cbm_data.py` & `eu_cbm_hat-0.6.5/scripts/running/run_zz_in_temp_dir_without_eu_cbm_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from eu_cbm_hat import module_dir
 orig_path = Path(module_dir) / "tests/eu_cbm_data"
 # Copy ZZ test data to a temporary directory
 shutil.copytree(orig_path, dest_path)
 
 # This has to happen after we copy ZZ data to a temporary directory
 from eu_cbm_hat.core.continent import continent
-runner = continent.combos['hat'].runners['ZZ'][-1]
+runner = continent.combos['reference'].runners['ZZ'][-1]
 # Create the AIDB symlink
 runner.country.aidb.symlink_all_aidb()
 runner.num_timesteps = 30
 # Run the test country ZZ
 runner.run(keep_in_ram=True, verbose=True, interrupt_on_error=True)
 
 # Remove the temporary directory
```

### Comparing `eu_cbm_hat-0.6.4/scripts/setup/activities_creation.py` & `eu_cbm_hat-0.6.5/scripts/setup/activities_creation.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/setup/copy_zz_from_libcbm_data.py` & `eu_cbm_hat-0.6.5/scripts/setup/copy_zz_from_libcbm_data.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/setup/make_interface.py` & `eu_cbm_hat-0.6.5/scripts/setup/make_interface.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/scripts/setup/save_interface.py` & `eu_cbm_hat-0.6.5/scripts/setup/save_interface.py`

 * *Files identical despite different names*

### Comparing `eu_cbm_hat-0.6.4/setup.py` & `eu_cbm_hat-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 this_dir = path.abspath(path.dirname(__file__))
 readme_path = path.join(this_dir, 'README.md')
 with open(readme_path, encoding='utf-8') as handle: readme = handle.read()
 
 # Call setup #
 setup(
     name             = 'eu_cbm_hat',
-    version          = '0.6.4',
+    version          = '0.6.5',
     description      = 'eu_cbm_hat is a python package for running carbon'
                        ' budget simulations.',
     license          = 'EUPL',
     url              = 'https://gitlab.com/bioeconomy/eu_cbm/eu_cbm_hat',
     author           = 'Lucas Sinclair',
     author_email     = 'lucas.sinclair@me.com',
     maintainer       = 'Paul Rougieux',
```

